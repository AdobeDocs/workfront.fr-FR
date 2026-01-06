---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D''Ensemble De La Contrainte De Tâche : Doit Commencer Le'
description: Utilisez la contrainte de tâche Il faut commencer le (MSO) pour planifier une tâche de manière à ce qu’elle commence exactement à une date spécifique.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 98%

---

# Vue d’ensemble des contraintes de tâches : Il faut commencer le

Utilisez la contrainte de tâche Il faut commencer le (MSO) pour planifier une tâche de manière à ce qu’elle commence exactement à une date spécifique.

La contrainte Il faut commencer le planifie une tâche pour qu’elle commence exactement à l’heure et à la date que vous spécifiez dans le champ **Date de début prévue**.

>[!TIP]
>
>La mise à jour manuelle de la date de début prévue d’une tâche modifie la contrainte de la tâche, qui devient Il faut commencer le.

## Vue d’ensemble de la contrainte Il faut commencer le

Tenez compte des éléments suivants lors de la planification d’une tâche avec une contrainte Il faut commencer le :

* Les relations antérieures n’obligent pas cette tâche à être reprogrammée. Workfront ignore essentiellement toutes les relations antérieures de la tâche avec cette contrainte.
* La tâche affiche **À risque** si les relations antérieures commencent à traîner ou à être en retard.

* Lorsque vous déplacez ou copiez une tâche avec une contrainte MSO (Il faut commencer le) vers un autre projet, la contrainte de tâche ou les dates du projet peuvent changer en fonction des dates de la contrainte et des dates de début et de fin du projet. Les scénarios suivants sont possibles :

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
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
