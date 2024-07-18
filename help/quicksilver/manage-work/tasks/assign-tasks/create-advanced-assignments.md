---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Créer des affectations avancées
description: Vous pouvez gérer les affectations de tâche ou de problème à l’aide d’affectations avancées.
author: Alina
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 830ad0411084844ace1e1e543c3ebefcb558af80
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 15%

---

# Créer des affectations avancées

Vous pouvez gérer les affectations de tâche ou de problème à l’aide d’affectations avancées.

Vous pouvez ajuster les informations d’affectation suivantes lors d’affectations avancées :

* Affectez des utilisateurs à la tâche ou au problème (cette opération peut être réalisée en dehors d’une affectation avancée).
* Ajustez et redistribuez le nombre d’heures alloué à chaque personne désignée.
* Déterminez quel utilisateur doit être désigné comme propriétaire ou responsable Principal de la tâche ou du problème.
* Spécifiez le rôle que chaque utilisateur remplit lorsqu’il travaille sur la tâche ou le problème.
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>Lorsque les utilisateurs sont affectés au travail, leur disponibilité en fonction de leurs plannings affecte les Dates prévues et prévues des tâches et des problèmes. Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Zones d’Adobe Workfront où vous pouvez effectuer des affectations avancées

Cet article décrit comment accéder aux affectations avancées dans l’en-tête de la tâche ou du problème.

En outre, vous pouvez effectuer des affectations avancées dans les zones suivantes de Workfront :

* Dans les listes et les rapports lorsque le champ Affectations s’affiche dans la vue.
* Dans la section Affectations lors de la modification d’une tâche. Pour plus d’informations, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Dans l’en-tête de la tâche ou du problème, dans la zone Affectations .
* Dans l’équilibreur de charge de travail. Pour plus d’informations, voir [Attribuer manuellement le travail à l’aide de l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle : standard</p>
    <p>Actuellement : Travail ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès en modification aux tâches et problèmes</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribute ou supérieures pour une tâche ou un problème</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Effectuer des affectations avancées

1. Accédez au projet auquel vous souhaitez affecter une tâche ou un problème.
1. Cliquez sur **Tâches** ou **Problèmes** dans le panneau de gauche, puis cliquez sur le nom d’une tâche ou d’un problème dans la liste.

   >[!TIP]
   >
   >Vous pouvez effectuer des affectations avancées directement sur la tâche ou la liste de problèmes si au moins deux personnes sont affectées. Cliquez à l’intérieur du champ **Affectations** sur la même ligne que la tâche ou le problème, puis cliquez sur l’ **icône Personnes** pour ouvrir la fenêtre Affectations avancées. Passez à l’étape 5 pour continuer à créer des affectations avancées.\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. Cliquez sur **Attribuer à** dans le champ **Affectations** dans l’en-tête de la tâche ou du problème.

   Ou

   Cliquez sur le nom des affectations si la tâche ou le problème est déjà assigné.

1. Cliquez sur **Avancé**.

   ![Cliquez sur Avancé](assets/assignments-box-in-task-header.png)

1. Dans le champ **Rechercher des personnes, des rôles et des équipes**, commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!NOTE]
   >
   >Si le nom de l’utilisateur ou utilisatrice contient un caractère spécial, vous devez l’inclure dans le champ de recherche.

1. (Facultatif) Continuez à ajouter des personnes désignées dans la zone **Rechercher des personnes, des rôles ou des équipes** pour ajouter plusieurs ressources à la tâche ou au problème.

   >[!TIP]
   >
   >* Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
   >
   >
   >* Lors de l’ajout d’une affectation d’utilisateur, notez l’avatar, le rôle de Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques.
   >Les personnes doivent être associées à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
   >Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
   >   
   >   * Réaffectez l’élément de travail aux ressources actives.
   >   * Associez les personnes d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.
   >

   <!-- SHOULD BE THIRD BULLET POINT IN TIP TABLE WHEN THIS FEATURE IS RELEASED 
    * <span class="preview">When adding a job role assignment, you can search for the job role or location. Select the System/Default Job Role to use the default billing rate for the assignment, or select a Rate Card Job Role to override the rate at the assignment level. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
    -->

1. Pour chaque utilisateur de la colonne **Assignation**, spécifiez les informations suivantes :


   * **Propriétaire** : passez la souris sur le nom de la personne désignée et cliquez sur **Effectuer un Principal** dans le champ Propriétaire si vous souhaitez marquer la personne désignée comme propriétaire de la tâche ou de la question. Une case à cocher verte indique que l’utilisateur spécifié est le Contact Principal de la tâche ou du problème. Adobe Workfront marque le premier utilisateur ou rôle de tâche que vous affectez à une tâche ou à un problème en tant que propriétaire ou attribution de Principal. Une équipe ne peut pas être désignée comme propriétaire Principal d’une tâche ou d’un problème.

     >[!IMPORTANT]
     >
     >Selon la manière dont votre administrateur Workfront ou votre administrateur de groupe configure les préférences de votre projet, Workfront peut utiliser le planning du propriétaire de la tâche pour calculer la chronologie de la tâche lorsque plusieurs utilisateurs sont affectés à la tâche. Pour plus d’informations sur plusieurs tâches assignées, reportez-vous à la section &quot;Affecter plusieurs utilisateurs à une tâche&quot; de l’article [Attribuer des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Allocations** : lorsque le type de durée d’une tâche est Simple, spécifiez le nombre d’heures pendant lesquelles chaque utilisateur ou rôle de tâche doit être affecté à la tâche. La somme de toutes les heures affectées pour chaque utilisateur est égale au nombre indiqué dans le champ **Heures planifiées** au bas de la colonne Allocations. Dans tous les autres cas, indiquez le pourcentage de temps (ou d’allocation) que vous souhaitez que la personne désignée passe à résoudre la tâche ou le problème.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >
     >
     >   
     >   
     >   * Après avoir modifié manuellement les affectations d’affectation sur les tâches, les Heures planifiées des tâches peuvent se mettre à jour en conséquence. Pour plus d’informations, voir la section &quot;Mise à jour des heures planifiées de la tâche lors de la gestion des affectations utilisateur&quot; dans l’article [Aperçu des heures planifiées](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * Vous ne pouvez pas modifier manuellement les affectations d’affectation en cas de problème.
     >   * Vous ne pouvez pas modifier manuellement les affectations des équipes affectées à des tâches.
     >   
     >

   * **Rôle du cessionnaire :** Sélectionnez le rôle que l’utilisateur doit utiliser lors de la réalisation de cette affectation.  Le rôle de Principal de l’utilisateur s’affiche par défaut. Cliquez dans la zone Rôle du cessionnaire pour sélectionner un autre rôle.  Lorsque vous affectez d’abord la tâche ou le problème à un rôle, puis ajoutez un utilisateur qui peut remplir ce rôle comme seconde affectation, la liste des utilisateurs suggérés est filtrée pour les utilisateurs qui peuvent remplir les rôles déjà affectés à la tâche et au problème.

     ![Rôle du cessionnaire](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **Type de durée** : cette option est disponible uniquement pour les tâches. Cliquez sur le nom du type de durée et sélectionnez un type de durée dans le menu déroulant. Pour plus d’informations sur les types de durée, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Durée :** Vous pouvez mettre à jour ce champ pour une tâche lorsque vous disposez des autorisations de gestion de la tâche.

     Pour plus d’informations, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Lors de la modification en masse d’informations d’affectation, une boîte de dialogue similaire s’affiche pour affecter des utilisateurs, des heures, une affectation et le propriétaire de la tâche.

   * **Heures planifiées** : lorsque le type de durée est Attribution calculée ou Simple, mettez à jour le nombre d’heures planifiées. Par conséquent, les pourcentages d’attribution ou les heures pour chaque ressource sont répartis uniformément. Workfront calcule les Heures planifiées lorsque le Type de durée est Basé sur le travail calculé ou l’effort. Pour plus d’informations, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).


1. Cliquer sur **Enregistrer**.
