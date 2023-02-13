---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Création d’un dossier avec des webhooks de document
description: Création d’un dossier avec des webhooks de document
author: John
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 1b11a4c5f0fdf1987e9f02f7aa06ec6ec36426d3
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 7%

---


# Création d’un dossier avec des webhooks de document

Crée un dossier dans un répertoire donné.

## URL

POST /createFolder

## Paramètres de requête

| **Nom** | **Description** |
|---|---|
| parentId  | Identifiant du dossier dans lequel le dossier doit être créé. |
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
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
