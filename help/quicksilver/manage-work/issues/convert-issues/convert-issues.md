---
product-area: projects
navigation-topic: convert-issues
title: Vue d’ensemble des problèmes de conversion dans Adobe Workfront
description: Si vous devez travailler plus pour résoudre un problème après sa soumission, vous pouvez convertir ce problème en projet ou en tâche.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 100%

---

# Vue d’ensemble des problèmes de conversion dans Adobe Workfront

Si vous devez travailler plus pour résoudre un problème après sa soumission, vous pouvez convertir ce problème en projet ou en tâche.

Pour plus d’informations sur la conversion de problèmes en tâches, voir [Convertir un problème en tâche dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md).

Pour plus d’informations sur la conversion de problèmes en projets, voir [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Considérations relatives à la conversion de problèmes

* Lors de la conversion de problèmes en tâches ou en projets, la plupart des informations du problème sont transférées à la tâche ou au projet, sauf exceptions spécifiées dans cet article.
* L’administrateur ou administratrice Workfront ou de groupes a déjà défini les préférences pour ce qui arrive à un problème, sa résolution et l’accès de son contact principal lorsqu’il est converti en projet ou en tâche, comme indiqué dans la section [Configurer des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Workfront supprime les approbations associées aux problèmes lors de la conversion.
* Workfront remplace l’objet de résolution du problème lorsque vous le convertissez en tâche ou en projet. La nouvelle tâche ou le nouveau problème devient le nouvel objet de résolution du problème après la conversion.
* Tenez compte des points suivants :

   * Pendant la conversion, on vous demandera peut-être si vous souhaitez conserver le problème et sa résolution liés projet ou la tâche que vous créez.
   * Si vous conservez le problème, le statut et le pourcentage terminé du projet ou de la tâche mettent automatiquement à jour le statut et le pourcentage terminé du problème lorsque des modifications se produisent sur le projet, la tâche ou le problème, ou lorsque Workfront recalcule la chronologie.

* Lors de la conversion d’un problème en une tâche ou un projet, le problème est supprimé de la zone Accueil de la personne affectée au problème.

* Lors de la conversion d’un problème, les autorisations liées aux problèmes originaux ne sont pas transférées vers l’objet converti (tâche ou projet).

* Lors de la conversion d’un problème en projet à l’aide d’un modèle, la plupart des informations du modèle sont transférées vers le nouveau projet. Cependant, certaines informations provenant du problème peuvent également être transférées vers le nouveau projet. Pour plus d’informations, voir la section [Vue d’ensemble des champs du projet lors de la conversion d’un problème en projet à l’aide d’un modèle](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) dans cet article.
* Lors de la conversion d’un problème, tous les documents ou leurs informations ne sont pas déplacés vers le nouvel objet vers lequel le problème est converti. Les éléments suivants sont inclus lorsque vous convertissez un problème auquel sont associés des documents ou des liens vers des documents :

   * Document
   * Le document est lié à des services tiers, tels que Google Drive ou SharePoint.
   * Versions
   * Les épreuves ne sont incluses que lorsque l’option **Conserver le problème original et lier sa résolution à cette tâche** n’est pas sélectionnée.
   * Les approbations de documents ne sont pas incluses lorsque vous convertissez un problème auquel des documents et des liens de documents sont joints.

* Si vous avez décidé de conserver le problème dans la conversion et que des documents y sont joints, le document et ses versions sont copiés dans le projet ou la tâche. Les épreuves et les approbations de document ne sont pas copiés dans le projet ou la tâche.
* Si vous avez décidé de ne pas conserver le problème dans la conversion et que des documents y sont joints, le document, ses versions et les épreuves sont transférés vers le projet ou la tâche. Les approbations de document ne seront pas transférées vers le projet ou la tâche.
* Si des documents et des dossiers sont liés au problème original de services tiers, tels que Google Drive, que vous gardiez le problème ou non pendant la conversion, ces liens seront copiés dans le nouvel objet.
* Les commentaires de problème sont également copiés dans la tâche ou le projet converti à partir du problème, mais les personnes taguées ne seront pas transférées.
* Si vous souhaitez transférer des informations de formulaire personnalisé du problème vers le projet ou la tâche vers lequel vous le convertissez, assurez-vous que vous disposez d’un formulaire personnalisé de projet ou de tâche qui comprend les mêmes champs que ceux que vous souhaitez transférer depuis le problème. Pour plus d’informations, voir [Transférer des données de formulaire personnalisé lors de la conversion d’un objet](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## Vue d’ensemble des champs d’un projet lors de la conversion d’un problème en projet à l’aide d’un modèle {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

Lors de la conversion d’un problème en projet, vous pouvez le convertir en projet vierge ou utiliser un modèle.

Pour plus d’informations, voir [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

Lors de l’utilisation d’un modèle, certains champs renseignés sur le modèle sont transférés vers le projet créé à partir du problème converti. D’autres champs sont transférés vers le projet à partir du problème converti.

Le tableau suivant répertorie les informations sur le projet et indique si elles sont transférées depuis le modèle ou le problème :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Description</td> 
   <td> <p>La description du problème est transférée au nouveau projet. </p> <p> S’il n’existe aucune description du problème, la description du modèle est transférée au projet. </p> <p>Si le champ Description est vide à la fois pour le problème et pour le modèle, le champ est vide sur le projet. </p> </td> 
  </tr> 
  <tr> 
   <td>Statut</td> 
   <td>Statut par défaut sélectionné pour le groupe sur le modèle. Si le modèle n’est pas associé au groupe, le statut du projet est défini sur le statut par défaut par l’administrateur ou l’administratrice Workfront dans la zone Préférences de projet dans Configuration. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences du projet à l’échelle du système</a>.</td> 
  </tr> 
  <tr> 
   <td>Priorité</td> 
   <td><p>Est transféré à partir du problème.</p>
   <p>Lorsque vous utilisez un modèle pour le projet converti, vous avez la possibilité de modifier manuellement la priorité. Si vous choisissez de ne pas la modifier, la priorité du problème est transférée au projet. 
    </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>L’URL du problème est transférée au nouveau projet. </p> <p> Si aucune URL n’est spécifiée dans le problème, l’URL du modèle est transférée au projet. </p> <p>Si le champ URL est vide à la fois pour le problème et pour le modèle, le champ est vide sur le projet. </p> </td> 
  </tr> 
  <tr> 
   <td>Type de condition du projet</td> 
   <td>Est transféré à partir du modèle.</td> 
  </tr> 
  <tr> 
   <td>Statut du projet</td> 
   <td>Correspond à la préférence par défaut au niveau du système, déterminée par l’administrateur ou administratrice Workfront dans la zone Configuration. Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Définir une condition personnalisée comme condition par défaut pour les projets</a>.</td> 
  </tr> 
  <tr> 
   <td>Planifier à partir de</td> 
   <td>Est transféré à partir du modèle.</td> 
  </tr> 
  <tr> 
   <td>Dates de projets</td> 
   <td> 
    <ul> 
     <li> <p><b>Date de début prévue</b> : le temps de travail le plus proche basé sur le temps de travail du planning du modèle doit être présélectionné, en fonction du fuseau horaire du planning du modèle. Ce champ est désactivé si le champ Planifier à partir de est défini sur À partir de l’achèvement. </p> </li> 
     <li> <p><b>Date d’achèvement prévue</b> : le temps de travail le plus proche, basé sur le temps de travail du planning du modèle, doit être présélectionné, en fonction du fuseau horaire de planning du modèle. Ce champ est désactivé si le champ Planifier à partir de est défini sur Dès le début. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Est transféré à partir du modèle. Sinon, ce champ est vide.</td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>Est transféré à partir du modèle. Sinon, ce champ est vide.</td> 
  </tr> 
  <tr> 
   <td>Groupe</td> 
   <td><p> Les scénarios suivants sont possibles :</p>
     <ul><li>Si un groupe est spécifié pendant la conversion, il devient le groupe du projet.</li>
     <li>Si vous effectuez une conversion vers un projet à l’aide d’un modèle et qu’un groupe est présent sur le modèle, et que vous ne spécifiez pas de groupe pendant la conversion, le groupe du modèle devient le groupe du nouveau projet.</li>
      <li> S’il n’y a aucun groupe sur le modèle et que vous ne spécifiez pas de groupe pendant la conversion, le groupe du projet du problème d’origine devient le groupe du nouveau projet.</li> </ul>
      </td> 
  </tr> 
  <tr> 
   <td>Entreprise</td>    
   <td>  Est transféré à partir du modèle. Sinon, ce champ est vide.</td>

</tr> 
  <tr> 
   <td>Propriétaire du projet</td> 
   <td>Est transféré à partir du champ Propriétaire du modèle sur le modèle. Sinon, il est défini sur la personne connectée qui effectue la conversion. </td> 
  </tr> 
  <tr> 
   <td>Sponsor du projet</td> 
   <td>Est transféré à partir du champ Modèle de sponsor sur le modèle. Sinon, ce champ est vide.</td> 
  </tr> 
  <tr> 
   <td>Gestionnaire des ressources</td> 
   <td>Est transféré à partir du modèle. Sinon, ce champ est vide.</td> 
  </tr> 
  <tr> 
   <td>Paramètres de la tâche</td> 
   <td>Est transféré à partir du modèle.</td> 
  </tr> 
  <tr> 
   <td>Paramètres de l'événement</td> 
   <td>Est transféré à partir du modèle. </td> 
  </tr> 
  <tr> 
   <td>Accès</td> 
   <td> <p>Est transféré depuis la section Accès du modèle. </p> </td> 
  </tr> 
  <tr> 
   <td>Approbations</td> 
   <td>Est transféré à partir du modèle. Les approbations associées au problème sont supprimées lors de la conversion. </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p>  </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p>  </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## Consulter les informations du problème d’origine sur les projets et les tâches {#view-original-issue-information-on-projects-and-tasks}

Vous pouvez consulter les informations du problème d’origine dans les listes et les rapports de projets et de tâches ou dans la zone Détails du projet. Pour plus d’informations sur la création de rapports, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Le tableau suivant illustre les champs du problème visibles à partir des projets et des tâches convertis.

| Champs du problème | Champ du projet ou de la tâche | Liste ou rapport de projet | Zone Détails du projet | Liste ou rapport de tâche | Zone Détails de la tâche |
|---|---|---|---|---|---|
| Nom de l’événement | Nom du problème converti | ✔ | ✔ | ✔ | ✔ |
| Contact principal | Nom du créateur ou de la créatrice du problème converti | ✔ | `✔` | ✔ |  |
| Date d’entrée | Date d’entrée de l’événement converti | ✔ |  | ✔ |  |


>[!CAUTION]
>
>Si le contact principal d’un problème change ou si le problème n’est plus lié au projet ou à la tâche une fois le problème converti, le nom du créateur ou de la créatrice du problème converti n’est pas mis à jour et affiche le contact principal d’origine du problème au moment de la conversion.
