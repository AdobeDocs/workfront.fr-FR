---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de version 2018.1 bêta 2
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.1 bêta 2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 14 décembre 2017. Il sera disponible dans l’environnement de production en mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 2%

---

# Activité de version 2018.1 bêta 2

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.1 bêta 2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 14 décembre 2017. Il sera disponible dans l’environnement de production en mars 2018.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.1, voir  [Présentation de l’activité de la version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version 2018.1 bêta 2 contient des améliorations pour les administrateurs de Workfront et d’autres utilisateurs :

**Pour les administrateurs**

* [Administration des groupes pour les utilisateurs et les modèles de mise en page](#group-administration-for-users-and-layout-templates)

**Pour tous les utilisateurs**

* [Affichage à l’écran large du système](#system-wide-widescreen-display)
* [Redimensionner l’instantané de la chronologie sur le diagramme de Gantt](#resize-timeline-snapshot-on-the-gantt-chart)
* [Plan de ressource interactif dans l’analyse de cas](#interactive-resource-planner-in-the-business-case)
* [Visualisation dans le planificateur de ressources - Graphique d’affectation des utilisateurs](#visualization-in-the-resource-planner-user-allocation-chart)
* [Améliorations de la zone d’accueil](#improvements-in-the-home-area)
* [Nouvelles améliorations de la visionneuse de correctifs](#new-proofing-viewer-improvements) 

## Administration des groupes pour les utilisateurs et les modèles de mise en page {#group-administration-for-users-and-layout-templates}

Vous pouvez désormais désigner des administrateurs de groupe dans Workfront. Le champ Propriétaire du groupe a été renommé Administrateur de groupe. Les utilisateurs désignés comme administrateurs de groupe disposent d’autorisations supplémentaires pour gérer les utilisateurs et les modèles de mise en page pour les groupes qu’ils gèrent.

* [Gestion des utilisateurs par administrateur de groupe](#user-management-by-group-administrator)
* [Gestion des modèles de mise en page par administrateurs de groupe](#layout-template-management-by-group-administrators)

### Gestion des utilisateurs par administrateur de groupe {#user-management-by-group-administrator}

Nous introduisons le nouveau concept de **administrateur de groupe**. Pour ce faire, la variable **Propriétaire du groupe** a été renommé **administrateur de groupe** et les utilisateurs désignés comme administrateurs de groupe disposent d’autorisations supplémentaires pour gérer les utilisateurs et les groupes.

En plus des autorisations que le propriétaire du groupe devait auparavant gérer pour les utilisateurs, l’administrateur du groupe dispose désormais des droits d’accès supplémentaires suivants lors de la gestion des utilisateurs au sein des groupes où ils sont définis en tant qu’administrateur de groupe :

* Connectez-vous en tant qu’autre utilisateur appartenant à un groupe qu’il gère.
* Réinitialisez le mot de passe d’un autre utilisateur appartenant à un groupe qu’il gère.
* Créez des modèles de mise en page gérés par leur groupe. 

Avant cette modification, seul l’administrateur Workfront pouvait exécuter ces fonctions.

Pour plus d’informations sur les administrateurs de groupe, voir la section &quot;Comprendre les administrateurs de groupe&quot; dans [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Gestion des modèles de mise en page par administrateurs de groupe {#layout-template-management-by-group-administrators}

Nous introduisons le nouveau concept de **Groupe avec accès Administration** que vous pouvez associer à un modèle de mise en page.

L’utilisateur désigné comme administrateur de groupe sur ce groupe a accès à la gestion de ce modèle de mise en page et à la création de modèles de mise en page où les groupes qu’il gère sont les groupes administratifs des modèles. 

Avant cette modification, seul l’administrateur Workfront pouvait créer des modèles de mise en page.

Pour plus d’informations sur la création de modèles de mise en page, voir &quot;Création et gestion de modèles de mise en page&quot;.

## Affichage à l’écran large du système {#system-wide-widescreen-display}

Lorsque vous affichez une page dans Workfront, l’intégralité de la fenêtre du navigateur est désormais automatiquement remplie et s’ajuste à la taille de l’écran.

Avant cette modification, seules les pages associées aux objets suivants s’affichaient sur un écran large :

* Projets
* Tâches
* Problèmes
* Rapports
* Tableaux de bord
* Calendriers

## Redimensionner l’instantané de la chronologie sur le diagramme de Gantt {#resize-timeline-snapshot-on-the-gantt-chart}

Vous pouvez maintenant développer l’instantané de la chronologie pour afficher l’intégralité du projet dans le diagramme de Gantt.

Avant cette amélioration, vous pouvez sélectionner un point spécifique sur l’instantané de la chronologie pour y accéder dans le diagramme de Gantt.

Pour plus d’informations sur la configuration de l’affichage des informations sur le graphique Gantt, voir [Configuration de l’affichage des informations sur le diagramme de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Plan de ressource interactif dans l’analyse de cas {#interactive-resource-planner-in-the-business-case}

En tant que gestionnaire de ressources, vous pouvez désormais ajouter des groupes de ressources dans la section Budget des ressources de l’analyse de cas. Vous pouvez également budgéter les ressources de votre projet à l’aide du planificateur de ressources au niveau du projet. Le budget de vos ressources pour un projet génère le coût du travail budgété du projet.

Avant cette modification, vous pouvez afficher les informations de budget des ressources dans l’Analyse de cas si le projet avait été budgété pour des ressources dans le planificateur global de ressources.

Pour plus d’informations sur l’exécution des ressources de projet de budget dans l’Analyse de cas, voir [Ressources budgétaires dans l’analyse de cas](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualisation dans le planificateur de ressources - Graphique d’affectation des utilisateurs {#visualization-in-the-resource-planner-user-allocation-chart}

Vous pouvez maintenant afficher l’affectation planifiée globale de tous les utilisateurs par rapport à leur disponibilité dans un graphique dans le planificateur de ressources. Le graphique est disponible lorsque vous sélectionnez **Afficher par utilisateur** dans le planificateur de ressources.

Le graphique présente les informations suivantes :

* % de disponibilité sans sur-allocation de tous les utilisateurs
* % de sur-allocation pour tous les utilisateurs
* % de sous-utilisation pour tous les utilisateurs
* Il existe une surallocation pour au moins un utilisateur durant cette période

Avant cette modification, vous ne pouviez afficher l’affectation et la disponibilité de chaque utilisateur qu’au format tabulaire.

Pour plus d’informations sur le graphique d’affectation des utilisateurs dans le planificateur de ressources, voir [Présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Améliorations de la zone d’accueil {#improvements-in-the-home-area}

Plusieurs améliorations sont désormais disponibles dans la zone Accueil, notamment :

* Améliorations de l’apparence

   * Le panneau de droite est désormais plus grand, ce qui permet d’avoir plus d’espace pour les informations sur les tâches et les problèmes.
   * Les éléments en retard s’affichent désormais dans une couleur rouge plus claire lorsqu’ils sont sélectionnés dans le panneau de gauche.
   * Vous pouvez désormais afficher plus facilement la relation entre le panneau de gauche et le panneau de droite. Le document sélectionné dans le panneau de gauche pointe vers le panneau de droite.

* Les champs par défaut s’affichent pour les éléments sélectionnés. 

  Pour plus d’informations sur les champs par défaut, voir &quot;Création et gestion des modèles de mise en page&quot;.

* Après avoir cliqué sur &quot;Travailler dessus&quot; sur une requête, les champs associés au problème s’affichent dans le panneau de droite.

  Pour plus d’informations sur l’utilisation des requêtes de la zone d’accueil, voir [Gérer les requêtes de travail et d’équipe dans la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) in [Gérer les requêtes de travail et d’équipe dans la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Pointez sur un avatar utilisateur sur un élément de travail du panneau de gauche pour afficher le nom de l’utilisateur.
* Développez la zone &quot;En retard&quot; du panneau de gauche pour afficher tous les éléments en retard (lorsque cette zone est réduite, seuls les 5 premiers éléments s’affichent).
* Après avoir marqué un élément comme terminé, il reste dans le panneau de gauche jusqu’à ce que vous sélectionniez un autre élément.\
  Pour plus d’informations sur l’affichage des éléments terminés, voir [Afficher des éléments dans la liste des tâches de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) in [Afficher des éléments dans la liste des tâches de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Pour plus d’informations sur l’utilisation de la nouvelle zone d’accueil, ainsi que sur les différences de fonctionnalités entre Mon travail et Accueil, voir [Utilisation de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Nouvelles améliorations de la visionneuse de correctifs  {#new-proofing-viewer-improvements}

* [Mise en page et conception améliorées](#improved-layout-and-design)
* [Recherche de commentaires par nombre de commentaires](#search-comments-by-comment-number)
* [Option permettant de modifier le commentaire en regard de l’indicateur de balisage](#option-to-edit-comment-next-to-the-markup-indicator)
* [Marquer tous les commentaires comme lus](#mark-all-comments-as-read)
* [Amélioration du menu de gauche](#left-menu-improvements)

### Mise en page et conception améliorées {#improved-layout-and-design}

L’aspect de la visionneuse de vérification est mis à jour. Les zones suivantes de la visionneuse de vérification ont été mises à jour :

* Zone de miniatures

  Pour plus d’informations sur l’utilisation de la zone de miniatures, voir dans .

* Zone de commentaires\
  Pour plus d’informations sur la zone de commentaires, voir .
* Zone de menu gauche

### Recherche de commentaires par nombre de commentaires {#search-comments-by-comment-number}

Désormais, lorsque vous recherchez la liste de commentaires dans la visionneuse de vérification, vous pouvez saisir le numéro du commentaire dans le champ de recherche. La liste des commentaires est ensuite filtrée pour afficher le commentaire que vous avez recherché. 

Pour plus d’informations, voir .

### Option permettant de modifier le commentaire en regard de l’indicateur de balisage {#option-to-edit-comment-next-to-the-markup-indicator}

Vous pouvez désormais modifier plus facilement un commentaire existant. Après avoir cliqué sur un indicateur de commentaire sur le BAT, une icône d’édition s’affiche en regard du ballon. 

Avant cette modification, vous deviez cliquer sur l’icône Modifier dans la zone Commentaire.  

Pour plus d’informations, voir .

### Marquer tous les commentaires comme lus {#mark-all-comments-as-read}

Lors de l’affichage d’un document dans la visionneuse de vérification, vous pouvez désormais marquer tous les commentaires comme étant lus.

### Amélioration du menu de gauche {#left-menu-improvements}

Le menu situé sur le côté gauche de la visionneuse de vérification contient les améliorations suivantes :

* Aspect mis à jour
* Icône en haut du menu pour afficher ou masquer le menu

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* Pointez sur le menu pour développer automatiquement le menu afin d’afficher les libellés en plus des icônes. (Ou activez l’option pour conserver le menu toujours dans la vue réduite.)
