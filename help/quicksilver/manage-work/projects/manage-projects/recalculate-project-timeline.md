---
product-area: projects
navigation-topic: manage-projects
title: Recalculer les délais d’un projet
description: Recalculer les chronologies permet aux gestionnaires de déterminer l’impact de différents facteurs liés au projet sur la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévues.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 9%

---

# Recalculer les délais d’un projet

Recalculer les chronologies permet aux gestionnaires de déterminer l’impact de différents facteurs liés au projet sur la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévues.

Les modifications apportées aux plannings, aux congés du personnel et à d’autres éléments en dehors de la portée d’un projet n’ont pas d’incidence immédiate sur la chronologie du projet. La chronologie du projet est affectée lorsque la chronologie est recalculée. Les influences externes ne prennent effet sur votre projet que lorsque le nouveau calcul est effectué.

Cet article décrit comment le recalcul de la chronologie se produit.

## Conditions d’accès

<!--drafted for P&P: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Le recalcul automatique de la chronologie se produit sans accès spécial pour les utilisateurs impliqués dans le projet.

Cependant, vous devez disposer des droits d’accès suivants pour recalculer manuellement la chronologie d’un projet :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p>Administrateur système pour recalculer la chronologie de tous les projets du système</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion d’un projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## recalcul automatique

Par défaut, les chronologies de projet sont automatiquement recalculées tous les jours lorsque la portée du projet change ou toutes les nuits. L’administrateur de Workfront détermine s’il faut calculer automatiquement les chronologies toutes les nuits ou à chaque changement de portée en gérant les paramètres Chronologies dans la zone Préférences du projet de la configuration. Pour plus d’informations, voir [Configuration des recalculations de la chronologie pour les projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>Si le délai d’un projet dépasse 15 ans, le recalcul automatique est désactivé pour ce projet. Vous pouvez uniquement sélectionner un type de mise à jour du manuel pour un projet de plus de 15 ans. Si vous définissez les dates du projet sur moins de 15 ans, vous devez recalculer manuellement votre chronologie une fois avant qu’elle ne soit calculée automatiquement.

* [Nouveau calcul automatique des chronologies de projet](#automatic-recalculation-of-project-timelines)
* [Actions qui déclenchent un nouveau calcul automatique des chronologies de projet](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### recalcul automatique des calendriers du projet {#automatic-recalculation-of-project-timelines}

Adobe Workfront recalcule les chronologies tous les jours uniquement pour les projets pour lesquels toutes les conditions suivantes sont remplies :

* avoir un état actuel ;
* Le type de mise à jour du projet est défini sur Automatique ou Automatique et Après modification

  Pour plus d’informations sur le type de mise à jour de projet, voir [Présentation du type de mise à jour de projet](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* avoir une date de dernière mise à jour au cours des trois derniers mois ;\
  L’administrateur de Workfront peut modifier cette fonctionnalité par défaut, comme décrit dans la section [Configuration des recalculs de la chronologie pour les projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* La date du dernier calcul de la chronologie du projet ne figure pas dans la journée civile en cours. Cela signifie que la date du dernier calcul de la chronologie du projet est antérieure à 00:00 du jour en cours.

Vous pouvez configurer la fréquence de mise à jour de la chronologie de votre projet. Lorsque la chronologie du projet est mise à jour, elle est recalculée en fonction des modifications apportées au projet.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Pour plus d’informations, voir [Sélectionner le type de mise à jour de projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### Actions qui déclenchent un nouveau calcul automatique des chronologies de projet {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Diverses modifications de portée dans la durée d’un projet recalculent automatiquement la chronologie du projet, notamment les actions suivantes :

* Mise à jour de l’état de la tâche.
* Déplacement d’une tâche vers un autre projet.
* Mise à jour de la date planifiée ou de la date de fin planifiée des tâches.
* Mise à jour du type de durée, de la contrainte de tâche ou du nombre de personnes désignées pour les tâches.
* Mise à jour des relations de prédécesseur de tâche.
* Ajouter une validation à une tâche qui ajoute également du temps à la Date d’achèvement planifiée de la tâche.\
  Pour plus d’informations sur les paramètres d’approbation, voir [Configuration des paramètres d’approbation globaux](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## recalcul manuel {#manual-recalculation}

En tant que propriétaire de projet, vous pouvez recalculer manuellement les chronologies pour les projets individuels. L’administrateur Workfront peut manuellement recalculer toutes les chronologies dans Workfront.

* [Recalculer les chronologies pour des projets individuels ou en bloc](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [recalculer manuellement les chronologies en bloc dans la zone Modifier les projets](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Recalculer les chronologies pour tous les projets du système (administrateurs Workfront uniquement)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Recalculer les chronologies pour des projets individuels ou en bloc {#recalculate-timelines-for-individual-projects-or-in-bulk}

Vous pouvez recalculer la chronologie d’un projet dans Workfront à partir de la page du projet ou d’une liste de projets ou d’un rapport.

1. Accédez au projet pour lequel vous souhaitez recalculer la chronologie et cliquez sur l’icône **Plus** ![](assets/qs-more-menu.png) située à gauche du nom du projet.

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Accédez à une liste de projets ou à un rapport et sélectionnez un ou plusieurs projets, puis cliquez sur l’icône **Plus** ![](assets/qs-more-menu.png) en haut de la liste.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lorsque vous recalculez en bloc leur calendrier afin d’assurer des performances optimales. Certaines choses qui peuvent rendre un projet trop complexe peuvent être des dépendances ou des affectations multiples ou un grand nombre de champs personnalisés.

1. Cliquez sur **Recalculer la chronologie**.

   Une fois la frise chronologique recalculée, un message s’affiche indiquant que le recalcul a réussi.

   >[!TIP]
   >
   >Avant que le recalcul de la chronologie ne soit terminé, certaines dates prévues ou prévues peuvent s’afficher en grisé. Cela signifie que le recalcul n&#39;est pas encore terminé et que les dates peuvent être modifiées.

### recalculer manuellement les chronologies en bloc dans la zone Modifier les projets {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Vous pouvez recalculer manuellement les chronologies de plusieurs projets en les modifiant en bloc.

>[!TIP]
>
>En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lors de leur modification en bloc afin d’assurer des performances optimales. Certaines choses qui peuvent rendre un projet trop complexe peuvent être des dépendances ou des affectations multiples ou un grand nombre de champs personnalisés.

1. Accédez à une liste de projets.
1. Sélectionnez plusieurs projets dans la liste, puis cliquez sur **Modifier**.
1. Cliquez sur **Paramètres**, puis sélectionnez **Recalculer les chronologies**.

1. Cliquez sur **Enregistrer les modifications**.

### Recalculer les chronologies pour tous les projets du système (administrateurs Workfront uniquement) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Les administrateurs de Workfront peuvent exécuter le diagnostic Recalculate Timeline pour recalculer immédiatement toutes les chronologies du système Workfront. Cela permet à tous les chefs de projet de voir immédiatement l’influence des modifications externes sur les dates prévues et prévues.

Pour plus d’informations sur le nouveau calcul des chronologies pour l’ensemble du site Workfront, consultez la section &quot;Recalculer les chronologies pour l’ensemble de l’instance Workfront&quot; dans [Configuration des recalculations de la chronologie pour les projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
