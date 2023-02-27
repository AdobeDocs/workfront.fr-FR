---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtention de contenu de document via Webhooks
description: Renvoie les octets bruts d’un document
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '53'
ht-degree: 7%

---

# Obtention de contenu de document via Webhooks

Renvoie les octets bruts d’un document

## URL

GET /download

## Paramètres de requête

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> ID du document.</td> 
  </tr> 
 </tbody> 
</table>

## réponse

octets bruts du document.

**Exemple :**:  [https://www.acme.com/api/download?id=123456](https://www.acme.com/api/download?id=123456)
