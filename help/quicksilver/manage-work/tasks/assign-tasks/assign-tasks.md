---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Affecter des tâches
description: Vous pouvez affecter des tâches aux utilisateurs, rôles ou équipes pour indiquer qui est responsable de l’exécution des tâches. Vous pouvez affecter une tâche à plusieurs ressources à la fois.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 7b0da61c301fe8f1f24aa27a469952fbd46987c5
workflow-type: tm+mt
source-wordcount: '1985'
ht-degree: 14%

---

# Affecter des tâches

<!--Audited: 07/2024-->

<!--remove the span class preview from everywhere but the Rate Card roles references must stay in yellow; replace the intro with preview and fast track only but not sure if with the link to third quarter release?!-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elles sont disponibles uniquement dans l’environnement de prévisualisation pour toutes les clientes et tous les clients ou dans l’environnement de production pour les clientes et les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activer ou désactiver le versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Vue d’ensemble de la version du quatrième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md).</span>

Vous pouvez affecter des tâches aux utilisateurs, aux rôles de tâche ou aux équipes pour indiquer qui est responsable de l’exécution des tâches. Vous pouvez affecter une tâche à plusieurs ressources à la fois.

>[!TIP]
>
>Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
>
>Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
>
>* Réaffectez l’élément de travail aux ressources actives.
>* Associez les personnes d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.
>

Le nombre d’utilisateurs affectés à une tâche et le planning de la tâche Propriétaire peuvent modifier les dates planifiées d’une tâche, ce qui entraîne la modification de la chronologie du projet. Pour plus d’informations sur l’impact de l’affectation de plusieurs utilisateurs à une tâche, voir [Présentation de la modification des affectations de tâche](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

En plus de cet article, nous vous recommandons de lire les articles suivants pour plus d’informations sur l’affectation de tâches :

* [Présentation de la modification des affectations de tâche](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Présentation des affectations dynamiques](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Effectuer des affectations dynamiques](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Créer des affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Modifier plusieurs affectations d’utilisateurs dans une liste de tâches](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Planification d’une présentation de projet](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Présentation de la tâche Date d’achèvement prévue](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Définition de la date d’achèvement prévue du projet](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Vue d’ensemble de l’affectation du travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Conditions d’accès

<!-- Audited: 07/2024-->

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
   <p>Actuellement : Travail ou licence supérieure</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets et tâches</p> <p>Affichage ou accès supérieur aux utilisateurs</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>


*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Considérations relatives à plusieurs affectations pour les rôles de tâche, les équipes et les utilisateurs

Tenez compte des points suivants lorsque vous affectez plusieurs ressources à une tâche :

* Les utilisateurs peuvent avoir plusieurs rôles de tâche associés à leur profil. Pour plus d’informations sur l’association d’utilisateurs à des rôles de tâche, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Si vous affectez plusieurs utilisateurs à une tâche ou à un problème, le premier utilisateur que vous sélectionnez est désigné automatiquement comme propriétaire de la tâche ou du problème.
Pour plus d’informations sur la modification de ce paramètre, voir les informations sur l’option Créer un Principal dans l’article [Créer des affectations avancées](create-advanced-assignments.md).

* Une équipe ne peut pas être une personne désignée par Principal pour une tâche ou un problème. Seul un utilisateur ou un rôle de tâche peut être désigné comme Principal sur une tâche ou un problème.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Les tâches et les problèmes d’un projet peuvent être affectés en premier à une ou plusieurs équipes ou rôles de tâche. Lorsque le projet est prêt à démarrer, il doit peut-être également être affecté aux utilisateurs :

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Équipes</td>
   <td>Si vous attribuez une tâche à une équipe et que vous affectez également un utilisateur, la tâche reste assignée à l’équipe et à l’utilisateur, même si l’utilisateur n’est pas membre de l’équipe.</td>
  </tr>
  <tr>
   <td>Fonctions</td>
   <td><p>Si vous affectez une tâche ou un problème à un ou plusieurs rôles, puis que vous affectez également un utilisateur, décide quel rôle de tâche associer à l’utilisateur supplémentaire (le cas échéant), selon les règles suivantes :</p>
     <ul>
      <li>Si un seul rôle de tâche est attribué et qu’il correspond au rôle principal de l’utilisateur (configuré dans son profil), la tâche ou le problème est attribué uniquement à cet utilisateur.</li>
      <li>Si plusieurs rôles sont affectés et qu’au moins l’un d’eux correspond à l’un des autres rôles de l’utilisateur, la tâche ou le problème est affecté à l’utilisateur (le rôle est sélectionné de manière aléatoire s’il existe plusieurs correspondances), ainsi que tout autre rôle affecté.</li>
      <li>Si au moins un rôle de tâche est attribué et qu’il n’existe aucune correspondance avec les rôles de tâche de l’utilisateur, la tâche ou le problème est affecté à la fois au rôle ou aux rôles et à l’utilisateur.</li>
     </ul>
   <p>Pour plus d’informations sur le rôle principal d’un utilisateur et d’autres rôles, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Modification du profil d’un utilisateur</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Attribuer une seule tâche

1. Accédez à une tâche que vous souhaitez affecter.
1. Cliquez sur **Attribuer à** dans le champ **Affectations** dans l’en-tête de la tâche.

   Ou

   Cliquez sur le nom des affectations si la tâche est déjà affectée.

   ![Affectations](assets/assignments-box-in-task-header.png)

1. Utilisez l’une des méthodes suivantes :

   * Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe que vous souhaitez affecter, puis cliquez dessus lorsqu’il apparaît dans la liste.


     >[!TIP]
     >
     >Lors de l’ajout d’une affectation d’utilisateur, notez l’avatar, le rôle de Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les personnes doivent être associées à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
     >
     >Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >
     ><span class="preview">Lors de l’ajout d’une affectation de rôle de tâche, vous pouvez rechercher le rôle ou l’emplacement de la tâche. Sélectionnez un rôle dans la liste Rôles de tâche pour utiliser le taux de facturation par défaut pour l’affectation ou sélectionnez un rôle de tâche Carte de taux pour utiliser le taux de facturation dans la carte de taux. Pour plus d’informations sur les cartes de taux, voir [Gestion des cartes de taux](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * (Conditionnel) Cliquez sur l’un des noms dans les listes <span class="preview">**Affectations proposées**</span>, **Utilisateur et équipes**, **Rôles de tâche** ou <span class="preview">**Rôles de carte de taux**</span> lors de leur affichage. Consultez [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md) pour en savoir plus.

     Vous pouvez commencer à saisir le nom d’un utilisateur, d’une équipe ou d’un rôle de tâche à affecter à la tâche, puis le sélectionner lorsqu’il s’affiche dans la liste.

   * Cliquez sur **Avancé**

     Pour plus d’informations sur la façon d’effectuer des affectations avancées, voir [Création d’affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Cliquer sur **Enregistrer**.
1. (Facultatif et conditionnel) Cliquez sur l’icône **X** en regard du nom de l’affectation dans le panneau droit de la tâche pour supprimer une affectation, si vous avez cliqué sur **Avancé**.

## Attribuer une tâche dans une liste

Vous pouvez affecter des tâches dans une liste ou un rapport lorsque l’un des champs d’affectation est visible dans la vue de la liste. Il s’agit d’un moyen plus rapide d’affecter des tâches. Cet article décrit comment modifier des affectations pour une tâche dans une liste. Pour plus d’informations sur la modification de plusieurs affectations pour plusieurs tâches dans une liste, voir [Modification de plusieurs affectations d’utilisateurs dans une liste de tâches](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Selon le champ visible dans la vue, vous pouvez affecter les entités suivantes à la tâche :

| champ | Entités affectées |
|---|---|
| **Attribuer À** | Attribuer un utilisateur |
| **Affecté** | Attribuer un utilisateur |
| **Affectations** | Affectation d’utilisateurs, de rôles de tâche ou d’équipes |

Pour affecter des tâches dans une liste :

1. Accédez à la liste des tâches auxquelles les champs Affecté à, Affecté ou Affectation sont affichés dans la vue.
1. (Facultatif) Cliquez sur le menu déroulant **Enregistrement automatique** et sélectionnez l’une des options suivantes :

   | Option | Description des options |
   |---|---| 
   | Enregistrement automatique | Les modifications que vous apportez aux tâches sont automatiquement enregistrées et vous ne pouvez pas les annuler. |
   | Enregistrement manuel | Vous devez enregistrer vos modifications manuellement. Vous pouvez annuler vos modifications avant de les enregistrer. |
   | Planification chronologique | Vous devez enregistrer vos modifications manuellement. Vous pouvez annuler vos modifications avant de les enregistrer. L’enregistrement de vos modifications et de toutes les dépendances du projet est plus rapide que lors de la sélection de l’enregistrement manuel. |

   Pour plus d’informations sur l’enregistrement des tâches lorsque vous les modifiez dans une liste, voir [Modifier les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Pour affecter des tâches, effectuez l’une des opérations suivantes :

   * Cliquez dans les champs **Affecté à** ou **Affecté** et commencez à saisir le nom d’un utilisateur actif que vous souhaitez affecter à la tâche, puis cliquez dessus lorsqu’il s’affiche dans la liste.
   * Cliquez dans le champ **Affectations** et commencez à saisir le nom d’un utilisateur, d’un rôle de tâche ou d’une équipe actif à affecter à la tâche, puis cliquez dessus lorsqu’il s’affiche dans la liste.

     >[!TIP]
     >
     >Lors de l’ajout d’une affectation d’utilisateur, notez l’avatar, le rôle de Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les personnes doivent être associées à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
     >
     >Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >
     ><span class="preview">Lors de l’ajout d’une affectation de rôle de tâche, vous pouvez rechercher le rôle ou l’emplacement de la tâche. Sélectionnez un rôle de tâche pour utiliser le taux de facturation par défaut pour l’affectation ou un rôle de tâche Carte de taux pour utiliser le taux de facturation dans la carte de taux. Pour plus d’informations sur les cartes de taux, voir [Gestion des cartes de taux](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. (Conditionnel) Lorsqu’il est visible dans le champ **Affectations**, cliquez sur l’icône **Personnes** dans le coin supérieur droit de la zone Affectations pour ouvrir la zone **Affectations avancées** et créer des affectations avancées.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   Pour plus d’informations, voir [Création d’affectations avancées](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Vous ne pouvez pas effectuer d’affectations avancées à partir des champs Affecté à ou Affecté .

1. Après avoir ajouté les personnes désignées à la tâche, appuyez sur Entrée ou cliquez n’importe où sur la page pour enregistrer vos modifications si vous avez sélectionné Enregistrement automatique. Sinon, cliquez sur **Enregistrer**.

## Affectation de plusieurs tâches à un utilisateur

1. Accédez à la liste des tâches que vous souhaitez affecter en bloc.
1. (Conditionnel) Assurez-vous que l’option **Enregistrement automatique** est sélectionnée si vous vous trouvez dans la liste des tâches d’un projet.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas modifier les tâches en bloc lors de l’enregistrement manuel des tâches sur un projet.

1. Sélectionnez plusieurs tâches dans la liste des tâches.
1. Cliquez sur **Modifier**.

   La boîte de dialogue **Modifier les tâches** s’ouvre.

1. Dans la zone **Affectations**, sélectionnez la zone **Assignation**, puis commencez à saisir le nom d’un utilisateur, d’un rôle de tâche ou d’une équipe que vous souhaitez affecter à toutes les tâches.

   >[!IMPORTANT]
   >
   >Si l’une des tâches est déjà affectée, les ressources que vous indiquez ici sont ajoutées aux tâches au lieu de remplacer les ressources existantes sur les tâches.

1. (Facultatif) Sélectionnez le bouton radio dans la colonne **Propriétaire de la tâche** pour indiquer quelle ressource est la personne désignée principale ou le propriétaire de la tâche, lorsque vous affectez plusieurs ressources à la tâche. Cette option n’est pas disponible pour les équipes.
1. (Conditionnel) Spécifiez l’ **affectation %** pour chaque ressource affectée à la tâche si toutes les tâches que vous avez sélectionnées ont un type de durée d’affectation pilotée par l’effort ou calculée. Cela indique le temps que ces ressources doivent consacrer à l’exécution de la tâche. Cette option n’est disponible que pour les utilisateurs et les rôles de tâche.

   Ou

   Spécifiez la valeur **Heures** pour chaque ressource affectée à la tâche si toutes les tâches que vous avez sélectionnées ont un type de durée simple. Le total de toutes les heures pour toutes les ressources doit être égal au nombre d’ Heures planifiées pour la tâche.

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas spécifier le pourcentage d’allocation ou le nombre d’heures par ressource si les tâches que vous avez sélectionnées ont des types de durée différents ou si les tâches que vous avez sélectionnées ont des types de durée différents.

   Pour plus d’informations sur le type de durée sur les tâches, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Facultatif) Sélectionnez un rôle que l’utilisateur doit remplir pour la tâche dans le menu déroulant **Choisir un rôle** de la colonne **Rôle du cessionnaire** lorsque vous affectez des utilisateurs à des tâches. Si vous ne sélectionnez pas de rôle, Workfront sélectionne automatiquement le rôle de Principal de l’utilisateur.

1. (Facultatif) Si vous souhaitez supprimer des personnes désignées existantes de toutes les tâches, effectuez l’une des opérations suivantes :

   1. Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe que vous souhaitez supprimer de la tâche, puis sélectionnez-le lorsqu’il apparaît dans la liste et cliquez sur **Supprimer le cessionnaire** pour supprimer d’autres cessionnaires.
   1. Cliquez sur **Supprimer tous les cessionnaires existants** pour supprimer tous les cessionnaires de toutes les tâches sélectionnées.

1. Cliquez sur **Enregistrer les modifications**.
1. (Facultatif et conditionnel) Lorsque les champs Affectés à ou Affectations s’affichent dans votre liste de tâches, cliquez dans l’une de ces colonnes pour une tâche, puis cliquez sur l’ **icône X** en regard du nom d’une personne désignée pour la supprimer de la tâche.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


