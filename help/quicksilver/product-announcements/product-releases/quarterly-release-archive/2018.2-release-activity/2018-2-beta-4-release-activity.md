---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.2, version bêta 4
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.2 de Beta 4. Cette fonctionnalité sera disponible dans l’environnement Aperçu le 17 mai 2018. Il sera disponible dans l’environnement de production en juillet 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# Activité Version 2018.2, version bêta 4

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.2 de Beta 4. Cette fonctionnalité sera disponible dans l’environnement Aperçu le 17 mai 2018. Il sera disponible dans l’environnement de production en juillet 2018.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.2, voir  [Présentation de l’activité de version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La version 2018.2 de Beta 4 contient les améliorations apportées aux administrateurs Workfront et aux autres utilisateurs :

**Pour les administrateurs**

* [Paramètre système : informations de session dans les pages externes](#system-setting-session-information-in-external-pages)

**Pour Tous Les Utilisateurs**

* [Améliorations des limites de travail en cours sur la carte Kanban](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [Interface améliorée pour la configuration des états pour une équipe agile](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [Liste de travail mise à jour (panneau de gauche) dans la zone d’accueil](#updated-work-list-left-panel-in-the-home-area)
* [Nouvelle visionneuse de vérification de l’appli de bureau pour le contenu interactif (multimédia enrichi)](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content) 
* [Exporter la vue utilisateur dans le planificateur de ressources](#export-the-user-view-in-the-resource-planner)
* [Prise en charge des pilotes d’équipe Google](#support-for-google-team-drives)
* [Nouvelle limite d’exportation pour le diagramme de Gantt](#new-export-limit-for-the-gantt-chart)
* [ L’option Coller à partir du Presse-papiers s’affiche maintenant sous forme de codé lors de l’utilisation d’Internet Explorer ou de Safari ](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [Nouvel environnement Beta pour Android avec de nouvelles fonctionnalités](#new-beta-environment-for-android-along-with-new-features)
* [Exemples de filtres pour les messages d’abonnement à un événement](#examples-of-filters-for-event-subscriptions-messages)

## Améliorations des limites de travail en cours sur le conseil de Kanban {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### Configuration des limites de travail en cours pour chaque colonne du panorama Kanban

Vous pouvez maintenant configurer les limites de travail en cours pour chaque colonne du panorama Kanban. 

Avant cette modification, vous ne pouviez configurer qu&#39;une seule limite de travaux en cours qui s&#39;appliquait à toutes les colonnes du panorama Kanban. 

Pour plus d’informations, voir la section  [ Configurez la limite de travail en cours ](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) dans l’article  [Configurez Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

### Mettre à jour la limite de travail en cours directement à partir du conseil de Kanban

Désormais, les membres de l’équipe disposant des droits d’édition de l’équipe peuvent mettre à jour la limite de travaux en cours directement à partir du panorama Kanban.

Avant cette modification, vous ne pouviez mettre à jour la limite de travail en cours que depuis la zone Paramètres de l’équipe .

Pour plus d’informations, voir  dans l’article .

## Interface améliorée pour la configuration des états d’une équipe agile {#improved-interface-for-configuring-statuses-for-an-agile-team}

Mise à jour de l’interface de configuration des statuts d’une équipe agile avec les améliorations suivantes :

* Nouvelle apparence
* Réorganiser les colonnes d’état par glisser-déposer 

Pour plus d’informations, voir les articles suivants :

* [Configurer Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [Configurer Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Mise à jour de la liste de travail (panneau de gauche) dans la zone d’accueil {#updated-work-list-left-panel-in-the-home-area}

La liste de tâches de la zone Accueil contient les améliorations suivantes :

* Les éléments non lus apparaissent maintenant avec un bogue et un point bleu.

  Les éléments affichés en dehors de la zone Accueil sont toujours affichés comme Non lus dans la zone Accueil.

  Pour plus d’informations, voir [Afficher les éléments dans la liste de travail dans la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Les problèmes sont désormais identifiés par une icône de problème qui s’affiche en regard du problème.
* Les validations sont désormais distinguées par type de validation, le type de validation étant affiché. Les types d’approbation possibles sont Tâche, Projet, Problème, Accès, Document, Frise chronologique et Bon à tirer.

  Avant cette modification, les approbations n&#39;étaient distinguées que par le mot &quot;approbation&quot;.

* Les éléments se distinguent désormais par leur disponibilité à démarrer. Les options possibles sont Prêt à démarrer, Pas prêt ou Utilisation.

  Ces informations ne sont pas affichées pour les validations car les validations sont toujours prêtes à démarrer.

* Une icône de document s’affiche sous le nom de l’élément chaque fois qu’un document est joint à l’élément.
* Vous pouvez désormais réduire et développer des regroupements dans la liste des tâches afin de mieux contrôler les informations visibles. Les regroupements sont En retard, Projets, Dates et Terminé.

  Par défaut, la section Cette semaine est développée et tous les autres regroupements sont réduits.

* Choisissez si vous souhaitez trier les éléments par date d’achèvement prévue ou par date de validation.
* Le nombre d’éléments de chaque groupement s’affiche désormais entre parenthèses en regard du titre du groupement.

  Ce nombre n’est pas disponible pour le groupement Terminé.

  Pour plus d’informations, voir [Afficher les éléments dans la liste de travail dans la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Redimensionnez la liste des tâches par glisser-déplacer. Vous pouvez redimensionner la liste de travail pour qu’elle consume jusqu’à la moitié de l’écran. La taille que vous définissez est conservée la prochaine fois que vous accédez à Accueil.

  Avant cette modification, la taille de la liste de tâches ne pouvait pas être modifiée.

* Pour les requêtes, l’avatar de l’utilisateur qui a effectué la requête s’affiche désormais, avec le texte &quot;[nom_approbateur]&quot; pour votre approbation.
* Lors de la création d’une tâche personnelle, le bouton &quot;À faire&quot; est désormais intitulé &quot;Personnel&quot;.

  Pour plus d’informations, voir [Créer des tâches à partir de la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) dans l’article [Créer des tâches à partir de la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Les éléments en retard sont indiqués comme en retard uniquement après une heure au-delà de la date d’achèvement planifiée.

Pour plus d’informations sur la zone d’accueil, voir [Utilisation de la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nouvelle visionneuse de vérification de l’appli de bureau pour le contenu interactif (multimédia enrichi) {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

La nouvelle visionneuse de vérification de l’appli de bureau vous permet de tester le contenu interactif. Contrairement à la visionneuse de vérification héritée et à la nouvelle visionneuse de vérification qui s’exécute dans le navigateur, la visionneuse est une application qui s’exécute sur votre poste de travail.

Avant la nouvelle visionneuse de vérification de l’appli de bureau, vous ne pouviez tester le contenu interactif que dans la visionneuse de vérification de l’ancienne version. 

La visionneuse de vérification de l’appli de bureau comprend les améliorations suivantes par rapport à la visionneuse de vérification de l’ancienne version pour la vérification du contenu interactif :

* Vérifier les sites non sécurisés (HTTP)

  La visionneuse de vérification héritée vous a permis de consulter uniquement les sites sécurisés (HTTPS).

* Examinez les sites protégés par iframe (les sites protégés contre l’affichage dans un iframe).

  La visionneuse de vérification héritée ne prenait pas en charge la révision pour les sites protégés contre l’affichage dans un iFrame.

* Affichez le contenu avec des résolutions préconfigurées pour divers appareils. Vous pouvez, par exemple, voir comment le contenu s’affiche dans différentes résolutions de bureau standard ou sur des appareils individuels tels qu’iPhone 8. 

Pour plus d’informations sur le téléchargement, l’installation et l’utilisation de la visionneuse de vérification de l’appli de bureau, voir .

Pour plus d’informations sur les différences de fonctionnalités entre la visionneuse de vérification de l’appli de bureau et les visionneuses de vérification de l’appli de bureau basées sur un navigateur, voir [Différences entre la visionneuse de vérification de l’appli de bureau et la présentation de la visionneuse de vérification de l’appli de bureau](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

## Exportation de la vue utilisateur dans le planificateur de ressources {#export-the-user-view-in-the-resource-planner}

Nous avions temporairement désactivé l’exportation des données à partir du planificateur de ressources lors de son affichage dans la vue utilisateur afin de résoudre certains problèmes de performances. Avec cette version, nous réactivons l’exportation des données lors de l’affichage du planificateur de ressources dans la vue utilisateur.

Pour plus d’informations sur l’exportation des données du planificateur de ressources vers Excel, consultez la section &quot;Option d’exportation&quot; dans la [présentation de la navigation du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Pour participer à notre programme bêta actuel pour le planificateur de ressources, voir [Resource Planner Performance Beta.](http://community.workfront.com/discussions/community-home/digestviewer/viewthread?GroupId=457&amp;MessageKey=8b018ed9-97a2-4f9d-a93b-01a7b09b6350&amp;CommunityKey=0425cafc-f0ec-47fc-be20-a21dc073d520&amp;tab=digestviewer&amp;ReturnUrl=%2fdiscussions%2fcommunity-home%2fdigestviewer%3fCommunityKey%3d0425cafc-f0ec-47fc-be20-a21dc073d520)

## Paramètre système : informations de session dans les pages externes {#system-setting-session-information-in-external-pages}

L’administrateur Workfront peut désormais restreindre l’utilisation des informations de session (par exemple, l’ID de session) lors de la création d’une page externe.

Avant cette modification, les utilisateurs qui pouvaient créer des pages externes pouvaient utiliser n’importe quelle information de session lors de l’incorporation d’autres sites dans un tableau de bord Workfront. 

Pour plus d’informations sur la configuration de vos préférences système dans Workfront, voir [Configuration des préférences de sécurité système](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Prise en charge des pilotes d’équipe Google {#support-for-google-team-drives}

Vous pouvez désormais lier un document ou un dossier situé sur un lecteur Google Team à partir de Workfront.

Avant cette amélioration, vous pouviez lier un document ou un dossier situé uniquement sur Google My Drive.

Pour plus d’informations sur la liaison de documents et de dossiers de diverses applications à Workfront, voir [Liaison de documents à partir d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Nouvelle limite d’exportation pour le diagramme de Gantt {#new-export-limit-for-the-gantt-chart}

Vous pouvez désormais exporter jusqu’à 500 tâches dans le diagramme de Gantt.

Auparavant, vous pouviez uniquement exporter jusqu’à 250 tâches.

Pour plus d’informations, voir [Export du diagramme de Gantt vers PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## L’option Coller à partir du Presse-papiers s’affiche maintenant sous forme de coche lors de l’utilisation d’Internet Explorer ou de Safari. {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

L’option Coller à partir du Presse-papiers s’affiche désormais sous forme grisée lors de l’utilisation des navigateurs Internet Explorer ou Safari, avec une info-bulle expliquant que seuls les navigateurs Chrome et Firefox sont pris en charge pour cette fonctionnalité.

Avant cette modification, cette option ne s’affichait pas dans Internet Explorer ou Safari. 

Pour plus d’informations sur le collage d’images à partir du Presse-papiers, voir [Collage d’images à partir du Presse-papiers](../../../../documents/managing-documents/paste-image-clipboard.md).

## Nouvel environnement Beta pour Android avec de nouvelles fonctionnalités {#new-beta-environment-for-android-along-with-new-features}

Vous pouvez désormais découvrir les fonctionnalités les plus récentes sur lesquelles notre équipe travaille pour l’application mobile avant qu’elles ne soient publiées au grand public en vous inscrivant pour devenir un testeur bêta. Cet environnement est actuellement pris en charge pour l’application mobile Workfront uniquement pour les téléphones Android.

Pour plus d’informations sur l’inscription à un testeur bêta pour l’application mobile Workfront, voir .

Les améliorations suivantes sont désormais disponibles sur la version bêta de l’application mobile :

* Page Nouveau compte

  Vous pouvez désormais afficher les informations de votre compte et gérer vos paramètres mobiles, envoyer des commentaires ou vous déconnecter de la nouvelle page Compte .

  Avant cette amélioration, vous ne pouviez pas afficher les informations de votre compte sur l’application mobile et accéder à vos paramètres, envoyer des commentaires et vous déconnecter à partir du menu principal de Workfront.

* Nouveau panneau inférieur de navigation

  Une barre de navigation plus visible est désormais disponible au bas de votre écran, qui lance toutes les zones de l’application mobile.

  Avant cette amélioration, les domaines des fonctionnalités étaient répertoriés dans le menu principal de Workfront. Le menu principal de Workfront a été supprimé et remplacé par la nouvelle barre de navigation inférieure.

  Pour plus d’informations sur la configuration de la nouvelle barre de navigation, voir la section &quot;Configuration de votre application mobile&quot; dans .

* Nouveau mode Liste des notifications

  L’aspect amélioré de la liste Notifications vous permet de différencier facilement les notifications de votre liste en fonction de leur type et de leur lecture.

* La zone de recherche a été déplacée vers une position plus visible.

* Nouvelle expérience de connexionIl existe une nouvelle expérience de connexion plus simple.

* Nouvelle expérience de tutoriel

  De nouveaux tutoriels sont désormais disponibles pour guider brièvement les utilisateurs dans l’application lorsqu’ils se connectent pour la première fois. Avant cette expérience, les tutoriels étaient lancés uniquement lorsque les utilisateurs accédaient à des zones de fonctionnalités spécifiques.

## Exemples de filtres pour les messages d’abonnement à un événement {#examples-of-filters-for-event-subscriptions-messages}

Pour démontrer comment filtrer les abonnements à des événements afin de ne recevoir que les messages relatifs à votre organisation, vous pouvez désormais utiliser des fragments de code pour filtrer le flux des événements qui se rapportent à vos points de terminaison. Pour en savoir plus sur l&#39;affichage des exemples de filtrage, voir [Filtrage des messages d&#39;abonnement d&#39;événement](../../../../wf-api/api/filter-event-sub-messages.md).
