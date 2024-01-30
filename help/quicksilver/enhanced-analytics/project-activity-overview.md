---
title: Visualisation de l’activité de projet dans les analyses améliorées
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: La visualisation de l’activité de projet affiche une vue globale des activités au niveau du projet (les activités de chaque personne affectée au projet) qui se sont produites au cours d’une période spécifique. Vous pouvez vous concentrer sur les activités d’un projet ou comparer les activités d’un projet à d’autres projets dans Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Visualisation de l’activité de projet dans les analyses améliorées

<!-- Audited: 12/2023 -->

La visualisation de l’activité de projet affiche une vue globale des activités au niveau du projet (les activités de chaque personne affectée au projet) qui se sont produites au cours d’une période spécifique. Vous pouvez vous concentrer sur les activités d’un projet ou comparer les activités d’un projet à d’autres projets dans Adobe Workfront.

>[!NOTE]
>
>La visualisation Activité par équipe se comporte de la même manière que cette visualisation, mais la visualisation Activité par équipe affiche l’activité de l’équipe d’accueil pour tous les projets.\
>Pour plus d’informations sur la visualisation de l’activité par équipe, voir [Visualisation de l’activité par équipe dans les analyses améliorées](../enhanced-analytics/activity-by-team-overview.md).

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
   <td>   <p>Nouveau :</p> 
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

## Présentation de la visualisation de l’activité de projet

Les activités du projet s’affichent de différentes couleurs pour résumer des événements spécifiques d’un projet sur une période donnée :

* **Utilisateurs connectés**: les zones violettes indiquent que les personnes affectées au projet se sont connectées ce jour-là. Une ombre plus sombre indique un nombre plus élevé de personnes se connectant.

  ![](assets/project-activity-users-logged-in.png)

* **Modification de l’état de la tâche**: des zones roses montrent que des personnes ont modifié l’état d’une tâche pour le projet ce jour-là. Une nuance plus foncée indique un nombre plus élevé de statuts de tâche changeant.

  ![](assets/project-activity-task-status-changes.png)

* **Tâches terminées**: les zones bleues indiquent que les personnes ont effectué une tâche pour le projet. Une nuance plus foncée indique un nombre plus élevé de tâches en cours d’exécution.

  ![](assets/project-activity-tasks-completed.png)

Le survol d’une zone indique le nombre exact de fois où l’action a été effectuée au cours d’un jour donné. Vous pouvez sélectionner un projet pour afficher la ventilation de ces activités par chaque contributeur individuel du projet.

L’affichage de ces informations vous permet de déterminer les éléments suivants :

* L’activité sur un projet spécifique.
* Activité d’un projet par rapport à d’autres projets.
* Quels utilisateurs travaillent sur un projet et à quelle fréquence ?

Pour savoir comment obtenir les meilleures données pour cette visualisation, voir [Présentation des analyses améliorées](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisation de l’activité Projet

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon-16x12.png), puis sélectionnez **Analytics**.
1. (Facultatif) Pour utiliser une autre période, sélectionnez de nouvelles dates de début et de fin dans le filtre de période.

   ![](assets/filters-select-date-range-350x344.png)

   Pour plus d’informations sur l’utilisation du filtre de période, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Si vous sélectionnez une période supérieure à 3 mois, la visualisation de l’activité de projet n’affiche aucune donnée.

1. (Conditionnel) Si vous devez limiter l’ensemble de données du projet, sélectionnez les filtres à utiliser et appliquez-les.

   Pour plus d’informations sur l’ajout de filtres dans les analyses améliorées, voir [Application de filtres dans les analyses améliorées](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Une fois que vous avez ajouté des filtres, les données de 50 projets au maximum s’affichent et les filtres restent actifs même après avoir quitté la page ou vous être déconnecté de Workfront.

1. (Facultatif) Pour effectuer un zoom avant sur une période, sélectionnez un point de la visualisation pour le début de la période et faites glisser le curseur jusqu’à la fin de la période.

   Toutes les autres visualisations se mettent à jour sur la même période et un filtre de période est créé.

   ![](assets/timeframe-filter-350x220.png)

1. (Facultatif) Pour modifier le mode de tri des projets, cliquez sur le bouton **Tri par** , puis sélectionnez une nouvelle option de tri :

   * **A à Z**
   * **Z - A**
   * **Date d’achèvement prévue**
   * **Date de début planifiée**

   Toutes les autres visualisations de la page sont mises à jour pour correspondre à votre sélection de tri.

1. (Conditionnel) S’il existe plus de 50 projets dans votre jeu de données, utilisez les flèches situées dans le coin inférieur gauche de la visualisation pour passer d’un groupe de 50 projets à un autre.

   Toutes les autres visualisations de la page sont mises à jour pour correspondre à votre sélection de page.

   ![](assets/pagination-350x118.png)

1. Cliquez sur un projet dans la visualisation pour afficher plus de détails sur le projet.

   La liste se développe pour afficher les activités de chaque contributeur individuel du projet.

1. Pointez sur une zone pour afficher la date à laquelle les utilisateurs ont terminé une action, ainsi que le nombre de fois où l’action a été terminée pour cette journée.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Facultatif) Pour exporter les données de visualisation, cliquez sur le bouton **Icône Exporter** ![](assets/export.png) dans le coin supérieur droit de la visualisation, sélectionnez le format d’exportation :

   * **Graphique (PNG)**
   * **Tableau de données (XSLX)**

