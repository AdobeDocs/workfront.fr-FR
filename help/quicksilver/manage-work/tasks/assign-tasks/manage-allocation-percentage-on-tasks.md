---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gérer le pourcentage d'affectation des utilisateurs ou des rôles pour les tâches
description: La durée quotidienne prévue pour qu’une ressource dédiée travaille sur une tâche est exprimée par le pourcentage d’affectation. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou de l’utilisatrice ou du projet) auquel une ressource est affectée pendant toute la durée de la tâche.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/tpBEkOgTsJSJ-dk-gKZ6uLyCk4j4vP4nMIQ5-ciHMAI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 444
ht-degree: 84%

---

# Gérer le pourcentage d’affectation des utilisateurs et des utilisatrices ou des rôles pour les tâches

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->


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
   <td>Package Adobe Workfront</td> 
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
   <p>Modifiez les autorisations pour mettre à jour le pourcentage de répartition dans la zone Modifier la tâche.</p>
   <!--
   Not true anymore: 
   <p><b>NOTE</b></p>
   <p> You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a>.</p>
   -->
   </td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

   Il se peut que l’un de ces écrans s’affiche selon le Workfront ou le package de workflow de votre entreprise.

   ![Modifier le pourcentage d’affectation](assets/advanced-assignments-allocation-percentage.png)

   ![Modifier le pourcentage d’affectation](assets/new-aa-allocation-by-percentage.png)

1. Cliquer sur **Enregistrer**.
