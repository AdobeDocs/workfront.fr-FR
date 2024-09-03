---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtenir du contenu de document via Webhooks
description: Renvoie les octets bruts d’un document
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 100%

---

# Obtenir du contenu de document via Webhooks

Renvoie les octets bruts d’un document

## URL

GET /download

## Paramètres de requête

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>ID</p> </td> 
   <td>Identifiant du document.</td> 
  </tr> 
 </tbody> 
</table>

## Réponse

Octets bruts du document.

**Exemple** : - `https://www.acme.com/api/download?id=123456`
