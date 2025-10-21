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
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '75'
ht-degree: 89%

---


# Supprimer un document ou un dossier (pas encore implémenté)

Supprime un document ou un dossier avec l’ID donné dans le système externe. La suppression d’un dossier supprime également le contenu du dossier.

## URL

PUT /delete

## Paramètres de requête

| Nom | Description |
|---|---|
| documentId | Identifiant du document à supprimer |
| folderId | Identifiant du dossier à supprimer |



## Réponse

Chaîne JSON indiquant le succès ou l’échec, tel que spécifié dans la section Gestion des erreurs ci-dessous.

### Exemple

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
