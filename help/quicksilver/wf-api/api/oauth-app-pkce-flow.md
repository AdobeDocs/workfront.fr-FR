---
content-type: api
navigation-topic: api-navigation-topic
title: Utilisation du flux PKCE pour les applications OAuth 2
description: Utilisation du flux PKCE pour les applications OAuth 2
author: John
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 03df0ad329255e86780c03bbb4541e0a0a526381
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux PKCE

PKCE est un flux d’autorisation sécurisé qui fonctionne bien avec les applications d’actualisation dynamique telles que les applications mobiles, mais qui est utile pour tous les clients OAuth2. Au lieu d’un secret client statique, PKCE utilise une chaîne générée dynamiquement, éliminant ainsi le risque de fuite d’un secret client.

## Présentation de PKCE

Un flux PKCE comprend les étapes suivantes. Les étapes de cette section sont présentées à titre d’information uniquement. Pour effectuer ces procédures, reportez-vous aux autres sections de cet article.

1. Le client crée la variable `code_challenge` en transformant la variable `code_verifier` using `S256` cryptage.

1. Le client redirige le navigateur vers la page de connexion OAuth2, ainsi que le `code_challenge`. Vous devez enregistrer votre application (client) afin qu’OAuth2 puisse accepter la demande d’autorisation. Après l’enregistrement, votre application peut rediriger le navigateur vers OAuth2.

1. Le serveur d’autorisation OAuth2 redirige l’invite d’authentification vers l’utilisateur.

1. L’utilisateur s’authentifie à l’aide de l’une des options de connexion configurées. Une page de consentement répertoriant les autorisations qu’OAuth2 accordera à l’application peut s’afficher.

1. OAuth2 redirige vers votre application avec une `authorization code`.

1. Votre application envoie ce code, ainsi que la variable `code_verifier`, à OAuth2.

1. Le serveur d’autorisation OAuth2 transforme la variable `code_verifier` en utilisant la variable `code_challenge_method` à partir de la demande d’autorisation initiale et vérifie le résultat par rapport à la variable `code_challenge`. Si la valeur des deux chaînes correspond, le serveur a vérifié que les requêtes provenaient du même client et émet une `access token`.

1. OAuth2 renvoie la variable `access token`et éventuellement une `refresh token`.

1. Votre application peut désormais utiliser ces jetons pour appeler le serveur de ressources, tel qu’une API au nom de l’utilisateur.

1. Le serveur de ressources valide le jeton avant de répondre à la requête.


## Configuration de votre application

Avant de pouvoir implémenter l’autorisation, vous devez enregistrer votre application dans OAuth2 en créant une intégration d’application à partir de Workfront.

Pour plus d’informations sur la création de l’application OAuth2, voir [Création d’une application web OAuth2 mono-page à l’aide de PKCE ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Création d’applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## Création de la clé de bon à tirer pour l’échange de code

Tout comme le flux de code d’autorisation standard, votre application commence par rediriger le navigateur de l’utilisateur vers votre serveur d’autorisation. `/authorize` point de terminaison . Cependant, dans ce cas, vous devez également relever un défi de code.

Votre première étape consiste à générer un vérificateur de code et un défi à relever.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Vérificateur de code</td>
        <td>
          <p>Chaîne compatible avec les URL aléatoire avec une longueur minimale de 43 caractères</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Problème de code</td>
        <td>
          <p>Hachage SHA-256 codé URL de base64 du vérificateur de code.</p>
        </td>
      </tr>
    </tbody>
</table>


Vous devez ajouter du code dans votre application cliente pour créer le vérificateur de code et le défi de code.

Le code de générateur PKCE crée une sortie similaire à ce qui suit :

>[!INFO]
>
>**Exemple:**
>
>
```
>{
>
>
  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>
>
  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>
>
}
>```

Votre application enregistre la variable `code_verifier` pour plus tard, et envoie la variable `code_challenge` ainsi que la demande d’autorisation auprès de votre serveur d’autorisation. `/authorize` URL.

## Demande de code d’autorisation

Si vous utilisez le serveur d’autorisation personnalisé par défaut, l’URL de votre demande est similaire à ce qui suit :

>[!INFO]
>
>**Exemple:**
>
>
>
```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>
>
&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Notez les paramètres transmis :

* `client_id` correspond à l’identifiant du client de l’application OAuth2 que vous avez créée dans lors de la configuration de l’application.

   Pour plus d’informations, voir Création d’une application web OAuth2 mono-page à l’aide de PKCE dans Création d’applications OAuth2 pour les intégrations Workfront.

* `response_type` is `code`, car l’application utilise le type d’octroi Code d’autorisation .

* `redirect_uri` est l’emplacement de rappel vers lequel l’agent utilisateur est dirigé, ainsi que la variable `code`. Celui-ci doit correspondre à l’une des URL de redirection que vous avez spécifiées lors de la création de votre application OAuth2.

* `code_challenge_method` est la méthode de hachage utilisée pour générer le défi, qui est toujours `S256` pour les applications Workfront Oauth2 qui utilisent PKCE.

* `code_challenge` est le défi de code utilisé pour PKCE.


## Échange du code des jetons

Pour échanger le code d’autorisation contre un jeton d’accès, transmettez-le à votre serveur d’autorisation. `/token` le point de terminaison , ainsi que la variable `code_verifier`.

>[!INFO]
>
>**Exemple:**
>
>
```
>/token \\
>
>
  --header 'accept: application/json' \\
>
>
  --header 'cache-control: no-cache' \\
>
>
  --header 'content-type: application/x-www-form-urlencoded' \\
>
>
  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> Contrairement au flux de code d’autorisation ordinaire, cet appel ne nécessite pas l’en-tête d’autorisation avec l’ID client et le secret. C’est pourquoi cette version du flux du code d’autorisation est appropriée pour les applications natives telles que les applications mobiles ou les applications d’une seule page qui n’ont pas de serveur principal.

Notez les paramètres transmis :

* `grant_type` is `authorization_code`, car l’application utilise le type d’octroi Code d’autorisation .

* `redirect_uri` doit correspondre à l’URI utilisé pour obtenir le code d’autorisation.

* `code` est le code d’autorisation que vous avez reçu du point de terminaison /authorized .

* `code_verifier` est le vérificateur de code PKCE que votre application a généré dans [Création de la clé de bon à tirer pour l’échange de code](#Create).

* `client_id` identifie votre client et doit correspondre à la valeur pré-enregistrée dans OAuth2.


Si le code est toujours valide et que le vérificateur de code correspond, votre application reçoit un jeton d’accès.

>[!INFO]
>
>**Exemple:**
>
>
```
>{
>
>
    "access\_token": "eyJhd\[...\]Yozv",
>
>
    "expires\_in": 3600,
>
>
    "token\_type": "Bearer"
>
>
}
>```

## Validation du jeton d’accès

Lorsque votre application transmet une demande avec un jeton d’accès, le serveur de ressources doit la valider.

Vous pouvez valider votre jeton d’accès avec un appel API similaire à ce qui suit :

>[!INFO]
>
>**Exemple:**
>
>
```
>/attask/api/<api version>/proj/search \\
>
>
  --header 'sessionID: <access\_token>' \\
>```

## Demande d’un jeton d’actualisation

Pour demander un jeton d’actualisation, vous pouvez effectuer un appel POST à l’API, comme suit :

>[!INFO]
>
>**Exemple:**
>
>
```
>/token \\
>
>
  --header 'accept: application/json' \\
>
>
  --header 'cache-control: no-cache' \\
>
>
  --header 'content-type: application/x-www-form-urlencoded' \\
>
>
  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
