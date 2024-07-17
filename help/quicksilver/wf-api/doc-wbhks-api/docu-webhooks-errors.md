---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Gestion des erreurs de Document Webhooks
description: Gestion des erreurs de Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 9%

---

# Gestion des erreurs de Document Webhooks

Des problèmes peuvent survenir lors du traitement des demandes d’API. Cela doit être géré de manière cohérente sur tous les points de terminaison de l’API. Lorsqu’une erreur se produit, le fournisseur webhook doit inclure un code d’erreur dans l’en-tête de la réponse. Les codes d’erreur incluent :

* 403 - Interdit. Indique que les jetons de requête sont manquants ou non valides ou que les informations d’identification associées aux jetons n’ont pas accès à la ressource spécifiée. Pour les fournisseurs de webhook basés sur OAuth, Adobe Workfront tente de récupérer les nouveaux jetons d’accès.

* 404 - Introuvable. Indique que le fichier ou le dossier spécifié n’existe pas.

* 500 - Erreur interne du serveur. Tout autre type d&#39;erreur.

* Description de l’erreur dans le corps de la réponse selon le format suivant :

  ```
  {status: "error"
   error: "Sample error message"}
  ```
