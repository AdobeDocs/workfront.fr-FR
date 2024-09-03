---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Téléchargement de fichiers via Document Webhooks
description: Téléchargement de fichiers via Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 100%

---


# Téléchargement de fichiers via Document Webhooks

Le chargement d’un fichier vers un fournisseur de services de stockage de documents est un processus en deux étapes qui nécessite deux points d’entrée API distincts. Adobe Workfront commence le processus de chargement en appelant /uploadInit. Ce point d’entrée renvoie un identifiant de document qui est ensuite transmis à /upload lors du chargement des octets du document. Selon le système de stockage de documents sous-jacent, il peut être nécessaire de créer un document vide et de mettre à jour le contenu du document ultérieurement.

Ajoutés à la version 1.1 de cette spécification, l’identifiant du document et l’identifiant de la version du document peuvent être utilisés pour extraire des informations supplémentaires de Workfront.

**Exemple :** si le système de gestion des documents souhaite obtenir des informations supplémentaires sur le document, le code d’implémentation du webhook pourrait utiliser l’identifiant du document pour récupérer ces informations à l’aide de l’API RESTful de Workfront. Selon une bonne pratique, ces informations peuvent provenir de champs de données personnalisées sur le document et sur la tâche, le problème ou le projet qu’il contient.

## Méthode POST

**URL**

POST /uploadInit

### Paramètres de requête

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

## Réponse

Métadonnées du fichier, telles que définies par le point d’entrée /metadata. Cela inclut l’ID de document utilisé par le fournisseur.

**Exemple :**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## Méthode PUT

Charge les octets d’un document vers le fournisseur du webhook.

**URL**

PUT /upload

## Paramètres de requête

| Nom | Description |
|---|---|
| ID | Identifiant du document qui vient d’être créé. |


**Corps de la requête**

Octets du contenu brut du document.

**Réponse**

```
{
result: "success"
}
```

ou

```
{
result: "fail"
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
