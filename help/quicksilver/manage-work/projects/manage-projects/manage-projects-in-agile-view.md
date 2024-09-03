---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Gérer un projet en vue Agile
description: Vous pouvez tirer parti des fonctionnalités Agile dans votre projet sans les difficultés administratives qui accompagnent généralement les pratiques Agile (comme la gestion des listes d’attente des équipes ou la création d’itérations).
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1423'
ht-degree: 100%

---

# Gérer un projet en vue Agile

<!-- Audited: 2/2024 -->

Vous pouvez tirer parti des fonctionnalités Agile dans votre projet sans les difficultés administratives qui accompagnent généralement les pratiques Agile (comme la gestion des listes d’attente des équipes ou la création d’itérations).

Si vous souhaitez travailler dans un environnement Agile qui utilise une liste d’attente d’équipe et vous permet de créer des itérations à partir des tâches de la liste d’attente, suivez les instructions de la section [Travailler dans un environnement Agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Actuel : Révision ou supérieur</p> 
   <p>Nouvelle : contributeur ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Accès en modification aux zones suivantes :</p> 
    <ul> 
     <li> <p>Projets</p> </li> 
     <li> <p>Rapports, tableaux de bord, calendriers</p> </li> 
     <li> <p>Filtres, Vues, Regroupements</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage sur le projet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Présentation des projets Agile

>[!NOTE]
>
>Cette section s’applique uniquement à la vue Agile héritée, et non à la vue Panorama d’un projet.

* [Fonctionnalités Agile dans un projet](#agile-functionality-in-a-project)
* [Différences entre l’utilisation de la vue Agile sur un projet et sur une itération](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Fonctionnalités Agile dans un projet {#agile-functionality-in-a-project}

La fonctionnalité Agile suivante est disponible lors de la gestion d’un projet dans une vue Agile :

* Statut d&#39;achèvement\
  Pour plus d’informations sur le statut d’achèvement, voir [Vue d’ensemble du statut d’achèvement de l’itération](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Storyboard\
  Pour plus d’informations sur les storyboards, voir la section [Panorama Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md).

Il existe des différences lors de l’utilisation de vues Agile sur un projet et le travail dans un environnement Agile pur (avec des listes d’attente et des itérations). Pour plus d’informations, voir [Différences entre l’utilisation de la vue Agile sur un projet et sur une itération](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) dans cet article.

### Différences entre l’utilisation de la vue Agile sur un projet et sur une itération {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Les tâches et les sous-tâches suivent différentes règles d’affichage dans une vue Agile de projet et sur le storyboard d’une itération](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board).
* [Les listes d’attente et les itérations ne sont pas utilisés dans la vue Agile](#backlogs-and-iterations-are-not-used).
* [L’ordre des tâches est conservé dans la vue Agile et ne peut pas être réorganisé](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered).
* [Les tâches sont mesurées uniquement en nombre d’heures prévues sur une liste de projets](#tasks-are-measured-only-in-planned-hours).
* [L’équipe Agile n’est pas utilisée dans une vue Agile](#the-agile-team-is-not-used).
* [Chaque utilisateur ou utilisatrice du projet peut afficher le projet dans une vue Agile différente.](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Les tâches et les sous-tâches suivent différentes règles d’affichage dans une vue Agile de projet et sur le storyboard d’une itération. {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Les tâches qui n’ont pas de tâche parent ni de sous-tâche sont toujours affichées sous la forme d’une seule carte d’histoire sur le storyboard de la vue Agile.\
  Par exemple, ces tâches apparaissent comme suit dans la vue de liste des projets :

  ![Liste de projets Agile : tâches sans parent ni sous-tâches](assets/agile-project-single-list-nwe.png)

  Ces tâches apparaissent comme suit dans la vue Agile du projet :

  ![Vue Agile du projet : tâches sans parent ni sous-tâches](assets/agile-project-singlecard-nwe.png)

* Les tâches parent qui comportent des sous-tâches sont toujours affichées dans la colonne **Histoires** du storyboard de la vue Agile. Les sous-tâches sont affichées dans le couloir de la tâche parent.\
  Par exemple, ces tâches apparaissent comme suit dans la vue de liste des projets :

  ![Liste de projets Agile : tâches avec parents et sous-tâches](assets/agile-project-parent-list-nwe.png)\
  Ces tâches apparaissent comme suit dans la vue Agile du projet :

  ![Vue Projet Agile : tâches avec parents et sous-tâches](assets/agile-project-parent-nwe.png)

* Les sous-tâches de deuxième niveau (sous-tâches de sous-tâches) s’affichent sous la forme d’une carte grise rattachée à la tâche parent directe.
* Les sous-tâches de troisième niveau (sous-tâches de sous-tâches de sous-tâches) ne s’affichent jamais dans la vue Agile.

#### Les listes d’attente et les itérations ne sont pas utilisées dans la vue Agile. {#backlogs-and-iterations-are-not-used}

Lors de l’affichage d’un projet dans une vue Agile, les composants Agile suivants ne sont pas utilisés :

* **Liste d’attente :** aucun liste d’attente n’est utilisée, car toutes les tâches du projet sont automatiquement affichées sous forme d’histoires.
* **Itérations :** plutôt que de créer des itérations pour définir les dates auxquelles le travail sera effectué, les jours actuellement désignés dans la chronologie du projet deviennent les jours ouvrés.

#### L’ordre des tâches est conservé dans la vue Agile et ne peut pas être modifié. {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

L’ordre dans lequel les tâches apparaissent dans un projet est conservé lorsque vous affichez le projet dans un storyboard Agile.

Vous ne pouvez pas modifier l’ordre des tâches du projet lorsque vous l’affichez dans une vue Agile. La modification de l’ordre des tâches pouvant affecter d’autres tâches qui peuvent avoir des dépendances, vous devez afficher le projet dans une vue standard afin de modifier l’ordre des tâches.

#### Les tâches sont mesurées uniquement en heures prévues dans une liste de projets. {#tasks-are-measured-only-in-planned-hours}

Les tâches d’un projet sont toujours mesurées en heures prévues.

Dans une itération, les tâches (histoires) peuvent être mesurées en heures ou en points.

#### L’équipe Agile n’est pas utilisée dans une vue Agile. {#the-agile-team-is-not-used}

Étant donné que les équipes Agile effectuent le travail dans les itérations qui leur sont affectées, les équipes Agile ne sont pas utilisées lors de l’affichage d’un projet dans une vue Agile.

Au lieu de cela, tous les utilisateurs et toutes les utilisatrices du projet deviennent l’équipe Agile pour ce projet.

#### Chaque utilisateur ou utilisatrice du projet peut afficher le projet dans une vue Agile différente. {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

Contrairement à une itération Agile, les utilisateurs et les utilisatrices d’un projet peuvent personnaliser leur propre vue Agile tandis que d’autres utilisateurs et utilisatrices utilisent une vue Agile différente.

Dans une itération Agile, les informations disponibles dans le storyboard Agile (telles que les colonnes de statuts disponibles) sont déterminées au niveau de l’équipe.

Pour plus d’informations sur la personnalisation d’une vue Agile, voir [Créer ou personnaliser une vue Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) dans [Créer ou modifier des vues dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Afficher un projet dans la vue Agile

1. Accédez au projet que vous souhaitez afficher dans une vue Agile, soit via la liste des tâches, soit via la liste des problèmes.
1. Cliquez sur l’icône **Vue panorama** ![Icône panorama](assets/board-icon-for-agile-view.png).

   La vue panorama du projet s’affiche par défaut.

   ![Vue panorama du projet](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Facultatif) Cliquez sur **Configurer** pour configurer les options des colonnes et des cartes.

   Pour plus d’informations, voir [Gérer les colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) et [Personnaliser les champs à afficher sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). Vous ne pouvez pas définir de politiques de colonne dans la vue panorama d’un projet.

1. (Facultatif) Cliquez sur **Utiliser la vue Agile héritée** pour utiliser la vue Agile héritée au lieu de la vue panorama.

1. (Facultatif – vue Agile héritée uniquement) Si vous avez créé une vue Agile personnalisée, ou si un autre utilisateur ou une autre utilisatrice a créé une vue Agile personnalisée et l’a partagée avec vous, vous pouvez l’afficher à la place de la vue Agile par défaut.

   Cliquez sur le menu déroulant **Vue**, puis cliquez sur la vue Agile personnalisée que vous souhaitez afficher.

   La vue Agile personnalisée est celle qui sera utilisée la prochaine fois que vous cliquerez sur l’icône **Agile**.

   Pour plus d’informations sur la création d’une vue Agile, voir [Créer et personnaliser des vues Agile](#create-and-customize-agile-views), ci-dessous.

   Le projet s’affiche dans la vue Agile personnalisée.

1. (Le cas échéant – vue Agile héritée uniquement) Si les tâches de votre projet utilisent des statuts autres que « Nouveau », « En cours » ou « Terminé » (statuts par défaut de la vue Agile), vous devez ajouter les statuts supplémentaires à la vue Agile pour que toutes les tâches ayant ces statuts s’affichent.

   Si les tâches ont un statut qui ne s’affiche pas dans le storyboard Agile, la tâche elle-même ne s’affiche pas dans le storyboard Agile (cependant, le pourcentage d’avancement de ces tâches contribue toujours au pourcentage d’avancement de toutes les tâches parent et au pourcentage d’avancement du projet global).

   Pour ajouter des statuts à la vue Agile, créez une vue Agile ou personnalisez une vue Agile existante, comme décrit dans la section [Créer et personnaliser des vues Agile](#create-and-customize-agile-views), ci-dessous.

1. (Facultatif) Pour revenir à la vue Liste, cliquez sur l’icône **Liste**.

## Créer et personnaliser des vues Agile {#create-and-customize-agile-views}

>[!NOTE]
>
>Cette section s’applique uniquement à la vue Agile héritée, et non à la vue Panorama d’un projet.

Comme pour les vues standard dans Workfront, vous pouvez personnaliser les vues Agile existantes ou créer de nouvelles vues Agile à partir de zéro. Contrairement aux vues standard, vous ne pouvez pas créer de vues Agile basées sur des vues Agile existantes.

Pour plus d’informations sur la création et la personnalisation de vues Agile, voir [Créer ou personnaliser une vue Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) dans l’article [Créer ou modifier des vues dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Partager une vue Agile existante

>[!NOTE]
>
>Cette section s’applique uniquement à la vue Agile héritée, et non à la vue Panorama d’un projet.

Vous pouvez partager une vue Agile que vous avez créée ou dont vous disposez les autorisations, de la même manière que n’importe quelle autre vue, filtre ou regroupement.

Pour plus d’informations, voir [Partager un filtre, une vue ou un regroupement](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Supprimer une vue Agile existante

>[!NOTE]
>
>Cette section s’applique uniquement à la vue Agile héritée, et non à la vue Panorama d’un projet.

Vous pouvez supprimer une vue Agile de la même manière que vous supprimez une vue, un filtre ou un regroupement.

Pour plus d’informations, voir [Supprimer des filtres, des vues et des regroupements](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
