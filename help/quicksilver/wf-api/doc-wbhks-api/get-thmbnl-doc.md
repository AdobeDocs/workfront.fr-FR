---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtention d’une miniature pour un document
description: Obtention d’une miniature pour un document
author: Becky
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 7%

---


# Obtention d’une miniature pour un document

Renvoie les octets de miniature bruts d’un document.

**URL**

GET /thumbnail

## Paramètres de requête

| Nom  | Description |
|---|---|
| id  | ID du document. |
| size  |  Largeur de la miniature. |


## réponse

Octets de miniature bruts.

**Exemple :**: https://www.acme.com/api/thumbnail?id=123456
