---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modifier les affectations de plusieurs utilisateurs et utilisatrices dans une liste de tâches
description: Lors de la gestion des affectations de tâche, vous pouvez simultanément les modifier pour plusieurs tâches à la fois à l’aide de la fonction d’édition en bloc d’une liste de tâches.
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 7b0da61c301fe8f1f24aa27a469952fbd46987c5
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 14%

---

# Modifier les affectations de plusieurs utilisateurs et utilisatrices dans une liste de tâches

<!--Audited: 07/2024-->

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Lors de la gestion des affectations de tâche, vous pouvez simultanément les modifier pour plusieurs tâches à la fois à l’aide de la fonction d’édition en bloc d’une liste de tâches.

Cet article fait référence à la modification de plusieurs affectations d’utilisateurs pour plusieurs tâches dans une liste de tâches. Reportez-vous également aux articles suivants pour modifier des affectations sur plusieurs tâches dans d’autres zones :

* Pour plus d’informations sur l’affectation de tâches à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’affectation de travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Pour plus d&#39;informations sur l&#39;affectation d&#39;une tâche à une ressource d&#39;une liste, voir [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

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
   <td> <p>Modifier l’accès aux projets et tâches</p> <p>Affichage ou accès supérieur aux utilisateurs</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribute ou supérieures pour les tâches</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Modification des affectations pour plusieurs tâches

1. Accédez à la liste contenant les tâches pour lesquelles vous souhaitez modifier les affectations.
1. (Facultatif) Créez un filtre pour afficher uniquement les tâches affectées à la personne désignée que vous souhaitez modifier.

   Par exemple, si votre projet contient un rôle spécifique comme responsable par défaut pour plusieurs tâches, vous pouvez créer un filtre pour afficher uniquement les tâches avec ce rôle comme responsable. Vous pouvez ensuite remplacer le rôle par un utilisateur spécifique.

   Pour plus d’informations sur la création d’un filtre, voir [Création ou modification de filtres](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Pour filtrer selon un rôle, sélectionnez **Rôles d’affectation**, puis cliquez sur **ID**.

   >[!TIP]
   >
   >N’utilisez pas le champ **Affecté à**. Cela permet de trouver uniquement le propriétaire du Principal pour la tâche au lieu des rôles pouvant lui être affectés.

   Ou

   Pour filtrer un utilisateur, sélectionnez **Assignment Users,**, puis cliquez sur **ID.**

   >[!TIP]
   >
   >N’utilisez pas le champ **Affecté à**. Cela permet de trouver uniquement le propriétaire du Principal pour la tâche au lieu de tous les utilisateurs qui pourraient leur être affectés.

1. Sélectionnez les tâches pour lesquelles vous souhaitez modifier les affectations, puis cliquez sur l&#39;icône **Modifier** ![](assets/edit-icon.png).

   La page Modifier les tâches s’affiche. Les éléments que vous modifiez s’affichent dans le coin supérieur gauche de la page.

1. Accédez à la section **Affectations** .
1. Pour ajouter ou supprimer des personnes désignées, effectuez l’une des opérations suivantes :

   >[!IMPORTANT]
   >
   >La suppression des personnes désignées peut affecter les heures de la tâche et les pourcentages d’attribution. Pour plus d’informations, reportez-vous à la section [Comment la suppression des personnes désignées affecte les heures de tâche et les pourcentages d’attribution](#how-removing-assignees-affects-task-hours-and-allocation-percentages) de cet article.

   * Pour ajouter une nouvelle personne désignée :

      1. Dans la section **Affectations**, sélectionnez **Cessionnaire**.

         Les informations communes à toutes les tâches sélectionnées s’affichent. Par exemple, si le même utilisateur est affecté à toutes les tâches, il s’affiche dans la colonne **Assignation**. Si des informations ne sont pas communes aux tâches sélectionnées, aucune information ne s’affiche.

      1. Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe, puis sélectionnez-le lorsqu’il s’affiche dans la liste. L’affectation est ajoutée et ne remplace pas les affectations actuelles sur les tâches sélectionnées.


     >[!TIP]
     >
     > * Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
     >   
     > * Lors de l’ajout d’une affectation d’utilisateur, notez l’avatar, le rôle de Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez. Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
     >   
     >     * Réaffectez l’élément de travail aux ressources actives.
     >     * Associez les personnes d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.


   * Pour supprimer des personnes désignées :

      1. Cliquez sur l’icône **X** en regard du nom de la personne désignée à supprimer si la personne désignée s’affiche dans la liste Affectations.

         Ou

         (Conditionnel) Si la personne désignée à supprimer ne s’affiche pas dans la section Affectations car elle n’est affectée qu’à certaines des tâches que vous avez sélectionnées, cliquez sur **Supprimer la personne désignée** et commencez à saisir le nom de la personne désignée à supprimer, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   * Pour supprimer tous les cessionnaires existants :

      1. Cliquez sur **Supprimer tous les cessionnaires existants**, puis sur **Oui, Supprimer tous les cessionnaires**.

         Cela supprime non seulement les personnes désignées courantes (personnes désignées qui s’affichent dans la boîte de dialogue de modification), mais également toutes les personnes désignées pour toutes les tâches sélectionnées.

     La suppression des utilisateurs des tâches peut affecter les heures de la tâche et les pourcentages d’attribution.

     Pour plus d’informations, voir [Présentation de la modification des affectations de tâche](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Facultatif) Modifiez l’une des options suivantes pour les personnes désignées :

   * (Conditionnel) **Affectation % ou Heures** : spécifiez un nouveau pourcentage d’affectation ou de nouvelles heures.

     >[!NOTE]
     >
     >Cette option ne peut être modifiée que si le type de durée est le même pour toutes les tâches en cours de modification. Lorsque le Type de durée est calculé sur Travail ou Effort, vous pouvez mettre à jour le % d’allocation. Lorsque le type de durée est simple, vous pouvez mettre à jour les Heures. Pour plus d’informations sur le type de durée, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Si le champ est vide, cela signifie que la valeur est différente d’une tâche à l’autre ; toutefois, vous pouvez toujours la modifier.

   * **Propriétaire de la tâche** : sélectionnez cette option pour faire de la personne désignée le propriétaire de la tâche pour toutes les tâches en cours de modification.
   * **Rôle du cessionnaire** : sélectionnez un rôle dans la liste déroulante. Si cette option n’est pas sélectionnée, Adobe Workfront sélectionne automatiquement le rôle de Principal de l’utilisateur.

1. Cliquez sur **Enregistrer les modifications.**
