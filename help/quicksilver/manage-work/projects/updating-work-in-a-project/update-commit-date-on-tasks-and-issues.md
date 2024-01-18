---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mise à jour des dates de validation pour les tâches et les problèmes
description: Vous pouvez mettre à jour manuellement la date de validation d’une tâche ou d’un problème auquel vous êtes affecté. Pour plus d’informations sur les dates de validation dans Adobe Workfront, voir Présentation de la date de validation.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Mise à jour des dates de validation pour les tâches et les problèmes

Vous pouvez mettre à jour manuellement la date de validation d’une tâche ou d’un problème auquel vous êtes affecté. Pour plus d’informations sur les dates de validation dans Adobe Workfront, voir [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Exigences d’accès

<!--Audited: 01/2024-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
   Pour les nouvelles licences :
   <ul>
   <li><p>Standard pour les tâches</p> </li>
   <li><p>Contributeur ou version ultérieure pour les problèmes</p></li>
   </ul>
   Pour les licences actuelles :
<ul>
   <li><p>Travail ou plus pour les tâches</p></li> 
   <li><p>Demande ou version ultérieure pour les problèmes</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux problèmes</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur la tâche ou le problème</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Avant de commencer, vous devez être affecté à la tâche ou au problème pour lequel vous devez mettre à jour la date de validation.

## Mise à jour des dates de validation pour les tâches et les problèmes

La mise à jour de la date de validation est identique pour les tâches et les problèmes.

1. Accédez à une tâche ou à un problème auquel vous êtes affecté en tant que **Propriétaire**.

   Pour plus d’informations sur la définition du propriétaire de la tâche pour un problème ou une tâche, consultez la section . [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) dans l’article [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Cliquez sur **Détails de la tâche** ou **Détails du problème** dans le panneau de gauche.
1. Cliquez sur **Présentation** pour l’étendre.
1. Mettez à jour le **Date de validation** champ .

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Cliquez sur **Enregistrer les modifications**.

   Ce qui suit se produit après avoir apporté cette modification : 

   * La date de validation et la date d’achèvement planifiée de la tâche ou du problème ne sont plus les mêmes.

     Au lieu de cela, la date de validation et la date d’achèvement prévue de la tâche ou du problème sont identiques.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Si vous utilisez la zone Mises à jour héritées, le propriétaire du projet est informé que vous avez suggéré une nouvelle date de validation pour la tâche ou le problème et que vous pouvez, à ce stade, mettre à jour la date d’achèvement planifiée de la tâche ou du problème afin qu’elle corresponde à la date de validation que vous avez suggérée. Cette fonctionnalité n’est pas prise en charge dans la nouvelle expérience de commentaire. Pour plus d’informations, voir [Nouvelle expérience de commentaires](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     Pour plus d’informations sur les notifications et les mises à jour déclenchées par cette modification, voir la section [Notifications et mises à jour déclenchées en modifiant la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) dans l’article [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
