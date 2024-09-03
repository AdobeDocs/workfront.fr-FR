---
title: Afficher la visualisation Activité par équipe dans l’analytique améliorée
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualisation Activité par équipe présente les activités qui se produisent pendant une période spécifique pour une équipe interne, ce qui vous permet de comprendre comment différentes équipes internes ont passé leur temps dans Adobe Workfront. Selon la configuration de votre équipe interne dans Workfront, cette visualisation peut vous donner différentes informations et répondre à différentes questions.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 100%

---

# Afficher la visualisation Activité par équipe dans l’analytique améliorée

<!-- Audited: 12/2023 -->

La visualisation Activité par équipe présente les activités qui se produisent pendant une période spécifique pour une équipe interne, ce qui vous permet de comprendre comment différentes équipes internes ont passé leur temps dans Adobe Workfront. Selon la configuration de votre équipe interne dans Workfront, cette visualisation peut vous donner différentes informations et répondre à différentes questions.

>[!NOTE]
>
>La visualisation de l’activité de projet est similaire à cette visualisation, mais elle affiche l’activité en fonction des personnes affectées à des projets plutôt que des personnes affectées à une équipe interne.\
>Pour plus d’informations sur la visualisation de l’activité de projet, voir [Afficher la visualisation de l’activité de projet dans l’analytique améliorée](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png){width="700"}

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans?lang=fr" target="_blank">Plan Workfront</a></td> 
   <td> <p>Entreprises ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe Workfront</a></td> 
   <td>
      <p>Nouveau :</p> 
         <ul><li>Light ou supérieur</li></ul>
      <p>Actuel :</p>
         <ul><li>Révision ou supérieur</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Afficher l’accès aux projets</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytique améliorée, reportez-vous à la section « Conditions préalables » de la section [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Comprendre la visualisation Activité par équipe

Les différentes activités s’affichent dans différentes couleurs pour résumer des événements spécifiques sur la période filtrée 

* **Personnes connectées dans** : les cases violettes indiquent que les personnes membres de l’équipe interne se sont connectées ce jour-là. Une nuance plus sombre indique un nombre plus élevé de personnes se connectant.

  ![](assets/project-activity-users-logged-in.png)

* **Changement de statut d’une tâche** : les cases roses indiquent que les personnes membres de l’équipe interne ont modifié le statut d’une tâche ce jour-là. Une nuance plus foncée indique un nombre plus élevé de changements de statut d’une tâche.

  ![](assets/project-activity-task-status-changes.png)

* **Tâches terminées** : les cases bleues indiquent que les personnes membres de l’équipe interne ont terminé une tâche ce jour-là. Une nuance plus foncée indique un nombre plus élevé de tâches terminées.

  ![](assets/project-activity-tasks-completed.png)

En pointant sur une case, vous pouvez voir le nombre exact de fois où l’action a été effectuée au cours d’un jour donné. Vous pouvez sélectionner une équipe pour afficher la répartition de ces activités par personne au sein de l’équipe interne.

Ces informations vous aident à déterminer :

* Les activités qui se produisent au sein d’une équipe interne et leur fréquence.
* Les équipes internes qui sont surchargées ou utilisent davantage le système.
* Si la répartition du travail est appropriée pour l’équipe domestique.

Pour savoir comment obtenir les meilleures données pour cette visualisation, voir [Vue d’ensemble d’Analytique améliorée](../enhanced-analytics/enhanced-analytics-overview.md).

## Afficher la visualisation d’activité par équipe

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon-16x12.png), puis sélectionnez **Analyse**.
1. Dans le panneau de gauche, sélectionnez **Personnes**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre des périodes.

   ![](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, voir [Appliquer des filtres dans l’analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Le cas échéant) Si vous n’avez pas défini votre filtre d’équipe, ajoutez-le et sélectionnez chaque équipe dont vous souhaitez voir les données.

   Pour plus d’informations sur l’ajout de filtres dans Analytique améliorée, voir la section [Appliquer des filtres dans Analytique améliorée](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois les filtres ajoutés, les données de 50 projets au maximum s’affichent et les filtres restent actifs même lorsque vous quittez la page ou en cas de déconnexion de Workfront.

1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période, puis faites-le glisser jusqu’à la fin de la période.

   Toutes les autres visualisations sont mises à jour sur la même période et un filtre de délai est créé.

   ![](assets/timeframe-filter-350x220.png)

1. Cliquez sur le nom d’une équipe

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   pour afficher plus de détails sur les activités terminées par l’équipe interne.

   La liste se développe pour afficher les activités de chaque personne affectée à l’équipe interne.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Pointez sur une zone colorée pour afficher la date à laquelle les personnes ont terminé une action, ainsi que le nombre de fois où l’action a été terminée cette journée.

   Des couleurs plus foncées indiquent une activité plus élevée.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur l’icône Exporter ![](assets/export.png) dans le coin supérieur droit de la visualisation, sélectionnez le format d’exportation :

   * **Graphique (PNG)**
   * **Table de données (XSLX)**

