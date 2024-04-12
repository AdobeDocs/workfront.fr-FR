---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mise à jour des dates de validation pour les tâches et les problèmes
description: Vous pouvez mettre à jour manuellement la date de validation d’une tâche ou d’un problème auquel vous êtes affecté. Pour plus d’informations sur les dates de validation dans Adobe Workfront, voir Présentation de la date de validation.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '409'
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

>[!NOTE]
>
>Vous pouvez demander à votre administrateur système ou de groupe d’ajouter le champ Date de validation à votre panneau Résumé, afin de faciliter sa mise à jour dans différentes zones de Workfront.
>
>Pour plus d’informations, voir les articles suivants :
>
>* [Aperçu du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personnalisation de l’accueil et du résumé à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


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

   * Le propriétaire du projet est informé dans une notification intégrée à Workfront que vous avez suggéré une nouvelle date de validation pour la tâche ou le problème.
   <!--* The Project Owner is notified in the Updates section that you have suggested a new Commit Date and they can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. This functionality is not supported in the new commenting experience. For information, see [The new commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). -->

   <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

   Pour plus d’informations sur les notifications et les mises à jour déclenchées par cette modification, voir la section &quot;Notifications et mises à jour déclenchées lors du changement de la date de validation&quot; de l’article. [Présentation de la date de validation](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->