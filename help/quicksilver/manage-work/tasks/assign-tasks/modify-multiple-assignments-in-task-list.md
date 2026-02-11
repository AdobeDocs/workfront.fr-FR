---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modifier plusieurs affectations d’utilisateurs dans une liste de tâches
description: Lors de la gestion des affectations de tâche, vous pouvez simultanément les modifier pour plusieurs tâches à la fois à l’aide de la fonction de modification en masse d’une liste de tâches.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 79%

---

# Modifier plusieurs affectations d’utilisateurs et utilisatrices dans une liste de tâches

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

Lors de la gestion des affectations de tâche, vous pouvez simultanément les modifier pour plusieurs tâches à la fois à l’aide de la fonction de modification en masse d’une liste de tâches.

Cet article fait référence à la modification de plusieurs affectations de personnes à plusieurs tâches dans une liste de tâches. Reportez-vous également aux articles suivants pour modifier des affectations à plusieurs tâches dans d’autres zones :

* Pour plus d’informations sur l’affectation de tâches à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’affectation de travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Pour plus d’informations sur l’affectation d’une tâche à une ressource d’une liste, voir [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

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
   <td> <p>Modifier l’accès aux projets et tâches</p> <p>Accès en affichage de niveau supérieur aux utilisateurs et utilisatrices</p> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td>
   <td>Autorisations de niveau Contributeur ou supérieur pour les tâches</td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

## Modifier les affectations pour plusieurs tâches

1. Accédez à la liste contenant les tâches pour lesquelles vous souhaitez modifier les affectations.
1. (Facultatif) Créez un filtre pour afficher uniquement les tâches affectées à la personne cessionnaire que vous souhaitez modifier.

   Par exemple, si votre projet contient un rôle spécifique comme rcessionnaire par défaut pour plusieurs tâches, vous pouvez créer un filtre pour afficher uniquement les tâches avec ce rôle comme cessionnaire. Vous pouvez ensuite remplacer le rôle par une personne spécifique.

   Pour plus d’informations sur la création d’un filtre, voir [Créer ou modifier des filtres](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Pour filtrer selon un rôle, sélectionnez **Rôles pour l’affectation**, puis cliquez sur **Identifiant**.

   >[!TIP]
   >
   >N’utilisez pas le champ **Affecté à**. Cela permet de trouver uniquement la personne propriétaire principale pour la tâche au lieu des rôles pouvant lui être affectés.

   Ou

   Pour filtrer une personne, sélectionnez **Affecter des utilisateurs et utilisatrices**, puis cliquez sur **Identifiant**.

   >[!TIP]
   >
   >N’utilisez pas le champ **Affecté à**. Cela permet de trouver uniquement la personne propriétaire principale pour la tâche au lieu de toutes les personnes qui pourraient être affectées.

1. Sélectionnez les tâches pour lesquelles vous souhaitez modifier les affectations, puis cliquez sur l&#39;icône **Modifier** ![Modifier](assets/edit-icon.png).

   1. Pour ajouter ou supprimer des personnes désignées, effectuez l’une des opérations suivantes :

      * Pour ajouter des personnes désignées, commencez à saisir leur nom dans le champ **Rechercher des personnes, des rôles ou des équipes**, puis sélectionnez-les lorsqu’elles s’affichent dans la liste.

        La nouvelle personne désignée est ajoutée aux personnes existantes pour les tâches sélectionnées.
      * Pour supprimer des personnes désignées, cliquez sur leur nom dans la zone **Supprimer une personne désignée**

        Ou

        Cliquez sur **Supprimer tous les cessionnaires existants**.

        Les cessionnaires sont supprimés de toutes les tâches sélectionnées.

        La suppression des personnes des tâches peut affecter les heures de la tâche et les pourcentages d’attribution.

        Pour plus d’informations, voir [Vue d’ensemble de la modification des affectations de tâche](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).


        >[!TIP]
        >
        >* Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
        >   
        >* Lors de l’ajout d’une affectation d’utilisateur ou d’utilisatrice, notez l’avatar, le rôle principal de l’utilisateur ou de l’utilisatrice ou son adresse e-mail, pour faire la distinction entre les utilisateurs et utilisatrices portant le même nom. Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez. Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez la section [Accorder l’accès aux utilisateurs et aux utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
        > 
        >   Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
        >   
        >* Réaffectez la tâche aux ressources actives.
        >* Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.


   1. (facultatif) Modifiez l’une des options suivantes pour les personnes cessionnaires :

      * (le cas échéant) **% d’attribution ou heures** : spécifiez un nouveau pourcentage d’attribution ou de nouvelles heures.

      >[!NOTE]
      >
      >Cette option ne peut être modifiée que si le type de durée est le même pour toutes les tâches en cours de modification. Lorsque le Type de durée est Calcul de travail ou Piloté par l’effort, vous pouvez mettre à jour le % d’allocation. Lorsque le type de durée est Simple, vous pouvez mettre à jour les heures. Pour plus d&#39;informations sur le type de durée, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      >
      >
      >Si le champ est vide, cela signifie que la valeur est différente d’une tâche à l’autre ; toutefois, vous pouvez toujours la modifier.

      * **Effectuer le Principal** : passez la souris sur les tâches sélectionnées et sélectionnez cette option pour que la personne désignée soit le propriétaire de la tâche pour toutes les tâches en cours de modification.
      * **Rôle de la personne cessionnaire** : sélectionnez un rôle dans la liste déroulante. Si cette option n’est pas sélectionnée, Adobe Workfront sélectionne automatiquement le rôle principal de la personne.
      * **Type de durée**
      * **Durée**
      * **Nombre d’heures prévues**

   1. Cliquer sur **Enregistrer**.

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->





