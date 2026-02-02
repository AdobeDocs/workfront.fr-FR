---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D''Ensemble Des Contraintes De Tâche : Dernière Heure Disponible'
description: La Dernière Heure Disponible (LAT) est un type de contrainte de tâche dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 93%

---

# Vue d’ensemble de la contrainte de tâche : Dernière Heure Disponible

La Dernière Heure Disponible (LAT) est un type de contrainte de tâche dans Adobe Workfront.

## Utiliser la contrainte de tâche Dernière Heure Disponible

Vous pouvez utiliser la contrainte LAT lorsque vous souhaitez planifier le début d’une tâche à la dernière heure disponible après avoir pris en compte les relations antérieure et ultérieure dans le projet.

Cette contrainte diffère d’Aussi Tôt Que Possible du fait qu’elle ne force pas à changer la planification des tâches antérieures ou ultérieures. En effet, elle n’affecte que le planning de la tâche à laquelle elle est associée, en la définissant sur la dernière heure disponible en fonction de sa relation avec d’autres tâches.

Pour plus d’informations sur la mise à jour de la contrainte de tâche, voir [Mettre à jour la contrainte de tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE: replaced with new article linked above) </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## La différence entre Dernière Heure Disponible et Aussi Tard Que Possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

La contrainte Dernière Heure Disponible est différente de la contrainte Aussi Tard Que Possible lorsque les critères suivants s’appliquent :

* Le projet est planifié à partir de la date de début.
* Les tâches du projet ont une relation antérieure.
* La tâche utlérieure présente une contrainte de tâche flexible.

Dans ce cas :

* **Dernière Heure Disponible :** l’utilisation de la contrainte Dernière Heure Disponible sur la tâche antérieure donne la priorité à la contrainte flexible de la tâche ultérieure.

  **Exemple :** par exemple, la tâche A est antérieure à la tâche B. La tâche A a la contrainte Dernière Heure Disponible et la tâche B la contrainte Aussi Tôt Que Possible. Dans ce cas, la tâche A est planifiée aussi près que possible du début du projet.

  ![Dernière contrainte de tâche de temps disponible dans la liste des tâches](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **Aussi Tard Que Possible :** dans ce scénario, l’utilisation de la contrainte Aussi Tard Que Possible sur la tâche antérieure donne la priorité à la tâche antérieure.

  **Exemple :** par exemple, la tâche A est antérieure à la tâche B. La tâche A a la contrainte Aussi Tard Que Possible et la tâche B la contrainte Aussi Tôt Que Possible. Dans ce cas, la tâche A est planifiée aussi près que possible de la fin du projet.

  ![Contrainte de tâche aussi tardive que possible dans la liste des tâches](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
