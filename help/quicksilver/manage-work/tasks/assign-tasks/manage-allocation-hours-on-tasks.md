---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gérer les heures d’attribution des utilisateurs et utilisatrices ou des rôles sur les tâches
description: Lors de l’affectation d’utilisateurs ou de rôles à une tâche, ils sont affectés à un certain nombre d’heures pour terminer la tâche. Vous pouvez modifier manuellement le nombre d’heures alloué à chaque utilisateur ou rôle de tâche lorsqu’il est affecté à une tâche, lorsque le type de durée de la tâche est Simple.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: ad5d6bfda24119076df8336ed291c0ba63e2c88a
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 15%

---

# Gérer les heures d’attribution des utilisateurs et utilisatrices ou des rôles sur les tâches

{{highlighted-preview}}

Lors de l’affectation d’utilisateurs ou de rôles à une tâche, ils sont affectés à un certain nombre d’heures pour terminer la tâche. Vous pouvez modifier manuellement le nombre d’heures alloué à chaque utilisateur ou rôle de tâche lorsqu’il est affecté à une tâche, lorsque le type de durée de la tâche est Simple.

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
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuer ou des autorisations supérieures à la tâche</p> <p>Modifier les autorisations pour mettre à jour les heures d’affectation dans la zone Modifier la tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Observations relatives à la modification des heures d’affectation d’une tâche

>[!IMPORTANT]
>
>Après avoir modifié manuellement les affectations pour chaque affectation sur les tâches, les Heures planifiées des tâches peuvent se mettre à jour en conséquence. Pour plus d’informations, voir la section [Mettre à jour les heures planifiées de la tâche lors de la gestion des affectations utilisateur](../../../manage-work/tasks/task-information/planned-hours.md#update) dans l’article [Présentation des heures planifiées](../../../manage-work/tasks/task-information/planned-hours.md).

* Le total des heures allouées aux ressources individuelles affectées à la tâche représente les Heures planifiées de la tâche.
* S’il existe une affectation d’utilisateur ou de rôle à une tâche, le nombre d’heures attribué à l’utilisateur ou au rôle correspond aux Heures planifiées de la tâche.
* Dans le cas de plusieurs affectations, chaque utilisateur ou rôle de tâche se voit attribuer un nombre égal d’heures pour travailler sur la tâche, par défaut, si le type de durée de la tâche est Simple. Pour plus d’informations, voir les articles suivants :

   * [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Vue d’ensemble du type de durée : simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Lorsque la tâche possède un type de durée simple, vous pouvez modifier manuellement le nombre d’heures allouées pour chaque utilisateur ou rôle de tâche afin d’indiquer que certains des personnes désignées peuvent avoir plus de temps pour travailler sur une tâche que d’autres.
* Vous ne pouvez pas modifier le nombre d’heures alloué aux équipes affectées aux tâches.
* Vous ne pouvez pas modifier manuellement l’attribution des rôles utilisateur ou de tâche pour les problèmes.
* Vous pouvez également gérer les affectations quotidiennes, hebdomadaires ou mensuelles des utilisateurs à des tâches ou des problèmes en utilisant l’équilibreur de charge de travail. Pour plus d’informations, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modification des heures d’affectation d’utilisateur ou de rôle pour une tâche

1. Accédez à une tâche pour laquelle vous souhaitez modifier les heures d’affectation.
1. Cliquez sur le bouton **Plus** menu ![](assets/qs-more-icon-on-an-object.png) en regard du nom de la tâche, puis cliquez sur **Modifier**, puis **Affectations**.

   Ou

   Cliquez sur le bouton **Affectations** dans l’en-tête de la tâche, puis cliquez sur **Avancé**.

1. Assurez-vous que la variable **Type de durée** de la tâche est **Simple**.
1. Modifiez la variable **Allocations** pour chaque responsable de tâche. Il s’agit d’affectations globales pour chaque affectation à cette tâche, pour toute la durée de la tâche. Cela peut également mettre à jour les heures planifiées globales de la tâche.

   Exemple d’image dans l’environnement de production :
   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

   <span class="preview">Exemple d’image dans l’environnement Aperçu :</span>
   ![Modifier les attributions](assets/advanced-assignments-duration-type-allocations.png)

1. Cliquer sur **Enregistrer**.
