---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Répertorie les métadonnées des fichiers ou des dossiers
description: Répertorie les métadonnées des fichiers ou des dossiers
author: Becky
feature: Workfront API
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 5%

---


# Obtenir la liste des éléments du contenu du dossier

Répertorie les métadonnées des fichiers et des dossiers d’un dossier donné.

**URL**

GET /files

## Paramètres de requête

| Nom  | Description |
|---|---|
| parentId  | ID du dossier. Pour obtenir les métadonnées du répertoire racine, utilisez la valeur &quot;/&quot;. |
| max  | Nombre maximal d’éléments à renvoyer. Utilisé pour la pagination. |
| offset  |  Décalage de page, utilisé conjointement avec &quot;max&quot;. |


## réponse

JSON contenant une liste de fichiers et de dossiers. Les métadonnées de chaque élément sont les mêmes que celles renvoyées par le point de terminaison /metadata .

**Exemple :** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ”,
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ”,
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
