---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gérer le pourcentage d’affectation des utilisateurs ou des rôles pour les tâches
description: Le pourcentage d’allocation représente la durée pendant laquelle une ressource affectée est planifiée pour travailler sur une tâche au cours d’une journée. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou du projet) au cours de laquelle une ressource est allouée tout au long de la tâche.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---

# Gérer le pourcentage d’affectation des utilisateurs ou des rôles pour les tâches

Le pourcentage d’allocation représente la durée pendant laquelle une ressource affectée est planifiée pour travailler sur une tâche au cours d’une journée. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou du projet) au cours de laquelle une ressource est allouée tout au long de la tâche.

>[!NOTE]
>
>Lorsque les utilisateurs sont affectés au travail, leur disponibilité en fonction de leurs plannings affecte les Dates prévues et prévues des tâches et des problèmes. Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuer ou des autorisations supérieures à la tâche</p> <p>Modifier les autorisations pour mettre à jour le pourcentage d’allocation dans la zone Modifier la tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Observations relatives à la modification des allocations de pourcentage pour les tâches

* Par défaut, les utilisateurs se voient attribuer un pourcentage égal de temps aux tâches auxquelles ils sont affectés.
* Vous pouvez modifier manuellement le pourcentage d’allocation pour les utilisateurs et les rôles de tâche affectés aux tâches uniquement lorsque le type de durée de la tâche est Basé sur le travail calculé ou l’effort.

   Pour plus d’informations, voir [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Vous ne pouvez pas modifier l’allocation de pourcentage pour les équipes affectées à des tâches.
* Vous ne pouvez pas modifier l’allocation en pourcentage pour les utilisateurs et les rôles de tâche affectés aux problèmes.

## Modification de l’allocation de pourcentage d’utilisateur ou de rôle pour une tâche

1. Accédez à une tâche pour laquelle vous modifiez l’affectation de pourcentage des ressources.
1. Cliquez sur le bouton **Plus** menu ![](assets/qs-more-icon-on-an-object.png) en regard du nom de la tâche, puis cliquez sur **Modifier**.

   Ou

   Cliquez sur le bouton **Affectations** dans l’en-tête de la tâche, puis cliquez sur **Avancé**.

1. Assurez-vous que la variable **Type de durée** de la tâche est l’une des suivantes :

   * Calcul de travail
   * Piloté par l&#39;effort

   >[!TIP]
   >
   >* Pour le type Durée d’affectation calculée , Workfront utilise la formule suivante pour calculer le pourcentage d’affectation de chaque personne désignée : `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Pour le type Durée simple , vous pouvez estimer les heures affectées à chaque ressource, et non le pourcentage d’allocation.


1. Cliquez sur **Affectations**, puis modifiez la variable **Allocations** pour chaque personne désignée pour la tâche.

   Vous pouvez uniquement modifier le pourcentage d’attribution pour les affectations d’utilisateurs et de rôles de tâche.

   Vous ne pouvez pas modifier le pourcentage d’allocation pour une équipe affectée à une tâche.

   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. Cliquer sur **Enregistrer**.
