---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Création d’affectations avancées
description: Vous pouvez gérer les affectations de tâche ou de problème à l’aide d’affectations avancées.
author: Alina
feature: Work Management
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Création d’affectations avancées

Vous pouvez gérer les affectations de tâche ou de problème à l’aide d’affectations avancées.

Vous pouvez ajuster les informations d’affectation suivantes lors d’affectations avancées :

* Affectez des utilisateurs à la tâche ou au problème (cette opération peut être réalisée en dehors d’une affectation avancée).
* Ajustez et redistribuez le nombre d’heures alloué à chaque personne désignée.
* Déterminez quel utilisateur doit être désigné comme propriétaire ou responsable Principal de la tâche ou du problème.
* Spécifiez le rôle que chaque utilisateur remplit lorsqu’il travaille sur la tâche ou le problème.

>[!NOTE]
>
>Lorsque les utilisateurs sont affectés au travail, leur disponibilité en fonction de leurs plannings affecte les Dates prévues et prévues des tâches et des problèmes. Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Zones d’Adobe Workfront où vous pouvez effectuer des affectations avancées

Cet article décrit comment accéder aux affectations avancées dans l’en-tête de la tâche ou du problème.

En outre, vous pouvez effectuer des affectations avancées dans les zones suivantes de Workfront :

* Dans les listes et les rapports lorsque le champ Affectations s’affiche dans la vue.
* Dans la section Affectations lors de la modification d’une tâche. Pour plus d’informations, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Dans l’en-tête de la tâche ou du problème, dans la zone Affectations .
* Dans l’équilibreur de charge de travail. Pour plus d’informations, voir [Affectation manuelle du travail à l’aide de l’équilibreur de charge](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

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
   <td> <p>Modifier l’accès aux tâches et aux problèmes</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuer ou accorder des autorisations supérieures à une tâche ou à un problème</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Effectuer des affectations avancées

1. Accédez au projet auquel vous souhaitez affecter une tâche ou un problème.
1. Cliquez sur **Tâches** ou **Problèmes** dans le panneau de gauche, cliquez sur le nom d’une tâche ou d’un problème dans la liste.

   >[!TIP]
   >
   >Vous pouvez effectuer des affectations avancées directement sur la tâche ou la liste de problèmes si au moins deux personnes sont affectées. Cliquez dans le **Affectations** sur la même ligne que la tâche ou le problème, puis cliquez sur l’icône **Icône Personnes** pour ouvrir la fenêtre Affectations avancées . Passez à l’étape 5 pour continuer à créer des affectations avancées.\
   >![](assets/nwe-advanced-assignments-350x55.png)   >

1. Cliquez sur **Attribuer à** dans le **Affectations** champ dans l’en-tête de la tâche ou du problème

   Ou

   Cliquez sur le nom des affectations si la tâche ou le problème est déjà assigné.

1. Cliquez sur **Avancé**.

   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. Dans le **Recherche de personnes, de rôles et d’équipes** , commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!NOTE]
   >
   >Si le nom de l’utilisateur contient un caractère spécial, vous devez l’inclure dans le champ de recherche.

1. (Facultatif) Continuez à ajouter des personnes désignées dans la variable **Recherche de personnes, de rôles ou d’équipes** pour ajouter plusieurs ressources à la tâche ou au problème.

   >[!TIP]
   >
   >* Vous pouvez affecter plusieurs utilisateurs, rôles de tâche ou équipes. Vous ne pouvez affecter que des utilisateurs, des rôles de tâche et des équipes principaux.
   >
   >
   >* Lors de l’ajout d’une affectation d’utilisateur, notez l’avatar, le rôle Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.
   >
   >
   >* Si un utilisateur, un rôle de tâche ou une équipe a été affecté avant d’être désactivé, il reste attribué à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
      >   
      >   * Réaffectez l’élément de travail aux principales ressources.
      >   * Associez les utilisateurs d’une équipe désactivée à une équipe principale et réaffectez l’élément de travail à l’équipe principale.


1. Pour chaque utilisateur de la variable **Cessionnaire** , indiquez les informations suivantes :


   * **Propriétaire**: Pointez sur le nom de la personne désignée, puis cliquez sur **Rendre Principal** dans le champ Propriétaire si vous souhaitez marquer la personne désignée comme propriétaire de la tâche ou de l’émission. Une case à cocher verte indique que l’utilisateur spécifié est le contact Principal de la tâche ou du problème. Adobe Workfront marque le premier utilisateur ou rôle de tâche que vous affectez à une tâche ou à un problème en tant que propriétaire ou attribution Principal. Une équipe ne peut pas être désignée comme propriétaire Principal d’une tâche ou d’un problème.

      >[!IMPORTANT]
      >
      >Selon la manière dont votre administrateur Workfront ou votre administrateur de groupe configure les préférences de votre projet, Workfront peut utiliser le planning du propriétaire de la tâche pour calculer la chronologie de la tâche lorsque plusieurs utilisateurs sont affectés à la tâche. Pour plus d’informations sur plusieurs tâches assignées, voir la section &quot;Affecter plusieurs utilisateurs à une tâche&quot; dans l’article [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Allocations** : Lorsque le Type de durée d’une tâche est simple, indiquez le nombre d’heures que chaque utilisateur ou rôle de tâche doit être affecté à la tâche. La somme de toutes les heures attribuées pour chaque utilisateur est égale au nombre indiqué dans la variable **Heures planifiées** au bas de la colonne Allocations. Dans tous les autres cas, indiquez le pourcentage de temps (ou d’allocation) que vous souhaitez que la personne désignée passe à résoudre la tâche ou le problème.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

      >[!TIP]
      >
      >
      >   
      >   
      >   * Après avoir modifié manuellement les affectations d’affectation sur les tâches, les Heures planifiées des tâches peuvent se mettre à jour en conséquence. Pour plus d’informations, reportez-vous à la section &quot;Mise à jour des heures planifiées de la tâche lors de la gestion des affectations utilisateur&quot; de l’article . [Présentation des heures planifiées](../../../manage-work/tasks/task-information/planned-hours.md).
      >   * Vous ne pouvez pas modifier manuellement les affectations d’affectation en cas de problème.
      >   * Vous ne pouvez pas modifier manuellement les affectations des équipes affectées à des tâches.


   * **Rôle du cessionnaire :** Sélectionnez le rôle que l’utilisateur doit utiliser lors de cette affectation.  Le rôle Principal de l’utilisateur s’affiche par défaut. Cliquez dans la zone Rôle du cessionnaire pour sélectionner un autre rôle.  Lorsque vous affectez d’abord la tâche ou le problème à un rôle, puis ajoutez un utilisateur qui peut remplir ce rôle comme seconde affectation, la liste des utilisateurs suggérés est filtrée pour les utilisateurs qui peuvent remplir les rôles déjà affectés à la tâche et au problème.

      ![](assets/advanced-assignments-box-select-a-role-350x243.png)

   * **Type de durée**: Cette option n’est disponible que pour les tâches. Cliquez sur le nom du type de durée et sélectionnez un type de durée dans le menu déroulant. Pour plus d’informations sur les types de durée, voir [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Durée :** Vous pouvez mettre à jour ce champ pour une tâche lorsque vous disposez des autorisations de gestion de la tâche.

      Pour plus d’informations, voir [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Lors de la modification en masse d’informations d’affectation, une boîte de dialogue similaire s’affiche pour affecter des utilisateurs, des heures, une affectation et le propriétaire de la tâche.

   * **Heures planifiées**: Lorsque le type de durée est Attribution calculée ou Simple, mettez à jour le nombre d’heures planifiées. Par conséquent, les pourcentages d’attribution ou les heures pour chaque ressource sont répartis uniformément. Workfront calcule les Heures planifiées lorsque le Type de durée est Basé sur le travail calculé ou l’effort. Pour plus d’informations, voir [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

      ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. Cliquer sur **Enregistrer**.
