---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Renommer un document ou un dossier (non encore implémenté)
description: Renommer un document ou un dossier
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 6%

---


# Renommer un document ou un dossier (non encore implémenté)

Renomme un document ou un dossier avec l’ID donné dans le système externe.

**URL**

PUT /rename

## Paramètres de requête

| Nom  | Description |
|---|---|
| id | ID du document ou du dossier à renommer |
| name  | Le nouveau nom du document ou du dossier |


## réponse

Chaîne JSON indiquant la réussite ou l’échec, comme indiqué dans la section Gestion des erreurs ci-dessous.

**Exemple :** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

renvoie

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
