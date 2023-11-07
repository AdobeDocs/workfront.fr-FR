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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 6%

---


# Suppression d’un document ou d’un dossier (non encore implémenté)

Supprime un document ou un dossier avec l’ID donné dans le système externe. La suppression d’un dossier supprime également le contenu du dossier.

## URL

PUT /delete

## Paramètres de requête

| Nom  | Description |
|---|---|
| documentId  | ID du document à supprimer |
| folderId  |  ID de dossier à supprimer |



## réponse

Chaîne JSON indiquant la réussite ou l’échec, comme indiqué dans la section Gestion des erreurs ci-dessous.

### Exemple

PUT https://www.example.com/api/deleteid=1234
* renvoie `status: "success"`

* renvoie `status: "failure", error: "File not found"`
