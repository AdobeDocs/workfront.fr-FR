---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Rechercher via Document Webhooks
description: Rechercher via Document Webhooks
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
TQID: https://experienceleague.adobe.com/flRrmTOPVSGP83tVYfKG9AZOT7CNZN4IeWZNsVwcOO4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 93%

---

# Rechercher via Document Webhooks

Renvoie les métadonnées des fichiers et dossiers renvoyés à partir d’une recherche. Cela peut être mis en œuvre sous la forme d’une recherche de texte intégral ou d’une requête de base de données classique. Adobe Workfront appelle le point d’entrée /search lorsque l’utilisateur ou l’utilisatrice effectue une recherche à partir du navigateur de fichier externe.

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
   <td>Expression ou terme de recherche.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(facultatif) Identifiant du dossier à partir duquel la recherche a été exécutée. Remarque : il s’agit d’un espace réservé pour une fonctionnalité future dans Workfront. Actuellement, Workfront ne transmet pas ce paramètre. </p> </td> 
  </tr> 
  <tr> 
   <td>max</td> 
   <td>Nombre maximal d’éléments à renvoyer. Utilisé pour la pagination.</td> 
  </tr> 
  <tr> 
   <td>offset</td> 
   <td> Décalage de page, utilisé conjointement avec « max ».</td> 
  </tr> 
 </tbody> 
</table>

 

## Réponse

JSON contenant une liste de métadonnées pour les fichiers et les dossiers correspondant à la requête. Le fournisseur de webhook détermine ce qui constitue une « correspondance ». Idéalement, il doit effectuer une recherche de texte intégral. Une recherche basée sur un nom de fichier fonctionne également.

**Exemple :**

Exemple : `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
