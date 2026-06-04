---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Supprimer un document ou un dossier
description: Supprimer un document ou un dossier
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
TQID: https://experienceleague.adobe.com/7-f8Z3qQQ2z7ZHHfSrGgJqIQCKdeqEoL96XlfCGzYSo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 75
ht-degree: 100%

---

# Supprimer un document ou un dossier (pas encore implémenté)

Supprime un document ou un dossier avec l’ID donné dans le système externe. La suppression d’un dossier supprime également le contenu du dossier.

## URL

PUT /delete

## Paramètres de requête

| Nom  | Description |
|---|---|
| documentId  | Identifiant du document à supprimer |
| folderId  |  Identifiant du dossier à supprimer |



## Réponse

Chaîne JSON indiquant le succès ou l’échec, tel que spécifié dans la section Gestion des erreurs ci-dessous.

### Exemple

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
