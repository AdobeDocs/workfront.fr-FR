---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: API Document Webhooks
description: API Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '3627'
ht-degree: 99%

---


# API Document Webhooks

Adobe Workfront Document Webhooks définit un ensemble de points d’entrée d’API par le biais desquels Workfront effectue des appels API autorisés à un fournisseur de documents externe. Cela permet à n’importe qui de créer un plug-in d’intergiciel pour n’importe quel fournisseur de stockage de documents.

L’expérience utilisateur des intégrations basées sur les webhooks sera similaire à celle des intégrations de documents existantes telles que Google Drive, Box et Dropbox. Par exemple, un utilisateur ou une utilisatrice de Workfront pourra effectuer les actions suivantes :

* Naviguer dans la structure des dossiers du fournisseur de documents externes
* Rechercher des fichiers
* Lier des fichiers à Workfront
* Charger des fichiers vers le fournisseur de documents externes
* Afficher une miniature du document

## Implémentation de référence

Pour aider à démarrer le développement d’une nouvelle implémentation de webhooks, Workfront fournit une implémentation de référence. Le code correspondant se trouve à l’adresse suivante : [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Cette implémentation est basée sur Java et permet à Workfront de connecter des documents sur un système de fichiers en réseau.

## Enregistrement d’une intégration de webhook

Les administrateurs et administratirces Workfront peuvent ajouter une intégration de webhook personnalisée pour leur société en naviguant vers Configuration > Documents > Intégrations personnalisées dans Workfront. À partir de la page Intégration personnalisée de la configuration, les administrateurs et administratrices peuvent afficher une liste des intégrations de webhook de documents existantes. Cette page permet d’ajouter, de modifier, d’activer et de désactiver des intégrations. Pour ajouter une intégration, cliquez sur le bouton « Ajouter une intégration ».

### Champs disponibles

Lors de l’ajout d’une intégration, l’administrateur ou administratrice saisit des valeurs pour les champs suivants :

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
   <td> <p>Emplacement de l’API de rappel. Lors des appels au système externe, Workfront ajoutera simplement le nom du point d’entrée à cette adresse. Par exemple, si l’administrateur ou administratrice a saisi l’URL de l’API de base, « https://www.mycompany.com/api/v1 », Workfront utilisera l’URL suivante pour obtenir les métadonnées d’un document : https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
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
   <td> <p>(OAuth2 uniquement) L’URL complète utilisée pour l’authentification de l’utilisateur ou utilisatrice. Workfront dirigera les utilisateurs et utilisatrices vers cette adresse dans le cadre du processus d’approvisionnement OAuth. Remarque : Workfront ajoutera un paramètre « state » à la chaîne de requête. Le fournisseur doit le renvoyer à Workfront en l’ajoutant à l’URI de redirection de Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL de jeton de point d’entrée</td> 
   <td> <p>(OAuth2 uniquement) L’URL d’API complète utilisée pour récupérer les jetons OAuth2. Elle est hébergée par le fournisseur de webhook ou le fournisseur de documents externes.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>ID client</td> 
   <td>(OAuth2 uniquement) ID du client OAuth2 pour cette intégration.</td> 
  </tr> 
  <tr> 
   <td>Clé secrète client</td> 
   <td> <p>(OAuth2 uniquement) Secret du client OAuth2 pour cette intégration.</p> </td> 
  </tr> 
  <tr> 
   <td>URI de redirection Workfront</td> 
   <td>  <p>(OAuth2 uniquement) Ce champ est en lecture seule et est généré par Workfront. Cette valeur est utilisée pour enregistrer cette intégration auprès du fournisseur de documents externes. Note : comme décrit ci-dessus pour l’URL d’authentification, le fournisseur doit ajouter le paramètre « state » et sa valeur à la chaîne de requête lors de la redirection.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(ApiKey uniquement) Utilisé pour effectuer des appels API autorisés vers le fournisseur de webhooks. La clé API émise par le fournisseur de webhooks.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Authentification

Workfront Document Webhooks prend en charge deux formes d’authentification différentes : OAuth2 et ApiKey. Dans les deux cas, Workfront transmet des jetons d’authentification dans l’en-tête lors d’un appel API.

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

### Ajouter des en-têtes de requête (optionnel)

En plus des jetons OAuth2 ou d’une ApiKey pour l’authentification, Workfront peut transmettre un ensemble prédéfini d’en-têtes au fournisseur de webhooks pour chaque appel API. L’administration Workfront peut le configurer lors de l’enregistrement ou de la modification d’une intégration Webook, comme décrit dans la section ci-dessus. Consultez la section « Enregistrer une intégration Webhook ».

Par exemple, cela peut être utilisé pour l’authentification de base. Pour cela, l’administration Workfront doit inclure les informations suivantes dans l’en-tête de la requête dans la boîte de dialogue de l’intégration personnalisée :

   Autorisation de base QWxhZGRpbjpvcGVuIHNlc2FtZQ==

où QWxhZGRpbjpvcGVuIHNlc2FtZQ== est une chaîne encodée en Base64 de « username:password ». Consultez la section « Authentification de base ». Si cet élément est ajouté, Workfront le transmettra dans l’en-tête de la requête HTTP, en plus des autres en-têtes de requête :

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## Spécifier les API

Vous trouverez ci-dessous une liste des API que le fournisseur de webhooks doit mettre en œuvre pour que Document Webhooks fonctionne.

### Obtenir des jetons OAuth2 (seule une authentification OAuth2 est nécessaire)

Renvoie le jeton d’actualisation et le jeton d’accès OAuth2 d’une personne authentifiée. Cette fonction est invoquée une fois lorsque la personne fournit un fournisseur de documents. Les appels suivants sont effectués pour obtenir un jeton d’accès mis à jour.

Requête HTTP POST /any/url

L’URL est configurable et correspond à la valeur de l’URL du point d’entrée de jeton sur la page Configuration de l’intégration personnalisée.

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
   <td> <p>Les valeurs comprennent « authorization_code » ou « refresh_token ». La valeur spécifiée indique lequel des deux paramètres sera transmis à cet appel API : code ou refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>code</td> 
   <td>dépend</td> 
   <td> <p>Le code d’autorisation envoyé à Workfront juste après que la personne a cliqué sur le bouton « Octroi ». Ceci n’est obligatoire que lorsque le type d’octroi est « authorization_code ». Le code d’octroi doit être de courte durée et expire généralement en 10 minutes ou moins.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>dépend</td> 
   <td> <p>Ceci n’est obligatoire que lors d’appels ultérieurs visant à récupérer un nouvel access_token, le précédent access_token ayant expiré. Lors de l’envoi de cette valeur, le paramètre grant_type doit être défini sur « refresh_token ».</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>oui</td> 
   <td>L’ID client configuré dans Workfront pour cette intégration personnalisée.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>oui</td> 
   <td>Le secret client configuré dans Workfront pour cette intégration personnalisée.</td> 
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
   <th>Type</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>Chaîne</td> 
   <td> <p>Un jeton utilisé pour effectuer des appels API autorisés au nom de la personne. Il doit expirer pour éviter les appels d’API non autorisés.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>Chaîne</td> 
   <td> <p>Un jeton de longue durée utilisé pour récupérer un nouvel access_token en appelant cette méthode d’API.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>(facultatif) Le temps (en secondes) avant l’expiration de l’access_token, généralement 3 600.</p></td> 
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

### Obtenir les métadonnées d’un fichier ou d’un dossier

Renvoie les métadonnées du fichier ou du dossier spécifié.

**URL**

GET /metadata?id=[ID du document ou du dossier]

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td>  <p>L’ID du fichier ou du dossier, tel qu’il est référencé par le fournisseur du webhook. Il est différent de l’identifiant de document de Workfront. Pour obtenir les métadonnées du répertoire racine, utilisez la valeur « / ».</p><p>Remarque : la longueur maximale de l’ID est de 255 caractères.</p></td> 
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
   <th>Type</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title</td> 
   <td>Chaîne</td> 
   <td>Nom du document ou du dossier</td> 
  </tr> 
  <tr> 
   <td>kind</td> 
   <td>Chaîne</td> 
   <td>Indique si cet élément est un fichier ou un dossier (« fichier » ou « dossier »).</td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td>Chaîne</td> 
   <td>ID du fichier ou du dossier.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Chaîne</td> 
   <td> <p>Chemin de l’URL utilisé par une personne pour visualiser le document dans une fenêtre de navigateur. L’URL peut être hébergée soit par le fournisseur de documents ou le fournisseur de stockage externe natif.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Chaîne</td> 
   <td> <p>Le chemin d’URL utilisé par une personne pour télécharger le document dans une fenêtre de navigateur. L’URL peut être hébergée soit par le fournisseur de documents ou le fournisseur de stockage externe natif.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Chaîne</td> 
   <td>Type MIME du fichier. (facultatif)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Chaîne</td> 
   <td>Dernière modification de ce fichier (date et heure au format RFC 3339)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Long</td> 
   <td>Taille du fichier en octets. (facultatif)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booléen</td> 
   <td>  <p>Indique si ce fichier ou dossier est en lecture seule pour la personne authentifiée.(facultatif)</p><p> </p></td> 
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
>La gestion des erreurs doit être cohérente pour tous les appels API. Voir la section « Gestion des erreurs » ci-dessous pour plus de détails.

### Obtenir une liste d’éléments d’un dossier

Renvoie les métadonnées des fichiers et des dossiers d’un dossier donné.

**URL**

GET /files

**Paramètres de requête**

| Nom | Description |
|---|---|
| parentId | L’identifiant du dossier. Pour obtenir les métadonnées du répertoire racine, utilisez la valeur « / ». |

{style="table-layout:auto"}

L’API Document Webhooks ne prend pas en charge la pagination pour le moment.

**Réponse**

Le fichier JSON contenant une liste de fichiers et de dossiers. Les métadonnées de chaque élément sont les mêmes que celles renvoyées par le point d’entrée /metadata.

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

### Effectuer une recherche

Renvoie les métadonnées des fichiers et dossiers renvoyés à partir d’une recherche. Cela peut être mis en œuvre sous la forme d’une recherche de texte intégral ou d’une requête de base de données classique. Workfront appelle le point d’entrée /search lorsque l’utilisateur ou l’utilisatrice effectue une recherche à partir du navigateur de fichiers externe.

**URL**

GET /search

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
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
   <td> <p>(Facultatif) ID de dossier à partir duquel la recherche s’est exécutée. Note : il s’agit d’un espace réservé pour une future fonctionnalité de Workfront. Actuellement, Workfront ne transmet pas ce paramètre. </p> </td> 
  </tr> 
  </tbody> 
</table>

L’API Document Webhooks ne prend pas en charge la pagination pour le moment.

 

**Réponse**

JSON contenant une liste de métadonnées pour les fichiers et les dossiers correspondant à la requête. Le fournisseur de webhook détermine ce qui constitue une « correspondance ». Idéalement, il doit effectuer une recherche de texte intégral. Une recherche basée sur un nom de fichier fonctionne également.

**Exemple :** `https://www.acme.com/api/search?query=test-query`

**Réponse**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Obtenir le contenu d’un document

Renvoie les octets bruts d’un document

**URL**

GET /download

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>ID</p> </td> 
   <td>Identifiant du document.</td> 
  </tr> 
 </tbody> 
</table>

 

**Réponse**

Octets bruts du document.

**Exemple :** `https://www.acme.com/api/download?id=123456`

### Obtenir une miniature pour un document

Renvoie les octets bruts de la miniature pour un document.

**URL**

GET /thumbnail

**Paramètres de requête**

| Nom | Description |
|---|---|
| ID | ID du document. |
| Taille | Largeur de la miniature |

{style="table-layout:auto"}

 

**Réponse**

Octets bruts de la miniature.

**Exemple :** `https://www.acme.com/api/thumbnail?id=123456`

### Charger un fichier - Partie 1 sur 2

Le chargement d’un fichier vers un fournisseur de services de stockage de documents est un processus en deux étapes qui nécessite deux points d’entrée API distincts. Workfront commence le processus de chargement en appelant /uploadInit. Ce point d’entrée renvoie un identifiant de document qui est ensuite transmis à /upload lors du chargement des octets du document. Selon le système de stockage de documents sous-jacent, il peut être nécessaire de créer un document vide et de mettre à jour le contenu du document ultérieurement.

Ajoutés à la version 1.1 de cette spécification, l’identifiant du document et l’identifiant de la version du document peuvent être utilisés pour extraire des informations supplémentaires de Workfront. Par exemple, si le système de gestion des documents souhaite obtenir des informations supplémentaires sur le document, le code d’implémentation du webhook pourrait utiliser l’identifiant du document pour récupérer ces informations à l’aide de l’API RESTful de Workfront. Selon une bonne pratique, ces informations peuvent provenir de champs de données personnalisées sur le document et sur la tâche, le problème ou le projet qu’il contient.

**URL**

POST /uploadInit

**Paramètres de requête**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId</td> 
   <td>L’identifiant du dossier parent, tel que référencé par le fournisseur du webhook.</td> 
  </tr> 
  <tr> 
   <td>filename</td> 
   <td>Nom du document</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Identifiant du document Workfront (ajouté dans la version 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId</td> 
   <td>Identifiant de la version du document Workfront (ajouté dans la version 1.1)</td> 
  </tr> 
 </tbody> 
</table>

 

**Réponse**

Métadonnées du fichier, telles que définies par le point d’entrée /metadata.

**Exemple :** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Réponse**

`[file_metadata]` comprend le nouvel identifiant du document utilisé par le fournisseur du document.

### Charger un fichier - Partie 2 sur 2

Charge les octets d’un document vers le fournisseur du webhook.

**URL**

PUT /upload

**Paramètres de requête**

| Nom | Description |
|---|---|
| ID | Identifiant du document qui vient d’être créé. |


 

**Corps de la requête**

Octets du contenu brut du document.

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

**Exemple :** `https://www.acme.com/api/upload?id=1234` *[octets de document inclus dans le flux de mise à jour]*

**Réponse**

```
{
"result":"success"
}
```

### Obtenir des informations sur le service

(Date de publication - à déterminer) Renvoie des informations sur le service, telles que ses caractéristiques et ses capacités. Workfront utilisera ces informations pour personnaliser l’interface d’utilisation de Workfront. Par exemple, si la mise en œuvre du webhook contient des actions personnalisées, le fichier JSON doit énumérer ces opérations dans le fichier JSON. Les utilisateurs et utilisatrices pourront alors invoquer ces actions à partir de Workfront.

**URL**

GET /serviceInfo

Paramètres de requête

Aucun. En outre, les appels à ce point d’entrée ne doivent pas nécessiter d’authentification.

**Réponse**

Fichier JSON contenant des informations sur ce service.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Type</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion</td> 
   <td>Chaîne</td> 
   <td>Version du webhook mise en œuvre par ce service. Il s’agit du numéro de version indiqué au début de la présente spécification.</td> 
  </tr> 
  <tr> 
   <td>version</td> 
   <td>Chaîne</td> 
   <td>Numéro de version interne de ce service. Ce numéro est déterminé par le fournisseur du service du webhook et n’est utilisé qu’à titre d’information.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher</td> 
   <td>Chaîne</td> 
   <td>Nom de l’entreprise qui fournit l’implémentation du webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Chaîne</td> 
   <td>Liste contenant les points d’entrée de l’API mis en œuvre par ce service. Ceci peut être utilisé pour s’assurer que l’interface d’utilisation dans Workfront reflète les capacités offertes par le fournisseur du webhook. Chaque élément de la liste doit inclure le nom du point d’entrée (tel que « search »).</td> 
  </tr> 
  <tr> 
   <td>customActions</td> 
   <td>Chaîne</td> 
   <td>  <p>Liste contenant les opérations personnalisées implémentées par ce webhook. Chaque élément de la liste comprend un nom et un nom d’affichage. Le nom d’affichage apparaît dans le menu déroulant « Actions sur le document » dans Workfront. En cliquant sur l’élément de la liste déroulante, l’action est déclenchée en appelant le point d’entrée /customAction du webhook.</p></td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** https://www.acme.com/api/serviceInfo

**Retours**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### Créer un dossier

(Ajouté dans la version 1.2) Crée un dossier dans un répertoire donné.
URL

POST /createFolder

**Paramètres de requête**

| Nom | Description |
|---|---|
| parentId | Identifiant du dossier dans lequel le dossier doit être créé |
| name | Nom du nouveau dossier |

{style="table-layout:auto"}

 

**Réponse**

Métadonnées du dossier nouvellement créé, telles que définies par le point d’entrée /metadata.

**Exemple :** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

returns

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

(Date de publication : à déterminer) Supprime un document ou un dossier avec l’identifiant donné dans le système externe. Supprimer un dossier entraîne également la suppression de son contenu.

URL

PUT /delete

**Paramètres de requête**

| Nom | Description |
|---|---|
| documentId | Identifiant du document à supprimer |
| folderId | Identifiant du dossier à supprimer |

{style="table-layout:auto"}

Réponse : chaîne JSON indiquant le succès ou l’échec, comme spécifié dans la section sur la gestion des erreurs ci-dessous.

**Exemple :** PUT https://www.acme.com/api/delete id=1234

returns

```
{
"status": "success" 
}
```

returns

```
{
"status": "failure", "error": "File not found"
}
```


### Renommer un document ou un dossier

(Date de publication : à déterminer) Renomme un document ou un dossier avec l’identifiant donné dans le système externe.

URL

PUT /rename

**Paramètres de requête**

| Nom | Description |
|---|---|
| ID | Identifiant du document ou du dossier à renommer |
| Nom | Nouveau nom du document ou du dossier |

{style="table-layout:auto"}

 

Réponse

Chaîne JSON indiquant le succès ou l’échec, tel que spécifié dans la section Gestion des erreurs ci-dessous.

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

### Effectuer une action personnalisée

(Date de publication - à déterminer) Ce point d’entrée permettra à un utilisateur ou une utilisatrice de Workfront (ou peut-être à un événement de workflow automatisé) d’effectuer une action dans le système externe. Le point d’entrée /customAction accepte un paramètre « nom », qui permet au fournisseur du webhook de mettre en œuvre plusieurs opérations personnalisées.

Le fournisseur du webhook enregistre les actions personnalisées avec Workfront en incluant les actions dans la réponse /serviceInfo dans customActions. Workfront charge cette liste lors de la configuration ou de l’actualisation du fournisseur du webhook dans Configuration > Documents > Intégrations personnalisées.\
![Exécuter une action personnalisée](assets/mceclip0-350x262.png)

Les utilisateurs et utilisatrices peuvent déclencher l’action personnalisée en sélectionnant la section dans « Actions sur le document ».\
![ Déclencher des actions personnalisées ](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**Paramètres de requête**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Nom</th>
   <th>Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>Identifiant spécifiant le type d’action à effectuer. Cette valeur correspond à l’une des valeurs customAction répertoriées par le point d’entrée /serviceInfo.</p></td>
  </tr>
  <tr>
   <td>documentId</td>
   <td>Identifiant du document Workfront pour lequel l’action est effectuée.</td>
  </tr>
  <tr>
   <td>documentVersionId</td>
   <td>Identifiant de la version du document Workfront pour lequel l’action est effectuée.</td>
  </tr>
 </tbody>
</table>

 

**Réponse**

Chaîne JSON indiquant le succès ou l’échec, tel que spécifié dans la section Gestion des erreurs ci-dessous. En cas d’échec (c’est-à-dire si le statut = «échec »), Workfront affichera le message d’erreur envoyé à l’utilisateur ou l’utilisatrice.

**Exemple :** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

response

```
{
"status": "success" 
}
```


## Gestion des erreurs

Des problèmes peuvent survenir lors du traitement des requêtes API. Cela doit être géré de manière cohérente dans tous les points d’entrée de l’API. Lorsqu’une erreur se produit, le fournisseur du webhook effectue les opérations suivantes :

* Inclure un code d’erreur dans l’en-tête de la réponse. Les codes d’erreur sont les suivants :

   * 403 - Interdit. Indique que les jetons de requête sont manquants ou non valides ou que les informations d’identification associées aux jetons n’ont pas accès à la ressource spécifiée. Pour les fournisseurs de webhooks basés sur OAuth, Workfront tentera de récupérer de nouveaux jetons d’accès.
   * 404 - Introuvable. Indique que le fichier ou le dossier spécifié n’existe pas.
   * 500 - Erreur interne du serveur. Tout autre type d’erreur.

* Décrivez l’erreur dans le corps de la réponse en suivant le format suivant :


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Tests

Pour vérifier que la mise en œuvre du webhook de votre document fonctionne correctement, effectuez les tests suivants : Il s’agit de tests manuels qui passent par l’interface web de Workfront et qui touchent indirectement les points d’entrée de la mise en œuvre de votre webhook.

### Conditions préalables

Pour effectuer ces tests, vous aurez besoin des éléments suivants :

* Un compte Workfront avec la gestion avancée des documents (ADM) activée.
* Un utilisateur ou une utilisatrice Workfront pour ce compte disposant des droits d’administration système.
* Instance de Document Webhook dont les points d’entrée HTTP sont accessibles à Workfront.

Ces tests supposent également que vous avez déjà enregistré votre instance Document Webhook dans Workfront sous Configuration > Documents > Intégrations personnalisées.

### Test 1 : allouer le service Document Webhook aux utilisateurs et aux utilisatrices

Teste l’URL d’authentification et l’URL du point d’entrée du jeton pour les fournisseurs de webhooks basés sur OAuth.

1. Dans Workfront, accédez à la page principale des documents en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Cliquez sur le menu déroulant « Ajouter des documents » et sélectionnez votre service Document Webhook sous « Ajouter un service ».
1. (Services OAuth uniquement) Après avoir effectué l’étape précédente, la page d’authentification OAuth2 de votre service s’affiche dans une fenêtre contextuelle. (Remarque : il se peut que vous soyez invité à vous connecter d&#39;abord à votre service.) Sur la page d’authentification, accordez à Workfront l’accès au compte de l’utilisateur en cliquant sur le bouton Approbation ou Autoriser .
1. Vérifiez que votre service a été ajouté à la liste déroulante « Ajouter des documents ». Si en premier lieu vous ne le voyez pas, essayez d’actualiser votre navigateur.

### Test 2 : lier un document dans Workfront teste les points d’entrée suivants : /files, /metadata.

1. Dans Workfront, accédez à la page principale des documents en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Sélectionnez votre service Document Webhook dans Ajouter des documents.
1. Dans la fenêtre modale, naviguez dans la structure des dossiers.
1. Assurez-vous de naviguer correctement dans la structure des dossiers.
1. Sélectionner et lier un document dans Workfront

### Test 3 : accéder à un document dans le système de gestion de contenu

Teste les points d’entrée suivants : /metadata (en particulier le viewLink).

1. Lier un document dans Workfront
1. Sélectionnez le document et cliquez sur le lien Ouvrir.
1. Vérifiez que le document s’ouvre dans un nouvel onglet.

### Test 4 : accéder à un document dans le système de gestion de contenu (avec connexion)

Teste les points d’entrée suivants : /metadata (en particulier le viewLink).

1. Vérifiez que votre connexion au système de gestion de contenu n’est pas effective.
1. Liez un document dans Workfront.
1. Sélectionnez le document et cliquez sur le lien Ouvrir.
1. Vérifiez que l’écran de connexion du système de gestion de contenu se charge dans un nouvel onglet.
1. Connectez-vous et vérifiez que cela vous dirige bien vers le document.

### Test 5 : télécharger le document à partir du système de gestion de contenu

Teste les points d’entrée suivants : /metadata (spécifiquement le downloadLink).

1. Liez un document dans Workfront.
1. Sélectionnez le document et cliquez sur le lien Télécharger.
1. Vérifiez que le téléchargement commence.

### Test 6 : rechercher du contenu

Teste les points d’entrée suivants : /search.

1. Dans Workfront, accédez à la page principale des documents en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Sélectionnez votre service Document Webhook dans Ajouter des documents.
1. Dans la fenêtre modale, effectuez une recherche.
1. Vérifiez que les résultats de la recherche sont corrects.

### Test 7 : envoyer un document de Workfront vers le système de gestion de contenu

Teste les points d’entrée suivants : /files, /uploadInit, /upload.

1. Dans Workfront, accédez à la page principale des documents en cliquant sur le lien Documents dans la barre de navigation supérieure.
1. Chargez un document dans Workfront à partir de votre ordinateur.
1. Accédez à la page des détails du document.
1. Dans le menu déroulant Actions du document, sélectionnez votre service Document Webhook dans Envoyer à...
1. Accédez au dossier de destination souhaité et cliquez sur le bouton Enregistrer.
1. Vérifiez que le document est chargé au bon endroit dans le système de gestion de contenu.

### Test 8 : afficher des miniatures dans Workfront

Teste les points d’entrée suivants : /thumbnail.

1. Liez un document dans Workfront.
1. Sélectionnez le document dans la liste.
1. Vérifiez que la vignette apparaît dans le panneau de droite.

### Test 9 : obtenir les octets de contenu

Teste les points d’entrée suivants : /download.

1. Liez un document dans Workfront.
1. Accédez à la page des détails du document.
1. Envoyez le document à Workfront en sélectionnant Actions du document > Envoyer à... > Workfront. Cela crée une nouvelle version du document dans Workfront.
1. Téléchargez le document à partir de Workfront en cliquant sur le lien Télécharger.

### Test 10 : actualiser le jeton d’accès (fournisseurs de webhooks basés sur OAuth2 uniquement)

Teste les points d’entrée suivants : URL du point d’entrée de jeton.

1. Mettre à disposition un service Document Webhook pour un utilisateur ou une utilisatrice
1. Annuler le jeton d’accès de l’utilisateur ou de l’utilisatrice soit 1) en attendant son expiration, soit 2) manuellement dans le système externe.
1. Actualisez le jeton d’accès dans Workfront. Vous pouvez le faire, par exemple, en liant un document dans Workfront. Vous savez que le jeton d’accès a été actualisé si vous avez été en mesure de naviguer jusqu’à un document et le lier.

>[!NOTE]
>
>Actuellement, la fonction « Envoyer à... » n’est pas disponible pour les documents liés. Elle sera ajoutée par l’équipe Workfront. Vous pouvez tester le point d’entrée /download en accédant manuellement au point d’entrée à l’aide d’un client REST, tel que Postman. Il est également possible de tester le point d’entrée /download en générant une épreuve numérique. Pour activer la relecture numérique, contactez l’équipe Workfront.

## Versions

* Version 1.0 (Date de publication : mai 2015)

   * Spécification initiale

* Version 1.1 (Date de publication : juin 2015)

   * Mise à jour de /uploadInit - Ajout de documentId et documentVersionId

* Version 1.2 (Date de publication : octobre 2015)

   * Ajout de /createFolder

