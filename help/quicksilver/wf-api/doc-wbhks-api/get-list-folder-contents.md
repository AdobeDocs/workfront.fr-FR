---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Répertorier les métadonnées des fichiers ou des dossiers
description: Répertorier les métadonnées des fichiers ou des dossiers
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 100%

---


# Obtenir la liste des éléments du contenu d’un dossier

Répertorier les métadonnées des fichiers et des dossiers pour un dossier donné.

**URL**

GET /files

## Paramètres de requête

| Nom | Description |
|---|---|
| parentId | L’identifiant du dossier. Pour obtenir les métadonnées du répertoire racine, utilisez la valeur « / ». |
| Max | Nombre maximal d’éléments à renvoyer. Utilisé pour la pagination. |
| Décalage | Décalage de page, utilisé conjointement avec « max ». |


## Réponse

Le fichier JSON contenant une liste de fichiers et de dossiers. Les métadonnées de chaque élément sont les mêmes que celles renvoyées par le point d’entrée /metadata.

**Exemple :** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
