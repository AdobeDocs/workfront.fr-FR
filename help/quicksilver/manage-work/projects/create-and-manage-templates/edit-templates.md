---
product-area: templates
navigation-topic: templates-navigation-topic
title: Modifier des modèles de projet
description: Vous pouvez modifier des modèles de projet pour prendre en compte les modifications apportées aux paramètres et aux processus du projet.
author: Alina
feature: Work Management
exl-id: da0fca31-6a50-4862-ad9a-a453ef968773
source-git-commit: 246750d2a7a053d74df2ceb150f14fdb50f32ade
workflow-type: tm+mt
source-wordcount: '4710'
ht-degree: 2%

---

# Modifier des modèles de projet

<!-- Audited: 2/2024 -->

<!--The Resource Pools part also duplicates in the "Working with Resource Pools" article-->

Vous pouvez modifier des modèles de projet pour prendre en compte les modifications apportées aux paramètres et aux processus du projet. Après avoir mis à jour et enregistré les modifications sur un modèle, les nouvelles modifications sont visibles dans les nouveaux projets lorsque les projets sont créés à l’aide du modèle. Les modifications que vous apportez au modèle ne concernent pas le projet qui utilise actuellement ce modèle.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td>
      <p>Nouveau : Standard</p>
      <p>Ou</p>
      <p>Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> 
    <ul> 
     <li> <p>Attribuez des autorisations à un modèle pour le modifier dans l’onglet Détails du modèle .</p> </li> 
     <li> <p>Gérer les autorisations d’un modèle pour le modifier dans la zone Modifier le modèle</p> </li> 
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Modifier un modèle {#edit-a-template}

<!--
Editing a template differs depending on what environment you choose. 

### Edit a template in the Production environment {#edit-a-template-in-the-production-environment} 

1. Go to the template you want to edit.
1. (Conditional) To edit limited information about the template,  click **Template Details** in the left panel, then go to the areas listed in the left panel to edit information for each area. 
1. To edit information in the Details section, click the **Edit** icon ![](assets/edit-icon.png), then select from any of the areas below, or click **Edit all** to edit information in all areas:

   * Overview
   * Custom Forms

     Names of customs forms display only if there are custom forms attached to the object.
   
   * Finance

   >[!TIP]
   >
   >For information about all fields that display in the Details area, continue with editing all fields using the Edit Template box below.

1. (Conditional) To edit all information about the template, click the **More** menu ![](assets/qs-more-icon-on-an-object.png) next to the name of the template, then click **Edit**.

   The **Edit Template** box opens. The sections in this box contain the same fields available in  the Template Details section .

1. Consider editing information in any of the following sections:

   * [Overview](#overview) 
   * [Finance](#finance) 
   * [Portfolio](#portfolio) 
   * [Settings](#settings) 
   * [Access](#access) 
   * [Custom Forms](#custom-forms) 
   * [Tasks](#tasks) 
   * [Issues](#issues) 
   * [Comment](#comment)

### Overview {#overview}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Overview**.

   ![](assets/edit-template-overview-with-tasks-and-issues-350x210.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong></td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong></td> 
      <td>Add additional information about the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Active</strong></td> 
      <td><p>Select this checkbox if you want the template to be active. Other users can find this template and attach it to projects when creating projects. Deselect this checkbox if you want to deactivate templates that are no longer used. Deactivated templates cannot be attached to projects. This is enabled by default. </p><p><b>TIP</b>
      
      You can deactivate a template from the template header as described in the [Activate or deactivate a template](#activate-or-deactivate-a-template) section in this article.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong></td> 
      <td>Specify a web link that relates to information about this template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule From</strong></td> 
      <td><p>Specify whether the project using this template is scheduled from the <strong>Start Date</strong>, or from the <strong>Completion Date</strong>. This selection determines the planned dates of the future tasks on the project using this template. </p><p>Select from the following: </p> 
       <ul> 
        <li><p><strong>Schedule From Start Date</strong>: The Start Date of the template is actually the Start Day. When you schedule a template from Start Date, Adobe Workfront calculates the Completion Day of the template based on the Duration of all the template tasks. The Start Day of the template becomes the Planned Start Date of the future project.</p></li> 
        <li><p><strong>Schedule from Completion Date</strong>: The Completion Date of the template is actually the Completion Day. When you schedule a template from Completion Date, Workfront calculates the Start Day of the template based on the Duration of all the template tasks. The Completion Day of the template becomes the Planned Completion Date of the future project. </p></li> 
       </ul><p>For more information about the Start and Completion Days of template tasks, see <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Overview of Start and Completion Days in a template</a>. </p><p>The Schedule From setting for templates is similar to that of projects. Your Workfront administrator selects the default Schedule From setting for the projects in your system. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition Type</strong></td> 
      <td><p>Select between the following Condition Types:</p> 
       <ul> 
        <li><strong>Manual:</strong> The project owner sets the Condition of the project on the project manually. <strong></strong></li> 
        <li><strong>Progress Status:</strong> Workfront automatically sets the Condition of the future project based on the Progress Status of tasks on the Critical Path. For more information about understanding Progress Status, see <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a>.</li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong></td> 
      <td><p>This is just a visual flag for you which allows you to prioritize your future projects. Select from the following options:</p> 
       <ul> 
        <li><p><strong>None</strong></p></li> 
        <li><p><strong>Low</strong></p></li> 
        <li><p><strong>Normal</strong></p></li> 
        <li><p><strong>High</strong></p></li> 
        <li><p><strong>Urgent</strong></p></li> 
       </ul><p><p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Owner</strong></td> 
      <td><p>The user who is designated as the Template Owner must be a Workfront active user. </p><p>Consider the following about the user designated as the Template Owner: </p> 
       <ul> 
        <li>They are automatically given Manage permissions to the template. </li> 
        <li>They are added to the project team and are automatically given Manage permissions to the project created from the template. </li> 
        <li>They become the Project Owner, when the project is created from this template. </li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Sponsor</strong></td> 
      <td><p>The user specified in this field becomes the Project Sponsor, when the template is added to the project. This user is added to the project team and is automatically given view permissions to the project. The user who is designated as the Template Sponsor must be a Workfront active user. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Manager</strong></td> 
      <td><p>The specified users are automatically given manage permissions to the future projects and can assign resources to the tasks and issues of the projects. You can specify more than one Resource Manager. </p></td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Group</strong></td> 
      <td><p>In the drop-down list, select the group that you want to be associated with projects created from the template. It can be a group of any level. </p><p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTES</b>
      
    <ul> 
    <li><p>In the Projects area on a group's page, when someone creates a project using a template that doesn't have a group selected, the system associates the currently open group with the project.</p><p>This is different from other areas where the system associates a user's Home Group with the project when the user creates the project using a template that doesn't have a group selected.</p>
    </li> 
      <li><p>If a user selects a template that has a group selected while creating a project—or while converting a task or issue to a project—the user can choose a different group for the project.</p></li> 
      <li>Though this field is available in templates only in the new Adobe Workfront experience, you can see it in lists and reports both there and in Adobe Workfront Classic. </li> 
      </ul> </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Company</strong></td> 
      <td><p>Specify the Company that you want to associate with the template. Only active companies display in the list.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Finance {#finance}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Finance**.

   ![](assets/edit-template-finance-with-tasks-and-issues-350x259.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Performance Index Method</strong></td> 
      <td><p>Specify whether the Earned Value metrics of the future project are calculated using hours or costs. For more information about the Performance Index Method, see <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a>. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Budget</strong></td> 
      <td><p>Specify a Budget for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Cost</strong></td> 
      <td><p>Specify the Fixed Cost for the projects that are created from this template. This is different than the Labor Cost which comes from the hours on the project and the Expense Cost which comes from the amount of expenses on the project. The Fixed Cost of a project is taken into account when calculating the Net Value of a project and it is part of the Budgeted Cost.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Revenue</strong></td> 
      <td><p>Specify the Fixed Revenue for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Currency</strong></td> 
      <td><p>Specify the currency for the future project, if it is different than the default currency of your system. This field is not visible if you have only the default currency in the system.<br>For more information about currency, see <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Require time to be approved for this project</strong></td> 
      <td><p>Select this option to require the Project Owner of the future project created from this template to approve time logged on the project. If you are using Billing Records and you select this option, only the approved hours on the project appear as available billable hours for the Billing Records. Approving time on the project is independent of approving timesheets. For more information about requiring time to be approved on a project, see <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Require time to be approved for a project</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Portfolio {#portfolio}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Portfolio**.

   ![](assets/edit-template-portfolio-with-tasks-and-issues-350x228.png)

1. Update the following fields:

   <table style="table-layout:auto">
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Portfolio</strong></td> 
      <td><p>Specify a Portfolio for the projects that are created from this template. You must create a Portfolio first, before it appears in the drop-down list. </p><p>Only active portfolios display in the list. For more information about creating portfolios, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Create a portfolio </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Program</strong></td> 
      <td><p>If you selected a Portfolio for the template, specify a <strong>Program</strong> for the future project. Some Portfolios might not have Programs. You must create a Program first, before it appears in this drop-down list. Only active programs display in the list.</p><p>For more information about creating programs, see <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Create a program</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Benefit</strong></td> 
      <td><p>Specify the Planned Benefit of the projects that are created from this template. The Planned Benefit is used in the Business Case of the project and the Portfolio Optimizer. </p><p>For more information about the Planned Benefit of a project, see <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>. The Planned Benefit of a project is taken into account when the Net Value of a project is calculated. </p><p>For more information about using the Portfolio Optimizer, see <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Manage projects in the Portfolio Optimizer</a> </p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Settings {#settings}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Settings**.

   ![](assets/edit-template-settings-with-tasks-and-issues-350x336.png)

1. Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Milestone Path</strong> </td> 
      <td> <p>Select a Milestone Path for the template. Only active milestone paths display in the list.<br>For more information about Milestone Paths, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Create a milestone path</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Mode</strong> </td> 
      <td> <p>Controls how the future project will be marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The project is marked Complete when all the tasks and issues are completed.</p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually select the Complete status for the project, when all the tasks and issues are completed. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Summary Completion Mode</strong> </td> 
      <td> <p>Controls how the parent tasks on the future project are marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The parent tasks are marked Complete and they update their percent complete automatically, as the children tasks are completed and the percent complete of the children is updated. </p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually update the percent complete and the status of the parent tasks, independently of what changes are made to the children tasks. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Update Type</strong> </td> 
      <td> <p>Controls when the changes you make to the timeline of the future project are saved on the project. </p> 
       <b>EXAMPLE </b> 
        <p>The following changes to the project trigger an update to the timeline of the project:</p> 
        <ul> 
         <li> <p>update the dates of tasks</p> </li> 
         <li> <p>change predecessor relationships<br></p> </li> 
         <li> <p>change parent-child relationships</p> </li> 
         <li> <p>add or remove assignments in addition to changing the task constraint or duration type.</p> </li> 
        </ul> 
       </div> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Automatic and On Change</strong> (Default setting): The future project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on (On Change). The project timeline is also updated each night (Automatic).<br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you perform an action on a task or project that triggers a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer recalculations display briefly as a question mark (between 1 and 5 seconds, or up to a minute for large projects). This indicates that the recalculation is not yet finished, and the dates are subject to change.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Change Only</strong>: The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Automatic Only</strong>: The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on. However, be aware that you chose this setting, as the project will not update at the same time that the changes are made.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Manual Only</strong>: The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.<br></p> </li> 
       </ul> <p>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule</strong> </td> 
      <td> <p>Select a schedule for your template. This will become the schedule of the project that is created from this template. This should be the same schedule assigned to most people that are working on the project. You must create a schedule before you can assign it to a template.<br>For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>. <br>If you have not created custom schedules in your system, the Default Schedule is selected. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>User Time Off</strong> </td> 
      <td> <p>Determines whether the time off of the Primary Assignee of a task adjusts the task planned dates. When you attach the template to an existing project, and the template has a different setting for this field than the project, the setting on the project remains unchanged. The default option for this setting for a new template is the same as the system-level project preference. </p> <p>For information about the project preferences at the System level, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> <p>For information about how this setting affects the task dates on a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.<br>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Consider user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template adjust according to the time off of the Primary Assignee of the task, if the time off occurs during the duration of the task. </p> </li> 
        <li> <p><strong>Ignore user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template remain as originally planned, even if the Primary Assignee of the task has time off during the duration of the task. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Leveling Mode</strong> </td> 
      <td> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Manual</strong>: you must manually level your resources on the project created from this template (this is the default setting)</p> </li> 
        <li> <p><strong>Automatic:</strong> Workfront levels the resources on the future project. <br>For more information about Resource Leveling, see <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Level Resources in the Gantt Chart </a>. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Risk</strong> </td> 
      <td> <p>Define the level of risk of the projects created from this template. The risk is just an indicator of how risky a project can be. You can prioritize the execution of your projects based on the level of risk.<br>Consider selecting from the following levels of risk:<br></p> 
       <ul> 
        <li> <p><strong>Very Low</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p><strong>Medium</strong> </p> </li> 
        <li> <p><strong>High</strong> </p> </li> 
        <li> <p><strong>Very High</strong> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Pools</strong> </td> 
      <td> <p>Specify the resource pools associated with the template. Resource pools are collections of users that are needed at the same time for the completion of a project. For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> <p> <p><b>NOTE</b> 
      
      When you edit templates in bulk, only the resource pools that are common to all the templates selected appear in this field. If the templates selected have no shared resource pools, this field will be empty. The resource pools you specify here will overwrite the templates' individual resource pools.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template. Your Workfront administrator or a user with administrative access to Approval Processes must define system-level or group-level project approval processes before you can associate them with a template. For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
      <ul> 
      <li>Only active approval processes display in the list. </li> 
      <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the template does not display in the list.</p> <p><b>IMPORTANT</b> 
      
      If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
      <li> <p>If you added a single-use approval process, it displays as "Custom" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p> 
      </li> 
      <li> <p>When bulk-editing templates, the following scenarios exist:</p> 
      <ul> 
         <li> <p>When you select templates from the same group, both system-level and group-level approval processes display in this field.</p> </li> 
         <li> <p>When you select templates from different groups, only system-level approval processes display in this field.</p> </li> 
         <li> <p>When any of the templates has a single-use approval process attached, it is replaced by the system-level you select. </p> </li> 
      </ul> </li> 
      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Filter Hour Types</strong> </td> 
      <td> <p>Consider the following:</p> <p>Select <strong>No</strong> to make all project-specific hour types available on the future project. (This is the default selection)</p> <p>Or</p> <p>Select <strong>Yes</strong> to make only a subset of the project-specific hour types available on the future project, then select the hour types you want to make available. (Hold the Shift key to select multiple hour types.)</p> <p>If you select this option, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). You must select at least one hour type; if you select this option and you do not select any hour types, all hour types are made available on the project.</p> <p>The same hour type selections must be made at the individual user level in order for the user to see these hour type options on the project. </p> <p>For more information about defining hour types at the user level, see the section <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Log time</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notification</strong> </td> 
      <td>Select the Reminder Notification that should be associated with the future project. You must configure Reminder Notifications for projects for this field to appear during editing a template. <br>For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.  
   Or
1. Click **Save Changes**.

### Access {#access}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Access**.

   ![](assets/edit-template-access-with-tasks-and-issues-350x241.png)

   The Access you specify for your template will become the Access of users associated with the project when the template is used to create a project.

   Specify the following **Access** information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to a task</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to a task. The user assigned to a task is automatically granted this access to the task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to a task is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to an issue</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to an issue. The user assigned to an issue is automatically granted this access to the issue. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to an issue is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone submits a request: Give them access</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the request. When they submit a request to the project, they are granted this access to the request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>People from the same company will inherit the same permissions for all requests</strong> </td> 
      <td> <p>Select this field if you want people from the same company to have the same access to all the requests on the project, whether they submitted them or not.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is given access to this project: Give them access to ...</strong> </td> 
      <td> <p>Select the access options that you want users to have on the project, if the project is shared with them. Select the specific options for their access, if they are designated as <strong>Viewers</strong>, <strong>Contributors</strong>, or <strong>Managers</strong> when sharing the project with them. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Custom Forms {#custom-forms}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Custom Forms**.

   ![edit_tempate_custom_forms.png](assets/edit-tempate-custom-forms-tasks-with-issues-sections-350x136.png)

1. Select the custom form or forms that you want to associate with the template. You must build the custom forms before they are available to select in this field.

   Only active custom forms display in the list. For more information about building custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   You can add up to ten custom forms to a template.

   The forms will be added to the project that is created from this template. 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Tasks {#tasks}

You can define the defaults that will be associated with all the new tasks when you add them to a project that is created from the template.

For information about how these settings affect creating new tasks, see [Create tasks overview](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Tasks**.

   ![](assets/edit-template-with-tasks-and-issue-sections-350x144.png)

1. In the **Task Default Approval Process** box, select the Approval Process you want to associate with all new tasks when you add them to a project created from this template. You must create an Approval Process for tasks before you can associate it with tasks. Only active approval processes display in the list. For more information about creating Approval Processes, see [Creating Approval Processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. In the **Task Default Custom Forms** box, select the custom form or forms that you want to associate with all new tasks when you add them to a project created from this template. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. For more information about building custom forms, see [Creating Custom Forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). You can associate up to ten custom forms with a task.
1. (Optional) **Select Use Work Effort to automatically calculate task Planned Hours** if you want to enable managing task effort by using&nbsp;Work Effort instead of Planned Hours in the project created from the template.
1. (Conditional and optional) If you selected Use Work Effort to automatically calculate task Planned Hours, click the drop-down menu to update the percentage for each level of Work Effort. The following percentage values are the defaults:
 
   | Work Effort level |Percentage value|
   |---|---|
   | Small |25% |
   | Medium |50% |
   | Large |75% |

  For information about using Work Effort to manage the effort on tasks on projects, see [Work Effort overview](../../../manage-work/tasks/task-information/work-effort.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Issues {#issues}

By editing issue settings, you can prevent users from adding issues inline in the future project created from the template.

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Issues**.

   ![](assets/edit-template-box-with-issues-nwe-350x171.png)

1. (Optional) Deselect the **Allow users to add issues inline** option. It is enabled by default.

   When disabling this option users cannot add issues inline to the project or the tasks in the Issues section, when the project is created from the template.

   >[!TIP]
   >
   >Disable this option if you want to enforce users to complete the New Issue Fields or the custom forms associated with new issues.

   When disabling this option, users with permissions to add issues to the project created from the template can do so by using the New Issue button or a request queue associated with the project.

   For more information about configuring issue settings on projects, see the [Issue Settings](../../../manage-work/projects/manage-projects/edit-projects.md#issue) section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

   For information about creating issues on projects, see [Create issues](../../../manage-work/issues/manage-issues/create-issues.md). 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Comment {#comment}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Comment**.

   ![edit_templates_comment.png](assets/edit-templates-comment-with-tasks-and-issues-350x177.png)

1. Specify a comment that you want to display in the updates stream of the template in the available field.

   This comment is visible for everyone with View access to the template and with access to view Notes.

1. Click **Save Changes**.

   Your changes will be submitted for this template.

   Now, when you use this template to create a project all these settings will transfer to the new project.


   <!--drafted section below for the edit template story: 
   remove this tag and add the Preview blurb at the top of this article in yellow, if it's not already there. Keep the "div class" tags below until 23.1 production: 


### Edit a template in the Preview environment {#edit-a-template-in-the-preview-environment}
-->

1. Accédez au modèle que vous souhaitez modifier.
1. (Conditionnel) Pour modifier des informations limitées sur le modèle, cliquez sur **Détails du modèle** dans le panneau de gauche, accédez ensuite aux zones répertoriées dans le panneau de gauche pour modifier les informations de chaque zone.
1. Pour modifier les informations de la section Détails, cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png), puis sélectionnez l’une des zones ci-dessous ou cliquez sur **Tout modifier** pour modifier les informations dans toutes les zones :

   * Vue d’ensemble
   * Formulaires personnalisés

   Les noms des formulaires douaniers ne s’affichent que s’il existe des formulaires personnalisés associés à l’objet.

   * Finances

   >[!TIP]
   >
   >Pour plus d’informations sur tous les champs qui s’affichent dans la zone Détails, continuez à modifier tous les champs à l’aide de la zone Modifier le modèle ci-dessous.

1. (Conditionnel) Pour modifier toutes les informations relatives au modèle, cliquez sur le bouton **Plus** menu ![](assets/qs-more-icon-on-an-object.png) en regard du nom du modèle, puis cliquez sur **Modifier**.

   La variable **Modifier le modèle** s’ouvre. Les sections de cette zone contiennent les mêmes champs que ceux disponibles dans la section Détails du modèle .

1. Tenez compte de la modification des informations dans l’une des sections suivantes :

   * [Nom du modèle](#template-name)
   * [Présentation](#overview-preview)
   * [Finance](#finance-preview)
   * [Formulaires personnalisés](#custom-forms-preview)
   * [Paramètres du projet](#project-settings)
   * [Paramètres des tâches](#task-settings)
   * [Paramètres de problème](#issue-settings)
   * [Accès](#access-preview)


### Nom de modèle{#template-name}

1. Commencez à modifier votre modèle comme décrit ci-dessus.
1. Dans le **Modifier le modèle** , cliquez sur **Nom du modèle**.
1. (Facultatif) Continuez à modifier les sections suivantes, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.



### Vue d’ensemble {#overview-preview}

1. Commencez à modifier votre modèle comme décrit ci-dessus.
1. Dans le **Modifier le modèle** , cliquez sur **Présentation**.

   ![](assets/edit-template-box-overview-section.png)

1. Mettez à jour les champs suivants :

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
         <tr> 
         <td role="rowheader"><strong>Description</strong></td> 
         <td>Ajoutez des informations supplémentaires sur le modèle.</td> 
       </tr> 
         <tr> 
         <td role="rowheader"><strong>Priorité</strong></td> 
         <td><p>Il s’agit simplement d’un indicateur visuel qui vous permet de prioriser vos projets futurs. Sélectionnez l’une des options suivantes :</p> 
         <ul> 
         <li><p><strong>Aucun</strong></p></li> 
         <li><p><strong>Faible</strong></p></li> 
         <li><p><strong>Normal</strong></p></li> 
         <li><p><strong>Élevé</strong></p></li> 
         <li><p><strong>Urgent</strong></p></li> 
         </ul><p><p>Selon les préférences du projet sélectionnées par votre administrateur Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur la modification des priorités, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Créer et personnaliser des priorités</a>.</p></p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>URL</strong></td> 
         <td>Indiquez un lien Web correspondant aux informations sur ce modèle.</td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>Type de condition</strong></td> 
       <td><p>Effectuez une sélection parmi les types de condition suivants :</p> 
         <ul> 
         <li><strong>Manuel :</strong> Le propriétaire du projet définit manuellement la condition du projet. <strong></strong></li> 
         <li><strong>État de progression :</strong> Workfront définit automatiquement la condition du futur projet en fonction de l’état d’avancement des tâches sur le chemin critique. Pour plus d’informations sur la compréhension de l’état de progression, voir <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Présentation de l’état de progression de la tâche</a>.</li> 
       </ul>
         </td> 
         </tr> 
       <tr> 
         <td role="rowheader"><strong>Mode horaire</strong></td> 
         <td><p>Indiquez si le projet utilisant ce modèle est planifié à partir du <strong>Date de début</strong>, ou depuis le <strong>Date d’achèvement</strong>. Cette sélection détermine les dates prévues des futures tâches du projet à l’aide de ce modèle. </p><p>Sélectionnez l’une des options suivantes : </p> 
       <ul> 
       <li><p><strong>Planifier à partir de la date de début</strong>: la Date de début du modèle est en fait le Jour de début. Lorsque vous planifiez un modèle à partir de la date de début, Adobe Workfront calcule le jour de fin du modèle en fonction de la durée de toutes les tâches du modèle. Le Jour de début du modèle devient la Date de début planifiée du futur projet.</p></li> 
       <li><p><strong>Planifier à partir de la date de fin</strong>: la date de fin du modèle correspond en fait au jour de fin. Lorsque vous planifiez un modèle à partir de la date de fin, Workfront calcule le jour de début du modèle en fonction de la durée de toutes les tâches du modèle. Le jour d’achèvement du modèle devient la Date d’achèvement planifiée du futur projet. </p></li> 
       </ul><p>Pour plus d’informations sur les jours de début et de fin des tâches de modèle, voir <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Présentation des jours de début et de fin dans un modèle</a>. </p><p>Le paramètre Planifier à partir des modèles est similaire à celui des projets. L’administrateur de Workfront sélectionne le paramètre de planification à partir de par défaut pour les projets de votre système. Pour plus d’informations sur la définition des paramètres par défaut d’un projet, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p></td> 
       </tr>

   <tr> 
         <td role="rowheader"><strong>Portfolio</strong></td> 
         <td><p>Spécifiez un Portfolio pour les projets créés à partir de ce modèle. Vous devez d’abord créer un Portfolio avant qu’il ne s’affiche dans la liste déroulante. </p><p>Seuls les portefeuilles actifs s’affichent dans la liste. Pour plus d’informations sur la création de portfolios, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Création d’un portfolio </a>.</p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Programme</strong></td> 
         <td><p>Si vous avez sélectionné un Portfolio pour le modèle, indiquez un <strong>Programme</strong> pour le futur projet. Certains Portfolios peuvent ne pas avoir de programmes. Vous devez d’abord créer un programme avant qu’il n’apparaisse dans cette liste déroulante. Seuls les programmes actifs s’affichent dans la liste.</p><p>Pour plus d’informations sur la création de programmes, voir <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Créer un programme</a>.</p></td> 
       </tr>  
       <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
         <td role="rowheader"><strong>Groupe</strong></td> 
         <td><p>Dans la liste déroulante, sélectionnez le groupe à associer aux projets créés à partir du modèle. Il peut s’agir d’un groupe de n’importe quel niveau. </p><p>Vous pouvez vous assurer que vous sélectionnez le groupe approprié en pointant dessus et en cliquant sur l’icône d’information. <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus de celui-ci et ses administrateurs.</p> <p><b>NOTES</b>

   <ul> 
       <li><p>Dans la zone Projets de la page d’un groupe, lorsqu’une personne crée un projet à l’aide d’un modèle pour lequel aucun groupe n’est sélectionné, le système associe le groupe ouvert au projet.</p><p>Cela diffère des autres zones où le système associe le groupe d’accueil d’un utilisateur au projet lorsque l’utilisateur crée le projet à l’aide d’un modèle dont le groupe n’est pas sélectionné.</p></li> 
       <li><p>Si un utilisateur sélectionne un modèle dont un groupe est sélectionné lors de la création d’un projet, ou lors de la conversion d’une tâche ou d’un problème en projet, il peut choisir un autre groupe pour le projet.</p></li> 
       <li>Bien que ce champ ne soit disponible dans les modèles que dans la nouvelle expérience Adobe Workfront, vous pouvez le voir dans les listes et les rapports à cet endroit et dans Adobe Workfront Classic. </li> 
         </ul> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Entreprise</strong></td> 
         <td><p>Indiquez la Société que vous souhaitez associer au modèle. Seules les entreprises actives s’affichent dans la liste.</p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Propriétaire du modèle</strong></td> 
         <td><p>L’utilisateur désigné comme propriétaire des modèles doit être un utilisateur actif Workfront. </p><p>Tenez compte des points suivants concernant l’utilisateur désigné comme propriétaire du modèle : </p> 
         <ul> 
         <li>Les autorisations Gérer leur sont automatiquement accordées au modèle. </li> 
         <li>Ils sont ajoutés à l’équipe du projet et reçoivent automatiquement les autorisations de gestion du projet créé à partir du modèle. </li> 
         <li>Ils deviennent le propriétaire du projet lorsque le projet est créé à partir de ce modèle. </li> 
         <li> Si l’utilisateur désigné comme propriétaire des modèles dispose d’un accès limité aux modèles ou aux projets à partir de son niveau d’accès, ses autorisations Gérer sur le modèle et sur les projets seront limitées. Par exemple, s’ils disposent uniquement de l’accès Affichage pour les modèles ou les projets dans leur niveau d’accès, ils recevront automatiquement l’autorisation Affichage pour le modèle et le projet lorsqu’ils seront désignés comme propriétaire de modèle.</li>
         </ul></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Sponsor du modèle</strong></td> 
         <td><p>L’utilisateur spécifié dans ce champ devient le parrain du projet, lorsque le modèle est ajouté au projet. Cet utilisateur est ajouté à l’équipe du projet et se voit attribuer automatiquement des autorisations d’affichage sur le projet. L’utilisateur désigné comme parrain de modèle doit être un utilisateur actif Workfront. </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Gestionnaire des ressources</strong></td> 
         <td><p>Les utilisateurs spécifiés disposent automatiquement des autorisations de gestion pour les projets futurs et peuvent affecter des ressources aux tâches et problèmes des projets. Vous pouvez spécifier plusieurs gestionnaires de ressources. </p></td> 
       </tr> 
      </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Finances {#finance-preview}

1. Commencez à modifier votre modèle comme décrit ci-dessus.
1. Dans le **Modifier le modèle** , cliquez sur **Finance**.

   ![](assets/edit-template-box-finance-section.png)

1. Mettez à jour les champs suivants :

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody>
       <tr> 
         <td role="rowheader"><strong> Devise</strong></td> 
         <td><p>Indiquez la devise du projet futur, si elle est différente de la devise par défaut de votre système. Ce champ n’est pas visible si vous avez uniquement la devise par défaut dans le système.<br>Pour plus d’informations sur la devise, voir <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurer les taux de change</a>.</p></td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>Budget</strong></td> 
       <td><p>Spécifiez un Budget pour les projets créés à partir de ce modèle.</p></td> 
       </tr>  
       <tr> 
         <td role="rowheader"><strong>Méthode d'indice de performances</strong></td> 
         <td><p>Choisissez la manière dont Workfront calculera les mesures de la valeur obtenue du futur projet. Choisissez l’une des options suivantes :
         <ul>
         <li>Basé sur les heures</li>
         <li>Basé sur les coûts</li>
         </ul>

   Pour plus d’informations sur la méthode d’index de performance, voir <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Définition de la méthode d’index de performance (PIM)</a>. </p></td>
   </tr> 
         <tr> 
         <td role="rowheader"><strong>Bénéfice prévu</strong></td> 
         <td><p>Indiquez l’avantage planifié des projets créés à partir de ce modèle. L’avantage planifié est utilisé dans l’analyse de cas du projet et dans Portfolio Optimizer. </p><p>Pour plus d’informations sur les avantages prévus d’un projet, voir <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Aperçu des avantages prévus du projet</a>. L’avantage planifié d’un projet est pris en compte lors du calcul de la valeur nette d’un projet. </p><p>Pour plus d’informations sur l’utilisation de Portfolio Optimizer, voir <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Gestion des projets dans Portfolio Optimizer</a> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Coûts fixes</strong></td> 
         <td><p>Indiquez le coût fixe des projets créés à partir de ce modèle. C'est différent du coût du travail qui provient des heures sur le projet et du coût des dépenses qui provient du montant des dépenses sur le projet. Le coût fixe d'un projet est pris en compte dans le calcul de la valeur nette d'un projet et fait partie du coût budgété.</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Revenus fixes</strong></td> 
       <td><p>Définissez les Recettes fixes pour les projets créés à partir de ce modèle.</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>L'approbation pour ce projet demande du temps</strong></td> 
       <td><p>Sélectionnez cette option pour exiger du propriétaire du projet à venir créé à partir de ce modèle qu’il approuve l’heure de connexion au projet. Si vous utilisez des enregistrements de facturation et que vous sélectionnez cette option, seules les heures approuvées sur le projet apparaissent comme des heures facturables disponibles pour les enregistrements de facturation. La validation du temps sur le projet est indépendante de la validation des feuilles de temps. Pour plus d’informations sur le temps nécessaire à l’approbation d’un projet, voir <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Requiert du temps pour approuver un projet</a>.</p></td> 
       </tr> 
       </tbody> 
      </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Formulaires personnalisés {#custom-forms-preview}

1. Commencez à modifier votre modèle comme décrit ci-dessus.
1. Dans le **Modifier le modèle** , cliquez sur **Forms personnalisée**.

   ![](assets/edit-template-box-custom-forms-section.png)

   Les noms des formulaires personnalisés déjà joints au modèle s’affichent dans le panneau de gauche.

1. Cliquez dans le **Ajouter un formulaire personnalisé** et sélectionnez le ou les formulaires personnalisés à associer au modèle. Vous devez créer les formulaires personnalisés avant qu’ils ne soient disponibles pour la sélection dans ce champ.

   Seuls les formulaires personnalisés actifs s’affichent dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   Vous pouvez ajouter jusqu’à dix formulaires personnalisés à un modèle.

   Les formulaires seront ajoutés au projet créé à partir de ce modèle.

1. (Facultatif) Mettez à jour les informations dans l’un des champs des formulaires personnalisés. Les informations seront transférées vers les projets qui seront créés à partir du modèle.

1. (Facultatif) Cliquez sur le **x** à droite d’un nom de formulaire personnalisé, puis cliquez sur **Supprimer** pour la supprimer du modèle.

1. (Facultatif) Continuez à modifier la section suivante, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Paramètres du projet {#project-settings}

1. Commencez à modifier votre modèle comme décrit ci-dessus.
1. Dans le **Modifier le modèle** , cliquez sur **Paramètres du projet**.

   ![](assets/edit-template-box-project-settings-section.png)

1. Mettez à jour les champs suivants :

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
       <td role="rowheader"><strong>Chemin Milestone</strong> </td> 
       <td> <p>Sélectionnez un Chemin d’accès Milestone pour le modèle. Seuls les chemins de jalon actifs s’affichent dans la liste.<br>Pour plus d’informations sur les chemins d’accès Milestone, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Création d’un chemin de jalon</a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Mode d’achèvement</strong> </td> 
         <td> <p>Contrôle la manière dont le futur projet sera marqué comme terminé. <br>Sélectionnez l’une des options suivantes :</p> 
         <ul> 
         <li> <p><strong>Automatique</strong>: le projet est marqué Terminé lorsque toutes les tâches et tous les problèmes sont terminés.</p> </li> 
         <li> <p><strong>Manuel</strong>: lorsque toutes les tâches et tous les problèmes sont terminés, vous devez sélectionner manuellement l’état Terminé du projet. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Mode d’achèvement du résumé</strong> </td> 
       <td> <p>Contrôle la manière dont les tâches parentes sur le futur projet sont marquées comme étant terminées. <br>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
       <li> <p><strong>Automatique</strong>: les tâches parentes sont marquées comme Terminé et elles mettent à jour leur pourcentage automatiquement, à mesure que les tâches enfants sont terminées et que le pourcentage d’enfants terminés est mis à jour. </p> </li> 
       <li> <p><strong>Manuel</strong>: vous devez mettre à jour manuellement le pourcentage terminé et l’état des tâches parents, indépendamment des modifications apportées aux tâches enfants. </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Type de mise à jour</strong> </td> 
         <td> <p>Contrôle le moment où les modifications que vous apportez à la chronologie du futur projet sont enregistrées dans le projet. </p> 
         <b>EXEMPLE </b> 
         <p>Les modifications suivantes apportées au projet déclenchent une mise à jour de la chronologie du projet :</p> 
         <ul> 
         <li> <p>mettre à jour les dates des tâches</p> </li> 
         <li> <p>changer les relations antérieures<br></p> </li> 
         <li> <p>changement des relations parents-enfants</p> </li> 
         <li> <p>ajouter ou supprimer des affectations en plus de modifier la contrainte de tâche ou le type de durée.</p> </li> 
         </ul> 
         </div> <p>Sélectionnez l’une des options suivantes :<br></p> 
         <ul> 
         <li> <p><strong>Automatique et Activé</strong> (Paramètre par défaut) : la chronologie du futur projet est mise à jour chaque fois qu’une modification se produit dans le projet ou dans un autre projet dont dépend la chronologie (Activé). La chronologie du projet est également mise à jour chaque nuit (automatique).<br>Il s’agit du paramètre recommandé pour ce champ, car il garantit que la chronologie du projet est toujours à jour.<br>Lorsque vous effectuez une action sur une tâche ou un projet qui déclenche un nouveau calcul de frise chronologique, toutes les dates disponibles sont immédiatement affichées, ce qui vous permet de continuer à travailler. Sur les projets comportant plus de 100 tâches, les dates nécessitant des nouveaux calculs plus longs s’affichent brièvement comme point d’interrogation (entre 1 et 5 secondes, ou jusqu’à une minute pour les projets volumineux). Cela indique que le recalcul n'est pas encore terminé et que les dates peuvent être modifiées.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Modifier uniquement</strong>: la chronologie du projet est mise à jour chaque fois qu’une modification se produit dans le projet ou dans un autre projet dont elle dépend. Vous pouvez sélectionner cette option si des modifications se produisent rarement dans le projet ou dans d’autres projets dont dépend la chronologie.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Automatique uniquement</strong>: la chronologie du projet est mise à jour chaque nuit ; elle n’est pas mise à jour immédiatement une fois les modifications effectuées.<br>Vous pouvez sélectionner cette option si de nombreuses modifications se produisent chaque jour dans le projet ou dans d’autres projets dont dépend la chronologie. Sachez toutefois que vous avez choisi ce paramètre, car le projet ne se mettra pas à jour en même temps que les modifications sont effectuées.<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>Manuel uniquement</strong>: la chronologie du projet est mise à jour uniquement lorsque vous sélectionnez l’option Recalculer les chronologies, comme décrit dans la section <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculer les calendriers du projet</a>.<br></p> </li> 
         </ul> <p>Vous pouvez sélectionner cette option si vous apportez simultanément de nombreuses modifications au projet et si vous souhaitez que le recalcul de la chronologie se produise une fois toutes les modifications effectuées (plutôt qu’après chaque modification individuelle).</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Planning</strong> </td> 
         <td> <p>Sélectionnez un planning pour votre modèle. Il deviendra le planning du projet créé à partir de ce modèle. Il doit s’agir du même planning que celui attribué à la plupart des personnes qui travaillent sur le projet. Vous devez créer un planning avant de pouvoir l'affecter à un modèle.<br>Pour plus d’informations sur la création de plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Création d’un planning</a>. <br>Si vous n’avez pas créé de plannings personnalisés dans votre système, la planification par défaut est sélectionnée. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Heure de désactivation de l’utilisateur</strong> </td> 
         <td> <p>Détermine si le délai de désactivation du cessionnaire Principal d’une tâche ajuste les dates planifiées de la tâche. Lorsque vous joignez le modèle à un projet existant et que le paramètre de ce champ est différent de celui du projet, le paramètre du projet reste inchangé. L’option par défaut de ce paramètre pour un nouveau modèle est la même que la préférence de projet au niveau du système. </p> <p>Pour plus d’informations sur les préférences du projet au niveau du système, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>. </p> <p>Pour plus d’informations sur l’impact de ce paramètre sur les dates de tâche d’un projet, voir <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modification de projets</a>.<br>Sélectionnez l’une des options suivantes :<br></p> 
         <ul> 
         <li> <p><strong>Tenir compte du temps d’arrêt de l’utilisateur dans les durées de tâche</strong>: lorsque vous sélectionnez cette option, les dates planifiées des tâches sur le projet créé à partir de ce modèle s’ajustent en fonction de la date de désactivation du Principal cessionnaire de la tâche, si la durée de la tâche est décalée. </p> </li> 
         <li> <p><strong>Ignorer le temps d’arrêt des utilisateurs dans les durées de tâche</strong>: lorsque vous sélectionnez cette option, les dates planifiées des tâches sur le projet créé à partir de ce modèle restent inchangées, même si le responsable Principal de la tâche a expiré pendant la durée de la tâche. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Mode de niveau des ressources</strong> </td> 
         <td> <p>Sélectionnez l’une des options suivantes :<br></p> 
         <ul> 
         <li> <p><strong>Manuel</strong>: vous devez mettre à niveau manuellement vos ressources sur le projet créé à partir de ce modèle (il s’agit du paramètre par défaut).</p> </li> 
         <li> <p><strong>Automatique :</strong> Workfront met à niveau les ressources sur le futur projet. <br>Pour plus d’informations sur le niveau de ressource, voir <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Ressources de niveau dans le diagramme de Gantt </a>. </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Risque</strong> </td> 
         <td> <p>Définissez le niveau de risque des projets créés à partir de ce modèle. Le risque n'est qu'un indicateur des risques que peut représenter un projet. Vous pouvez hiérarchiser l’exécution de vos projets en fonction du niveau de risque.<br>Envisagez de choisir parmi les niveaux de risque suivants :<br></p> 
         <ul> 
         <li> <p><strong>Très faible</strong> </p> </li> 
         <li> <p><strong>Faible</strong> </p> </li> 
         <li> <p><strong>Volume moyen</strong> </p> </li> 
         <li> <p><strong>Élevée</strong> </p> </li> 
         <li> <p><strong>Très élevé</strong> </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Pools de ressources</strong> </td> 
         <td> <p>Indiquez les pools de ressources associés au modèle. Les pools de ressources sont des groupes d’utilisateurs qui sont nécessaires en même temps pour la fin d’un projet. Pour plus d’informations sur les pools de ressources, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Présentation des pools de ressources </a>.</p> <p> <p><b>NOTE</b>

   Lorsque vous modifiez des modèles en bloc, seuls les pools de ressources communs à tous les modèles sélectionnés apparaissent dans ce champ. Si les modèles sélectionnés ne comportent aucun pool de ressources partagées, ce champ sera vide. Les pools de ressources que vous spécifiez ici remplaceront les pools de ressources individuels des modèles.</p> </p> </td>
   </tr>
       <tr> 
         <td role="rowheader"><strong>Type d’heures de filtre</strong> </td> 
         <td> <p>Tenez compte des points suivants :</p> <p>Sélectionner <strong>Non</strong> pour rendre tous les types d’heures spécifiques au projet disponibles sur le futur projet. (Il s’agit de la sélection par défaut)</p> <p>Ou</p> <p>Sélectionner <strong>Oui</strong> pour rendre disponible uniquement un sous-ensemble des types d’heures spécifiques au projet dans le futur projet, sélectionnez les types d’heures à rendre disponibles. (Maintenez la touche Maj enfoncée pour sélectionner plusieurs types d’heures.)</p> <p>Si vous sélectionnez cette option, seuls les types d’heures que vous sélectionnez sont disponibles lors de la journalisation des heures sur le projet (ou sur les tâches et problèmes dans le projet). Vous devez sélectionner au moins un type d’heure. Si vous sélectionnez cette option et que vous ne sélectionnez aucun type d’heure, tous les types d’heure sont disponibles sur le projet.</p> <p>Les mêmes sélections de type heure doivent être effectuées au niveau de chaque utilisateur pour que l’utilisateur puisse voir ces options de type heure sur le projet. </p> <p>Pour plus d’informations sur la définition des types d’heures au niveau de l’utilisateur, voir la section <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Temps de connexion</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Temps de connexion</a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Processus de validation</strong> </td> 
         <td> <p>Sélectionnez le processus de validation que vous souhaitez associer au modèle. L’administrateur Workfront ou un utilisateur disposant d’un accès administratif aux processus d’approbation doit définir des processus d’approbation de projet au niveau du système ou du groupe avant de pouvoir les associer à un modèle. Pour plus d’informations sur la création de processus de validation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les tâches</a>.</p> <p>Tenez compte des points suivants lors de l’ajout de processus de validation : </p> 
         <ul> 
         <li>Seuls les processus de validation actifs s'affichent dans la liste. </li> 
         <li> <p>Les processus de validation à l’échelle du système et spécifiques aux groupes s’affichent dans la liste. Un processus de validation associé à un groupe autre que celui du modèle ne s'affiche pas dans la liste.</p> <p><b>IMPORTANT</b>

   Si le groupe associé au modèle change, le processus de validation spécifique au groupe devient un processus de validation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation affectés ?</a>. </p> </li>
   <li> <p>Si vous avez ajouté un processus de validation à usage unique, il s’affiche sous la forme "Personnalisé" dans ce champ. Pour plus d’informations, voir <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associer un processus d’approbation nouveau ou existant au travail</a>. </p> 
         </li> 
         <li> <p>Lors de la modification en masse de modèles, les scénarios suivants se présentent :</p> 
         <ul> 
            <li> <p>Lorsque vous sélectionnez des modèles appartenant au même groupe, les processus de validation au niveau du système et du groupe s’affichent dans ce champ.</p> </li> 
            <li> <p>Lorsque vous sélectionnez des modèles issus de différents groupes, seuls les processus de validation au niveau du système s’affichent dans ce champ.</p> </li> 
            <li> <p>Lorsque l’un des modèles est associé à un processus de validation à usage unique, il est remplacé par le niveau système que vous sélectionnez. </p> </li> 
         </ul> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Notification de rappel</strong> </td> 
         <td>Sélectionnez la notification de rappel qui doit être associée au futur projet. Pour que ce champ s’affiche lors de la modification d’un modèle, vous devez configurer les notifications de rappel pour les projets. <br>Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configuration des notifications de rappel</a>.</td> 
       </tr> 
       </tbody> 
      </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.\
   Ou
1. Cliquer sur **Enregistrer**.

### Paramètres de la tâche {#task-settings}

Vous pouvez définir les valeurs par défaut qui seront associées à toutes les nouvelles tâches lorsque vous les ajoutez à un projet créé à partir du modèle.

Pour plus d’informations sur l’impact de ces paramètres sur la création de nouvelles tâches, voir [Présentation de la création de tâches](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Commencez à modifier votre modèle comme décrit ci-dessus.
1. Dans le **Modifier le modèle** , cliquez sur **Paramètres de tâche**.

   ![](assets/edit-template-box-tax-settings-section.png)

1. Dans le **Processus d’approbation par défaut de la tâche** sélectionnez le processus d’approbation à associer à toutes les nouvelles tâches lorsque vous les ajoutez à un projet créé à partir de ce modèle. Vous devez créer un processus d’approbation pour les tâches avant de pouvoir l’associer à des tâches. Seuls les processus de validation actifs s&#39;affichent dans la liste. Pour plus d’informations sur la création de processus d’approbation, voir [Création de processus de validation](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. Dans le **Task Default Custom Forms** sélectionnez le ou les formulaires personnalisés à associer à toutes les nouvelles tâches lorsque vous les ajoutez à un projet créé à partir de ce modèle. Vous devez créer les formulaires personnalisés avant qu’ils ne soient disponibles pour la sélection dans ce champ. Seuls les formulaires personnalisés actifs s’affichent dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir [Création d’un Forms personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Vous pouvez associer jusqu’à dix formulaires personnalisés à une tâche.
1. (Facultatif) Sélectionnez **Utiliser l’effort de travail pour calculer automatiquement les heures planifiées de la tâche** si vous souhaitez activer la gestion de l’effort de tâche en utilisant l’effort de travail au lieu des heures planifiées dans le projet créé à partir du modèle.
1. (Conditionnel et facultatif) Si vous avez sélectionné Utiliser l’effort de travail pour calculer automatiquement les heures planifiées de la tâche, cliquez sur le menu déroulant pour mettre à jour le pourcentage pour chaque niveau d’effort de travail. Les valeurs en pourcentage suivantes sont les valeurs par défaut :

   | Niveau de l’effort de travail | Valeur en pourcentage |
   |---|---|
   | Petite | 25 % |
   | Moyen | 50 % |
   | Grande | 75 % |

   Pour plus d’informations sur l’utilisation de l’effort de travail pour gérer l’effort sur les tâches sur les projets, voir [Présentation de l’effort de travail](../../../manage-work/tasks/task-information/work-effort.md).

1. (Facultatif) Continuez à modifier la section suivante, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Paramètres de l&#39;événement {#issue-settings}

En modifiant les paramètres des problèmes, vous pouvez empêcher les utilisateurs d’ajouter des problèmes en ligne dans le futur projet créé à partir du modèle.

1. Commencez à modifier votre modèle comme décrit ci-dessus.
1. Dans le **Modifier le modèle** , cliquez sur **Paramètres de problème**.

   ![](assets/edit-template-box-issue-settings-section.png)

1. (Facultatif) Désélectionnez l’option **Autoriser les utilisateurs à ajouter des problèmes en ligne** . Elle est activée par défaut.

   Lorsque vous désactivez cette option, les utilisateurs ne peuvent pas ajouter de problèmes en ligne au projet ou aux tâches de la section Problèmes, lorsque le projet est créé à partir du modèle.

   >[!TIP]
   >
   >Désactivez cette option si vous souhaitez obliger les utilisateurs à remplir les champs New Issue Fields ou les formulaires personnalisés associés aux nouveaux problèmes.

   Lorsque vous désactivez cette option, les utilisateurs autorisés à ajouter des problèmes au projet créé à partir du modèle peuvent le faire à l’aide du bouton Nouveau problème ou d’une file d’attente de requêtes associée au projet.

   Pour plus d’informations sur la configuration des paramètres de problème sur les projets, voir la section [Paramètres de problème](../../../manage-work/projects/manage-projects/edit-projects.md#issue) dans l’article [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

   Pour plus d’informations sur la création de problèmes sur les projets, voir [Création de problèmes](../../../manage-work/issues/manage-issues/create-issues.md).

1. (Facultatif) Continuez à modifier la section suivante, en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

### Accès {#access-preview}

1. Commencez à modifier votre modèle comme décrit ci-dessus.
1. Dans le **Modifier le modèle** , cliquez sur **Accès**.

   ![](assets/edit-template-box-access-section.png)

   L’ accès que vous spécifiez pour votre modèle devient l’ Accès des utilisateurs associés au projet lorsque le modèle est utilisé pour créer un projet.

   Spécifiez les **Accès** informations pour le modèle :

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
         <td role="rowheader"><strong>Lorsqu’une personne est affectée à une tâche</strong> </td> 
         <td> <p>Sélectionner parmi <strong>Affichage</strong>, <strong>Contribuez,</strong> ou <strong>Gérer</strong> accès à une tâche. L’utilisateur affecté à une tâche se voit automatiquement octroyer cet accès à la tâche. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Accordez également l’accès au projet</strong> </td> 
         <td> <p> Sélectionner parmi <strong>Affichage</strong>, <strong>Contribution</strong>, ou <strong>Gérer</strong> accès au projet. L’utilisateur affecté à une tâche se voit également automatiquement octroyer cet accès au projet. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Lorsqu’une personne est affectée à un problème</strong> </td> 
         <td> <p>Sélectionner parmi <strong>Affichage</strong>, <strong>Contribuez,</strong> ou <strong>Gérer</strong> accès à un problème. L’utilisateur affecté à un problème se voit automatiquement octroyer cet accès au problème. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Accordez également l’accès au projet</strong> </td> 
         <td> <p> Sélectionner parmi <strong>Affichage</strong>, <strong>Contribution</strong>, ou <strong>Gérer</strong> accès au projet. L’utilisateur affecté à un problème se voit également automatiquement octroyer cet accès au projet. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Lorsqu’une personne envoie une demande : donnez-lui un accès</strong> </td> 
         <td> <p> Sélectionner parmi <strong>Affichage</strong>, <strong>Contribution</strong>, ou <strong>Gérer</strong> accès à la requête. Lorsqu’ils envoient une demande au projet, ils se voient accorder cet accès à la demande qu’ils ont envoyée. Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partage d’un problème </a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Les personnes d’une même société hériteront des mêmes autorisations pour toutes les demandes.</strong> </td> 
         <td> <p>Sélectionnez ce champ si vous souhaitez que les personnes de la même société aient le même accès à toutes les demandes du projet, qu’elles les aient soumises ou non.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Lorsqu'une personne a accès à ce projet : lui donner accès à ...</strong> </td> 
         <td> <p>Sélectionnez les options d’accès que vous souhaitez que les utilisateurs disposent sur le projet, si le projet est partagé avec eux. Sélectionnez les options d’accès spécifiques, si elles sont désignées comme <strong>Visionneuses</strong>, <strong>Contributeurs</strong>, ou <strong>Chefs</strong> lors du partage du projet avec eux. </p> </td> 
       </tr> 
       </tbody> 
      </table>

1. (Facultatif) Continuez à modifier les sections suivantes en fonction des informations que vous souhaitez modifier.

   Ou

   Cliquer sur **Enregistrer**.

   Vos modifications seront envoyées pour ce modèle.

   Désormais, lorsque vous utilisez ce modèle pour créer un projet, tous ces paramètres sont transférés vers le nouveau projet.


## Modifier des modèles en bloc

Vous pouvez modifier des modèles en bloc et mettre à jour toutes leurs informations en même temps.

Pour modifier des modèles en bloc :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Modèles**.
1. Sélectionnez plusieurs modèles dans la liste.
1. Cliquez sur **Modifier**.

   La variable **Modifier les modèles** s’ouvre.

   ![](assets/edit-templates-in-bulk-box-nwe-350x327.png)

1. Cliquez sur les sections à gauche pour modifier tous les modèles sélectionnés.

   Pour plus d’informations sur l’édition d’informations sur les modèles, voir la section [Modifier un modèle](#edit-a-template) dans cet article.

1. Cliquez sur **Enregistrer les modifications**.

   Toutes les modifications que vous avez apportées sont désormais visibles sur tous les modèles sélectionnés.

## Ajouter des tâches à un modèle

Après avoir créé votre modèle et modifié ses informations, vous pouvez y ajouter des tâches.

L’ajout de tâches à un modèle est similaire à l’ajout de tâches à un projet.

Pour plus d’informations sur l’ajout de tâches à un projet, voir [Création de tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Lorsque vous ajoutez des tâches à un modèle, la durée du modèle et les jours de début et de fin du modèle changent en conséquence. Pour plus d’informations sur les jours de début et de fin du modèle et les tâches du modèle, voir [Présentation des jours de début et de fin dans un modèle](../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md).

## Ajouter des éléments supplémentaires à un modèle

Après avoir créé votre modèle et modifié ses informations, vous pouvez y ajouter d’autres éléments. Les éléments que vous ajoutez seront disponibles pour le projet lorsque vous le créez à partir du modèle.

L’ajout des éléments suivants à un modèle est identique à leur ajout à un projet :

* Documents
* Risques

  Pour plus d’informations sur la création de risques, voir [Créer et modifier des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md#create)  dans l’article [Créer et modifier des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

* Processus d&#39;approbation

  Pour plus d’informations sur l’association des processus de validation au travail, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

* Taux de facturation

  Pour plus d’informations sur le remplacement des taux de facturation d’un projet, voir [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Frais

  Pour plus d’informations sur l’ajout de dépenses, voir [Gestion des dépenses de projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Groupes de rubriques et rubriques de la file d’attente

  Pour plus d’informations sur l’ajout de groupes de rubriques et de rubriques de file d’attente à un projet ou à un modèle, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Vous pouvez ajouter les éléments suivants aux tâches du modèle :

* Documents
* Frais

  Pour plus d’informations sur l’ajout de dépenses, voir [Gestion des dépenses de projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Approbations

  Pour plus d’informations sur l’association des validations au travail, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).


## Activation ou désactivation d’un modèle

Vous pouvez désactiver un modèle si vous souhaitez que les utilisateurs ne puissent pas le trouver et créer des projets à partir de celui-ci. Vous ne pouvez pas joindre un modèle désactivé aux projets ni l’utiliser pour créer un projet.

Les modèles désactivés n’affectent pas les projets existants qui ont été créés à l’aide de ces derniers.

Pour désactiver un modèle :

1. Accédez à un modèle actif, puis cliquez sur le bouton **Plus** ![](assets/qs-more-icon-on-an-object.png) en regard du nom du modèle, puis cliquez sur **Désactiver**.

   ![](assets/deactivate-template-link-in-more-menu.png)

   Le modèle n’est plus actif et les utilisateurs ne peuvent plus le trouver pour créer des projets à partir de celui-ci.
1. (Facultatif) Cliquez sur le bouton **Plus** ![](assets/qs-more-icon-on-an-object.png) en regard du nom du modèle, puis cliquez sur **Activer**.

   Le modèle est maintenant actif et peut être joint à des projets ou utilisé pour créer des projets.