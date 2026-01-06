---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Définir la date d'achèvement prévue du projet
description: La date d’achèvement prévue d’un projet est la date à laquelle le projet doit être achevé.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 65%

---

# Définir la date d’achèvement prévue du projet

<!-- Audited: 4/2025 -->

La date d&#39;achèvement planifiée d&#39;un projet est la date à laquelle le projet est prêt à se terminer.

Les dates de début et d’achèvement prévues d’un projet dépendent des dates des tâches du projet. Cet article décrit la façon dont vous pouvez définir manuellement ou automatiquement la date d’achèvement prévue d’un projet. Pour plus d’informations sur la date d’achèvement prévue d’une tâche, voir la section [Vue d’ensemble de la date d’achèvement prévue de la tâche](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

La date d’achèvement prévue d’un projet peut être définie manuellement ou automatiquement, selon que vous planifiez le projet à partir de la date de début ou de la date d’achèvement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>
   New: Standard

   Or

   Current: Plan </p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Définir manuellement la date d’achèvement prévue d’un projet

Vous devez définir manuellement la date d’achèvement prévue d’un projet lorsque vous planifiez le projet à partir de sa date d’achèvement.

>[!NOTE]
>
>Lorsque vous définissez manuellement la date d’achèvement prévue d’un projet, Workfront calcule automatiquement la date de début prévue du projet en fonction de la durée de toutes les tâches.


Pour planifier un projet à partir de la date d’achèvement, procédez comme suit :

{{step1-to-projects}}

1. Cliquez sur **Nouveau projet**, puis sélectionnez **Nouveau projet** dans la liste déroulante.

   Pour plus d’informations sur la création de projets, voir l’article [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

1. Sélectionnez **Détails du projet** dans le panneau de gauche.

1. Cliquez sur l’icône **Modifier le projet** ![Modifier](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) dans le coin supérieur droit, puis sélectionnez **Aperçu** dans la liste déroulante qui s’affiche.

1. Dans la section **Dates du projet**, cliquez sur le champ **Mode de planification**, puis sélectionnez **Date d&#39;achèvement**.

1. Spécifiez la **Date d’achèvement prévue** du projet.
1. Cliquez sur **Enregistrer les modifications**.

   Lorsque vous commencez à ajouter des tâches à votre projet, la **Date de début prévue** du projet est calculée en fonction de la durée totale de toutes les tâches.

## Définir automatiquement la date d’achèvement prévue d’un projet

La date d’achèvement prévue d’un projet est automatiquement calculée par Workfront lorsque vous planifiez le projet à partir de la date de début.

Pour planifier un projet à partir de la date de début, procédez comme suit :

{{step1-to-projects}}

1. Cliquez sur **Nouveau projet**, puis sélectionnez **Nouveau projet** dans la liste déroulante qui s’affiche.

   Pour plus d’informations sur la création de projets, voir l’article [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

1. Sélectionnez **Détails du projet** dans le panneau de gauche.

1. Cliquez sur l’icône **Modifier le projet** ![Modifier](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) dans le coin supérieur droit, puis sélectionnez **Aperçu** dans la liste déroulante qui s’affiche.

1. Dans la section **Dates du projet**, cliquez sur le champ **Mode de planification**, puis sélectionnez **Date de début**.

1. Indiquez la **Date de début prévue** du projet.
1. Cliquez sur **Enregistrer les modifications**.

   Lorsque vous commencez à ajouter des tâches à votre projet, la **Date d’achèvement prévue** du projet est calculée en fonction de la durée totale de toutes les tâches.

   Pour plus d’informations sur la durée des tâches, voir l’article [Vue d’ensemble de la durée et du type des tâches](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   La date d’achèvement prévue du projet coïncide, dans ce cas, avec la date d’achèvement prévue de la dernière tâche du projet.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria. </p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task. </p>
<p>You can manually set the Planned Completion Date when creating a task, as described in the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints: </p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date is determined based on the following calculation: </p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
 The Update Type for the project must also be set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
