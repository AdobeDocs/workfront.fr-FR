---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Présentation des webhooks
description: Présentation des webhooks
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: eb738fa8cadaafb0332c5c78a3816d5c346c33b2
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# Présentation des webhooks

Les webhooks de document Adobe Workfront définissent un ensemble de points de terminaison d’API par le biais desquels Workfront effectue des appels d’API autorisés à un fournisseur de document externe. Cela permet à tous les utilisateurs de créer un module externe middleware pour n’importe quel fournisseur de stockage de documents.

![](assets/mceclip0-350x262.png)

L’expérience utilisateur des intégrations basées sur webhook est similaire à celle des intégrations de documents existantes, telles que Google Drive, Box et Dropbox. Par exemple, un utilisateur Workfront peut effectuer les actions suivantes :

* Parcourir la structure de dossiers du fournisseur de documents externe
* Recherche de fichiers
* Lier des fichiers à Workfront
* Chargement de fichiers dans le fournisseur de documents externe
* Affichage d’une miniature pour le document

**Implémentation de référence**

Pour accélérer le développement d’une nouvelle implémentation de webhooks, Workfront fournit des exemples d’implémentation de référence. Ces exemples se trouvent à l’adresse [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Les exemples sont basés sur Java et permettent à Workfront de connecter des documents sur un système de fichiers réseau. 

>[!NOTE]
>
>Les ressources sur GitHub ne sont que des exemples et ne peuvent pas exécuter une mise en oeuvre.

## Versions

* Version 1.0 (Date de publication - mai 2015) : spécification initiale

* Version 1.1 (Date de publication - juin 2015). Mise à jour de /uploadInit : ajout de documentId et documentVersionId

* Version 1.2 (Date de publication - octobre 2015) : ajout de /createFolder

* Versions à venir (Date de publication - à déterminer) :

   * Ajout de /delete
   * Ajout de /rename
   * Ajout de /serviceInfo
   * Ajout de /customAction
   * Ajouter pagination et parentId à /search
