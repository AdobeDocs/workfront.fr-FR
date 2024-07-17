---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gérer les heures d’attribution des utilisateurs et utilisatrices ou des rôles sur les tâches
description: Lors de l’affectation d’utilisateurs ou de rôles à une tâche, ils sont affectés à un certain nombre d’heures pour terminer la tâche. Vous pouvez modifier manuellement le nombre d’heures alloué à chaque utilisateur ou rôle de tâche lorsqu’il est affecté à une tâche, lorsque le type de durée de la tâche est Simple.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 28%

---

# Gérer les heures d’attribution des utilisateurs et utilisatrices ou des rôles sur les tâches

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elles sont disponibles uniquement dans l’environnement de prévisualisation pour toutes les clientes et tous les clients ou dans l’environnement de production pour les clientes et les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activer ou désactiver le versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, consultez la [présentation du troisième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

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
   <td> <p>Travail ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux tâches</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribute ou supérieures pour la tâche</p> <p>Modifier les autorisations pour mettre à jour les heures d’affectation dans la zone Modifier la tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Observations relatives à la modification des heures d’affectation d’une tâche

>[!IMPORTANT]
>
>Après avoir modifié manuellement les affectations pour chaque affectation sur les tâches, les Heures planifiées des tâches peuvent se mettre à jour en conséquence. Pour plus d’informations, consultez la section [Mise à jour des heures planifiées de la tâche lors de la gestion des affectations utilisateur](../../../manage-work/tasks/task-information/planned-hours.md#update) dans l’article [Aperçu des heures planifiées](../../../manage-work/tasks/task-information/planned-hours.md).

* Le total des heures allouées aux ressources individuelles affectées à la tâche représente les Heures planifiées de la tâche.
* S’il existe une affectation d’utilisateur ou de rôle à une tâche, le nombre d’heures attribué à l’utilisateur ou au rôle correspond aux Heures planifiées de la tâche.
* Dans le cas de plusieurs affectations, chaque utilisateur ou rôle de tâche se voit attribuer un nombre égal d’heures pour travailler sur la tâche, par défaut, si le type de durée de la tâche est Simple. Pour plus d’informations, consultez les articles suivants :

   * [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Vue d’ensemble du type de durée : simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Lorsque la tâche possède un type de durée simple, vous pouvez modifier manuellement le nombre d’heures allouées pour chaque utilisateur ou rôle de tâche afin d’indiquer que certains des personnes désignées peuvent avoir plus de temps pour travailler sur une tâche que d’autres.
* Vous ne pouvez pas modifier le nombre d’heures alloué aux équipes affectées aux tâches.
* Vous ne pouvez pas modifier manuellement l’attribution des rôles utilisateur ou de tâche pour les problèmes.
* Vous pouvez également gérer les affectations quotidiennes, hebdomadaires ou mensuelles des utilisateurs à des tâches ou des problèmes en utilisant l’équilibreur de charge de travail. Pour plus d’informations, voir [Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Modification des heures d’affectation d’utilisateur ou de rôle pour une tâche

1. Accédez à une tâche pour laquelle vous souhaitez modifier les heures d’affectation.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png) en regard du nom de la tâche, puis cliquez sur **Modifier**, puis sur **Affectations**.

   Ou

   Cliquez sur la zone **Affectations** dans l’en-tête de la tâche, puis cliquez sur **Avancé**.

1. Assurez-vous que le **type de durée** de la tâche est **Simple**.
1. Modifiez les **Allocations** pour chaque personne désignée pour la tâche. Il s’agit d’affectations globales pour chaque affectation à cette tâche, pour toute la durée de la tâche. Cela peut également mettre à jour les heures planifiées globales de la tâche.

   Exemple d’image dans l’environnement de production :
   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

   <span class="preview">Exemple d’image dans l’environnement de prévisualisation :</span>
   ![Modifier les attributions](assets/advanced-assignments-duration-type-allocations.png)

1. Cliquer sur **Enregistrer**.
