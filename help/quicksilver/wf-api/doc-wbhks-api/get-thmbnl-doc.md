---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtenir une miniature pour un document
description: Obtenir une miniature pour un document
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 100%

---


# Obtenir une miniature pour un document

Renvoie les octets bruts de la miniature pour un document.

**URL**

GET /thumbnail

## Paramètres de requête

| Nom | Description |
|---|---|
| ID | ID du document. |
| Taille | La largeur de la vignette. |


## Réponse

Octets bruts de la miniature.

**Exemple :** https://www.acme.com/api/thumbnail?id=123456
