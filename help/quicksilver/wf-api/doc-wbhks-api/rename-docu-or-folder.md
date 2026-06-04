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
TQID: https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 81
ht-degree: 100%

---

# Renommer un document ou un dossier (pas encore implémenté)

Renomme un document ou un dossier avec l’ID donné dans le système externe.

**URL**

PUT /rename

## Paramètres de requête

| Nom  | Description |
|---|---|
| ID | Identifiant du document ou du dossier à renommer |
| Nom  | Nouveau nom du document ou du dossier |


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
