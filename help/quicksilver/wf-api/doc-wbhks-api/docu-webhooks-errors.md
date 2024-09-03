---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Gestion des erreurs des webhooks de document
description: Gestion des erreurs des webhooks de document
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 100%

---

# Gestion des erreurs des webhooks de document

Des problèmes peuvent survenir lors du traitement des requêtes d’API. Des solutions cohérentes doivent être proposées pour tous les points d’entrée d’API. Lorsqu’une erreur se produit, le fournisseur de webhooks doit inclure un code d’erreur dans l’en-tête de la réponse. Les codes d’erreur sont les suivants :

* 403 - Interdit. Indique que les jetons de requête sont manquants ou non valides ou que les informations d’identification associées aux jetons n’ont pas accès à la ressource spécifiée. Pour les fournisseurs de webhooks basés sur OAuth, Adobe Workfront tente de récupérer de nouveaux jetons d’accès.

* 404 - Introuvable. Indique que le fichier ou le dossier spécifié n’existe pas.

* 500 - Erreur interne du serveur. Tout autre type d’erreur.

* Description de l’erreur dans le corps de la réponse selon le format suivant :

  ```
  {status: "error"
   error: "Sample error message"}
  ```
