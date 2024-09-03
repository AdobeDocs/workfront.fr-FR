---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Authentification pour Document Webhooks
description: Authentification pour Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 100%

---

# Authentification pour Document Webhooks

## Authentification

Adobe Workfront Document Webhooks prend en charge deux formes d’authentification différentes : OAuth2 et ApiKey. Dans les deux cas, Workfront transmet des jetons d’authentification dans l’en-tête lors d’un appel API.

### OAuth2

OAuth2 permet à Workfront d’effectuer des appels API autorisés à un fournisseur de webhooks au nom d’un utilisateur ou d’une utilisatrice. Avant cela, l’utilisateur ou l’utilisatrice doit connecter son compte de fournisseur de documents externe à Workfront et octroyer à Workfront l’accès

pour agir en son nom. Ce processus de liaison ne s’opère qu’une seule fois pour chaque personne. Voici comment cela fonctionne :

1. La personne commence la procédure de connexion de l’intégration webhook à son compte. La méthode actuelle pour effectuer cette opération consiste à cliquer sur la liste déroulante « Ajouter un document » > « Ajouter un service » > Nom de l’intégration personnalisée.
1. Workfront dirige la personne vers l’URL d’authentification, ce qui peut l’inviter à se connecter au fournisseur de documents externe. Cette page est hébergée par le fournisseur de webhooks ou le système externe de gestion des documents. Dans ce cas, Workfront ajoute le paramètre « state » à l’URL d’authentification. Cette valeur doit être renvoyée à Workfront en ajoutant la même valeur à l’URI de retour Workfront lors de l’étape ci-dessous.
1. Une fois connectée au système externe (ou si elle est déjà connectée), la personne est dirigée vers une page « Authentification », ce qui explique pourquoi Workfront demande l’accès pour effectuer une série d’actions pour le compte de la personne.
1. Si l’utilisateur ou l’utilisatrice clique sur le bouton « Autoriser », le navigateur redirige vers l’URI de redirection Workfront, en ajoutant « code=`<code>` » à la chaîne de requête. Du fait de la spécification OAuth2, ce jeton est de courte durée. La chaîne de requête doit également comporter le paramètre « state=`<sent_by_workfront>` ».
1. Workfront traite cette requête et effectue un appel API vers l’URL de point d’entrée du jeton avec le code d’autorisation.
1. L’URL de point d’entrée du jeton renvoie un jeton d’actualisation et un jeton d’accès.
1. Workfront stocke ces jetons et fournit une intégration des webhooks complète pour cette personne.
1. Désormais, Workfront peut effectuer des appels API autorisés vers le fournisseur de webhooks.Lors de ces appels, Workfront envoie le jeton d’accès dans l’en-tête de requête HTTP comme indiqué ci-dessous :

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Si le jeton d’accès a expiré, Workfront appelle l’URL de point d’entrée du jeton pour récupérer un nouveau jeton d’accès, puis effectue une nouvelle tentative d’appel API autorisé avec le nouveau jeton d’accès.

### ApiKey

Il est beaucoup plus simple d’effectuer des appels API autorisés vers un fournisseur de webhooks avec ApiKey plutôt qu’avec OAuth2. Lors d’un appel API, Workfront transmet simplement les noms d’utilisateur ou d’utilisatrice ApiKey et Workfront dans l’en-tête de la requête HTTP :

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Le fournisseur de webhooks peut utiliser le nom d’utilisateur ou d’utilisatrice pour accorder des autorisations spécifiques à l’utilisateur ou l’utilisatrice. L’efficacité est optimale lorsque les deux systèmes se connectent à LDAP à l’aide de l’authentification unique (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
