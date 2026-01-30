---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mettre à jour les dates d'engagement pour les tâches et les événements
description: Vous pouvez mettre à jour manuellement la date d’engagement d’un objet (tâche ou problème) qui vous est affecté. Pour plus d’informations sur les dates d’engagement dans Adobe Workfront, voir Vue d’ensemble de la date d’engagement.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 76%

---


# Mettre à jour les dates d’engagement pour les tâches et les problèmes

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Vous pouvez mettre à jour manuellement la date d’engagement d’un objet (tâche ou problème) qui vous est affecté. Pour plus d’informations sur les dates d’engagement dans Adobe Workfront, voir [Vue d’ensemble de la date d’engagement](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Conditions d’accès

<!--Audited: 01/2024-->

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <ul>
   <li><p>Standard pour les tâches</p> </li>
   <li><p>Contribution ou licence supérieure pour les problèmes</p></li>
   </ul>
   <p>Ou</p>
<ul>
   <li><p>Travail ou licence supérieure plus pour les tâches</p></li> 
   <li><p>Demande ou niveau supérieur pour les problèmes</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux tâches et aux problèmes</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion sur la tâche ou le problème</p>
   <p> Vous devez être affecté à la tâche ou à l'événement pour mettre à jour la date de validation </p>
    </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   New:
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   Current:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p>
   <p> You must be assigned to the task or issue to update the commit date </p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Conditions préalables

Avant de pouvoir modifier la date d’engagement d’une tâche ou d’un problème, l’objet (tâche ou problème) dont vous devez mettre à jour la date d’engagement doit vous être affecté.

## Mettre à jour les dates d’engagement pour les tâches et les problèmes


Vous pouvez mettre à jour la date d’engagement d’une tâche ou d’un problème dans les zones suivantes de Workfront :

* Section Détails d’une tâche ou d’un problème
* L’en-tête de la tâche ou du problème

  Votre administrateur Workfront ou de groupe doit ajouter la date d’engagement à l’en-tête de tâche ou d’événement de votre modèle de mise en page pour l’afficher à partir de la page de la tâche ou de l’événement.
Pour plus d’informations, voir [Personnaliser les en-têtes d’objets à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

La mise à jour de la date d’engagement est identique pour les tâches et les problèmes.

>[!NOTE]
>
>Vous pouvez demander à votre administrateur ou administratrice système ou de groupe d’ajouter le champ Date d’engagement à votre panneau Résumé, afin de faciliter sa mise à jour dans différentes zones de Workfront.
>
>Pour plus d’informations, consultez les articles suivants :
>
>* [Vue d’ensemble du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personnaliser le panneau Résumé à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Accédez à un élément (tâche ou problème) qui vous est affecté en tant que **Personne propriétaire**.

   Pour plus d’informations sur la définition de la personne propriétaire de la tâche pour un problème ou une tâche, consultez la section [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) dans l’article [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Conditionnel et facultatif) Si votre administrateur de Workfront ou de groupe a ajouté la date d’engagement à l’en-tête de votre tâche ou de votre événement, cliquez sur le champ **Date d’engagement** dans l’en-tête, puis sélectionnez une date dans le calendrier. Si la date d’engagement ne figure pas dans l’en-tête, procédez comme suit.

   ![Date d’engagement dans l’en-tête de la tâche](assets/commit-date-task-header.png)

1. Cliquez sur **Détails de la tâche** ou **Détails du problème** dans le panneau de gauche.
1. Cliquez sur **Vue d’ensemble** pour développer la section.
1. Mettez à jour le champ **Date d’engagement**.

   ![Modification de la date d’engagement de la tâche mise en surbrillance dans la page de détails](assets/task-commit-date-edit-highlighted-details-page.png)

1. Cliquez sur **Enregistrer les modifications**.

   Voici ce qui se produit après avoir apporté cette modification :

   * La date d’engagement et la date d’achèvement prévue de la tâche ou du problème ne sont plus les mêmes.

     Au lieu de cela, la date d’engagement et la date d’achèvement projetée de la tâche ou du problème sont identiques.

     ![Date d’achèvement prévue de la tâche mise en surbrillance](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Le ou la propriétaire du projet reçoit une notification intégrée à Workfront, selon laquelle vous avez suggéré une nouvelle date d’engagement pour la tâche ou le problème.
   * Dans la section Mises à jour, la personne propriétaire du projet est informée que vous avez suggéré une nouvelle date d’engagement et qu’elle peut, à ce stade, mettre à jour la date d’achèvement prévue de la tâche ou du problème pour qu’elle corresponde à la date d’engagement que vous avez suggérée.

     ![La notification du propriétaire du projet dans le flux de mise à jour dont la date de validation affecte la chronologie du projet](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![Project owner notification in update stream that commit date affects the project timeline](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Pour plus d’informations sur les notifications et les mises à jour déclenchées par cette modification, voir la section Notifications et mises à jour déclenchées en modifiant la date d’engagement de l’article [Vue d’ensemble des dates d’engagement](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->
