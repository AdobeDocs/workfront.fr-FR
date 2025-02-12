---
navigation-topic: use-the-gantt-chart
title: Afficher les informations dans le [!UICONTROL graphique de Gantt]
description: Le graphique de Gantt de la liste des tâches et le graphique de Gantt de la liste des projets affichent des informations sur les projets et les tâches.
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 98%

---

# Afficher les informations dans le [!UICONTROL graphique de Gantt]

Le [!UICONTROL graphique de Gantt] de la liste des tâches et le [!UICONTROL graphique de Gantt] de la liste des projets affichent des informations sur les projets et les tâches.

## Conditions d’accès

Vous devez disposer des éléments suivants pour suivre les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Vue d’ensemble des licences*</td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur aux projets et aux tâches.</p> <p><b>NOTE</b>

Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour plus d’informations sur la manière dont un un administrateur ou une administratrice de [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès [!UICONTROL View] ou un accès supérieur au projet.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez l’administration de [!DNL Workfront].

## Localiser le [!UICONTROL graphique de Gantt]

Vous pouvez localiser le graphique de Gantt de la liste des tâches et le [!UICONTROL graphique de Gantt] de la liste des projets dans plusieurs zones dans Workfront. Pour plus d’informations, voir [Commencer avec le [!UICONTROL graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

## Afficher les tâches sur le [!UICONTROL chemin critique]

Dans le [!UICONTROL graphique de Gantt] de la liste des projets, les tâches qui ne figurent pas sur le [!UICONTROL chemin critique] s’affichent sous la forme de lignes horizontales bleu clair. Les tâches qui se trouvent sur le [!UICONTROL chemin critique] d’un projet s’affichent sous la forme de lignes horizontales rouges.

Pour plus d’informations sur les tâches se trouvant sur le [!UICONTROL chemin critique], voir [Vue d’ensemble du [!UICONTROL chemin critique du projet]](../../../manage-work/tasks/manage-tasks/critical-path.md).

## Afficher des informations sur la tâche dans le [!UICONTROL graphique de Gantt] de la liste des projets

Vous pouvez afficher des informations sur la tâche d’un projet directement à partir de la liste des projets. Les tâches sont répertoriées sous le nom de chaque projet.

>[!NOTE]
>
>Vous ne pouvez pas modifier des tâches à partir du [!UICONTROL graphique de Gantt] de la liste des projets.

Vous pouvez afficher des informations sur la tâche d’un projet directement à partir d’une liste de projets dans les zones suivantes :

* Dans la zone [!UICONTROL Projets]
* Dans un portfolio
* Dans un programme

Pour afficher les tâches d’un projet à partir d’une liste de projets, procédez comme suit :

1. Accédez à l’une des zones mentionnées ci-dessus.

   Par exemple, à partir du [!UICONTROL Menu principal], cliquez sur **[!UICONTROL Projets]**.

   Une liste de projets s’affiche.

1. Cliquez sur l’icône **[!UICONTROL Graphique Gantt]** ![Icône Gantt](assets/gantt-icon-nwe.png) dans le coin supérieur droit de l’écran.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. Cliquez sur l’icône **[!UICONTROL Afficher la liste des tâches]**.

1. Dans la liste des projets située à gauche, cliquez sur la flèche de liste déroulante en regard du nom du projet pour afficher toutes les tâches qu’il contient.\
   Cette opération affiche des informations concernant la tâche sur le [!UICONTROL graphique de Gantt].\
   ![Show_task_list_enabled_project_expand.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Imprimer]** dans le coin supérieur droit pour exporter le [!UICONTROL graphique de Gantt].

   >[!NOTE]
   >
   >Le [!UICONTROL graphique de Gantt] de la liste des projets exporte uniquement les projets. Les informations sur les tâches ne sont pas incluses.

## Modifier la période pour laquelle les informations s’affichent dans le [!UICONTROL graphique de Gantt]

Vous pouvez ajuster la période affichée sur le [!UICONTROL graphique de Gantt] pour voir les informations à un niveau granulaire, ou vous pouvez accéder rapidement à un affichage par jour, semaine, mois, trimestre ou année :

* [Modifier la période à un niveau granulaire](#change-the-time-period-on-a-granular-level)
* [Afficher des informations par jour, semaine, mois, trimestre ou année](#view-information-by-day-week-month-quarter-or-year)

### Modifier la période à un niveau granulaire {#change-the-time-period-on-a-granular-level}

1. Pointez sur la chronologie du [!UICONTROL graphique de Gantt], puis faites glisser l’indicateur de zoom de gauche à droite pour développer ou contracter la chronologie.\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### Afficher des informations par jour, semaine, mois, trimestre ou année {#view-information-by-day-week-month-quarter-or-year}

1. Dans le [!UICONTROL graphique de Gantt], cliquez sur le menu déroulant de la période.

   ![Options de chronologie](assets/timeline-options.png)

1. Sélectionnez une période parmi les options disponibles suivantes :

   * **[!UICONTROL Tout adapter]** : cette option affiche la chronologie de l’ensemble du projet.
   * **[!UICONTROL Tous les projets]** : cette option est disponible uniquement dans le graphique de Gantt de liste de projets.
   * **[!UICONTROL Année]**
   * **[!UICONTROL Trimestre]**
   * **[!UICONTROL Mois]**
   * **[!UICONTROL Semaine]**
   * **[!UICONTROL Jour]**

1. (Facultatif) Sélectionnez une période plus granulaire, telle que [!UICONTROL Semaine] ou [!UICONTROL Jour], puis cliquez et faites glisser la barre de défilement horizontale au bas du [!UICONTROL graphique de Gantt] pour vous déplacer de gauche à droite sur la chronologie du projet.\
   Un instantané de chronologie du [!UICONTROL graphique de Gantt] s’affiche pour montrer l’intégralité du projet.

   >[!TIP]
   >
   >L’instantané de chronologie ne s’affiche qu’après que vous avez cliqué sur la barre de défilement horizontale.

   ![extended_gantt_minimap_with_composition__1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. (Facultatif) Cliquez n’importe où dans l’instantané de chronologie pour accéder à un point spécifique de la durée du projet.\
   Ou\
   Faites glisser les poignées de la visionneuse d’instantanés pour sélectionner une période spécifique afin de l’afficher dans le [!UICONTROL graphique de Gantt] principal.

## Utiliser des filtres, des vues et des regroupements

Le [!UICONTROL graphique de Gantt] est une représentation visuelle des informations actuellement affichées dans la liste des tâches. Vous pouvez appliquer des filtres, des vues et des regroupements aux objets répertoriés dans les deux [!UICONTROL graphiques de Gantt].

>[!CAUTION]
>
>Vous ne pouvez pas appliquer de filtres, de vues et de regroupements lorsque vous sélectionnez l’enregistrement [!UICONTROL manuel] du [!UICONTROL planning de la chronologie] pour enregistrer les modifications apportées à votre liste de tâches. Pour plus d’informations sur l’enregistrement des modifications apportées aux tâches dans une liste, voir [Modifier les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Les filtres et les regroupements que vous appliquez à la liste sont répercutés à la fois sur les [!UICONTROL graphiques de Gantt] de la liste des projets et de la liste des tâches, et sont également inclus lors de l’export des graphiques Gantt :

* Filtres\
   Vous pouvez appliquer un filtre à la liste afin de contrôler les informations affichées dans le [!UICONTROL graphique de Gantt].\
   Pour plus d’informations sur l’application d’un filtre, voir [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Regroupements\
   Les regroupements que vous appliquez à la liste sont répercutés sur le [!UICONTROL graphique de Gantt].\
   Pour plus d’informations sur l’application d’un regroupement, voir [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Les vues ne sont pas reflétées dans le [!UICONTROL graphique de Gantt]. Cependant, lorsque vous exportez le [!UICONTROL graphique de Gantt] (comme décrit dans la section [Exporter le [!UICONTROL graphique de Gantt] au format PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)), la liste des tâches est exportée en plus du [!UICONTROL graphique de Gantt], avec la Vue actuelle appliquée à la liste.

## Configurer les options d’affichage

Vous pouvez choisir le type d’informations qui s’affiche dans les deux [!UICONTROL graphiques de Gantt]. Pour plus d’informations, voir [Configurer l’affichage des informations sur le [!UICONTROL graphique de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).
