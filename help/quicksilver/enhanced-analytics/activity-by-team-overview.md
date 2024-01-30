---
title: Visualisation de l’activité par équipe dans les analyses améliorées
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualisation Activité par équipe présente les activités qui se produisent pendant une période spécifique pour une équipe d’accueil, ce qui vous permet de comprendre comment différentes équipes d’accueil ont passé leur temps dans Adobe Workfront. Selon la configuration de votre équipe d’accueil dans Workfront, cette visualisation peut vous donner différentes informations et répondre à différentes questions.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Visualisation de l’activité par équipe dans les analyses améliorées

<!-- Audited: 12/2023 -->

La visualisation Activité par équipe présente les activités qui se produisent pendant une période spécifique pour une équipe d’accueil, ce qui vous permet de comprendre comment différentes équipes d’accueil ont passé leur temps dans Adobe Workfront. Selon la configuration de votre équipe d’accueil dans Workfront, cette visualisation peut vous donner différentes informations et répondre à différentes questions.

>[!NOTE]
>
>La visualisation de l’activité Projet est similaire à cette visualisation, mais elle affiche l’activité en fonction des personnes affectées à des projets plutôt que des personnes affectées à une équipe d’accueil.\
>Pour plus d’informations sur la visualisation de l’activité de projet, voir [Visualisation de l’activité de projet dans les analyses améliorées](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png){width="700"}

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Formule Workfront</a></td> 
   <td> <p>Professionnel ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a></td> 
   <td>
      <p>Nouveau :</p> 
         <ul><li>Clair ou plus élevé</li></ul>
      <p>Actuel :</p>
         <ul><li>Révision ou version ultérieure</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Affichage de l’accès aux projets</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Pour connaître les conditions préalables à l’utilisation d’Analytics amélioré, reportez-vous à la section &quot;Conditions préalables&quot; de la section [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Présentation de la visualisation de l’activité par équipe

Les différentes activités s’affichent dans différentes couleurs pour résumer des événements spécifiques sur la période filtrée :

* **Utilisateurs connectés**: les zones violettes indiquent que les membres de l’équipe d’accueil se sont connectés ce jour-là. Une ombre plus sombre indique un nombre plus élevé de personnes se connectant.

  ![](assets/project-activity-users-logged-in.png)

* **Modification de l’état de la tâche**: des cases roses montrent que les membres de l’équipe d’accueil ont modifié l’état d’une tâche ce jour-là. Une nuance plus foncée indique un nombre plus élevé de statuts de tâche changeant.

  ![](assets/project-activity-task-status-changes.png)

* **Tâches terminées**: les cases bleues indiquent que les membres de l’équipe d’accueil ont effectué une tâche ce jour-là. Une nuance plus foncée indique un nombre plus élevé de tâches en cours d’exécution.

  ![](assets/project-activity-tasks-completed.png)

Le survol d’une zone indique le nombre exact de fois où l’action a été effectuée au cours d’un jour donné. Vous pouvez sélectionner une équipe pour afficher la ventilation de ces activités par personne au sein de l’équipe d’accueil.

L’affichage de ces informations vous permet de déterminer les éléments suivants :

* Activités se déroulant au sein d’une équipe d’accueil et à quelle fréquence.
* Ce que les équipes domestiques sont surchargées ou utilisent plus le système.
* Si la répartition du travail est appropriée pour l’équipe d’accueil.

Pour savoir comment obtenir les meilleures données pour cette visualisation, voir [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisation de l’activité par équipe

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon-16x12.png), puis sélectionnez **Analytics**.
1. Dans le panneau de gauche, sélectionnez **Personnes**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre de période.

   ![](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Conditionnel) Si vous n’avez pas défini le filtre Équipe, ajoutez le filtre Équipe et sélectionnez chaque équipe pour laquelle vous souhaitez afficher des données.

   Pour plus d’informations sur l’ajout de filtres dans les analyses améliorées, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois que vous avez ajouté des filtres, les données de 50 projets au maximum s’affichent et les filtres restent actifs même après avoir quitté la page ou vous être déconnecté de Workfront.

1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période et faites glisser le curseur jusqu’à la fin de la période.

   Toutes les autres visualisations se mettent à jour sur la même période et un filtre de période est créé.

   ![](assets/timeframe-filter-350x220.png)

1. Clic sur le nom d’une équipe

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   pour afficher plus de détails sur les activités terminées par l’équipe d’accueil.

   La liste se développe pour afficher les activités de chaque personne affectée à l’équipe d’accueil.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Pointez sur une zone colorée pour afficher la date à laquelle les utilisateurs ont terminé une action, ainsi que le nombre de fois où l’action a été terminée cette journée.

   Des couleurs plus foncées indiquent une activité plus élevée.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur l’icône Exporter . ![](assets/export.png) dans le coin supérieur droit de la visualisation, sélectionnez le format d’exportation :

   * **Graphique (PNG)**
   * **Tableau de données (XSLX)**

