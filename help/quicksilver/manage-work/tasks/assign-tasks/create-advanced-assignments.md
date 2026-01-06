---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Créer des affectations avancées
description: Vous pouvez gérer les affectations de tâches ou d'événements à l'aide d'affectations avancées.
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 79%

---

# Créer des affectations avancées

<!-- Audited: 11/2025-->

<!--remove the bullet indicated when we get rid of the new/old experience of editing tasks-->


<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Vous pouvez gérer les affectations de tâches ou d&#39;événements à l&#39;aide d&#39;affectations avancées.

Vous pouvez ajuster les informations d’affectation suivantes lors d’affectations avancées :

* Affectez des utilisateurs et utilisatrices à la tâche ou au problème (cette opération peut être réalisée en dehors d’une affectation avancée).
* Ajustez et redistribuez le nombre d’heures affecté à chaque personne cessionnaire.
* Déterminez quelle personne doit être la propriétaire ou la cessionnaire principale de la tâche ou du problème.
* Spécifiez le rôle de chaque personne lorsqu’elle travaille sur la tâche ou le problème.
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>Lors de l’affectation d’utilisateurs et utilisatrices au travail, leur disponibilité en fonction de leurs plannings affecte les Dates prévues et prévisionnelles des tâches et des problèmes. Pour plus d’informations sur les plannings, voir [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Zones d’Adobe Workfront où vous pouvez effectuer des affectations avancées.

Cet article décrit comment accéder à des affectations avancées dans l’en-tête de la tâche ou de l’événement.

En outre, vous pouvez effectuer des affectations avancées dans les zones suivantes de Workfront :

* Dans les listes et les rapports lorsque le champ Affectations s’affiche dans la vue.
* Dans la section Affectations lors de la modification d’une tâche. Pour plus d&#39;informations, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md). <!--When we remove the old/ new experience: take this bullet out completely; in the new Edit Task experience, this is no longer possible-->
* Dans l’en-tête de la tâche ou du problème, dans la zone Affectations.
* Dans l’équilibreur de charge de travail. Pour plus d’informations, voir [Attribuer manuellement du travail à l’aide de l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

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
   <td role>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux tâches et aux problèmes</p>  </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p>Autorisations de niveau Contributeur ou supérieur pour la tâche ou l’événement</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer des affectations avancées

1. Accédez au projet auquel vous souhaitez attribuer une tâche ou un problème.
1. Cliquez sur **Tâches** ou **Problèmes** dans le panneau de gauche, puis sur le nom d’une tâche ou d’un problème dans la liste.

   >[!TIP]
   >
   >Vous pouvez effectuer des affectations avancées directement dans la liste des tâches ou des événements. Cliquez dans le champ **Affectations** sur la même ligne que la tâche ou l&#39;événement, puis cliquez sur **Avancé** au bas de la liste ou sur l&#39;icône **Personnes** dans le coin supérieur droit de la zone Affectations, pour ouvrir la fenêtre Affectations avancées. Passez à l’étape 5 pour continuer à créer des affectations avancées.
   >![Cliquez sur Avancé ou sur l’icône Personnes](assets/access-aa-from-lists.png)

1. Cliquez sur **Affecter à** dans le champ **Affectations** dans l’en-tête de la tâche ou du problème.

   Ou

   Cliquez sur l&#39;un des noms affectés si la tâche ou l&#39;événement est déjà affecté.

1. Cliquez sur **Avancé**.

   ![Cliquez sur Avancé](assets/assignments-from-task-header-0825.png)

1. Dans le champ **Rechercher des personnes, des rôles et des équipes**, commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!NOTE]
   >
   >Si le nom de l’utilisateur ou utilisatrice contient un caractère spécial, vous devez l’inclure dans le champ de recherche.

1. (Facultatif) Continuez à ajouter des personnes désignées dans la zone **Rechercher des personnes, des rôles et des équipes** pour ajouter plusieurs ressources à la tâche ou à l’événement.

   >[!TIP]
   >
   >* Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
   >
   >
   >* Lors de l’ajout d’une affectation d’utilisateur ou d’utilisatrice, notez l’avatar, le rôle principal de l’utilisateur ou de l’utilisatrice ou son adresse e-mail, pour faire la distinction entre les utilisateurs et utilisatrices portant le même nom.
   >Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
   >Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs et aux utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
   >   
   >   * Réaffectez la tâche aux ressources actives.
   >   * Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.

1. Pour chaque utilisateur ou utilisatrice de la colonne **Personne cessionnaire**, indiquez les informations suivantes :

   * **Personne propriétaire** : passez la souris sur le nom de la personne cessionnaire et cliquez sur **Principal** dans le champ Personne propriétaire si vous souhaitez marquer la personne cessionnaire comme propriétaire de la tâche ou du problème. Une case à cocher verte indique que la personne en question est le Contact principal de la tâche ou du problème. Adobe Workfront marque la première personne ou fonction que vous affectez à une tâche ou à un problème comme propriétaire ou affectation principale. Une équipe ne peut pas être désignée comme propriétaire principal d’une tâche ou d’un problème.

     >[!IMPORTANT]
     >
     >Selon la manière dont votre équipe d’administration Workfront ou votre administrateur ou administratrice de groupes configure les préférences de votre projet, Workfront peut utiliser le planning de la personne propriétaire de la tâche pour calculer la chronologie de la tâche lorsque plusieurs utilisateurs et utilisatrices sont affectés à la tâche. Pour plus d’informations sur les tâches à plusieurs personnes cessionnaires, voir la section « Affecter plusieurs utilisateurs et utilisatrices à une tâche » dans l’article [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Allocations** : lorsque le type de durée d’une tâche est Simple, indiquez le nombre d’heures auxquelles chaque utilisateur ou utilisatrice ou fonction doit être affecté à la tâche. La somme de toutes les heures affectées de chaque utilisateur ou utilisatrice est égale au nombre indiqué dans le champ **Nombre d’heures prévues** au bas de la colonne Allocations. Dans tous les autres cas, indiquez le pourcentage de temps (ou d’affectation) que la personne désignée doit consacrer à la résolution de la tâche ou du problème.

     >[!TIP]
     >   
     >   * Après avoir modifié manuellement les allocations d’affectation sur les tâches, le nombre d’heures prévues des tâches peut se mettre à jour. Pour plus d’informations, voir la section « Mettre à jour le nombre d’heures prévues de la tâche lors de la gestion des affectations des utilisateurs et utilisatrices » dans l’article [Vue d’ensemble du nombre d’heures prévues](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * Vous ne pouvez pas modifier manuellement les allocations d’affectation sur les problèmes.
     >   * Vous ne pouvez pas modifier manuellement les affectations des équipes affectées à des tâches.

   * **Rôle du ou de la cessionnaire :** sélectionnez le rôle que l’utilisateur ou utilisatrice doit utiliser pour cette affectation.  Le rôle principal de l’utilisateur ou utilisatrice s’affiche par défaut. Cliquez dans la zone **Rôle du cessionnaire** pour sélectionner un autre rôle. Lorsque vous affectez d’abord la tâche ou le problème à un rôle, puis que vous ajoutez un utilisateur ou une utilisatrice qui peut assumer ce rôle comme seconde affectation, la liste des utilisateurs et utilisatrices suggérés est filtrée pour afficher ceux qui peuvent assumer les rôles déjà affectés à la tâche et au problème.

     ![Rôle de la personne cessionnaire](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **Type de durée** : cette option n’est disponible que pour les tâches. Cliquez sur le nom du type de durée et sélectionnez un type de durée dans le menu déroulant. Pour plus d’informations sur les types de durée, voir [Vue d’ensemble de la durée et du type de durée des tâches](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Durée :** vous pouvez mettre à jour ce champ pour une tâche si vous disposez des autorisations de gestion de la tâche.

     Pour plus d’informations, voir [Vue d’ensemble de la durée et du type de durée des tâches](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Lors de la modification en masse d’informations d’affectation, une boîte de dialogue similaire s’affiche pour affecter des utilisateurs et utilisatrices, des heures, une affectation et le propriétaire de la tâche.

   * **Nombre d’heures prévues** : lorsque le type de durée est Calcul d’affectation ou Simple, mettez à jour le nombre d’heures prévues. Ensuite, les pourcentages d’affectation ou les heures de chaque ressource sont répartis uniformément. Workfront calcule le nombre d’heures prévues lorsque le type de durée est Calcul de travail ou Piloté par l’effort. Pour plus d’informations, voir [Vue d’ensemble de la durée et du type de durée des tâches](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. Cliquer sur **Enregistrer**.
