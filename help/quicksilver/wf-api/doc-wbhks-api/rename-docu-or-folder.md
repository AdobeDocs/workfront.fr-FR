---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Renommer un document ou un dossier (pas encore implémenté)
description: Renommer un document ou un dossier
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 100%

---


# Renommer un document ou un dossier (pas encore implémenté)

Renomme un document ou un dossier avec l’ID donné dans le système externe.

**URL**

PUT /rename

## Paramètres de requête

| Nom | Description |
|---|---|
| ID | Identifiant du document ou du dossier à renommer |
| Nom | Nouveau nom du document ou du dossier |


## Réponse

Chaîne JSON indiquant le succès ou l’échec, tel que spécifié dans la section Gestion des erreurs ci-dessous.

**Exemple :** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

returns

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
