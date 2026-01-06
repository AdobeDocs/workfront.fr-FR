---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Aperçu de la date de début prévue du projet
description: Les dates de début et d’achèvement prévues d’un projet dépendent des dates des tâches du projet. Cet article décrit la date de début prévue d’un projet.
author: Alina
feature: Work Management, Projects
role: User
exl-id: a1223d81-3fb8-42d1-9a7d-c58d1f0fcd36
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 96%

---

# Vue d’ensemble de la Date de début prévue du projet

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: ???</p>
<p>This needs to be split in two articles, and add one to the Tasks area.</p>
<p>Linked to Understanding the Projected Start Date for Projects, Tasks, and Issues; Project Condition article. Linked to Managing User Allocations.) </p>
</div>
-->

Les dates de début et d’achèvement prévues d’un projet dépendent des dates des tâches du projet. Cet article décrit la date de début prévue d’un projet. Pour plus d’informations sur la date de début prévue d’une tâche, voir [Vue d’ensemble de la date de début prévue d’une tâche](../../../manage-work/tasks/task-information/task-planned-start-date.md).

La date de début prévue d’un projet peut être définie manuellement ou automatiquement, selon que vous planifiez le projet à partir de la date de début ou de la date d’achèvement.

## Définir manuellement la date de début prévue d’un projet

Vous devez définir manuellement la date de début prévue d’un projet si vous planifiez le projet à partir de la date de début.

>[!NOTE]
>
>Lorsque vous définissez manuellement la date de début prévue d’un projet, Workfront calcule automatiquement la date d’achèvement prévue du projet en fonction de la durée de toutes les tâches.

Pour plus d’informations sur la définition de la date de début prévue d’un projet, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted below, to keep this as an overview article)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner, then click <strong>Projects</strong>. </li>
<li value="2"> <p>  Click  <strong>New Project</strong> then <strong>New Project</strong>. </p> <p>For more information about creating projects, see <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Create a project</a>.</p> </li>
<li value="3">  Click the <strong>Edit Project</strong> icon in the upper-right corner. </li>
<li value="4">In the <strong>Schedule From</strong> field, select <strong>Start Date</strong>.</li>
<li value="5">Specify the <strong>Planned Start Date</strong> of the project.</li>
<li value="6"> <p>Click <strong>Save Changes</strong>.</p> <p>As you start adding tasks to your project, the <strong>Planned Completion Date</strong> of the project calculates based on the total Duration of all of the tasks. </p> </li>
</ol>
-->

## Définir automatiquement la date de début prévue d’un projet

La date de début prévue d’un projet est automatiquement définie lorsque vous créez le projet des manières suivantes :

* À partir de zéro et lorsque vous planifiez le projet à partir de la date d’achèvement.

  La date de début prévue est automatiquement calculée par Adobe Workfront, en fonction de la date d’achèvement que vous sélectionnez et de la durée de toutes les tâches du projet.

  Pour plus d’informations sur la création d’un projet à partir de zéro, voir [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

* En l’important à partir de Microsoft Project.

  La date de début prévue est la date de début du projet dans Microsoft Project.

  Pour plus d’informations sur l’importation d’un projet à partir de Microsoft Project, voir [Importer un projet à partir de Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* En l’important à l’aide des Kickstarts Workfront, lorsque vous êtes administrateur ou administratrice Workfront.

  La date de début prévue correspond toujours à la date et à l’heure de votre ordinateur, sauf indication contraire dans le champ setPlannedStartDate de la feuille de projet du fichier Kickstart.

  Pour plus d’informations sur l’import de données à l’aide de Kickstart, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Pour plus d’informations sur l’import de projets à l’aide de Kickstarts, consultez la section [Scénario Kickstart : préparer simplement l’import de projets et de tâches](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:drafted it, to keep this as an overview article)</p>
<p>To schedule a project from Completion Date:</p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner, then click <strong>Projects</strong>. </li>
<li value="2"> <p>  Click  <strong>New Project</strong> then <strong>New Project</strong>. </p> <p>For more information about creating projects, see <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Create a project</a>.</p> </li>
<li value="3">  Click the <strong>Edit Project</strong> icon in the upper-right corner. </li>
<li value="4">In the <strong>Schedule From</strong> field, select <strong>Completion Date</strong>.</li>
<li value="5">Specify the <strong>Planned Completion Date</strong> of the project.</li>
<li value="6"> <p>Click <strong>Save Changes</strong>.</p> <p>As you start adding tasks to your project, the <strong>Planned Start Date</strong> of the project calculates based on the total Duration of all of the tasks, counting backwards from the Planned Completion Date. </p> <p>For more information about Task Duration, see the article <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> <p>The Planned Start Date of the project coincides, in this case, with the Planned Start Date of the first task on the project.</p> </li>
</ol>
</div>
-->

## Date de début prévue d’une tâche

Vous pouvez soit spécifier la date de début prévue d’une tâche, soit laisser Workfront la calculer en fonction de certains critères.

Pour plus d’informations sur la date de début prévue d’une tâche, voir [Vue d’ensemble de la date de début prévue d’une tâche](../../../manage-work/tasks/task-information/task-planned-start-date.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<p>(NOTE: drafted and this content was moved to the article linked in the above paragraph)</p>
<p>The Planned Start Date of a task</p>
<p>You can either specify the Planned Start Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria. </p>
<ul>
<li><a href="#manually-set-the-planned-start-date-of-a-task" class="MCXref xref">Manually set the Planned Start Date of a task</a> </li>
<li><a href="#how-the-planned-start-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Start Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Start Date of a task</strong></p>
<p>Setting the Planned Start Date of a task depends on the type of Task Constraint you assign to the task. </p>
<p>You can manually set the Planned Start Date when creating a task, as described in the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Start Date when you select any of the following Task Constraints: </p>
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
<td> <p>Must Start On</p> <p>Start No Earlier Than</p> <p>Start No Later Than</p> </td>
<td> <p><span class="s1">The Planned Completion Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Completion Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Start Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Start Date of a task:</p>
<ul>
<li> <p>The Start Date preference setting in the Tasks & Issues area in Setup</p> <p>Your Workfront or group administrator can determine whether a new task starts on the same date as the project's Planned Start Date or on the day you create the task.</p> <p>For information about Tasks & Issues preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p> </li>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a></p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Start Date, when the project is scheduled from Start Date.</li>
<li> <p>The time off schedule of the Primary Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 1 marked for Time-off, the task Planned Start Date becomes June 2. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <span href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md"><a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a></span> and <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Start Date is determined based on the following calculation: </p>
<p><code>Planned Start Date = Planned Completion Date - Task Duration</code> </p>
<p>For example, if your task has a Completion Date of September 16 and a duration of 10 days, the Planned Start Date is September 6.</p> <note type="note">  The Update Type for the project must also be set to 'Automatic and On Change' or 'Automatically' in order for the Planned Hours and Duration to be automatically adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
