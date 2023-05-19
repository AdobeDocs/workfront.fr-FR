---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Gestion d’un projet en mode Agile
description: Plans requis, types de licence et accès à l’équipe de planification Adobe Workfront, à l’équipe Pro, à l’entreprise ou à l’entreprise Workfront Type de licence Révision, travail ou Planifier dans le modèle d’accès Modifiez l’accès et la possibilité de créer des rapports, des tableaux de bord et des calendriers.
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '1296'
ht-degree: 0%

---

# Gestion d’un projet en mode Agile

Plans, types de licence et accès requis

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Formule Adobe Workfront</a> </p> </td> 
   <td> <p>Équipe, Pro, Entreprise ou Entreprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Type de licence Workfront</p> </td> 
   <td> <p>Révision, travail ou plan </p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
  --> 
 </tbody> 
</table>

Vous pouvez tirer parti des fonctionnalités agiles de votre projet

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(such as story boards and burndown charts)
</MadCap:conditionalText>
-->

 sans les défis administratifs qui accompagnent généralement les pratiques agiles (comme la gestion du retard d’une équipe ou la création d’itérations).

Si vous souhaitez travailler dans un environnement agile qui utilise un journal d’équipe et vous permet de créer des itérations à partir des tâches du journal, suivez les instructions de la section [Travailler dans un environnement agile](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifiez l’accès aux zones suivantes :</p> 
    <ul> 
     <li> <p>Projets</p> </li> 
     <li> <p>Rapports, tableaux de bord, calendriers</p> </li> 
     <li> <p>Filtres, Vues, Regroupements</p> </li> 
    </ul> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations pour le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Présentation des projets agiles

* [Fonctionnalité agile dans un projet](#agile-functionality-in-a-project)
* [Différences entre l’utilisation de la vue Agile d’un projet et celle d’une itération](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Fonctionnalité agile dans un projet {#agile-functionality-in-a-project}

La fonctionnalité agile suivante est disponible lors de la gestion d’un projet dans une vue agile :

* Statut d&#39;achèvement\
   Pour plus d’informations sur l’état d’achèvement, voir [Aperçu de l’état d’achèvement de l’itération](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Story board\
   Pour plus d’informations sur le tableau de bord, voir [Tableau de bord](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) .

Il existe des différences lors de l’utilisation de vues agiles sur un projet par rapport à un environnement agile pur (avec des logs et des itérations). Pour plus d’informations, voir [Différences entre l’utilisation de la vue Agile d’un projet et celle d’une itération](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) dans cet article.

### Différences entre l’utilisation de la vue Agile d’un projet et celle d’une itération {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Les tâches et les sous-tâches suivent différentes règles d’affichage sur le panorama des articles](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Les logs et itérations sont inutilisés](#backlogs-and-iterations-are-not-used)
* [L’ordre des tâches est conservé dans la vue Agile et ne peut pas être réorganisé.](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [Les tâches ne sont mesurées que dans les heures planifiées](#tasks-are-measured-only-in-planned-hours)
* [L’équipe agile n’est pas utilisée](#the-agile-team-is-not-used)
* [Chaque utilisateur du projet peut afficher le projet dans une vue Agile différente.](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Les tâches et les sous-tâches suivent différentes règles d’affichage sur le panorama des articles {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Les tâches qui n’ont pas de tâche parent ni de sous-tâche sont toujours affichées sous la forme d’une seule carte d’article sur le panorama d’articles.\
   Par exemple, ces tâches apparaissent comme suit dans la vue de liste des projets :

   ![Liste de projets agile : tâches sans parent ni sous-tâches](assets/agile-project-single-list-nwe.png) Ces tâches apparaissent comme suit dans la vue agile du projet :

   ![Vue agile du projet - tâches sans parent ni sous-tâches](assets/agile-project-singlecard-nwe.png)

* Les tâches parentes qui comportent des sous-tâches sont toujours affichées dans le **Histoires** de l’éditeur. Les sous-tâches sont affichées dans le couloir de la tâche parent.\
   Par exemple, ces tâches apparaissent comme suit dans la vue de liste des projets :

   ![Liste de projets agile : tâches avec des parents et des sous-tâches](assets/agile-project-parent-list-nwe.png)\
   Ces tâches apparaissent comme suit dans la vue agile du projet :

   ![Agile project view : tâches avec parents et sous-tâches](assets/agile-project-parent-nwe.png)

* Les sous-tâches de deuxième niveau (sous-tâches des sous-tâches) s’affichent sous la forme d’une carte grise suspendue de la tâche parent immédiate.
* Les sous-tâches de troisième niveau (sous-tâches de sous-tâches) ne s’affichent jamais sur le tableau de bord.

#### Les logs et itérations sont inutilisés {#backlogs-and-iterations-are-not-used}

Lors de l’affichage d’un projet dans une vue agile, les composants agiles suivants ne sont pas utilisés :

* **Backlog :** Aucun journal en souffrance n’est utilisé, car toutes les tâches du projet sont automatiquement affichées sous forme d’articles.
* **Itérations :** Plutôt que de créer des itérations pour définir les dates auxquelles le travail sera effectué, les jours actuellement désignés dans la chronologie du projet deviennent les jours ouvrés.

#### L’ordre des tâches est conservé dans la vue Agile et ne peut pas être réorganisé. {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

L’ordre dans lequel les tâches apparaissent dans un projet est conservé lorsque vous affichez le projet dans un tableau de bord agile.

Vous ne pouvez pas lire les tâches du projet lorsque vous le visualisez dans une vue agile. La modification de l’ordre des tâches pouvant affecter d’autres tâches pouvant avoir des dépendances, vous devez afficher le projet dans une vue standard afin de modifier l’ordre des tâches.

#### Les tâches ne sont mesurées que dans les heures planifiées {#tasks-are-measured-only-in-planned-hours}

Les tâches d’un projet sont toujours mesurées en heures planifiées.

Dans une itération, les tâches (histoires) peuvent être mesurées en heures ou en points.

#### L’équipe agile n’est pas utilisée {#the-agile-team-is-not-used}

Comme les équipes agiles terminent le travail sur les itérations qui leur sont affectées, les équipes agiles ne sont pas utilisées lors de l’affichage d’un projet dans une vue agile.

Au lieu de cela, tous les utilisateurs du projet deviennent l’équipe agile pour ce projet.

#### Chaque utilisateur du projet peut afficher le projet dans une vue Agile différente. {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

Contrairement à une itération agile, les utilisateurs d’un projet peuvent personnaliser la vue agile pour eux-mêmes, tandis que d’autres utilisateurs utilisent une vue agile différente.

Dans une itération agile, les informations disponibles sur le tableau de bord agile (telles que les colonnes d’état disponibles) sont déterminées au niveau de l’équipe.

Pour plus d’informations sur la personnalisation d’une vue agile, voir  [Création ou personnalisation d’une vue agile](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in  [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## Affichage d’un projet en mode Agile

1. Accédez au projet que vous souhaitez afficher dans une vue agile.
1. Cliquez sur le bouton **Agile** icône .\
   ![Icône Agile](assets/agile-icon-nwe.png)\
   Le projet s’affiche dans la vue agile par défaut.\
   Si vous avez précédemment affiché le projet dans une vue agile personnalisée, le projet s’affiche dans cette vue plutôt que dans la vue agile par défaut.

1. (Facultatif) Si vous avez créé une vue agile personnalisée, ou si un autre utilisateur a créé une vue agile personnalisée et l’a partagée avec vous, vous pouvez l’afficher à la place de la vue agile par défaut.\
   Cliquez sur le bouton **Affichage** menu déroulant, puis cliquez sur la vue agile personnalisée que vous souhaitez afficher.

   La vue agile personnalisée est utilisée la prochaine fois que vous cliquez sur le bouton **Agile** icône .\
   Pour plus d’informations sur la création d’une vue agile, voir [Créer et personnaliser des vues Agile](#create-and-customize-agile-views).\
   Le projet s’affiche dans la vue agile personnalisée.

1. (Conditionnel) Si les tâches de votre projet utilisent des états autres que &quot;Nouveau&quot;, &quot;En cours&quot; ou &quot;Terminé&quot; (états par défaut de la vue Agile), vous devez ajouter les états supplémentaires à la vue Agile pour que toutes les tâches de ces états s’affichent.\
   Si les tâches sont dans un état qui ne s’affiche pas sur le tableau de bord agile, la tâche elle-même ne s’affiche pas sur le tableau de bord agile (cependant, le pourcentage d’achèvement de ces tâches contribue toujours au pourcentage d’achèvement de toutes les tâches parentes et le pourcentage d’achèvement du projet global).\
   Pour ajouter des états à la vue agile, créez une vue agile ou personnalisez une vue agile existante, comme décrit dans la section &quot;Créer ou personnaliser une vue agile&quot; de l’article. [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Facultatif) Pour revenir au mode Liste, cliquez sur le bouton **Liste** icône .\
   ![](assets/list-icon.png)

## Créer et personnaliser des vues Agile {#create-and-customize-agile-views}

Comme pour les vues standard dans Workfront, vous pouvez personnaliser les vues agiles existantes ou créer de nouvelles vues agiles à partir de zéro. Contrairement aux vues standard, vous ne pouvez pas créer de vues agiles basées sur des vues agiles existantes.

Pour plus d’informations sur la création et la personnalisation des vues agiles, voir la section &quot;Créer ou personnaliser une vue agile&quot; de l’article. [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## Partage d’une vue Agile existante

Pour plus d’informations sur le partage d’une vue agile, voir [Partage d’un filtre, d’une vue ou d’un regroupement](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Suppression d’une vue agile existante

Pour plus d’informations sur la suppression d’une vue, voir la section &quot;Supprimer une vue&quot; de l’article [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 
