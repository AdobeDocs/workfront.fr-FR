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
TQID: https://experienceleague.adobe.com/-LE1gxQ9aViRNuN0sI14HlZaIcLc6Mmm8XmS1zaRCFQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 55
ht-degree: 100%

---

# Obtenir une miniature pour un document

Renvoie les octets bruts de la miniature pour un document.

**URL**

GET /thumbnail

## Paramètres de requête

| Nom  | Description |
|---|---|
| ID  | ID du document. |
| Taille  |  La largeur de la vignette. |


## Réponse

Octets bruts de la miniature.

**Exemple :** https://www.acme.com/api/thumbnail?id=123456
