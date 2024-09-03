---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de la version 2018.1 bêta 2
description: Cette page décrit l’ensemble des modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version 2018.1 bêta 2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement de prévisualisation le 14 décembre 2017. Elles seront disponibles dans l’environnement de production en mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 100%

---

# Activité de la version 2018.1 bêta 2

Cette page décrit l’ensemble des modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version 2018.1 bêta 2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement de prévisualisation le 14 décembre 2017. Elles seront disponibles dans l’environnement de production en mars 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées dans la version 2018.1, consultez [Vue d’ensemble de l’activité de la version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version 2018.1 bêta 2 contient des améliorations pour les administrateurs et administratrices Workfront et pour les autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices**

* [Administration de groupes pour les utilisateurs et utilisatrices et modèles de mise en page](#group-administration-for-users-and-layout-templates)

**Pour tous les utilisateurs et utilisatrices**

* [Affichage au format écran large dans l’ensemble du système](#system-wide-widescreen-display)
* [Redimensionnement de l’instantané de la chronologie sur le graphique de Gantt](#resize-timeline-snapshot-on-the-gantt-chart)
* [Planificateur de ressources interactif dans le Business Case](#interactive-resource-planner-in-the-business-case)
* [Visualisation dans le planificateur de ressources - Graphique d’affectation des utilisateurs et des utilisatrices](#visualization-in-the-resource-planner-user-allocation-chart)
* [Améliorations de la zone d’accueil](#improvements-in-the-home-area)
* [Nouvelles améliorations de la visionneuse de relecture](#new-proofing-viewer-improvements)

## Administration de groupes pour les utilisateurs et utilisatrices et modèles de mise en page {#group-administration-for-users-and-layout-templates}

Vous pouvez désormais désigner des administrateurs et administratrices de groupe dans Workfront.Le champ Propriétaire du groupe a été renommé Administrateur ou administratrice du groupe. Les utilisateurs et utilisatrices désignés comme administrateurs et administratrices de groupe disposent d’autorisations supplémentaires pour gérer les utilisateurs et les utilisatrices ainsi que les modèles de disposition pour les groupes qu’ils gèrent.

* [Gestion des utilisateurs et des utilisatrices par l’administrateur ou l’administratrice de groupe](#user-management-by-group-administrator)
* [Gestion des modèles de disposition par les administrateurs et administratrices de groupe](#layout-template-management-by-group-administrators)

### Gestion des utilisateurs et des utilisatrices par l’administrateur ou l’administratrice de groupe {#user-management-by-group-administrator}

Nous introduisons le nouveau concept d’**administrateur ou d’administratrice de groupe**. Pour ce faire, le champ **Propriétaire du groupe** a été renommé **administrateur ou administratrice de groupe** et les utilisateurs et utilisatrices désignés comme administrateurs et administratrices de groupe disposent d’autorisations supplémentaires pour gérer les utilisateurs et les utilisatrices ainsi que les groupes.

En plus des autorisations que le ou la propriétaire du groupe devait auparavant gérer pour les utilisateurs et les utilisatrices, l’administrateur ou administratrice du groupe dispose désormais des droits d’accès supplémentaires suivants lors de la gestion des utilisateurs et des utilisatrices au sein des groupes où ils sont définis en tant qu’administrateur ou administratrice de groupe :

* Se connecter en tant qu’autre utilisateur ou utilisatrice appartenant à un groupe sous sa responsabilité.
* Réinitialiser le mot de passe d’un autre utilisateur ou d’une autre utilisatrice appartenant à un groupe sous sa responsabilité.
* Créer des modèles de disposition gérés par son groupe.  

Avant cette modification, seul l’administrateur ou l’administratrice Workfront pouvait réaliser ces opérations.

Pour plus d’informations concernant les administrateurs et administratrices de groupe, consultez la section « Présentation des administrateurs et administratrices de groupe » dans [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Gestion des modèles de disposition par les administrateurs et administratrices de groupe {#layout-template-management-by-group-administrators}

Nous introduisons le nouveau concept de **Groupe avec accès Administration** que vous pouvez associer à un modèle de mise en page.

L’utilisateur ou l’utilisatrice désigné comme administrateur ou administratrice de ce groupe a accès à la gestion de ce modèle de mise en page et à la création de modèles de mise en page, les groupes sous sa responsabilité étant les groupes d’administration des modèles. 

Avant cette modification, seul l’administrateur ou l’administratrice Workfront pouvait créer des modèles de disposition.

Pour plus d’informations concernant la création de modèles de disposition, consultez « Création et gestion de modèles de disposition ».

## Affichage au format écran large dans tout le système {#system-wide-widescreen-display}

Lorsque vous affichez une page dans Workfront, l’intégralité de la fenêtre du navigateur est désormais automatiquement remplie et s’ajuste à la taille de l’écran.

Avant cette modification, seules les pages associées aux objets suivants s’affichaient au format écran large :

* Projets
* Tâches
* Problèmes
* Rapports
* Tableaux de bord
* Calendriers

## Redimensionner l’instantané de la chronologie sur le graphique de Gantt {#resize-timeline-snapshot-on-the-gantt-chart}

Vous pouvez désormais développer l’instantané de la chronologie pour afficher l’intégralité du projet dans le graphique de Gantt.

Avant cette amélioration, vous pouviez sélectionner un point spécifique sur l’instantané de la chronologie pour y accéder dans le graphique de Gantt.

Pour plus d’informations sur la configuration de l’affichage des informations sur le graphique de Gantt, voir [Configurer l’affichage des informations sur le graphique de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Planificateur de ressources interactif dans le Business Case {#interactive-resource-planner-in-the-business-case}

En tant que gestionnaire de ressources, vous pouvez désormais ajouter des groupes de ressources dans la section Établissement du budget de ressources de le Business Case. Vous pouvez également budgéter les ressources de votre projet à l’aide du planificateur de ressources à l’échelle du projet. Le budget de vos ressources pour un projet génère le coût budgété de la main-d’œuvre du projet.

Avant cette modification, vous pouviez afficher les informations de l’établissement du budget de ressources dans le Business Case si le projet avait été budgété pour des ressources dans le planificateur global de ressources.

Pour plus d’informations sur l’exécution de l’établissement du budget de ressources du projet dans l’analyse de cas, voir [Ressources budgétaires dans l’analyse de cas](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualisation dans le planificateur de ressources - Graphique d’attribution des utilisateurs et utilisatrices {#visualization-in-the-resource-planner-user-allocation-chart}

Vous pouvez désormais afficher l’attribution prévue globale de tous les utilisateurs et de toutes les utilisatrices par rapport à leur disponibilité dans un graphique dans le planificateur de ressources. Le graphique est disponible lorsque vous sélectionnez **Afficher par utilisateur et utilisatrice** dans le planificateur de ressources.

Le graphique présente les informations suivantes :

* % de disponibilité sans sur-allocation de tous les utilisateurs
* % de sur-allocation pour tous les utilisateurs
* % de sous-utilisation pour tous les utilisateurs
* Il existe une surallocation pour au moins un utilisateur durant cette période

Avant cette modification, vous ne pouviez afficher l’attribution et la disponibilité de chaque utilisateur et utilisatrice qu’au format tabulaire.

Pour plus d’informations sur le graphique d’attribution des utilisateurs et utilisatrices dans le planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Améliorations de la zone Accueil {#improvements-in-the-home-area}

Plusieurs améliorations sont désormais disponibles dans la zone Accueil, notamment :

* Améliorations de l’aspect

   * Le panneau de droite est désormais plus grand, offrant plus d’espace pour les informations relatives aux tâches et aux problèmes.
   * Les éléments en retard sont désormais affichés en rouge plus clair lorsqu’ils sont sélectionnés dans le panneau de gauche.
   * Vous pouvez désormais afficher plus facilement la relation entre le panneau de gauche et le panneau de droite. Le document sélectionné dans le panneau de gauche pointe vers le panneau de droite.

* Les champs par défaut s’affichent pour les éléments sélectionnés. 

  Pour plus d’informations sur les champs par défaut, voir « Créer et gérer des modèles de disposition ».

* Après avoir cliqué sur « Travailler sur ce projet » sur une demande, les champs associés au problème s’affichent dans le panneau de droite.

  Pour plus d’informations sur l’utilisation des demandes de la zone Accueil, voir [Gérer les demandes de travail et d’équipe dans la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) dans [Gérer les demandes de travail et d’équipe dans la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Pointez vers un avatar utilisateur/utilisatrice sur un élément de travail du panneau de gauche pour afficher le nom de l’utilisateur ou de l’utilisatrice.
* Développez la zone « En retard » du panneau de gauche pour afficher tous les éléments en retard (lorsque cette zone est réduite, seuls les 5 premiers éléments s’affichent).
* Après avoir marqué un élément comme terminé, il reste dans le panneau de gauche jusqu’à ce que vous sélectionniez un autre élément.\
  Pour plus d’informations sur l’affichage des éléments terminés, voir [Afficher des éléments dans la liste de travail de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) dans [Afficher des éléments dans la liste de travail de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Pour plus d’informations sur l’utilisation de la nouvelle zone Accueil, ainsi que sur les différences de fonctionnalités entre Mon travail et Accueil, voir [Utiliser la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nouvelles améliorations de la visionneuse de relecture {#new-proofing-viewer-improvements}

* [Disposition et conception améliorées](#improved-layout-and-design)
* [Rechercher des commentaires par numéro de commentaire](#search-comments-by-comment-number)
* [Option permettant de modifier le commentaire en regard de l’indicateur de balisage](#option-to-edit-comment-next-to-the-markup-indicator)
* [Marquer tous les commentaires comme lus](#mark-all-comments-as-read)
* [Amélioration du menu de gauche](#left-menu-improvements)

### Disposition et conception améliorées {#improved-layout-and-design}

L’aspect de la visionneuse de relecture est mis à jour. Les zones suivantes de la visionneuse de relecture ont été mises à jour :

* Zone de miniatures

  Pour plus d’informations sur l’utilisation de la zone de miniatures, voir dans :

* Zone de commentaires\
  Pour plus d’informations sur la zone de commentaires, voir :
* Zone du menu de gauche

### Rechercher des commentaires par numéro de commentaire {#search-comments-by-comment-number}

Désormais, lorsque vous recherchez la liste de commentaires dans la visionneuse de relecture, vous pouvez saisir le numéro du commentaire dans le champ de recherche. La liste des commentaires est ensuite filtrée pour afficher le commentaire que vous avez recherché. 

Pour plus d’informations, voir :

### Option permettant de modifier le commentaire en regard de l’indicateur de balisage {#option-to-edit-comment-next-to-the-markup-indicator}

Vous pouvez désormais modifier plus facilement un commentaire existant. Après avoir cliqué sur un indicateur de commentaire sur l’épreuve, une icône de modification s’affiche en regard du ballon. 

Avant cette modification, vous deviez cliquer sur l’icône Modifier dans la zone Commentaire.  

Pour plus d’informations, voir :

### Marquer tous les commentaires comme lus {#mark-all-comments-as-read}

Lors de l’affichage d’un document dans la visionneuse de relecture, vous pouvez désormais marquer tous les commentaires comme étant lus.

### Amélioration du menu de gauche {#left-menu-improvements}

Le menu situé sur le côté gauche de la visionneuse de relecture contient les améliorations suivantes :

* Aspect mis à jour
* Icône en haut du menu pour afficher ou masquer le menu

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* Placez le pointeur de la souris sur le menu pour développer automatiquement le menu afin d’afficher les libellés en plus des icônes. (Ou activez l’option permettant de conserver le menu dans l’affichage réduit.)
