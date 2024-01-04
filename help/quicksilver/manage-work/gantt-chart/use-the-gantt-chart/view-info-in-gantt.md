---
navigation-topic: use-the-gantt-chart
title: Afficher les informations dans le  [!UICONTROL Graphique Gantt]
description: Le diagramme de Gantt de la liste des tâches et le diagramme de Gantt de la liste des projets affichent des informations sur les projets et les tâches.
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# Afficher les informations dans le  [!UICONTROL Graphique Gantt]

La liste des tâches [!UICONTROL Graphique Gantt] et liste des projets [!UICONTROL Graphique Gantt] afficher des informations sur les projets et les tâches.

## Exigences d’accès

Pour suivre les étapes de cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Quelconque </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Présentation des licences*</td> 
   <td> <p>[!UICONTROL Review] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès à [!UICONTROL View] ou supérieur à Projects and Tasks</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur au projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Recherchez la variable  [!UICONTROL Graphique Gantt]

Vous pouvez localiser le diagramme de Gantt de la liste des tâches et la liste des projets. [!UICONTROL Graphique Gantt] de plusieurs zones dans Workfront. Pour plus d’informations, voir [Prise en main de la fonction [!UICONTROL Graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

## Afficher les tâches sur la page [!UICONTROL Chemin critique]

Dans la liste des projets [!UICONTROL Graphique Gantt], les tâches qui ne figurent pas sur la variable [!UICONTROL Chemin critique] s’affichent sous la forme de lignes horizontales bleu clair. Tâches qui se trouvent sur la page [!UICONTROL Chemin critique] d’un projet s’affiche sous la forme de lignes horizontales rouges.

Pour plus d’informations sur les tâches de la variable [!UICONTROL Chemin critique], voir [Présentation du projet [!UICONTROL Chemin critique]](../../../manage-work/tasks/manage-tasks/critical-path.md).

## Affichage des informations sur la tâche dans la liste des projets [!UICONTROL Graphique Gantt]

Vous pouvez afficher les informations sur la tâche d’un projet directement à partir de la liste des projets. Les tâches sont répertoriées sous le nom de chaque projet.

>[!NOTE]
>
>Vous ne pouvez pas modifier des tâches à partir de la liste des projets. [!UICONTROL Graphique Gantt].

Vous pouvez afficher les informations de tâche d’un projet directement à partir d’une liste de projets dans les zones suivantes :

* Dans le [!UICONTROL Projets] area
* Dans un Portfolio
* Dans un programme

Pour afficher les tâches d’un projet à partir d’une liste de projets :

1. Accédez à l’une des zones mentionnées ci-dessus.

   Par exemple, à partir de la variable [!UICONTROL Menu Principal], cliquez sur **[!UICONTROL Projets]**.

   Une liste de projets s’affiche.

1. Cliquez sur le bouton **[!UICONTROL Graphique Gantt]** icon ![](assets/gantt-icon-nwe.png) dans le coin supérieur droit de l’écran.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. Cliquez sur le bouton **[!UICONTROL Afficher la liste des tâches]** Icône

1. Dans la liste des projets située à gauche, cliquez sur la flèche de liste déroulante en regard du nom du projet pour afficher toutes les tâches qu’il contient.\
   Cette opération affiche les informations sur la tâche dans la variable  [!UICONTROL Graphique Gantt].\
   ![Show_task_list_enabled_project_expand.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. (Facultatif) Cliquez sur le **[!UICONTROL Imprimer]** dans le coin supérieur droit pour exporter le [!UICONTROL Graphique Gantt].

   >[!NOTE]
   >
   >Liste des projets [!UICONTROL Graphique Gantt] exporte uniquement les projets. Les informations sur la tâche ne sont pas incluses.

## Modifier la période pour laquelle les informations s’affichent dans la variable [!UICONTROL Graphique Gantt]

Vous pouvez ajuster la période affichée sur la page [!UICONTROL Graphique Gantt] pour afficher les informations à un niveau granulaire, vous pouvez également accéder rapidement à un affichage par jour, semaine, mois, trimestre ou année :

* [Modifier la période à un niveau granulaire](#change-the-time-period-on-a-granular-level)
* [Affichage des informations par jour, semaine, mois, trimestre ou année](#view-information-by-day-week-month-quarter-or-year)

### Modifier la période à un niveau granulaire {#change-the-time-period-on-a-granular-level}

1. Passez la souris sur la chronologie de  [!UICONTROL Graphique Gantt], puis faites glisser l’indicateur de zoom de gauche à droite pour développer ou contracter la chronologie.\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### Affichage des informations par jour, semaine, mois, trimestre ou année {#view-information-by-day-week-month-quarter-or-year}

1. Dans le  [!UICONTROL Graphique Gantt], cliquez sur le menu déroulant de la période.

   ![](assets/timeline-options.png)

1. Sélectionnez une période parmi les options disponibles suivantes :

   * **[!UICONTROL Ajuster tout]**: cette option affiche la chronologie de l’ensemble du projet.
   * **[!UICONTROL Tous les projets]**: cette option est disponible uniquement dans le diagramme de Gantt de liste de projets.
   * **[!UICONTROL Année]**
   * **[!UICONTROL Trimestre]**
   * **[!UICONTROL Mois]**
   * **[!UICONTROL Semaine]**
   * **[!UICONTROL Jour]**

1. (Facultatif) Sélectionnez une période plus granulaire, telle que [!UICONTROL Semaine] ou [!UICONTROL Jour], puis cliquez et faites glisser la barre de défilement horizontale au bas de la  [!UICONTROL Graphique Gantt] pour passer de gauche à droite sur la ligne de temps du projet.\
   instantané de la chronologie de la variable [!UICONTROL Gantt] s’affiche pour afficher l’intégralité du projet.

   >[!TIP]
   >
   >L’instantané de la chronologie ne s’affiche qu’après avoir cliqué sur la barre de défilement horizontale.

   ![extended_gantt_minimap_with_composition__1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. (Facultatif) Cliquez n’importe où dans l’instantané de la ligne temporelle pour accéder à un point spécifique de la durée du projet.\
   Ou\
   Faites glisser les poignées de la visionneuse d’instantanés pour sélectionner une période spécifique afin de l’afficher dans la fenêtre principale. [!UICONTROL Gantt].

## Utilisation de filtres, de vues et de regroupements

La variable [!UICONTROL Graphique Gantt] est une représentation visuelle des informations actuellement affichées dans la liste des tâches. Vous pouvez appliquer des filtres, des vues et des regroupements aux objets répertoriés dans les deux [!UICONTROL Graphique Gantt]s.

>[!CAUTION]
>
>Vous ne pouvez pas appliquer de filtres, de vues et de groupements lorsque vous sélectionnez [!UICONTROL Manuel] save [!UICONTROL Planification chronologique] pour enregistrer les modifications apportées à votre liste de tâches. Pour plus d’informations sur l’enregistrement des modifications apportées aux tâches dans une liste, voir [Editer les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Les filtres et les regroupements que vous appliquez à la liste sont répercutés à la fois sur la liste des projets et la liste des tâches.  [!UICONTROL Graphique Gantt]s et sont également inclus lors de l’exportation des graphiques Gantt :

* Filtres\
   Vous pouvez appliquer un Filtre à la liste afin de contrôler les informations affichées dans la variable [!UICONTROL Graphique Gantt].\
   Pour plus d’informations sur l’application d’un filtre, voir  [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Regroupements\
   Les regroupements que vous appliquez à la liste sont répercutés sur le [!UICONTROL Graphique Gantt].\
   Pour plus d’informations sur l’application d’un groupement, voir  [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Les vues ne sont pas reflétées dans la variable [!UICONTROL Graphique Gantt]. Cependant, lorsque vous exportez le [!UICONTROL Graphique Gantt] (comme décrit dans la section  [Exportez le [!UICONTROL Graphique Gantt] vers le PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)), la liste des tâches est exportée en plus de la fonction [!UICONTROL Graphique Gantt], avec l’affichage actif appliqué à la liste.

## Configuration des options d’affichage

Vous pouvez choisir le type d’informations qui s’affiche dans les deux [!UICONTROL Graphiques Gantt]. Pour plus d’informations, voir [Configurez l’affichage des informations sur le [!UICONTROL Graphique Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).
