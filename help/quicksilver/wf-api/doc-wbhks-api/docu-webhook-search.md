---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Rechercher via Document Webhooks
description: Rechercher via Document Webhooks
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 11%

---

# Rechercher via Document Webhooks

Renvoie les métadonnées des fichiers et dossiers renvoyés à partir d’une recherche. Cela peut être mis en oeuvre sous la forme d’une recherche de texte intégral ou d’une requête de base de données classique. Adobe Workfront appelle le point de terminaison /search lorsque l’utilisateur effectue une recherche à partir du navigateur de fichiers externe.

## URL

GET /search

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
   <td>query</td> 
   <td>Terme ou expression à rechercher.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(facultatif) ID de dossier à partir duquel la recherche s’est exécutée. Remarque : Il s’agit d’un espace réservé pour une future fonctionnalité de Workfront. Actuellement, workfront ne transmet pas ce paramètre. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>Nombre maximal d’éléments à renvoyer. Utilisé pour la pagination.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> Décalage de page, utilisé conjointement avec "max".</td> 
  </tr> 
 </tbody> 
</table>

 

## Réponse

JSON contenant une liste de métadonnées pour les fichiers et les dossiers correspondant à la requête. Ce qui constitue une &quot;correspondance&quot; est déterminé par le fournisseur webhook. Idéalement, il doit effectuer une recherche de texte intégral. Une recherche basée sur un nom de fichier fonctionne également.

**Exemple :**

Exemple : `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
