---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Chargement de fichiers via les webhooks de document
description: Chargement de fichiers via les webhooks de document
author: Becky
feature: Workfront API
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%

---


# Chargement de fichiers via les webhooks de document

Le téléchargement d’un fichier vers un fournisseur de stockage de documents est un processus en deux étapes qui nécessite deux points de terminaison d’API distincts. Adobe Workfront commence le processus de chargement en appelant /uploadInit . Ce point de terminaison renvoie un ID de document qui est ensuite transmis à /upload lors du téléchargement des octets de document. Selon le système de stockage de documents sous-jacent, il peut être nécessaire de créer un document de longueur zéro, puis de mettre à jour le contenu du document ultérieurement.

Ajouté à la version 1.1 de cette spécification, l’ID de document et l’ID de version de document peuvent être utilisés pour récupérer des informations supplémentaires auprès de Workfront.

**Exemple :** Si le système Document Management souhaite obtenir des informations supplémentaires sur le document, le code de mise en oeuvre webhook peut utiliser l’ID de document pour récupérer ces informations à l’aide de l’API RESTful de Workfront. En règle générale, ces informations peuvent provenir de champs de données personnalisés sur le document et contiennent une tâche, un problème ou un projet.

## Méthode du POST

**URL**

POST /uploadInit

### Paramètres de requête

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
   <td>L’ID de version de document Workfront (ajouté dans la version 1.1) </td> 
  </tr> 
 </tbody> 
</table>

## réponse

Métadonnées du fichier, telles que définies par le point de terminaison /metadata . Cela inclut l’ID de document utilisé par le fournisseur.

**Exemple:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Méthode du PUT

Télécharge les octets d’un document vers le fournisseur webhook.

**URL**

PUT /upload

## Paramètres de requête

| Nom  | Description |
|---|---|
| id  |  ID du document, qui vient d’être créé. |


**Corps de requête**

octets de contenu brut du document.

**Réponse**

```
{
result: “success”
}
```

ou

```
{
result: “fail”
}
```

**Exemple**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

response

```
{
result:"success"
}
```
