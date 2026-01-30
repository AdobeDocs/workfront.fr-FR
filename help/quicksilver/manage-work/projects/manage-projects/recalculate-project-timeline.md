---
product-area: projects
navigation-topic: manage-projects
title: Recalculer les chronologies de projet
description: Recalculer les chronologies permet aux personnes chargées de la gestion de déterminer l’impact de différents facteurs liés au projet sur la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévisionnelles.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 58%

---

# Recalculer les chronologies des projets

<!--Audited: 06/2025-->

Recalculer les chronologies permet aux personnes chargées de la gestion de déterminer l’impact de différents facteurs liés au projet sur la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévisionnelles.

Les modifications apportées aux plannings, aux congés du personnel et à d’autres éléments en dehors de la portée d’un projet n’ont pas d’incidence immédiate sur la chronologie du projet. La chronologie du projet est affectée lorsque la chronologie est recalculée. Les influences externes ne prennent effet sur votre projet que lorsque le nouveau calcul est effectué.

Cet article décrit comment le recalcul de la chronologie se produit.

Le recalcul automatique de la chronologie se produit sans accès spécial pour les utilisateurs impliqués dans le projet. En outre, vous pouvez recalculer manuellement la chronologie.

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
   <td> <p>Standard</p> 
    <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> <p>Administrateur ou administratrice système pour recalculer la chronologie de tous les projets du système.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion d’un projet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Standard </p> 
    <p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Recalcul automatique

Par défaut, les chronologies des projets sont automatiquement recalculées tous les jours lorsque la portée des projets change ou toutes les nuits. L’administrateur Workfront détermine s’il faut calculer automatiquement les chronologies toutes les nuits ou avec chaque modification de la portée en gérant les paramètres des chronologies dans les Préférences du projet de la Configuration. Pour plus d’informations, voir [Configurer les nouveaux calculs de chronologie pour les projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!IMPORTANT]
>
>* Si la chronologie d&#39;un projet dépasse 15 ans, le recalcul automatique est désactivé pour ce projet et vous ne pouvez sélectionner qu&#39;un type de mise à jour manuelle. Si vous définissez les dates du projet sur moins de 15 ans, vous devez recalculer manuellement votre chronologie une fois avant qu’elle ne soit calculée automatiquement.
>* Pour les environnements Sandbox de prévisualisation et d’actualisation personnalisée, le recalcul nocturne est désactivé et les chronologies du projet ne sont pas recalculées automatiquement. Vous devez recalculer manuellement la chronologie du projet pour les environnements de prévisualisation et de sandbox d’actualisation personnalisée.
>* Si un projet est complexe, le recalcul automatique de la chronologie peut ne pas se produire.
> Un exemple de projet complexe peut être un projet avec plusieurs dépendances, un grand nombre de tâches, plusieurs prédécesseurs interprojets ou plusieurs indentations de tâches.
> Workfront place un avertissement à droite du nom du projet sur la page du projet pour informer les utilisateurs que la chronologie du projet doit être recalculée manuellement. Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour le projet peuvent recalculer manuellement la chronologie.
>
>   ![Avertissement de projet pour recalculer la chronologie](assets/project-warning-to-manually-recalculate-timeline.png)
>

* [Recalcul automatique des chronologies des projets](#automatic-recalculation-of-project-timelines)
* [Actions qui déclenchent un recalcul automatique des chronologies des projets.](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)



### Recalcul automatique des chronologies des projets {#automatic-recalculation-of-project-timelines}

Workfront recalcule les chronologies quotidiennement uniquement pour les projets où toutes les conditions suivantes sont remplies :

* Ont un statut Actuel.
* Le type de mise à jour du projet est défini sur Automatique ou Automatique et En cas de modification.

  Pour plus d’informations, voir [Présentation du type de mise à jour de projet](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Disposer d’une date de dernière mise à jour au cours des 3 derniers mois. Un administrateur Workfront peut modifier cette fonctionnalité par défaut. Pour plus d’informations, voir [Configurer les nouveaux calculs de chronologie pour les projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* La dernière date de calcul de la chronologie du projet ne se situe pas dans la journée calendaire en cours. Cela signifie que la dernière date de calcul de la chronologie du projet est antérieure à 00:00 du jour en cours.

Vous pouvez configurer la fréquence de mise à jour de la chronologie de votre projet. Lorsque la chronologie du projet est mise à jour, elle est recalculée en fonction des modifications apportées au projet.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Pour plus d’informations, voir [Sélectionner le type de mise à jour du projet.](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click  <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
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

### Actions qui déclenchent un recalcul automatique des chronologies des projets. {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Diverses modifications de portée dans la durée d’un projet recalculent automatiquement la chronologie du projet, notamment les actions suivantes :

* Mettre à jour le statut de la tâche.
* Déplacer une tâche vers un autre projet.
* Mettre à jour la date prévue ou de la date d’achèvement prévue des tâches.
* Mettre à jour le type de durée, la contrainte de tâche ou le nombre de personnes cessionnaires pour les tâches.
* Mettre à jour les relations antérieures de la tâche.
* Ajouter une approbation à une tâche, entraînant l’ajout d’heures à la date d’achèvement prévue de la tâche.\
  Pour plus d’informations sur les paramètres d’approbation, consultez la section [Configurer des paramètres d’approbation globaux](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Recalcul manuel {#manual-recalculation}

En tant que personne propriétaire de projet, vous pouvez recalculer manuellement les chronologies de projets individuels. L’administration Workfront peut recalculer manuellement toutes les chronologies dans Workfront.

* [Recalculer les chronologies pour des projets individuels ou en bloc](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Recalculer manuellement les chronologies en bloc dans la zone Modifier les projets](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Recalculer les chronologies pour tous les projets du système (réservé à l’administration Workfront)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Recalculer les chronologies pour des projets individuels ou en bloc {#recalculate-timelines-for-individual-projects-or-in-bulk}

Vous pouvez recalculer la chronologie d’un projet dans Workfront à partir de la page du projet ou d’une liste de projets ou d’un rapport.

1. Accédez au projet pour lequel vous souhaitez recalculer la chronologie et cliquez sur l’icône **Plus** ![Menu Plus](assets/qs-more-menu.png) à gauche du nom du projet.

   Ou

   Accédez à une liste ou à un rapport de projet et sélectionnez un ou plusieurs projets, puis cliquez sur l’icône **Plus** ![Menu Plus](assets/qs-more-menu.png) en haut de la liste.

   ![Recalculer la chronologie des expressions avec la liste déroulante finances](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lors du recalcul de leur chronologie en bloc pour assurer des performances optimales. La complexité d’un projet dépend de facteurs tels que le nombre de dépendances, d’affectations et de champs personnalisés.

1. Cliquez sur **Recalculer la chronologie**. La chronologie est recalculée et un message de réussite s’affiche à l’écran.

   >[!TIP]
   >
   >Avant que le recalcul de la chronologie ne soit terminé, certaines dates prévues ou estimées peuvent être grisées. Cela signifie que le recalcul n’est pas encore terminé et que les dates sont susceptibles d’être modifiées.

### Recalculer manuellement les chronologies en bloc dans la zone Modifier les projets {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Vous pouvez recalculer manuellement les chronologies de plusieurs projets en les modifiant en bloc.

>[!TIP]
>
>En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lors de leur modification en bloc afin d’assurer des performances optimales. La complexité d’un projet dépend de facteurs tels que le nombre de dépendances, d’affectations et de champs personnalisés.

1. Accédez à une liste de projets.
1. Sélectionnez plusieurs projets dans la liste, puis cliquez sur **Modifier**.
1. Cliquez sur **Paramètres**, puis sélectionnez **Recalculer les chronologies**.

1. Cliquez sur **Enregistrer les modifications**.

### Recalculer les chronologies pour tous les projets du système (réservé à l’administration Workfront) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

L’administration Workfront peut exécuter le diagnostic Recalculer les chronologies afin de recalculer immédiatement toutes les chronologies du système Workfront. Cela permet à toutes les personnes gestionnaires de projet de voir immédiatement l’influence des modifications externes sur les dates prévues et prévisionnelles.

Pour plus d’informations sur le recalcul des chronologies pour l’ensemble du site Workfront, consultez la section Recalculer les chronologies pour l’ensemble de l’instance Workfront dans [Configurer les recalculs des chronologies pour les projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

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
<li> <p><strong>Automatic and On Change:</strong> This is the default setting. The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.  <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong> The project timeline is updated only when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
