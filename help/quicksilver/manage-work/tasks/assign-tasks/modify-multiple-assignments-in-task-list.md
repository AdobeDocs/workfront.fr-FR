---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Modifier plusieurs affectations d’utilisateurs dans une liste de tâches
description: Lors de la gestion des affectations de tâche, vous pouvez simultanément les modifier pour plusieurs tâches à la fois à l’aide de la fonction de modification en masse d’une liste de tâches.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 94%

---

# Modifier plusieurs affectations d’utilisateurs et utilisatrices dans une liste de tâches

<!--Audited: 07/2024-->

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Lors de la gestion des affectations de tâche, vous pouvez simultanément les modifier pour plusieurs tâches à la fois à l’aide de la fonction de modification en masse d’une liste de tâches.

Cet article fait référence à la modification de plusieurs affectations de personnes à plusieurs tâches dans une liste de tâches. Reportez-vous également aux articles suivants pour modifier des affectations à plusieurs tâches dans d’autres zones :

* Pour plus d’informations sur l’affectation de tâches à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’affectation de travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Pour plus d’informations sur l’affectation d’une tâche à une ressource d’une liste, voir [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard</p>
   <p>Actuellement : Travail ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux projets et tâches</p> <p>Accès en affichage de niveau supérieur aux utilisateurs et utilisatrices</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de contribution ou de niveau supérieur pour des tâches</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Sélectionnez les tâches pour lesquelles vous souhaitez modifier les affectations, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png).

   La page Modifier les tâches s’affiche. Les éléments que vous modifiez s’affichent dans le coin supérieur gauche de la page.

1. Accédez à la section **Affectations**.
1. Pour ajouter ou supprimer des cessionnaires, effectuez l’une des opérations suivantes :

   >[!IMPORTANT]
   >
   >La suppression de cessionnaires peut affecter les heures de la tâche et les pourcentages d’allocation. Pour plus d’informations, voir la section [Impact de la suppression de cessionnaires sur les heures de tâche et les pourcentages d’allocation](#how-removing-assignees-affects-task-hours-and-allocation-percentages) dans cet article.

   * Pour ajouter un ou une cessionnaire :

      1. Dans la section **Affectations**, sélectionnez **Cessionnaire**.

         Les informations communes à toutes les tâches sélectionnées s’affichent. Par exemple, si la même personne est affectée à toutes les tâches, elle s’affiche dans la colonne **Cessionnaire**. Si des informations ne sont pas communes aux tâches sélectionnées, aucune information ne s’affiche.

      1. Commencez à saisir le nom d’une personne, d’un rôle ou d’une équipe, puis sélectionnez-le lorsqu’il s’affiche dans la liste. L’affectation est ajoutée et ne remplace pas les affectations actuelles sur les tâches sélectionnées.


     >[!TIP]
     >
     > * Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
     >   
     > * Lors de l’ajout d’une affectation d’utilisateur ou d’utilisatrice, notez l’avatar, le rôle principal de l’utilisateur ou de l’utilisatrice ou son adresse e-mail, pour faire la distinction entre les utilisateurs et utilisatrices portant le même nom. Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez. Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez la section [Accorder l’accès aux utilisateurs et aux utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
     >   
     >     * Réaffectez la tâche aux ressources actives.
     >     * Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.


   * Pour supprimer des personnes cessionnaires :

      1. Cliquez sur l’**icône X** en regard du nom de la personne cessionnaire que vous souhaitez supprimer si cette dernière s’affiche dans la liste Affectations.

         Ou

         (le cas échéant) Si la personne cessionnaire à supprimer ne s’affiche pas dans la section Affectations, car elle n’est affectée qu’à certaines des tâches que vous avez sélectionnées, cliquez sur **Supprimer la personne cessionnaire** et commencez à saisir le nom de la personne cessionnaire à supprimer, puis cliquez sur le nom qui apparaît dans la liste déroulante.

   * Pour supprimer toutes les personnes cessionnaires existantes :

      1. Cliquez sur **Supprimer toutes les personnes cessionnaires existantes**, puis sur **Oui, supprimer toutes les personnes cessionnaires**.

         Cela supprime non seulement les délégataires communs (délégataires affichés dans la boîte de dialogue de modification), mais aussi tous les délégataires pour toutes les tâches sélectionnées.

     La suppression des personnes des tâches peut affecter les heures de la tâche et les pourcentages d’attribution.

     Pour plus d’informations, voir [Vue d’ensemble de la modification des affectations de tâche](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (facultatif) Modifiez l’une des options suivantes pour les personnes cessionnaires :

   * (le cas échéant) **% d’attribution ou heures** : spécifiez un nouveau pourcentage d’attribution ou de nouvelles heures.

     >[!NOTE]
     >
     >Cette option ne peut être modifiée que si le type de durée est le même pour toutes les tâches en cours de modification. Lorsque le Type de durée est Calcul de travail ou Piloté par l’effort, vous pouvez mettre à jour le % d’allocation. Lorsque le type de durée est Simple, vous pouvez mettre à jour les heures. Pour plus d&#39;informations sur le type de durée, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Si le champ est vide, cela signifie que la valeur est différente d’une tâche à l’autre ; toutefois, vous pouvez toujours la modifier.

   * **Propriétaire de la tâche** : sélectionnez cette option pour que la personne cessionnaire soit le propriétaire de la tâche pour toutes les tâches en cours de modification.
   * **Rôle de la personne cessionnaire** : sélectionnez un rôle dans la liste déroulante. Si cette option n’est pas sélectionnée, Adobe Workfront sélectionne automatiquement le rôle principal de la personne.

1. Cliquez sur **Enregistrer les modifications.**
