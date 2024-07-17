---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Créer un dossier avec Document Webhooks
description: Créer un dossier avec Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 33%

---


# Créer un dossier avec Document Webhooks

Crée un dossier dans un répertoire donné.

## URL

POST /createFolder

## Paramètres de requête

| **Nom** | **Description** |
|---|---|
| parentId  | ID de dossier dans lequel le dossier doit être créé |
| name  | Nom du nouveau dossier |




**Réponse**

Métadonnées du dossier nouvellement créé, telles que définies par le point de terminaison /metadata .

## Exemple

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

renvoie

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"",
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
