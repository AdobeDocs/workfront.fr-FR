---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D''Ensemble De La Contrainte De Tâche : Doit Se Terminer Le'
description: Vous pouvez utiliser la contrainte de tâche Il Faut Finir Le (MFO) pour planifier la fin d’une tâche à une date spécifique.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 98%

---

# Vue d’ensemble de la contrainte de tâche : Il Faut Finir Le

Vous pouvez utiliser la contrainte de tâche Il Faut Finir Le (MFO) pour planifier la fin d’une tâche à une date spécifique.

La contrainte Il Faut Finir Le planifie un tâche pour qu’elle se termine exactement à l’heure et à la date spécifiées dans le champ **Date d’achèvement prévue**.

>[!TIP]
>
>La mise à jour manuelle de la Date d’achèvement prévue d’une tâche modifie la contrainte de la tâche en lui donnant le statut Il Faut Finir Le.

## Vue d’ensemble de la contrainte de tâche Il Faut Finir Le

Tenez compte de ce qui suit lors de la planification d’une tâche avec une contrainte Il Faut Finir Le :

* Les relations de tâche antérieure ne forcent pas la replanification de la tâche. Adobe Workfront ignore pour l’essentiel les relations avec la tâche antérieure.
* La tâche s’affiche comme **En danger** si les tâches antérieures commencent à prendre du retard ou sont en retard.

* Lorsque vous déplacez ou copiez une tâche avec une contrainte MFO vers un autre projet, la contrainte de tâche ou les dates du projet peuvent changer en fonction des dates de contrainte et des dates de début et de fin du projet. Les scénarios suivants sont possibles :

   * Lorsque le projet de destination est planifié à partir du début :

      * Lorsque la date de contrainte de la tâche est antérieure à la date de début prévue du projet, la contrainte de tâche passe à Aussi Tôt Que Possible.
      * Lorsque la date de contrainte de la tâche est postérieure à la date d’achèvement prévue du projet, la date d’achèvement prévue du projet est modifiée pour correspondre à la date de contrainte d’achèvement de la tâche.

      * Lorsque le projet de destination est planifié à partir de l’achèvement :

         * Lorsque la date de contrainte de la tâche est postérieure à la date d’achèvement du projet, la contrainte de la tâche passe à Aussi Tard Que Possible.
         * Lorsque la date de contrainte de la tâche est antérieure à la date de début prévue du projet, la date de début prévue du projet change pour correspondre à la date de contrainte de début de la tâche.

      * Quel que soit le planning du projet, lorsque la date de contrainte de la tâche se trouve entre les dates de début et d’achèvement du projet, aucune modification n’est apportée à la contrainte de tâche ou aux dates du projet.

  Pour plus d’informations sur le déplacement de tâches, voir [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md). Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche, voir [Mettre à jour la contrainte de tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
