---
content-type: api
navigation-topic: api-navigation-topic
title: Utilisation du flux PKCE pour les applications OAuth 2
description: Utilisation du flux PKCE pour les applications OAuth 2
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 2%

---

# Configurer et utiliser les applications OAuth2 personnalisées de votre organisation à l’aide du flux PKCE

PKCE est un flux d’autorisation sécurisé qui fonctionne bien avec les applications d’actualisation dynamique telles que les applications mobiles, mais qui est utile pour tous les clients OAuth2. Au lieu d’un secret client statique, PKCE utilise une chaîne générée dynamiquement, éliminant ainsi le risque de fuite d’un secret client.

## Présentation de PKCE

Un flux PKCE comprend les étapes suivantes. Les étapes de cette section sont présentées à titre d’information uniquement. Pour effectuer ces procédures, reportez-vous aux autres sections de cet article.

1. Le client crée le `code_challenge` en transformant le `code_verifier` à l’aide du chiffrement `S256`.

1. Le client redirige le navigateur vers la page de connexion OAuth2, ainsi que le `code_challenge` généré. Vous devez enregistrer votre application (client) afin qu’OAuth2 puisse accepter la demande d’autorisation. Après l’enregistrement, votre application peut rediriger le navigateur vers OAuth2.

1. Le serveur d’autorisation OAuth2 redirige l’invite d’authentification vers l’utilisateur.

1. L’utilisateur s’authentifie à l’aide de l’une des options de connexion configurées. Une page de consentement répertoriant les autorisations qu’OAuth2 accordera à l’application peut s’afficher.

1. OAuth2 redirige vers votre application avec un `authorization code`.

1. Votre application envoie ce code, ainsi que le `code_verifier`, à OAuth2.

1. OAuth2 Authorization Server transforme l’ `code_verifier` à l’aide de l’ `code_challenge_method` à partir de la demande d’autorisation initiale et vérifie le résultat par rapport à l’ `code_challenge`. Si la valeur des deux chaînes correspond, le serveur a vérifié que les demandes provenaient du même client et va émettre un `access token`.

1. OAuth2 renvoie le `access token` et éventuellement un `refresh token`.

1. Votre application peut désormais utiliser ces jetons pour appeler le serveur de ressources, tel qu’une API au nom de l’utilisateur.

1. Le serveur de ressources valide le jeton avant de répondre à la requête.


## Configuration de votre application

Avant de pouvoir implémenter l’autorisation, vous devez enregistrer votre application dans OAuth2 en créant une intégration d’application à partir de Workfront.

Pour plus d’informations sur la création de l’application OAuth2, voir [Création d’une application web OAuth2 sur une seule page à l’aide de PKCE](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) dans [Création d’applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.


## Création de la clé de bon à tirer pour l’Exchange de code

Tout comme le flux de code d’autorisation standard, votre application commence par rediriger le navigateur de l’utilisateur vers le point de terminaison `/authorize` de votre serveur d’autorisation. Cependant, dans ce cas, vous devez également relever un défi en matière de code.

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
>**Exemple :**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

Votre application enregistre le `code_verifier` pour plus tard et envoie le `code_challenge` avec la demande d’autorisation à l’URL `/authorize` de votre serveur d’autorisation.

## Demande de code d’autorisation

Si vous utilisez le serveur d’autorisation personnalisé par défaut, l’URL de votre demande est similaire à ce qui suit :

>[!INFO]
>
>**Exemple :**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Notez les paramètres transmis :

* `client_id` correspond à l’identifiant du client de l’application OAuth2 que vous avez créée dans lors de la configuration de l’application.

  Pour plus d’informations, voir Création d’une application web OAuth2 mono-page à l’aide de PKCE dans Création d’applications OAuth2 pour les intégrations Workfront.

* `response_type` est `code`, car l’application utilise le type d’octroi Code d’autorisation .

* `redirect_uri` est l’emplacement de rappel vers lequel l’agent utilisateur est dirigé, ainsi que le `code`. Celui-ci doit correspondre à l’une des URL de redirection que vous avez spécifiées lors de la création de votre application OAuth2.

* `code_challenge_method` est la méthode de hachage utilisée pour générer le défi, qui est toujours `S256` pour les applications Workfront Oauth2 qui utilisent PKCE.

* `code_challenge` est le défi de code utilisé pour PKCE.


## Exchange du code des jetons

Pour exchange du code d’autorisation d’un jeton d’accès, transmettez-le au point de terminaison `/token` de votre serveur d’autorisation avec le `code_verifier`.

>[!INFO]
>
>**Exemple :**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> Contrairement au flux de code d’autorisation ordinaire, cet appel ne nécessite pas l’en-tête d’autorisation avec l’ID client et le secret. C’est pourquoi cette version du flux du code d’autorisation est appropriée pour les applications natives telles que les applications mobiles ou les applications d’une seule page qui n’ont pas de serveur principal.

Notez les paramètres transmis :

* `grant_type` est `authorization_code`, car l’application utilise le type d’octroi Code d’autorisation .

* `redirect_uri` doit correspondre à l’URI utilisé pour obtenir le code d’autorisation.

* `code` est le code d’autorisation que vous avez reçu du point de terminaison /authorized.

* `code_verifier` est le vérificateur de code PKCE que votre application a généré dans [Création de la clé de bon à tirer pour l’Exchange de code](#Create).

* `client_id` identifie votre client et doit correspondre à la valeur pré-enregistrée dans OAuth2.


Si le code est toujours valide et que le vérificateur de code correspond, votre application reçoit un jeton d’accès.

>[!INFO]
>
>**Exemple :**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## Validation du jeton d’accès

Lorsque votre application transmet une demande avec un jeton d’accès, le serveur de ressources doit la valider.

Vous pouvez valider votre jeton d’accès avec un appel API similaire à ce qui suit :

>[!INFO]
>
>**Exemple :**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Demande d’un jeton d’actualisation

Pour demander un jeton d’actualisation, vous pouvez effectuer un appel POST à l’API, comme suit :

>[!INFO]
>
>**Exemple :**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
