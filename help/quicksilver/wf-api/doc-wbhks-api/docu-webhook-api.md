---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: API Document Webhooks
description: API Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '3620'
ht-degree: 3%

---


# API Document Webhooks

Les webhooks de document Adobe Workfront définissent un ensemble de points de terminaison d’API par le biais desquels Workfront effectue des appels d’API autorisés à un fournisseur de document externe. Cela permet à tous les utilisateurs de créer un module externe middleware pour n’importe quel fournisseur de stockage de documents.

L’expérience utilisateur des intégrations basées sur webhook est similaire à celle des intégrations de documents existantes, telles que Google Drive, Box et Dropbox. Par exemple, un utilisateur Workfront peut effectuer les actions suivantes :

* Parcourir la structure de dossiers du fournisseur de documents externe
* Recherche de fichiers
* Lier des fichiers à Workfront
* Chargement de fichiers dans le fournisseur de documents externe
* Affichage d’une miniature pour le document

## Implémentation de référence

Pour accélérer le développement d’une nouvelle implémentation de webhooks, Workfront fournit une implémentation de référence. Vous trouverez le code pour cela à l’adresse [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Cette implémentation est basée sur Java et permet à Workfront de connecter des documents sur un système de fichiers réseau.

## Enregistrement d’une intégration Webhook

Les administrateurs Workfront peuvent ajouter une intégration webhook personnalisée pour leur entreprise en accédant à Configuration > Documents > Intégrations personnalisées dans Workfront. Sur la page Intégration personnalisée de Configuration, les administrateurs peuvent afficher une liste des intégrations Webhook de document existantes. Depuis cette page, les intégrations peuvent être ajoutées, modifiées, activées et désactivées. Pour ajouter une intégration, cliquez sur le bouton &quot;Ajouter une intégration&quot;.

### Champs disponibles

Lors de l’ajout d’une intégration, l’administrateur saisit les valeurs des champs suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de champ</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nom</td> 
   <td>Nom de cette intégration.</td> 
  </tr> 
  <tr> 
   <td>URL API de base</td> 
   <td> <p>Emplacement de l’API de rappel. Lors d’appels au système externe, Workfront ajoute simplement le nom du point de terminaison à cette adresse. Par exemple, si l’administrateur a saisi l’URL de l’API de base " https://www.mycompany.com/api/v1", Workfront utilise l’URL suivante pour obtenir les métadonnées d’un document : https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Paramètres de requête</td> 
   <td> <p>Les valeurs optionnelles à ajouter à la chaîne de requête de chaque appel API. Par exemple, access_type</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Type d'authentification</td> 
   <td>OAuth2 ou ApiKey</td> 
  </tr> 
  <tr> 
   <td>URL d'authentification</td> 
   <td> <p>(OAuth2 uniquement) URL complète utilisée pour l’authentification de l’utilisateur. Workfront accède aux utilisateurs à cette adresse dans le cadre du processus d’approvisionnement OAuth. Remarque : Workfront ajoute un paramètre "state" à la chaîne de requête. Le fournisseur doit transmettre cette information à Workfront en l’ajoutant à l’URI de redirection Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL de jeton de point d’entrée</td> 
   <td> <p>(OAuth2 uniquement) URL complète de l’API utilisée pour récupérer les jetons OAuth2. Il est hébergé par le fournisseur webhook ou le fournisseur de document externe</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>ID client</td> 
   <td>(OAuth2 uniquement) ID client OAuth2 pour cette intégration</td> 
  </tr> 
  <tr> 
   <td>Clé secrète client</td> 
   <td> <p>(OAuth2 uniquement) Secret client OAuth2 pour cette intégration</p> </td> 
  </tr> 
  <tr> 
   <td>URI de redirection Workfront</td> 
   <td>  <p>(OAuth2 uniquement) Il s’agit d’un champ en lecture seule généré par Workfront. Cette valeur est utilisée pour enregistrer cette intégration auprès du fournisseur de documents externe. Remarque : Comme décrit ci-dessus pour l’URL d’authentification, le fournisseur doit ajouter le paramètre "state" et sa valeur à la chaîne de requête lors de l’exécution de la redirection.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(ApiKey uniquement) Utilisé pour effectuer des appels API autorisés au fournisseur webhook. Clé API émise par le fournisseur webhook.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Authentification

Les webhooks de documents Workfront prennent en charge deux formes d’authentification différentes : OAuth2 et ApiKey. Dans les deux cas, Workfront transmet des jetons d’authentification dans l’en-tête lors d’un appel API.

### OAuth2

OAuth2 permet à Workfront d’effectuer des appels API autorisés à un fournisseur de webhook au nom d’un utilisateur. Avant cela, l’utilisateur doit connecter son compte de fournisseur de documents externe à Workfront et octroyer Workfront.

l&#39;accès pour agir en leur nom. Ce processus de prise en main ne se produit qu’une seule fois pour chaque utilisateur. Voici comment cela fonctionne :

1. L’utilisateur commence à connecter l’intégration webhook à son compte. Pour ce faire, cliquez sur la liste déroulante &quot;Ajouter un document&quot; > &quot;Ajouter un service&quot; > Nom de l’intégration personnalisée.
1. Workfront navigue dans l’URL d’authentification de l’utilisateur, ce qui peut l’inviter à se connecter au fournisseur de documents externe. Cette page est hébergée par le fournisseur webhook ou le système externe de gestion des documents. Dans ce cas, Workfront ajoute un paramètre &quot;state&quot; à l’URL d’authentification. Cette valeur doit être retransmise à Workfront en ajoutant la même valeur à l’URI de retour Workfront à l’étape ci-dessous.
1. Une fois connecté au système externe (ou si l’utilisateur est déjà connecté), il est dirigé vers une page &quot;Authentification&quot;, ce qui explique que Workfront demande l’accès pour effectuer un ensemble d’actions pour le compte de l’utilisateur.
1. Si l’utilisateur clique sur le bouton &quot;Autoriser&quot;, le navigateur effectue une redirection vers l’ URI de redirection Workfront , en ajoutant &quot;code=`<code>`&quot; à la chaîne de requête. Selon la spécification OAuth2, ce jeton est de courte durée. La chaîne de requête doit également comporter le paramètre &quot;state=`<sent_by_workfront>`&quot; suivant.
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

### Ajout d’en-têtes de requête (facultatif)

Outre l’utilisation de jetons OAuth2 ou d’une ApiKey pour l’authentification, Workfront peut envoyer un ensemble prédéfini d’en-têtes au fournisseur webhook pour chaque appel API. Un administrateur Workfront peut configurer cette configuration lors de l’enregistrement ou de la modification d’une intégration de Webook, comme décrit dans la section ci-dessus. Voir Enregistrement d’une intégration Webhook.

Par exemple, cela peut être utilisé pour l’authentification de base. Pour ce faire, l’administrateur de Workfront ajoute les informations d’en-tête de requête suivantes dans la boîte de dialogue Intégration personnalisée :

   Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==

où QWxhZGRpbjpvcGVuIHNlc2FtZQ== est une chaîne codée en base 64 de &quot;username:password&quot;. Voir Authentification de base . A condition que cela ait été ajouté, Workfront transmettra cette information dans l’en-tête de requête HTTP, en plus des autres en-têtes de requête :

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## Spécification de l’API

Vous trouverez ci-dessous une liste des API que le fournisseur webhook doit implémenter pour que les webhooks de document fonctionnent.

### Obtention de jetons OAuth2 (authentification OAuth2 requise uniquement)

Renvoie le jeton d’actualisation OAuth2 et le jeton d’accès pour un utilisateur authentifié. Il est appelé une fois lorsque l’utilisateur a configuré un fournisseur de documents. Les appels suivants sont effectués pour obtenir un jeton d’accès mis à jour.

POST de requêtes HTTP /any/url

L’URL est configurable et correspond à la valeur de l’URL Point d’entrée du jeton sur la page de configuration de l’intégration personnalisée.

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Requis</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>oui</td> 
   <td> <p>Les valeurs comprennent "authorization_code" ou "refresh_token". La valeur spécifiée indique lequel des deux paramètres sera transmis à cet appel API : code ou refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>code</td> 
   <td>dépend</td> 
   <td> <p>Code d’autorisation envoyé à Workfront juste après que l’utilisateur a cliqué sur le bouton "Accorder". Cela n’est nécessaire que lorsque le type d’octroi est "authorization_code". Le code d’autorisation doit être de courte durée, expirant généralement en 10 minutes ou moins.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>dépend</td> 
   <td> <p>Cela n’est nécessaire que lors d’appels ultérieurs pour récupérer un nouveau jeton d’accès, étant donné que le jeton d’accès précédent a expiré. Lors de l’envoi de cette valeur, définissez le paramètre grant_type sur "refresh_token".</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>oui</td> 
   <td>Identifiant du client configuré dans Workfront pour cette intégration personnalisée.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>oui</td> 
   <td> Secret client configuré dans Workfront pour cette intégration personnalisée.</td> 
  </tr> 
 </tbody> 
</table>

 

**Réponse**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Type </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>Chaîne</td> 
   <td> <p>Jeton utilisé pour effectuer des appels API autorisés pour le compte de l’utilisateur. Cet délai doit expirer pour empêcher les appels d’API non autorisés.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>Chaîne</td> 
   <td> <p>Jeton de longue durée utilisé pour récupérer un nouveau jeton d’accès en appelant cette méthode d’API.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>(facultatif) La durée (en secondes) précédant l’expiration de access_token, généralement 3 600.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Exemple**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**Réponse**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### Obtention de métadonnées pour un fichier ou un dossier

Renvoie les métadonnées du fichier ou du dossier spécifié.

**URL**

GET /metadata?id=[ID de document ou de dossier]

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>L’identifiant du fichier ou du dossier, tel que référencé par le fournisseur webhook. Différent de l’ID de document Workfront. Pour obtenir les métadonnées du répertoire racine, utilisez la valeur "/".</p><p>Remarque : La longueur maximale de l’ID est de 255 caractères.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Réponse**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom </th> 
   <th>Type </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Chaîne </td> 
   <td>Nom du document ou du dossier</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>Chaîne </td> 
   <td>Indique si cet élément est un fichier ou un dossier (fichier ou dossier)</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Chaîne </td> 
   <td>ID du fichier ou du dossier.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Chaîne </td> 
   <td> <p>Chemin d’accès à l’URL utilisé par un utilisateur pour afficher le document dans une fenêtre de navigateur. L’URL peut être hébergée soit par le fournisseur de documents, soit par le fournisseur de stockage externe natif.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Chaîne </td> 
   <td> <p>Chemin d’accès URL utilisé par un utilisateur pour télécharger le document dans une fenêtre de navigateur. L’URL peut être hébergée soit par le fournisseur de documents, soit par le fournisseur de stockage externe natif.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Chaîne </td> 
   <td>Type MIME du fichier. (facultatif)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Chaîne </td> 
   <td>Dernière modification de ce fichier (horodatage RFC 3339 formaté)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Long</td> 
   <td>  Taille du fichier en octets. (facultatif)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booléen</td> 
   <td>  <p> Indique si ce fichier ou ce dossier est en lecture seule pour l’utilisateur authentifié.(facultatif)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** `https://www.acme.com/api/metadata?id=12345`

**Réponse**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>La gestion des erreurs doit être cohérente pour tous les appels API. Pour plus d’informations, reportez-vous à la section &quot;Gestion des erreurs&quot; ci-dessous.

### Obtention d’une liste d’éléments dans un dossier

Renvoie les métadonnées des fichiers et des dossiers d’un dossier donné.

**URL**

GET /files

**Paramètres de requête**

| Nom  | Description |
|---|---|
| parentId  | ID du dossier. Pour obtenir les métadonnées du répertoire racine, utilisez la valeur &quot;/&quot;. |

{style="table-layout:auto"}

L’API Document Webhooks ne prend actuellement pas en charge la pagination.

**Réponse**

JSON contenant une liste de fichiers et de dossiers. Les métadonnées de chaque élément sont les mêmes que celles renvoyées par le point de terminaison /metadata .

**Exemple :** `https://www.acme.com/api/files?parentId=123456`

**Réponse**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### Exécution d’une recherche

Renvoie les métadonnées des fichiers et dossiers renvoyés à partir d’une recherche. Cela peut être mis en oeuvre sous la forme d’une recherche de texte intégral ou d’une requête de base de données classique. Workfront appelle le point de terminaison /search lorsque l’utilisateur effectue une recherche à partir du navigateur de fichiers externe.

**URL**

GET /search

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>query</td> 
   <td>Terme ou expression à rechercher.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(facultatif) ID de dossier à partir duquel la recherche s’est exécutée. Remarque : Il s’agit d’un espace réservé pour une future fonctionnalité de Workfront. Actuellement, workfront ne transmet pas ce paramètre. </p> </td> 
  </tr> 
  </tbody> 
</table>

L’API Document Webhooks ne prend actuellement pas en charge la pagination.

 

**Réponse**

JSON contenant une liste de métadonnées pour les fichiers et les dossiers correspondant à la requête. Ce qui constitue une &quot;correspondance&quot; est déterminé par le fournisseur webhook. Idéalement, il doit effectuer une recherche de texte intégral. Une recherche basée sur un nom de fichier fonctionne également.

**Exemple :** `https://www.acme.com/api/search?query=test-query`

**Réponse**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Obtention du contenu d’un document

Renvoie les octets bruts d’un document

**URL**

GET /download

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> ID du document.</td> 
  </tr> 
 </tbody> 
</table>

 

**Réponse**

octets bruts du document.

**Exemple :** `https://www.acme.com/api/download?id=123456`

### Obtenir une vignette pour un document

Renvoie les octets de miniature bruts d’un document.

**URL**

GET /thumbnail

**Paramètres de requête**

| Nom  | Description |
|---|---|
| id  | ID du document. |
| size  |  Largeur de la miniature |

{style="table-layout:auto"}

 

**Réponse**

Octets de miniature bruts.

**Exemple :** `https://www.acme.com/api/thumbnail?id=123456`

### Chargement d’un fichier - Partie 1 de 2

Le téléchargement d’un fichier vers un fournisseur de stockage de documents est un processus en deux étapes qui nécessite deux points de terminaison d’API distincts. Workfront commence le processus de chargement en appelant /uploadInit . Ce point de terminaison renvoie un ID de document qui est ensuite transmis à /upload lors du téléchargement des octets de document. Selon le système de stockage de documents sous-jacent, il peut être nécessaire de créer un document de longueur zéro, puis de mettre à jour le contenu du document ultérieurement.

Ajouté à la version 1.1 de cette spécification, l’ID de document et l’ID de version de document peuvent être utilisés pour récupérer des informations supplémentaires auprès de Workfront. Par exemple, si le système de gestion des documents souhaite des informations supplémentaires sur le document, le code de mise en oeuvre webhook peut utiliser l’ID de document pour récupérer ces informations à l’aide de l’API RESTful de Workfront. En règle générale, ces informations peuvent provenir de champs de données personnalisés sur le document et contiennent une tâche, un problème ou un projet.

**URL**

POST /uploadInit

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>Identifiant du dossier parent, tel que référencé par le fournisseur webhook.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>Nom du document.</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>L’ID de document Workfront (ajouté dans la version 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>ID de version de document Workfront (ajouté dans la version 1.1)</td> 
  </tr> 
 </tbody> 
</table>

 

**Réponse**

Métadonnées du fichier, telles que définies par le point de terminaison /metadata .

**Exemple :** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Réponse**

`[file_metadata]` comprend le nouvel ID de document utilisé par le fournisseur de documents.

### Chargement d’un fichier - Partie 2 de 2

Télécharge les octets d’un document vers le fournisseur webhook.

**URL**

PUT /upload

**Paramètres de requête**

| Nom  | Description |
|---|---|
| id  |  ID du document, qui vient d’être créé. |


 

**Corps de requête**

octets de contenu brut du document.

**Réponse**

```
{
"result": "success"
}
```

ou

```
{
"result": "fail"
}
```

**Exemple :** `https://www.acme.com/api/upload?id=1234` *[octets de document inclus dans le flux de mise à jour]*

**Réponse**

```
{
"result":"success"
}
```

### Obtention d’informations sur le service 

(Date de publication - À déterminer) Renvoie des informations sur le service, telles que les fonctionnalités. Workfront utilisera ces informations pour personnaliser l’interface utilisateur dans Workfront. Par exemple, si l’implémentation du webhook contient des actions personnalisées, le fichier JSON doit répertorier ces opérations dans le fichier JSON. Les utilisateurs pourront alors appeler ces actions à partir de Workfront.

**URL**

GET /serviceInfo

Paramètres de requête

Aucun. En outre, les appels à ce point de terminaison ne doivent pas nécessiter d’authentification.

**Réponse**

JSON contenant des informations sur ce service

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Type </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>Chaîne </td> 
   <td>Version du webhook implémentée par ce service. Il s’agit du numéro de version répertorié en haut de cette spécification.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Chaîne </td> 
   <td>Numéro de version interne de ce service. Ce nombre est déterminé par le fournisseur de services webhook et utilisé à des fins d’information uniquement.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher </td> 
   <td>Chaîne </td> 
   <td>Nom de la société qui fournit l’implémentation du webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Chaîne </td> 
   <td>Liste contenant les points de terminaison de l’API implémentés par ce service. Cela peut être utilisé pour s’assurer que l’interface utilisateur de Workfront reflète les fonctionnalités offertes par le fournisseur webhook. Chaque élément de la liste doit inclure le nom du point de terminaison (par exemple, "recherche").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Chaîne</td> 
   <td>  <p>Liste contenant les opérations personnalisées implémentées par ce webhook. Chaque élément de liste comprend un nom et un nom d’affichage. Le nom d’affichage s’affiche dans la liste déroulante "Actions de document" dans Workfront. Cliquez sur l’élément dans la liste déroulante pour appeler l’action dans le webhook en appelant le point de terminaison /customAction .</p></td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** https://www.acme.com/api/serviceInfo

**Renvoie**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### Création d’un dossier

(Ajout dans la version 1.2) Crée un dossier dans un répertoire donné.
URL

POST /createFolder

**Paramètres de requête**

| Nom  | Description |
|---|---|
| parentId  | ID de dossier dans lequel le dossier doit être créé |
| name  | Nom du nouveau dossier |

{style="table-layout:auto"}

 

**Réponse**

Métadonnées du dossier nouvellement créé, telles que définies par le point de terminaison /metadata .

**Exemple :** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

renvoie

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### Supprimer un document ou un dossier

(Date de publication - À déterminer) Supprime un document ou un dossier avec l’ID donné dans le système externe. La suppression d’un dossier entraîne celle de son contenu.

URL

PUT /delete

**Paramètres de requête**

| Nom  | Description |
|---|---|
| documentId  | ID du document à supprimer |
| folderId  |  ID de dossier à supprimer |

{style="table-layout:auto"}

Réponse Chaîne JSON indiquant un succès ou un échec, comme indiqué dans la section Gestion des erreurs ci-dessous.

**Exemple :** PUT https://www.acme.com/api/delete id=1234

renvoie

```
{
"status": "success" 
}
```

renvoie

```
{
"status": "failure", "error": "File not found"
}
```


### Renommer un document ou un dossier

(Date de publication - à déterminer) Renomme un document ou un dossier avec l’ID donné dans le système externe.

URL

PUT /rename

**Paramètres de requête**

| Nom  | Description |
|---|---|
| id | ID du document ou du dossier à renommer |
| name  | Nom du nouveau document ou dossier |

{style="table-layout:auto"}

 

Réponse

Chaîne JSON indiquant la réussite ou l’échec, comme indiqué dans la section Gestion des erreurs ci-dessous.

**Exemple :**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### Exécution d’une action personnalisée

(Date de publication - à déterminer) Ce point de terminaison permet à un utilisateur Workfront (ou peut-être à un événement de workflow automatisé) d’effectuer une action dans le système externe. Le point d’entrée /customAction accepte un paramètre &quot;name&quot;, qui permet au fournisseur webhook d’implémenter plusieurs opérations personnalisées.

Le fournisseur de webhook enregistre des actions personnalisées avec Workfront en incluant les actions dans la réponse /serviceInfo sous customActions. Workfront charge cette liste lors de la configuration ou de l’actualisation du fournisseur webhook sous Configuration > Documents > Intégrations personnalisées.\
![](assets/mceclip0-350x262.png)

Les utilisateurs peuvent déclencher l’action personnalisée en sélectionnant la section située sous &quot;Actions de document&quot;.\
![](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**Paramètres de requête**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Nom </th>
   <th>Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>Identifiant spécifiant le type d’action à effectuer. Cette valeur correspond à l’une des valeurs customAction répertoriées par le point d’entrée /serviceInfo .</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>Identifiant du document de travail pour lequel l’action est en cours d’exécution.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> Identifiant de version de document du plan de travail pour lequel l’action est effectuée.</td>
  </tr>
 </tbody>
</table>

 

**Réponse**

Chaîne JSON indiquant la réussite ou l’échec, comme indiqué dans la section Gestion des erreurs ci-dessous. En cas d’échec (c.-à-d. status = &quot;failure&quot;), Workfront affiche le message d’erreur fourni à l’utilisateur.

**Exemple :** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

response

```
{
"status": "success" 
}
```


## Gestion des erreurs

Des problèmes peuvent survenir lors du traitement des demandes d’API. Cela doit être géré de manière cohérente sur tous les points de terminaison de l’API. Lorsqu’une erreur se produit, le fournisseur webhook effectue les opérations suivantes :

* Incluez un code d’erreur dans l’en-tête de réponse. Les codes d’erreur incluent :

   * 403 - Interdit. Indique que les jetons de requête sont manquants ou non valides ou que les informations d’identification associées aux jetons n’ont pas accès à la ressource spécifiée. Pour les fournisseurs de webhook basés sur OAuth, Workfront tente de récupérer les nouveaux jetons d’accès.
   * 404 - Introuvable. Indique que le fichier ou le dossier spécifié n’existe pas.
   * 500 - Erreur interne du serveur. Tout autre type d&#39;erreur.

* Décrivez l’erreur dans le corps de la réponse en utilisant le format suivant :


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Tests

Pour vérifier que l’implémentation de webhook de votre document fonctionne correctement, exécutez les tests suivants. Il s’agit de tests manuels qui passent par l’interface web de Workfront et atteignent indirectement les points de terminaison de votre implémentation de webhook.

### Conditions préalables

Pour exécuter ces tests, vous aurez besoin des éléments suivants :

* un compte Workfront avec la fonction Advanced Document Management (ADM) activée ;
* Un utilisateur Workfront pour ce compte avec les droits d’administrateur système
* Une instance Webhook de document, dont les points de terminaison HTTP sont accessibles par Workfront

Ces tests supposent également que vous avez déjà enregistré votre instance Document Webhook dans Workfront sous Configuration > Documents > Intégrations personnalisées.

### Test 1 : Configuration du service Document Webhook pour un utilisateur

Teste l’URL d’authentification et l’URL du point de terminaison du jeton pour les fournisseurs WebHook basés sur OAuth.

1. Dans Workfront, accédez à la page Documents principale en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Cliquez sur la liste déroulante Ajouter des documents et sélectionnez votre service Document Webhook sous Ajouter un service.
1. (Services OAuth uniquement) Une fois l’étape précédente terminée, le chargement de la page d’authentification OAuth2 de votre service s’affiche dans une fenêtre contextuelle. (Remarque : vous pouvez être invité à vous connecter à votre service en premier.) Sur la page d’authentification, accordez à Workfront l’accès au compte de l’utilisateur en cliquant sur le bouton Approbation ou Autoriser .
1. Vérifiez que votre service a été ajouté à la liste déroulante Ajouter des documents . Si vous ne le voyez pas initialement, essayez d’actualiser votre navigateur.

### Test 2 : lier un document à Workfront Tests les points de terminaison suivants : /files, /metadata

1. Dans Workfront, accédez à la page Documents principale en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Sélectionnez votre service Document Webhook sous Ajouter des documents.
1. Dans le modal, parcourez la structure de dossiers.
1. Vérifiez que vous pouvez naviguer correctement dans la structure de dossiers.
1. Sélection et liaison d’un document à Workfront

### Test 3 : Accédez à un document dans le système de gestion de contenu

Teste les points de terminaison suivants : /metadata (en particulier viewLink)

1. Liaison d’un document à Workfront
1. Sélectionnez le document et cliquez sur le lien Ouvrir .
1. Vérifiez que le document s’ouvre dans un nouvel onglet.

### Test 4 : Accédez à un document dans le système de gestion de contenu (avec connexion).

Teste les points de terminaison suivants : /metadata (en particulier viewLink)

1. Assurez-vous d’être déconnecté du système de gestion de contenu.
1. Liez un document à Workfront.
1. Sélectionnez le document et cliquez sur le lien Ouvrir .
1. Vérifiez que l’écran de connexion du système de gestion de contenu se charge dans un nouvel onglet.
1. Connectez-vous et vérifiez que vous êtes connecté au document.

### Test 5 : Téléchargez le document à partir du système de gestion de contenu

Teste les points de terminaison suivants : /metadata (en particulier downloadLink)

1. Liez un document à Workfront.
1. Sélectionnez le document et cliquez sur le lien Télécharger .
1. Vérifiez que le téléchargement commence.

### Test 6 : Recherche de contenu

Teste les points de terminaison suivants : /search

1. Dans Workfront, accédez à la page Documents principale en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Sélectionnez votre service Document Webhook sous Ajouter des documents.
1. Dans le modal, effectuez une recherche.
1. Vérifiez que les résultats de la recherche sont corrects.

### Test 7 : envoyer le document de Workfront vers le système de gestion de contenu

Teste les points de terminaison suivants : /files, /uploadInit, /upload

1. Dans Workfront, accédez à la page Documents principale en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Téléchargement d’un document vers Workfront à partir de votre ordinateur
1. Accédez à la page des détails du document.
1. Dans la liste déroulante Actions de document , sélectionnez votre service Document Webhook sous Envoyer à...
1. Accédez au dossier de destination de votre choix et cliquez sur le bouton Enregistrer .
1. Vérifiez que le document est téléchargé au bon emplacement dans le système de gestion de contenu.

### Test 8 : Affichage des miniatures dans Workfront

Teste les points de terminaison suivants : /thumbnail

1. Liez un document à Workfront.
1. Sélectionnez le document dans la liste.
1. Vérifiez que la miniature s’affiche dans le panneau de droite.

### Test 9 : Obtention des octets de contenu

Teste les points de terminaison suivants : /download

1. Liez un document à Workfront.
1. Accédez à la page des détails du document.
1. Envoyez le document à Workfront en sélectionnant Actions du document > Envoyer à... > Workfront. Une nouvelle version de document est alors créée dans Workfront.
1. Téléchargez le document à partir de Workfront en cliquant sur le lien Télécharger .

### Test 10 : Actualiser le jeton d’accès (fournisseurs OAuth2 Webhook uniquement)

Teste les points de terminaison suivants : URL du point de terminaison du jeton

1. Configuration d’un service Document Webhook pour un utilisateur
1. Invalidez le jeton d’accès de l’utilisateur par 1 ) en attendant son expiration ou 2) en l’invalidant manuellement dans le système externe.
1. Actualisez le jeton d’accès dans Workfront. Vous pouvez le faire, par exemple, en liant un document à Workfront. Vous savez que le jeton d’accès s’est correctement actualisé si vous avez pu accéder à un document et le lier.

>[!NOTE]
>
>Actuellement, l’option Envoyer à... n’est pas disponible pour les documents liés. Cela sera ajouté par Workfront. Vous pouvez tester le point de terminaison /download en appuyant manuellement sur le point de terminaison à l’aide d’un client REST, tel que Postman. Vous pouvez également tester le point de terminaison /download en générant un BAT numérique. Pour l’activer, contactez Workfront.

## Versions

* Version 1.0 (Date de publication - mai 2015)

   * Spécification initiale

* Version 1.1 (Date de publication - juin 2015)

   * Mise à jour de /uploadInit : ajout de documentId et documentVersionId

* Version 1.2 (Date de publication - octobre 2015)

   * Ajout de /createFolder

