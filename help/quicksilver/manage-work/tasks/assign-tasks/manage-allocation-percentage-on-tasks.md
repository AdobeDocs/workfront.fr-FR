---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gérer le pourcentage d'affectation des utilisateurs ou des rôles pour les tâches
description: La durée quotidienne prévue pour qu’une ressource dédiée travaille sur une tâche est exprimée par le pourcentage d’affectation. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou de l’utilisatrice ou du projet) auquel une ressource est affectée pendant toute la durée de la tâche.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 73%

---

# Gérer le pourcentage d’affectation des utilisateurs et des utilisatrices ou des rôles pour les tâches

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<div class="preview">

Les informations surlignées sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Les mêmes fonctionnalités seront également disponibles dans l’environnement de production pour tous les clients et clientes à partir d’une semaine à compter de la version préliminaire.

Pour plus d’informations, voir [Modernisation des interfaces](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>


La durée quotidienne prévue pour qu’une ressource dédiée travaille sur une tâche est exprimée par le pourcentage d’affectation. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou de l’utilisatrice ou du projet) auquel une ressource est affectée pendant toute la durée de la tâche.

Vous pouvez modifier le pourcentage de répartition lorsque vous effectuez des affectations avancées sur une tâche.

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
   <p>Modifiez les autorisations pour mettre à jour le pourcentage d’affectation dans la zone Modifier la tâche lors de la modification <span class="preview"> tâches à l’aide de l’ancienne expérience. Vous ne pouvez plus gérer le pourcentage de répartition dans la zone Modifier la tâche lors de la modification de tâches dans la nouvelle expérience.</span></p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Modifier les tâches</a>.</p></td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

## Considérations relatives à la modification des pourcentages d’affectation pour les tâches

* Par défaut, les utilisateurs et utilisatrices se voient attribuer un pourcentage égal de temps aux tâches auxquelles ils sont affectés.
* Vous pouvez modifier manuellement le pourcentage d’affectation pour les utilisateurs et utilisatrices et les fonctions affectés aux tâches uniquement lorsque le type de durée de la tâche est soit « Calcul de travail », soit « Piloté par l’effort ».

  Pour plus d’informations, consultez la section [Vue d’ensemble de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Vous ne pouvez pas modifier l’affectation de pourcentage pour les équipes affectées à des tâches.
* Vous ne pouvez pas modifier l’affectation de pourcentage pour les utilisateurs et utilisatrices et les fonctions affectés aux problèmes.

## Modifier l’affectation de pourcentage de l’utilisateur ou de l’utilisatrice ou l’affectation de rôle pour une tâche

1. Accédez à une tâche dont vous souhaitez modifier l’affectation de pourcentage des ressources.
1. Cliquez sur la zone **Affectations** dans l&#39;en-tête de la tâche, puis sur **Avancé**.

1. Assurez-vous que le **type de durée** de la tâche est l’un des suivants :

   * Calcul de travail
   * Piloté par l&#39;effort

   >[!TIP]
   >
   >* Pour le type de durée « Calcul d’affectation », Workfront utilise la formule suivante pour calculer le pourcentage d’affectation de chaque personne cessionnaire : `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Pour le type de durée « Simple », vous pouvez estimer les heures affectées à chaque ressource et non le pourcentage d’affectation.

1. Modifiez le champ **Allocations** pour chaque personne désignée à la tâche.

   Vous ne pouvez modifier le pourcentage d’affectation que pour les affectations d’utilisateurs et d’utilisatrices et pour les affectations de fonctions.

   Vous ne pouvez pas modifier le pourcentage d’affectation d’une équipe affectée à une tâche.

   ![Modifier le pourcentage d’affectation](assets/advanced-assignments-allocation-percentage.png)

1. Cliquer sur **Enregistrer**.
