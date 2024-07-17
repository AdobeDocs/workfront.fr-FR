---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtenir une vignette pour un document
description: Obtenir une vignette pour un document
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 42%

---


# Obtenir une vignette pour un document

Renvoie les octets de miniature bruts d’un document.

**URL**

GET /thumbnail

## Paramètres de requête

| Nom  | Description |
|---|---|
| id  | ID du document. |
| size  |  Largeur de la miniature. |


## Réponse

Octets de miniature bruts.

**Exemple :**: https://www.acme.com/api/thumbnail?id=123456
