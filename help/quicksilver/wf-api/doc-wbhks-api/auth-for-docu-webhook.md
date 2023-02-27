---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Authentification pour les webhooks de document
description: Authentification pour les webhooks de document
author: Becky
feature: Workfront API
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Authentification pour les webhooks de document

## Authentification

Les webhooks de documents Adobe Workfront prennent en charge deux formes d’authentification différentes : OAuth2 et ApiKey. Dans les deux cas, Workfront transmet des jetons d’authentification dans l’en-tête lors d’un appel API.

### OAuth2

OAuth2 permet à Workfront d’effectuer des appels API autorisés à un fournisseur de webhook au nom d’un utilisateur. Avant cela, l’utilisateur doit connecter son compte de fournisseur de documents externe à Workfront et octroyer Workfront.

l&#39;accès pour agir en leur nom. Ce processus de prise en main ne se produit qu’une seule fois pour chaque utilisateur. Voici comment cela fonctionne :

1. L’utilisateur commence à connecter l’intégration webhook à son compte. Pour ce faire, cliquez sur la liste déroulante &quot;Ajouter un document&quot; > &quot;Ajouter un service&quot; > Nom de l’intégration personnalisée.
1. Workfront navigue dans l’URL d’authentification de l’utilisateur, ce qui peut l’inviter à se connecter au fournisseur de documents externe. Cette page est hébergée par le fournisseur webhook ou le système externe de gestion des documents. Dans ce cas, Workfront ajoute un paramètre &quot;state&quot; à l’URL d’authentification. Cette valeur doit être retransmise à Workfront en ajoutant la même valeur à l’URI de retour Workfront à l’étape ci-dessous.
1. Une fois connecté au système externe (ou si l’utilisateur est déjà connecté), il est dirigé vers une page &quot;Authentification&quot;, ce qui explique que Workfront demande l’accès pour effectuer un ensemble d’actions pour le compte de l’utilisateur.
1. Si l’utilisateur clique sur le bouton &quot;Autoriser&quot;, le navigateur effectue une redirection vers l’ URI de redirection Workfront , en ajoutant &quot;code=`<code>`&quot; à la chaîne de requête. Selon la spécification OAuth2, ce jeton est de courte durée. La chaîne de requête doit également comporter le paramètre &quot;state=&quot;`<sent_by_workfront>`&quot;.
1. Workfront traite cette requête et effectue un appel API vers l’URL du point de terminaison du jeton avec le code d’autorisation.
1. L’URL Token Endpoint renvoie un jeton d’actualisation et un jeton d’accès.
1. Workfront stocke ces jetons et fournit entièrement l’intégration de webhook pour cet utilisateur.
1. À partir de ce moment, Workfront pourra effectuer des appels API autorisés au fournisseur webhook. Lors de ces appels, Workfront enverra le jeton d’accès dans l’en-tête de requête HTTP comme illustré ci-dessous :

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Si le jeton d’accès a expiré, Workfront appelle l’URL du point d’entrée du jeton pour récupérer un nouveau jeton d’accès, puis tente de nouveau l’appel API autorisé avec le nouveau jeton d’accès.

### ApiKey

Il est beaucoup plus simple d’effectuer des appels API autorisés à un fournisseur webhook à l’aide d’une ApiKey que OAuth2. Lors d’un appel API, Workfront transmet simplement le nom d’utilisateur ApiKey et Workfront dans l’en-tête de la requête HTTP : 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Le fournisseur Webhook peut utiliser le nom d’utilisateur pour appliquer des autorisations spécifiques à l’utilisateur. Cela fonctionne mieux lorsque les deux systèmes se connectent à LDAP à l’aide de l’authentification unique (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of “username:password”. See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
