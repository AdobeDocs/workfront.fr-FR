---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gérer les heures d'affectation des utilisateurs et des rôles pour les tâches
description: Lors de l’affectation de personnes ou de rôles à une tâche, un certain nombre d’heures de travail leur sont allouées pour accomplir la tâche. Vous pouvez modifier manuellement le nombre d’heures allouées à chaque personne ou fonction lors de l’affectation à une tâche, lorsque le type de durée de la tâche est Simple.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: d0be569333b0454e26f4d0de1078b0425cf81707
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 82%

---

# Gérer les heures d’affectation des personnes et des rôles sur les tâches

Les heures d&#39;affectation représentent le temps total prévu pour qu&#39;une ressource affectée travaille sur une tâche. Les heures représentent le temps alloué à un utilisateur un jour donné ou un jour de la semaine, une semaine ou un mois pendant toute la durée de la tâche.

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
   <p>Modifier les autorisations pour mettre à jour les heures d’affectation dans la boîte de modification de la tâche</p></td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à la modification des heures allouées à une tâche

>[!IMPORTANT]
>
>Après avoir modifié manuellement les allocations pour chaque affectation sur les tâches, le nombre d’heures prévues des tâches peut être mis à jour en conséquence. Pour plus d’informations, voir la section [Mettre à jour le nombre d’heures prévues de la tâche lors de la gestion des allocations pour les utilisateurs et utilisatrice](../../../manage-work/tasks/task-information/planned-hours.md#update) dans l’article [Vue d’ensemble du nombre d’heures prévues](../../../manage-work/tasks/task-information/planned-hours.md).

* Le total des heures allouées aux ressources individuelles affectées à la tâche représente le nombre total d’heures prévues de la tâche.
* Si une personne ou un rôle reçoit une affectation à une tâche, le nombre d’heures allouées à la personne ou au rôle correspond au nombre d’heures prévues de la tâche.
* En cas d’affectations multiples, chaque personne ou fonction se voit attribuer un nombre égal d’heures pour travailler sur la tâche, par défaut, si le type de durée de la tâche est simple. Pour plus d’informations, consultez les articles suivants :

   * [Vue d’ensemble de la durée des tâches et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Vue d’ensemble du type de durée : simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Lorsque la tâche a un type de durée simple, vous pouvez modifier manuellement le nombre d’heures allouées pour chaque utilisateur ou fonction afin d’indiquer que certains des cessionnaires de la tâche peuvent avoir plus de temps pour travailler sur une tâche que d’autres.
* Vous ne pouvez pas modifier le nombre d’heures allouées aux équipes affectées aux tâches.
* Vous ne pouvez pas modifier manuellement les allocations des personnes ou des fonctions pour les problèmes.
* Vous pouvez également gérer les allocations quotidiennes, hebdomadaires ou mensuelles des personnes pour les tâches ou les problèmes en utilisant l’équilibreur de charge de travail. Pour plus d’informations, voir [Gérer les allocations des utilisateurs dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modifier les heures allouées à une personne ou un rôle pour une tâche

1. Accédez à une tâche pour laquelle vous souhaitez modifier les heures allouées.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png) à côté du nom de la tâche, puis cliquez sur **Modifier**, puis sur **Affectations**.

   Ou

   Cliquez sur la zone **Affectations** dans l’en-tête de la tâche, puis cliquez sur **Avancé**.

1. Assurez-vous que le **type de durée** de la tâche est **Simple**.
1. Modifiez les **Allocations** pour chaque cessionnaire de tâche. Il s’agit d’allocations globales pour chaque affectation à cette tâche, pour toute la durée de la tâche. Cela peut également mettre à jour le nombre total d’heures prévues de la tâche.

   ![Modifier les attributions](assets/advanced-assignments-duration-type-allocations.png)

1. Cliquer sur **Enregistrer**.
