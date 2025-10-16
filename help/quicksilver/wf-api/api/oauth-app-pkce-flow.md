---
content-type: api
navigation-topic: api-navigation-topic
title: Utiliser le flux PKCE pour les applications OAuth2
description: Utiliser le flux PKCE pour les applications OAuth2
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: f9a154fa92217810b762ac48169512bc0bca7305
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 100%

---

# Configurer et utiliser les applications OAuth2 personnalisées de votre organisation à l’aide du flux PKCE

PKCE est un flux d’autorisation sécurisé qui fonctionne bien avec les applications à actualisation dynamique, telles que les applications mobiles, mais qui est utile pour tous les clients OAuth2. Au lieu d’utiliser un secret client statique, PKCE emploie une chaîne générée dynamiquement, éliminant ainsi le risque de fuite d’un secret client.

## Vue d’ensemble de PKCE

Un flux PKCE comprend les étapes suivantes. Les étapes de cette section sont présentées à titre d’information uniquement. Pour effectuer ces procédures, reportez-vous aux autres sections de cet article.

1. Le client crée `code_challenge` en transformant `code_verifier` à l’aide d’un chiffrement `S256`.

1. Le client dirige le navigateur vers la page de connexion OAuth2, avec le `code_challenge` généré. Vous devez enregistrer votre application (client) afin qu’OAuth2 puisse accepter la demande d’autorisation. Après l’enregistrement, votre application peut rediriger le navigateur vers OAuth2.

1. Le serveur d’autorisation OAuth2 redirige l’invite d’authentification vers l’utilisateur ou l’utilisatrice.

1. La personne s’authentifie à l’aide de l’une des options de connexion configurées. Une page de consentement répertoriant les autorisations qu’OAuth2 accordera à l’application peut s’afficher.

1. OAuth2 redirige vers votre application avec un `authorization code`.

1. Votre application envoie ce code, conjointement au `code_verifier`, à OAuth2.

1. Le serveur d’autorisation OAuth2 transforme le `code_verifier` en utilisant la `code_challenge_method` à partir de la demande d’autorisation initiale et vérifie le résultat par rapport au `code_challenge`. Si la valeur des deux chaînes correspond, cela signifie que le serveur a vérifié que les requêtes provenaient du même client et qu’il émettra un `access token`.

1. OAuth2 renvoie le `access token`, et éventuellement un `refresh token`.

1. Votre application peut désormais utiliser ces jetons pour appeler le serveur de ressources, tel qu’une API, au nom de l’utilisateur ou l’utilisatrice.

1. Le serveur de ressources valide le jeton avant de répondre à la requête.


## Configurer votre application

Avant de pouvoir implémenter l’autorisation, vous devez enregistrer votre application dans OAuth2 en créant une intégration d’application à partir de Workfront.

Pour obtenir des instructions sur la création de l’application OAuth2, voir la section [Créer une application web OAuth2 d’une seule page à l’aide de PKCE](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) dans [Créer des applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

>[!NOTE]
>
>Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.


## Créer la clé d’épreuve pour l’échange de code

Tout comme le flux de code d’autorisation standard, votre application commence par rediriger le navigateur de l’utilisateur ou l’utilisatrice vers le point d’entrée `/authorize` du serveur d’autorisation. Cependant, dans ce cas, vous devez également transmettre un code_challenge.

Votre première étape consiste à générer un code_verifier et un code_challenge.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Code_verifier</td>
        <td>
          <p>Chaîne URL aléatoire avec une longueur minimale de 43 caractères</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Code_challenge</td>
        <td>
          <p>Hachage SHA-256 codé par URL Base64 du code_verifier</p>
        </td>
      </tr>
    </tbody>
</table>


Vous devez ajouter du code dans l’application de votre client pour créer le code_verifier et le code_challenge.

Le code de générateur PKCE crée une sortie similaire à ce qui suit :

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

votre application enregistre le `code_verifier` pour plus tard, et envoie le `code_challenge` avec la demande d’autorisation à l’URL `/authorize` de votre serveur d’autorisation.

## Demander un code d’autorisation

Si vous utilisez le serveur d’autorisation personnalisé par défaut, l’URL de votre demande est similaire à ce qui suit :

>[!INFO]
>
>**Exemple :**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Notez les paramètres qui sont transmis :

* `client_id` correspond à l’identifiant du client de l’application OAuth2 que vous avez créée lors de la configuration de l’application.

  Pour obtenir des instructions, voir la section Créer une application web OAuth2 d’une seule page à l’aide de PKCE dans Créer des applications OAuth2 pour les intégrations Workfront.

* Le `response_type` est `code`, car l’application utilise le type d’octroi Code d’autorisation.

* `redirect_uri` est l’emplacement de rappel vers lequel l’agent de l’utilisateur ou l’utilisatrice est dirigé en même temps que le `code`. Il doit correspondre à l’un des URI de redirection que vous avez spécifiés lors de la création de votre application OAuth2.

* `code_challenge_method` est la méthode de hachage utilisée pour générer le code_challenge, qui est toujours `S256` pour les applications Workfront Oauth2 qui utilisent PKCE.

* `code_challenge` est le code_challenge utilisé pour PKCE.


## Échanger le code contre des jetons

Pour échanger le code d’autorisation contre un jeton d’accès, transmettez-le au point d’entrée `/token` de votre serveur d’autorisation, accompagné du `code_verifier`.

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
> Contrairement au flux de code d’autorisation habituel, cet appel ne nécessite pas d’en-tête d’autorisation avec l’identifiant et le secret du client. C’est pourquoi cette version du flux du code d’autorisation convient aux applications natives telles que les applications mobiles ou les applications à page unique qui n’ont pas de serveur principal.

Notez les paramètres qui sont transmis :

* Le `grant_type` est `authorization_code`, car l’application utilise le type d’octroi Code d’autorisation.

* `redirect_uri` doit correspondre à l’URI utilisé pour obtenir le code d’autorisation.

* `code` est le code d’autorisation que vous avez reçu du point d’entrée /authorize.

* `code_verifier` est le code_verifier PKCE que votre application a généré dans [Créer la clé de vérification pour l’échange de code](#Create).

* `client_id` identifie le client et doit correspondre à la valeur préenregistrée dans OAuth2.


Si le code est toujours valide et que le code_verifier correspond, votre application reçoit un jeton d’accès.

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

## Valider le jeton d’accès

Lorsque votre application transmet une requête avec un jeton d’accès, le serveur de ressources doit le valider.

Vous pouvez valider votre jeton d’accès à l’aide d’un appel API similaire au suivant :

>[!INFO]
>
>**Exemple :**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Demander un jeton d’actualisation

Pour demander un jeton d’actualisation, vous pouvez effectuer un appel POST à l’API, comme suit :

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
