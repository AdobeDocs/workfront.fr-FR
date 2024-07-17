---
navigation-topic: use-the-gantt-chart
title: Afficher les informations dans le [!UICONTROL diagramme de Gantt]
description: Le diagramme de Gantt de la liste des tâches et le diagramme de Gantt de la liste des projets affichent des informations sur les projets et les tâches.
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 8%

---

# Afficher les informations dans le [!UICONTROL diagramme de Gantt]

La liste des tâches [!UICONTROL Gantt Chart] et la liste des projets [!UICONTROL Gantt Chart] affichent des informations sur les projets et les tâches.

## Conditions d’accès

Pour suivre les étapes de cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Présentation des licences*</td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès à [!UICONTROL View] ou supérieur à Projects and Tasks</p> <p><b>NOTE</b>

Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Localisez le [!UICONTROL diagramme de Gantt]

Vous pouvez localiser le diagramme Gantt de la liste des tâches et le [!UICONTROL diagramme de Gantt] de plusieurs zones dans Workfront. Pour plus d’informations, voir [Prise en main du [!UICONTROL diagramme de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

## Afficher les tâches sur le [!UICONTROL chemin critique]

Dans la liste des projets [!UICONTROL Graphique de Gantt], les tâches qui ne se trouvent pas sur le [!UICONTROL chemin critique] s’affichent sous forme de lignes horizontales bleu clair. Les tâches qui se trouvent sur le [!UICONTROL chemin critique] d’un projet s’affichent sous la forme de lignes horizontales rouges.

Pour plus d’informations sur les tâches sur le [!UICONTROL chemin critique], voir [Présentation du projet [!UICONTROL chemin critique]](../../../manage-work/tasks/manage-tasks/critical-path.md).

## Afficher les informations sur la tâche dans la liste de projets [!UICONTROL Graphique de Gantt]

Vous pouvez afficher les informations sur la tâche d’un projet directement à partir de la liste des projets. Les tâches sont répertoriées sous le nom de chaque projet.

>[!NOTE]
>
>Vous ne pouvez pas modifier les tâches à partir de la liste de projets [!UICONTROL Graphique de Gantt].

Vous pouvez afficher les informations de tâche d’un projet directement à partir d’une liste de projets dans les zones suivantes :

* Dans la zone [!UICONTROL Projects]
* Dans un Portfolio
* Dans un programme

Pour afficher les tâches d’un projet à partir d’une liste de projets :

1. Accédez à l’une des zones mentionnées ci-dessus.

   Par exemple, dans le [!UICONTROL menu principal], cliquez sur **[!UICONTROL Projets]**.

   Une liste de projets s’affiche.

1. Cliquez sur l’icône **[!UICONTROL Gantt chart]** ![](assets/gantt-icon-nwe.png) dans le coin supérieur droit de l’écran.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. Cliquez sur l’icône **[!UICONTROL Afficher la liste des tâches]** .

1. Dans la liste des projets située à gauche, cliquez sur la flèche de liste déroulante en regard du nom du projet pour afficher toutes les tâches qu’il contient.\
   Cela affiche les informations sur la tâche sur le [!UICONTROL diagramme de Gantt].\
   ![Show_task_list_enabled_project_expand.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Imprimer]** dans le coin supérieur droit pour exporter le [!UICONTROL diagramme de Gantt].

   >[!NOTE]
   >
   >La liste de projets [!UICONTROL Gantt Chart] exporte uniquement les projets. Les informations sur la tâche ne sont pas incluses.

## Modifier la période pour laquelle les informations s’affichent dans le [!UICONTROL diagramme de Gantt]

Vous pouvez ajuster la période affichée sur le [!UICONTROL diagramme de Gantt] pour afficher les informations à un niveau granulaire, ou vous pouvez rapidement accéder à un affichage par jour, semaine, mois, trimestre ou année :

* [Modifier la période à un niveau granulaire](#change-the-time-period-on-a-granular-level)
* [Affichage des informations par jour, semaine, mois, trimestre ou année](#view-information-by-day-week-month-quarter-or-year)

### Modifier la période à un niveau granulaire {#change-the-time-period-on-a-granular-level}

1. Passez la souris sur la chronologie du [!UICONTROL diagramme de Gantt], puis faites glisser l’indicateur de zoom de gauche à droite pour développer ou contracter la chronologie.\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### Affichage des informations par jour, semaine, mois, trimestre ou année {#view-information-by-day-week-month-quarter-or-year}

1. Dans le [!UICONTROL diagramme de Gantt], cliquez sur le menu déroulant de la période.

   ![](assets/timeline-options.png)

1. Sélectionnez une période parmi les options disponibles suivantes :

   * **[!UICONTROL Ajuster tout]** : cette option affiche la chronologie de l’ensemble du projet.
   * **[!UICONTROL Tous les projets]** : cette option est disponible uniquement dans le diagramme de Gantt de liste de projets.
   * **[!UICONTROL Year]**
   * **[!UICONTROL Trimestre]**
   * **[!UICONTROL Mois]**
   * **[!UICONTROL Semaine]**
   * **[!UICONTROL Jour]**

1. (Facultatif) Sélectionnez une période plus granulaire, telle que [!UICONTROL Semaine] ou [!UICONTROL Jour], puis cliquez et faites glisser la barre de défilement horizontale au bas du [!UICONTROL Diagramme de Gantt] pour vous déplacer vers la gauche sur la ligne horaire du projet.\
   Un instantané de la chronologie du [!UICONTROL Gantt] s’affiche pour afficher l’ensemble du projet.

   >[!TIP]
   >
   >L’instantané de la chronologie ne s’affiche qu’après avoir cliqué sur la barre de défilement horizontale.

   ![étendu_gantt_minimap_with_composition__1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. (Facultatif) Cliquez n’importe où dans l’instantané de la ligne temporelle pour accéder à un point spécifique de la durée du projet.\
   Ou\
   Faites glisser les poignées de la visionneuse d’instantanés pour sélectionner une période spécifique afin de l’afficher dans le [!UICONTROL Gantt] principal.

## Utilisation de filtres, de vues et de regroupements

Le [!UICONTROL diagramme de Gantt] est une représentation visuelle des informations actuellement affichées dans la liste des tâches. Vous pouvez appliquer des filtres, des vues et des regroupements aux objets répertoriés dans les [!UICONTROL graphiques de Gantt].

>[!CAUTION]
>
>Vous ne pouvez pas appliquer de filtres, de vues et de regroupements lorsque vous sélectionnez [!UICONTROL Manuel] enregistrer [!UICONTROL  la planification de la chronologie] pour enregistrer les modifications apportées à votre liste de tâches. Pour plus d’informations sur l’enregistrement des modifications apportées aux tâches dans une liste, voir [Modifier les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Les filtres et les regroupements que vous appliquez à la liste sont répercutés à la fois sur la liste des projets et la liste des tâches [!UICONTROL Graphique de Gantt] et sont également inclus lors de l’exportation des graphiques de Gantt :

* Filtres\
   Vous pouvez appliquer un filtre à la liste afin de contrôler les informations affichées dans le [!UICONTROL diagramme de Gantt].\
   Pour plus d’informations sur l’application d’un filtre, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Regroupements\
   Les groupes que vous appliquez à la liste sont répercutés sur le [!UICONTROL diagramme de Gantt].\
   Pour plus d’informations sur l’application d’un groupement, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Les vues ne sont pas reflétées dans le [!UICONTROL diagramme de Gantt]. Cependant, lorsque vous exportez le [!UICONTROL diagramme de Gantt] (comme décrit dans la section [Exporter le [!UICONTROL diagramme de Gantt] vers le PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)), la liste des tâches est exportée en plus du [!UICONTROL diagramme de Gantt], avec la vue actuelle appliquée à la liste.

## Configuration des options d’affichage

Vous pouvez choisir le type d’informations qui s’affiche dans les [!UICONTROL Graphiques de Gantt]. Pour plus d’informations, voir [Configuration de l’affichage des informations sur le [!UICONTROL diagramme de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).
