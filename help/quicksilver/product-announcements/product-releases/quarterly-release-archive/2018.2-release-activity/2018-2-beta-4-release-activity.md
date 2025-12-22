---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de la version 2018.2 Beta 4
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation de la version 2018.2 Beta 4. La fonctionnalité sera disponible dans l’environnement de prévisualisation le 17 mai 2018. Elles seront disponibles dans l’environnement de production en juillet 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 99%

---

# Activité de la version 2018.2 Beta 4

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation de la version 2018.2 Beta 4.La fonctionnalité sera disponible dans l’environnement de prévisualisation le 17 mai 2018. Elles seront disponibles dans l’environnement de production en juillet 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.2, voir [Vue d’ensemble de l’activité Version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La version 2018.2 Beta 4 contient les améliorations apportées aux administrateurs et administratrices de Workfront, ainsi qu’aux autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices**

* [Paramètres du système : informations de session dans les pages externes](#system-setting-session-information-in-external-pages)

**Pour tous les utilisateurs et utilisatrices**

* [Améliorations de la limite du travail en cours (WIP) dans le tableau Kanban](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [Interface améliorée pour la configuration des statuts d’une équipe Agile](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [Mise à jour de la liste de travail (panneau de gauche) dans la zone d’accueil](#updated-work-list-left-panel-in-the-home-area)
* [Nouvelle visionneuse de relecture de bureau pour la relecture de contenu interactif (Rich Media)](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content)
* [Exporter la vue Utilisateur ou utilisatrice dans le planificateur de ressources](#export-the-user-view-in-the-resource-planner)
* [Prise en charge de Google Team Drives](#support-for-google-team-drives)
* [Nouvelle limite d’export pour le graphique de Gantt](#new-export-limit-for-the-gantt-chart)
* [L’option Coller depuis le presse-papiers est désormais grisée lors de l’utilisation d’Internet Explorer ou de Safari](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari).
* Nouvel environnement Beta pour Android et nouvelles fonctionnalités[](#new-beta-environment-for-android-along-with-new-features)
* [Exemples de filtres pour les messages d’abonnements aux événements](#examples-of-filters-for-event-subscriptions-messages)

## Améliorations de la limite du travail en cours (WIP) dans le tableau Kanban {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### Configurer les limites du travail en cours (WIP) pour chaque colonne du tableau Kanban

Vous pouvez désormais configurer les limites du travail en cours (WIP) pour chaque colonne du tableau Kanban. 

Avant cette modification, vous ne pouviez configurer qu’une seule limite WIP qui s’appliquait à toutes les colonnes du tableau Kanban. 

Pour plus d’informations, voir la section [Configurer la limite du travail en cours (WIP)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) dans l’article [Configurer Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

### Mettre à jour la limite du travail en cours (WIP) directement depuis le tableau Kanban

Désormais, les personnes membres de l’équipe disposant de droits de modification pour l’équipe peuvent mettre à jour la limite WIP directement depuis le tableau Kanban.

Avant cette modification, vous ne pouviez mettre à jour la limite WIP qu’à partir de la zone Paramètres de l’équipe.

Pour plus d’informations, voir dans l’article .

## Interface améliorée pour la configuration des statuts d’une équipe Agile {#improved-interface-for-configuring-statuses-for-an-agile-team}

L&#39;interface de configuration des statuts pour une équipe Agile a été mise à jour avec les améliorations suivantes :

* Nouvel aspect
* Réorganiser les colonnes de statut via glisser-déposer

Pour plus d’informations, voir les articles suivants :

* [Configurer Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [Configurer Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Mise à jour de la liste de travail (panneau de gauche) dans la zone d’accueil {#updated-work-list-left-panel-in-the-home-area}

La liste de travail de la zone d’accueil contient les améliorations suivantes :

* Les éléments non lus sont désormais mis en évidence par des caractères gras et un point bleu.

  Les éléments consultés en dehors de la zone d’accueil sont toujours affichés comme non lus dans la zone d’accueil.

  Pour plus d’informations, voir [Afficher les éléments de la liste de travail dans la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Les problèmes sont désormais distingués par une icône qui s’affiche à côté.
* Les approbations sont désormais distinguées par type d’approbation, ce dernier étant affiché. Les types d’approbation possibles sont Tâche, Projet, Problème, Accès, Document, Feuille de temps et Épreuve.

  Avant cette modification, les approbations se distinguaient uniquement par le mot « Approbation ».

* Les éléments se distinguent désormais par le fait qu’ils sont ou non prêts à démarrer. Les options possibles sont Prêt à démarrer, Non prêt ou En train de travailler sur.

  Cette information n’apparaît pas pour les approbations, car celles-ci sont toujours prêtes à démarrer.

* Une icône de document s’affiche sous le nom de l’élément chaque fois qu’un document est joint à l’élément.
* Vous pouvez désormais réduire et développer les groupes dans la liste de travail afin de mieux contrôler les informations visibles. Les regroupements sont les suivants : Retard, Projets, Dates et Terminé.

  Par défaut, la section Cette semaine est développée et tous les autres regroupements sont réduits.

* Choisissez de trier les éléments par date d’achèvement prévue ou par date d’engagement.
* Le nombre d’éléments dans chaque regroupement est désormais affiché entre parenthèses en regard du titre du regroupement.

  Ce nombre n’est pas disponible pour le regroupement Terminé.

  Pour plus d’informations, voir [Afficher les éléments de la liste de travail dans la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Redimensionner la liste de travail par glisser-déposer. Vous pouvez redimensionner la liste de travail pour qu’elle occupe jusqu’à la moitié de l’écran. La taille que vous avez définie est conservée la prochaine fois que vous accédez à Accueil.

  Avant cette modification, la taille de la liste de travail ne pouvait pas être modifiée.

* Pour les demandes, l’avatar de la personne qui a fait la demande est maintenant affiché, avec le texte « [Nom_approbateur ou approbatrice] souhaiterait votre approbation ».
* Lors de la création d’une nouvelle tâche personnelle, le bouton « À faire » est désormais intitulé « Personnel ».

  Pour plus d’informations, voir [Créer des éléments de travail à partir de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) dans l’article [Créer des éléments de travail à partir de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Les éléments en retard ne sont indiqués comme tels qu’une heure après la date d’achèvement prévue.

Pour plus d’informations sur la zone Accueil, voir [Utiliser la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nouvelle visionneuse de relecture de bureau pour la relecture de contenus interactifs (médias riches) {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

La nouvelle visionneuse de relecture de bureau vous permet de relire des contenus interactifs. Contrairement à la visionneuse de relecture héritée existante et à la nouvelle visionneuse de relecture qui s’exécutent dans le navigateur, la visionneuse de relecture de bureau est une application qui s’exécute sur votre poste de travail.

Avant la nouvelle visionneuse de relecture de bureau, vous ne pouviez relire le contenu interactif que dans la visionneuse de relecture héritée. 

La visionneuse de relecture de bureau comprend les améliorations suivantes par rapport à la visionneuse de relecture héritée pour la relecture de contenus interactifs :

* Réviser les sites (HTTP) non sécurisés

  La visionneuse de relecture héritée vous permettait d’examiner uniquement les sites sécurisés (HTTPS).

* Examiner les sites protégés contre les iframes (sites qui ne peuvent être visualisés dans un iframe).

  La visionneuse de relecture héritée ne prenait pas en charge l’examen des sites qui sont protégés contre l’affichage dans un iframe.

* Affichez le contenu avec des résolutions préconfigurées pour différents appareils. Vous pouvez, par exemple, voir comment le contenu s’affiche dans différentes résolutions de bureau standard ou sur des appareils individuels tels que l’iPhone 8. 

Pour plus d’informations sur le téléchargement, l’installation et l’utilisation de la visionneuse de relecture de bureau, voir .

Pour plus d’informations sur les différences de fonctionnalité entre la visionneuse de relecture de bureau et les visionneuses de relecture basées sur un navigateur, voir [Vue d’ensemble des différences entre la visionneuse de relecture web et la visionneuse de relecture de bureau](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

## Exporter la vue Utilisateur ou utilisatrice dans le planificateur de ressources {#export-the-user-view-in-the-resource-planner}

Nous avions temporairement désactivé l’exportation des données du planificateur de ressources lors de leur affichage dans la vue Utilisateur ou utilisatrice afin de résoudre certains problèmes de performances. Avec cette version, nous réactivons l’exportation des données lors de l’affichage du planificateur de ressources dans la vue Utilisateur ou utilisatrice.

Pour plus d’informations sur l’exportation des données du planificateur de ressources vers Excel, voir la section « Option d’exportation » dans [Vue d’ensemble de la navigation dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Pour participer à notre programme Beta actuel pour le planificateur de ressources, voir [Performances du planificateur de ressources (Beta)](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront).

## Paramètres du système : informations de session dans les pages externes {#system-setting-session-information-in-external-pages}

L’administrateur ou administratrice Workfront peut désormais restreindre l’utilisation des informations de session (par exemple, l’ID de session) lors de la création d’une page externe.

Avant cette modification, les personnes qui pouvaient créer des pages externes pouvaient utiliser toutes les informations de session lorsqu’elles intégraient d’autres sites dans un tableau de bord Workfront. 

Pour plus d’informations sur la configuration de vos préférences système dans Workfront, voir [Configurer les préférences de sécurité du système](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Prise en charge de Google Team Drive {#support-for-google-team-drives}

Vous pouvez désormais lier un document ou un dossier situé sur Google Team Drive à partir de Workfront.

Avant cette amélioration, vous pouviez lier un document ou un dossier situé uniquement sur Google My Drive.

Pour plus d’informations sur la liaison de documents et de dossiers de diverses applications à Workfront, consultez la section [Lier des documents à partir d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Nouvelle limite d’exportation pour le graphique de Gantt {#new-export-limit-for-the-gantt-chart}

Vous pouvez désormais exporter jusqu’à 500 tâches dans le graphique de Gantt.

Auparavant, vous ne pouviez exporter que 250 tâches.

Pour plus d’informations, consultez la section [Exporter le graphique de Gantt au format PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## L’option Coller à partir du presse-papiers s’affiche désormais en grisé lors de l’utilisation d’Internet Explorer ou Safari {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

L’option Coller à partir du presse-papiers s’affiche désormais en grisé lors de l’utilisation d’Internet Explorer ou Safari, avec une info-bulle expliquant que seuls les navigateurs Chrome et Firefox prennent en charge cette fonctionnalité.

Avant cette modification, cette option ne s’affichait pas lors de l’utilisation d’Internet Explorer ou Safari. 

Pour plus d’informations sur le collage d’images à partir du presse-papiers, consultez la section [Coller des images à partir du presse-papiers](../../../../documents/managing-documents/paste-image-clipboard.md).

## Nouvel environnement Beta pour Android avec de nouvelles fonctionnalités {#new-beta-environment-for-android-along-with-new-features}

Inscrivez-vous comme Beta-testeur ou Beta-testeuse et découvrez les fonctionnalités récentes de l’application mobile sur lesquelles notre équipe travaille, avant qu’elles ne soient accessibles au grand public. Cet environnement est actuellement pris en charge par l’application mobile Workfront uniquement pour les téléphones Android.

Pour plus d’informations sur la façon de s’inscrire en tant que Beta-testeur ou Beta-testeuse de l’application mobile Workfront, consultez .

Les améliorations suivantes sont désormais disponibles sur la version Beta de l’application mobile :

* Nouvelle page de compte

  Vous pouvez désormais consulter les informations relatives à votre compte, gérer vos paramètres mobiles, soumettre des commentaires ou vous déconnecter à partir de la nouvelle page de compte.

  Avant cette amélioration, il n’était pas possible de consulter les informations de votre compte, de modifier vos paramètres, de soumettre des commentaires ou de vous déconnecter via l’application mobile. Ces actions n’étaient réalisables que depuis le menu principal de Workfront.

* Nouveau panneau de navigation au bas de l’écran

  Une barre de navigation plus visible est maintenant accessible en bas de l’écran, facilitant l’accès à toutes les sections de l’application mobile.

  Avant cette amélioration, les fonctionnalités étaient répertoriés dans le menu principal de Workfront. Le menu principal de Workfront a été supprimé et remplacé par la nouvelle barre de navigation au bas de l’écran.

  Pour plus d’informations sur la configuration de la nouvelle barre de navigation, consultez la section « Configurer votre application mobile » dans .

* Nouvelle vue de la liste des notifications

  L’amélioration de l’aspect de la liste des notifications rend plus facile la distinction des notifications par leur nature et leur statut de lecture.

* La zone de recherche a été repositionnée à un endroit plus visible.

* Nouvelle expérience de connexion Une nouvelle expérience de connexion, plus fluide, a été conçue.

* Nouvelle expérience en matière de tutoriels

  De nouveaux tutoriels sont maintenant disponibles pour guider rapidement les utilisateurs et les utilisatrices lors de leur première connexion à l’application. Avant cette expérience, les tutoriels ne se lançaient que lorsque les utilisateurs et les utilisatrices accédaient à des zones de fonctionnalité spécifiques.

## Exemples de filtres pour les messages d’abonnements aux événements {#examples-of-filters-for-event-subscriptions-messages}

Des exemples de code sont désormais disponibles pour vous aider à filtrer les abonnements aux événements, afin de ne recevoir que les messages pertinents pour votre organisation et de gérer le flux d’événements entrant vers vos points d’entrée. Pour en savoir plus sur l’affichage des exemples de filtrage, consultez la section [Filtrer les messages d’abonnement aux événements](../../../../wf-api/api/filter-event-sub-messages.md).
