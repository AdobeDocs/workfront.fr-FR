---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gérer le pourcentage d’attribution des utilisateurs et utilisatrices ou des rôles sur les tâches
description: Le pourcentage d’allocation représente la durée pendant laquelle une ressource affectée est planifiée pour travailler sur une tâche au cours d’une journée. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou du projet) au cours de laquelle une ressource est allouée tout au long de la tâche.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: dd015fc356f65cc3d00a1c88ca0a8f2268283606
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 25%

---

# Gérer le pourcentage d’attribution des utilisateurs et utilisatrices ou des rôles sur les tâches

Le pourcentage d’allocation représente la durée pendant laquelle une ressource affectée est planifiée pour travailler sur une tâche au cours d’une journée. Il s’agit du pourcentage d’une journée de travail (selon le planning de l’utilisateur ou du projet) au cours de laquelle une ressource est allouée tout au long de la tâche.

>[!NOTE]
>
>Lorsque les utilisateurs sont affectés au travail, leur disponibilité en fonction de leurs plannings affecte les Dates prévues et prévues des tâches et des problèmes. Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux tâches</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribute ou supérieures pour la tâche</p> <p>Modifier les autorisations pour mettre à jour le pourcentage d’allocation dans la zone Modifier la tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Considérations relatives à la modification des allocations de pourcentage pour les tâches

* Par défaut, les utilisateurs se voient attribuer un pourcentage égal de temps aux tâches auxquelles ils sont affectés.
* Vous pouvez modifier manuellement le pourcentage d’allocation pour les utilisateurs et les rôles de tâche affectés aux tâches uniquement lorsque le type de durée de la tâche est Basé sur le travail calculé ou l’effort.

  Pour plus d’informations, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Vous ne pouvez pas modifier l’allocation de pourcentage pour les équipes affectées à des tâches.
* Vous ne pouvez pas modifier l’allocation en pourcentage pour les utilisateurs et les rôles de tâche affectés aux problèmes.

## Modification de l’allocation de pourcentage d’utilisateur ou de rôle pour une tâche

1. Accédez à une tâche pour laquelle vous modifiez l’affectation de pourcentage des ressources.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png) en regard du nom de la tâche, puis cliquez sur **Modifier**.

   Ou

   Cliquez sur la zone **Affectations** dans l’en-tête de la tâche, puis cliquez sur **Avancé**.

1. Assurez-vous que le **type de durée** de la tâche est l’un des suivants :

   * Calcul de travail
   * Piloté par l&#39;effort

   >[!TIP]
   >
   >* Pour le type Durée d’affectation calculée , Workfront utilise la formule suivante pour calculer le pourcentage d’affectation de chaque personne désignée : `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Pour le type Durée simple , vous pouvez estimer les heures affectées à chaque ressource, et non le pourcentage d’allocation.

1. Cliquez sur **Affectations**, puis modifiez les **Allocations** pour chaque personne désignée pour la tâche.

   Vous pouvez uniquement modifier le pourcentage d’attribution pour les affectations d’utilisateurs et de rôles de tâche.

   Vous ne pouvez pas modifier le pourcentage d’affectation d’une équipe affectée à une tâche.

   ![Modifier le pourcentage d’allocation](assets/advanced-assignments-allocation-percentage.png)

1. Cliquer sur **Enregistrer**.
