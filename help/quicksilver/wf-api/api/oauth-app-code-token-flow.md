---
content-type: api
navigation-topic: api-navigation-topic
title: Flux de code d’autorisation pour les applications OAuth2 personnalisées
description: Flux de code d’autorisation pour les applications OAuth2 personnalisées
author: Becky
feature: Workfront API
role: Developer
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: e41b0df5ee0ce092f0811b18c57f6865bbb3abee
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 95%

---


# Configurer et utiliser les applications OAuth2 personnalisées de votre organisation à l’aide du flux de code d’autorisation

Pour intégrer Workfront et permettre à votre application client de communiquer avec Workfront au nom de l’utilisateur ou de l’utilisatrice, vous devez procéder comme suit :

* Créer une application OAuth2
* Configurer l’application tierce
* Lien vers la page d’autorisation pour vos utilisateurs et utilisatrices
* Configurer le flux de code d’autorisation : les utilisateurs et utilisatrices se connectent à l’instance Workfront et consentent à ce que l’application cliente se connecte à Workfront en leur nom. Vous obtenez ainsi un code d’autorisation que vous échangerez contre des jetons d’accès et des jetons d’actualisation.
* Configurer le flux de jetons d’actualisation : dans ce flux, vous utilisez le jeton d’actualisation pour obtenir un nouveau jeton d’accès lorsque l’ancien a expiré.

## Créer une application OAuth2

Pour obtenir des instructions sur la création de l’application OAuth2, voir [Créer une application OAuth2 à l’aide des informations d’identification de l’utilisateur ou de l’utilisatrice (flux de code d’autorisation)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) dans [Créer des applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

>[!NOTE]
>
>Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.

## Lien vers la page d’autorisation pour vos utilisateurs et utilisatrices

Vos utilisateurs et utilisatrices doivent se connecter pour autoriser cette intégration dans leur propre compte. La page à autoriser a un format spécifique, décrit ici. Utilisez ces informations pour déterminer l’adresse de la page d’autorisation de l’application et fournissez à vos utilisateurs et utilisatrices cette adresse ou un lien vers celle-ci.

* URL complète du domaine de votre organisation. Exemple :

  ```
  https://myorganization.my.workfront.com
  ```


* `client_id` : ID client généré lors de la création de l’application OAuth2 dans Workfront.

* `redirect_uri` : cette URL doit être identique à l’URL de redirection que vous avez saisie dans Workfront lors de la création de l’application OAuth2. Vos utilisateurs et utilisatrices seront dirigés vers cette page après avoir autorisé l’application pour leur compte.

* `response_type` : la valeur doit être `code`.

L’URL de la page d’autorisation est donc la suivante :

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>Nous vous recommandons de créer un bouton ou un autre lien sur lequel vos utilisateurs et utilisatrices pourront cliquer pour être redirigés vers cette page.

## Configurer l’application tierce

L’application tierce peut avoir besoin d’être configurée. Le tableau suivant contient des informations sur les champs qui peuvent être nécessaires lors de la configuration de l’application tierce.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URI d’autorisation</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL du jeton</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Étendues</td> 
   <td>Il n’est pas nécessaire de préciser les étendues. </td> 
  </tr> 
 </tbody> 
</table>

## Configurer un flux de code d’autorisation

![](assets/oauth-2-authorization-code-flow.png)

Pour connecter vos utilisateurs et utilisatrices avec OAuth2, suivez le processus suivant :

1. Lorsque l’utilisateur ou l’utilisatrice ouvre la page d’autorisation, celle-ci redirige la personne vers la page de connexion de Workfront afin qu’elle puisse se connecter à Workfront. Si l’utilisateur ou l’utilisatrice a une configuration SSO, la page de connexion du fournisseur d’identité s’ouvre.

   Si la personne est déjà connectée sur Workfront sur ce même navigateur, ou si la personne se connecte avec succès à Workfront, elle est redirigée vers l’écran de consentement :

   ![](assets/consent-screen-350x227.png)

1. Si l’utilisateur ou l’utilisatrice autorise l’accès, la page est redirigée vers l’`redirect_url`. La redirection doit inclure les paramètres de requête suivants :

* `code` : code d’autorisation requis pour obtenir le jeton d’accès/d’actualisation.
* `domain` : domaine de votre organisation. Exemple : dans `myorganization.my.workfront.com`, le domaine est `myorganization`.
* `lane` : volet de votre requête. Exemple : dans `myorganization.preview.workfront.com`, le volet est `preview`.

  >[!IMPORTANT]
  >
  >Le `code` n’est valable que pendant 2 minutes. Vous devez donc obtenir les jetons d’actualisation et d’accès dans ce délai.

1. Lorsque vous disposez d’un code, vous pouvez demander des jetons d’accès et d’actualisation en envoyant le code ainsi que les informations d’identification de l’application cliente au point d’entrée `/integrations/oauth2/api/v1/token`.

   L’URL complète de la demande de jeton est la suivante :

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **Exemples :** exemple d’appel CURL à un point d’entrée de jeton :

   Exemple 1

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Authorization: Basic **<base64(client_id:client_secret)>**' \
      --header 'Content-Type: application/json' \
      --data-raw '{
      "code": "**<code>**",
      "grant_type": "**authorization_code**",
      "redirect_uri": "**<redirect_url>**"
      }'
   ```

   Exemple 2

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Content-Type: application/x-www-form-urlencoded' \
      --data-urlencode 'grant_type=**authorization_code**' \
      --data-urlencode 'redirect_uri=**<redirect_url>**' \
      --data-urlencode 'code=**<code>**' \
      --data-urlencode 'client_id=**<client_id>**' \
      --data-urlencode 'client_secret=**<client_secret>**'  
   ```


   >[!IMPORTANT]
   >
   > Le secret client a été généré lors de l’enregistrement de l’application dans Workfront. Vous devez le conserver dans un endroit sûr, car il est impossible de le récupérer en cas de perte.

   Lorsque tous les paramètres transmis sont corrects, le point d’entrée du jeton renvoie la payload suivante :

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   Le jeton d’accès est le même que celui de ```sessionID```, et il expire de la même manière qu’un ```sessionID``` normal.

   >[!IMPORTANT]
   >
   > Conservez le jeton d’actualisation dans un endroit sûr. Vous en aurez besoin pour obtenir un nouveau jeton d’actualisation lorsque l’ancien aura expiré. Workfront ne stocke pas votre jeton d’actualisation.

1. Maintenant que vous avez un jeton d’accès, vous pouvez faire des appels API à Workfront.

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## Configurer l’actualisation du jeton d&#39;accès

![](assets/refresh-access-token-flow-350x142.png)

Pour actualiser le jeton d’accès, nous devons à nouveau effectuer un appel « POST » vers le point d’entrée du jeton. Cette fois-ci, nous envoyons des données de formulaire différentes comme suit :

```
curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Authorization: Basic <base64(client_id:client_secret)>' \
--header 'Content-Type: application/json' \
--data-raw '{
   "grant_type": "refresh_token",
   "refresh_token": "<refresh_token>"
}'

###### OR

curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=refresh_token' \
--data-urlencode 'redirect_uri=<redirect_url>' \
--data-urlencode 'refresh_token=<refresh_token>' \
--data-urlencode 'client_id=<client_id>' \
--data-urlencode 'client_secret=<client_secret>'
```

Cela renvoie le résultat suivant :

```
{
  "token_type": "sessionID",
  "access_token": "string", // the value of sessionID
  "refresh_token": "string",
  "expires_in": 0,
  "wid": "string"
}
```

Encore une fois, le jeton d’accès est le `sessionID` qui peut être utilisé pour effectuer une requête API à Workfront.
