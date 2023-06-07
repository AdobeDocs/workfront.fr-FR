---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtention de contenu de document via Webhooks
description: Renvoie les octets bruts d’un document
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 9%

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

**Exemple**:  `https://www.acme.com/api/download?id=123456`
