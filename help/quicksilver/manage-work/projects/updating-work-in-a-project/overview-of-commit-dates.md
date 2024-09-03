---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Vue d’ensemble de la date d’engagement
description: La date d’engagement est la date à laquelle une personne affectée à une tâche ou à un problème s’engage à le terminer. Cette valeur est différente de la date d’achèvement prévue, car il s’agit d’une estimation plus réaliste de la date d’achèvement fournie par la personne directement responsable du travail.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 070b0525f0cb2880d3c7daf88777ba48968ce759
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 97%

---

# Vue d’ensemble des dates d’engagement

<!--Audited: 07/2024-->

<!-- <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

La date d’engagement est la date à laquelle une personne affectée à une tâche ou à un problème s’engage à le terminer.

Cette valeur est différente de la date d’achèvement prévue d’une tâche ou d’un problème, car il s’agit d’une estimation plus réaliste de la date d’achèvement indiquée par la personne responsable du travail.

Pour plus d’informations sur la date d’achèvement prévue, consultez la section [Vue d’ensemble de la date d’achèvement prévu de la tâche](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Vue d’ensemble de la date d’engagement

Tenez compte des points suivants lorsque vous travaillez avec des dates d’engagement :

* Seules les tâches et les problèmes ont une date d’engagement.
* Les dates d’engagement ne sont pas définies automatiquement par Adobe Workfront.\
  Lorsque vous créez une tâche ou un problème, aucune date d’engagement n’est affectée à la tâche ou au problème.
* Si on vous affecte une tâche ou un problème, vous pouvez définir la date d’engagement en effectuant l’une des opérations suivantes :

   * Laissez Workfront définir la date d’engagement de sorte qu’elle corresponde à la date d’achèvement prévue existante de la tâche ou du problème en cliquant sur Travailler sur ce projet, Démarrer le problème ou Démarrer la tâche sur la tâche ou le problème. Pour plus d’informations sur le remplacement du bouton Travailler sur ce projet par un bouton Démarrer, voir [Remplacer le bouton Travailler sur ce projet par un bouton Démarrer](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Définissez manuellement vous-même la date d’engagement en fonction de quand vous pensez terminer la tâche ou le problème. En tant que personne cessionnaire, il s’agit de votre estimation et de votre engagement envers la personne chargée de la gestion du projet de terminer la tâche ou le problème à une date spécifique. Pour plus d’informations, consultez la section [Mettre à jour les dates d’engagement pour les tâches et les problèmes](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

>[!NOTE]
>
>Pour modifier la date d’engagement, vous devez être la personne propriétaire de la tâche. Les utilisateurs et utilisatrices suivants ne peuvent pas modifier la date d’engagement d’une tâche :
>
>* Propriétaire du projet
>* Sponsor du projet
>* Gestionnaire des ressources
>* Administrateur ou administratrice système
>* Toute autre personne cessionnaire pour la tâche.
>* Toute autre personne disposant d’autorisations sur la tâche
>
>Pour plus d’informations sur la personne propriétaire de la tâche, consultez la section [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Localiser la date d’engagement des tâches et des problèmes

Vous pouvez retrouver la date d’engagement des tâches et des problèmes dans les zones suivantes de Workfront :

* La page de détails
* Panneau Résumé, une fois qu’un administrateur ou une administratrice Workfront ou de groupes l’a ajouté à votre modèle de mise en page. Pour plus d’informations, voir [Personnaliser l’accueil et le résumé à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* L’en-tête d’une tâche ou d’un problème, après qu’un administrateur de Workfront ou de groupe l’ait ajoutée à votre modèle de mise en page. Pour plus d’informations, voir [Personnaliser les en-têtes d’objets à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Notifications et mises à jour déclenchées en modifiant la date d’engagement {#notifications-and-updates-triggered-by-changing-the-commit-date}

Lorsqu’une personne cessionnaire d’une tâche ou d’un problème sélectionne une date d’engagement différente de la date d’achèvement prévue définie par la personne propriétaire du projet, un certain nombre de notifications et de mises à jour alertent la personne propriétaire du projet et d’autres utilisateurs et utilisatrices de cette modification.

>[!NOTE]
>
>Les modifications apportées à la date d’engagement ne modifient pas automatiquement les dates prévues et inversement.

La définition manuelle de la date d’engagement d’une tâche ou d’un problème déclenche les modifications suivantes :

* La modification de la date d’engagement est renseignée dans la section Mises à jour, sous les onglets Activité système et Tous pour la tâche ou le problème.

  ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  La modification de la date d’engagement s’affiche dans la zone Mises à jour de la tâche ou du problème lorsque l’administrateur ou l’administratrice de Workfront active cette mise à jour dans la zone Flux de mises à jour de Configuration.Pour plus d’informations, voir [Mises à jour suivies par le système](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

  Si une personne propriétaire de projet ne souhaite pas accepter la modification, nous lui recommandons de faire part de ses commentaires à l’utilisateur ou à l’utilisatrice qui propose une nouvelle date dans l’onglet Commentaires de la section Mises à jour, afin de lui demander de redéfinir la date d’engagement sur la date initialement prévue, ou de sélectionner une nouvelle date.

  Si une personne propriétaire de projet accepte la modification, la date d’achèvement prévue peut être ajustée manuellement afin qu’elle corresponde à la date d’engagement proposée par la personne affectée à l’élément en modifiant la tâche ou le problème.

  Vous devez disposer d’un accès en gestion à la tâche ou au projet pour le modifier.

  >[!TIP]
  >
  >Vous pouvez demander à votre administrateur ou administratrice système ou de groupe d’ajouter le champ Date d’engagement à votre panneau Résumé ou à l’en-tête, afin de faciliter sa mise à jour.
  >
  >Pour plus d’informations, consultez les articles suivants :
  >
  >* [Vue d’ensemble du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [Personnaliser l’accueil et le résumé à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [Personnaliser les en-têtes d’objet avec un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* La date d’achèvement prévisionnelle de la tâche ou du problème est définie sur la même date, car la tâche a maintenant une indication plus précise du moment où elle sera probablement terminée.

  Pour plus d’informations sur la date d’achèvement prévisionnelle, voir [Vue d’ensemble de la date d’achèvement prévisionnelle pour les projets, tâches et problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* La personne propriétaire du projet est informée dans la zone Notifications que la date d’engagement d’une tâche ou d’un problème a été modifiée.

  ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >La notification indiquant que la date d’engagement a changé est envoyée à la personne propriétaire du projet uniquement lorsque l’administrateur ou l’administratrice de Workfront active l’affichage de la date d’engagement dans la zone Flux de mise à jour de Configuration. Pour plus d’informations, voir [Mises à jour suivies par le système](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Pour plus d’informations sur les fonctionnalités supplémentaires disponibles lors de la mise à jour d’un élément de travail, voir [Mettre à jour le travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Pour plus d’informations sur la mise à jour des dates d’engagement pour les tâches et les problèmes, voir [Mettre à jour les dates d’engagement pour les tâches et les problèmes](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
