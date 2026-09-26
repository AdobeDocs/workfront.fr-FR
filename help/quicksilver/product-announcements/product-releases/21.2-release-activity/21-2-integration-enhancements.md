---
content-type: release-notes
keywords: notes,trimestriel,mise à jour,version
navigation-topic: 2021-2-release-activity
title: Améliorations apportées aux intégrations (version 21.2)
description: Cette page décrit toutes les améliorations apportées à l’intégration avec la version 21.2 de l’environnement prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir Vue d’ensemble de la version 21.2.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 82279305-d758-4ab3-b77c-8e65a3d19a9f
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 100%
---
# Améliorations apportées aux intégrations (version 21.2)

Cette page décrit toutes les améliorations apportées à l’intégration avec la version 21.2 de l’environnement prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir [Vue d’ensemble de la version 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Présentation d’Adobe Workfront pour XD

Nous sommes heureux d’annoncer le lancement de notre nouveau plug-in : Adobe Workfront pour XD. Ce plug-in vous permet d’accéder aux détails des éléments de travail, de collaborer avec vos collègues dans la zone des mises à jour et de soumettre des épreuves pour examen, le tout sans quitter XD. Rendez-vous sur le marketplace Adobe XD pour télécharger le plug-in dès aujourd’hui.

Pour en savoir plus sur ce que vous pouvez faire avec Adobe Workfront pour XD, voir [Gérer l’utilisation du module externe Adobe Workfront pour les applications Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-manage-work-toc.md).


## Rechercher des dossiers dans les intégrations de documents

Pour faciliter la navigation dans vos intégrations de documents, nous avons rendu possible la recherche de dossiers. Désormais, lorsque vous saisissez un terme dans la barre de recherche, Workfront renvoie les documents, dossiers et sous-dossiers dont le nom contient le terme de recherche.

Auparavant, les sous-dossiers ne pouvaient être localisés qu’en ouvrant les dossiers parent.

Pour plus d’informations, voir [Lier des documents à partir d’applications externes](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Amélioration de la sécurité lors du chargement de fichiers vers Google Drive

L’intégration de Google Drive prend désormais en charge les nouveaux protocoles de sécurité de Google.

Lors de la liaison, du chargement ou de la création de fichiers sur Google Drive à partir de la section Documents d’un objet Adobe Workfront, Workfront accède désormais à vos fichiers Google par le biais du sélecteur de fichiers Google. Cela limite l’accès et la visibilité de Workfront aux seuls fichiers Google que vous liez à Workfront.

Auparavant, l’accès aux fichiers s’effectuait par le biais d’une boîte de dialogue de fichier basée dans Workfront.

