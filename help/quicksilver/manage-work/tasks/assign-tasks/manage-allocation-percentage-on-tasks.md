---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gérer le pourcentage d'affectation des utilisateurs ou des rôles pour les tâches
description: La durée quotidienne prévue pour qu’une ressource dédiée travaille sur une tâche est exprimée par le pourcentage d’affectation. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou de l’utilisatrice ou du projet) auquel une ressource est affectée pendant toute la durée de la tâche.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 6ded38ef130fbcdde8d680f77f6db38fbd81efb4
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 97%

---

# Gérer le pourcentage d’affectation des utilisateurs et des utilisatrices ou des rôles pour les tâches

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

La durée quotidienne prévue pour qu’une ressource dédiée travaille sur une tâche est exprimée par le pourcentage d’affectation. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou de l’utilisatrice ou du projet) auquel une ressource est affectée pendant toute la durée de la tâche.

>[!NOTE]
>
>Lors de l’affectation d’utilisateurs et utilisatrices au travail, leur disponibilité en fonction de leurs plannings affecte les Dates prévues et prévisionnelles des tâches et des problèmes. Pour plus d’informations sur les plannings, consultez la section [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Travail ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Modifier l’accès aux tâches</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td>
   <td><p>Autorisations de contribution ou de niveau supérieur pour une tâche</p>
   <p>Modifier les autorisations pour mettre à jour le pourcentage d’affectation dans la zone de modification de la tâche</p></td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Change this sentence in the table:
<p>Edit permissions to update allocation hours in the Edit Task box</p>
To this:
<p>Edit permissions to update allocation hours in the Edit Task box in the Production environment. <span class="preview">You can no longer manage allocation percentage in the Edit task box in the Preview environment.</span></p>
-->

## Considérations relatives à la modification des pourcentages d’affectation pour les tâches

* Par défaut, les utilisateurs et utilisatrices se voient attribuer un pourcentage égal de temps aux tâches auxquelles ils sont affectés.
* Vous pouvez modifier manuellement le pourcentage d’affectation pour les utilisateurs et utilisatrices et les fonctions affectés aux tâches uniquement lorsque le type de durée de la tâche est soit « Calcul de travail », soit « Piloté par l’effort ».

  Pour plus d’informations, consultez la section [Vue d’ensemble de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Vous ne pouvez pas modifier l’affectation de pourcentage pour les équipes affectées à des tâches.
* Vous ne pouvez pas modifier l’affectation de pourcentage pour les utilisateurs et utilisatrices et les fonctions affectés aux problèmes.

## Modifier l’affectation de pourcentage de l’utilisateur ou de l’utilisatrice ou l’affectation de rôle pour une tâche

1. Accédez à une tâche dont vous souhaitez modifier l’affectation de pourcentage des ressources.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png) à côté du nom de la tâche, puis cliquez sur **Modifier**.

   Ou

   Cliquez sur la zone des **affectations** dans l’en-tête de la tâche, puis cliquez sur **Avancé**.

1. Assurez-vous que le **type de durée** de la tâche est l’un des suivants :

   * Calcul de travail
   * Piloté par l&#39;effort

   >[!TIP]
   >
   >* Pour le type de durée « Calcul d’affectation », Workfront utilise la formule suivante pour calculer le pourcentage d’affectation de chaque personne cessionnaire : `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Pour le type de durée « Simple », vous pouvez estimer les heures affectées à chaque ressource et non le pourcentage d’affectation.

1. Cliquez sur **Affectations**, puis modifiez les **Allocations** pour chaque personne cessionnaire de la tâche.

   Vous ne pouvez modifier le pourcentage d’affectation que pour les affectations d’utilisateurs et d’utilisatrices et pour les affectations de fonctions.

   Vous ne pouvez pas modifier le pourcentage d’affectation d’une équipe affectée à une tâche.

   ![Modifier le pourcentage d’affectation](assets/advanced-assignments-allocation-percentage.png)

1. Cliquer sur **Enregistrer**.
