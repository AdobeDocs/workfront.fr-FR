---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '« Vue d’ensemble de la contrainte de tâche : Aussi Tard Que Possible »'
description: Aussi Tard Que Possible (ALAP) est une contrainte de tâche Adobe Workfront qui place la date d’achèvement de la tâche aussi près que possible de la fin du projet.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 100%

---

# Vue d’ensemble de la contrainte de tâche : Aussi Tard Que Possible

Aussi Tard Que Possible (ALAP) est une contrainte de tâche Adobe Workfront qui place la date d’achèvement de la tâche aussi près que possible de la fin du projet.

L’utilisation de cette contrainte peut entraîner la replanification des tâches dépendantes ou antérieures.

Pour plus d’informations sur l’utilisation des tâches antérieures, voir [Utiliser les tâches antérieures](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

Aussi Tard Que Possible est la contrainte par défaut si un projet utilise un mode de planification de la date d’achèvement et que la valeur par défaut de système ou de groupe de la date de début d’une tâche est En fonction de la date prévue de projet.

Pour plus d’informations sur l’emplacement où définir la contrainte par défaut pour une nouvelle tâche, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Pour plus d’informations sur la mise à jour d’une contrainte de tâche, voir [Mettre à jour une contrainte de tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## Différence entre Dernière Heure Disponible et Aussi Tard Que Possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

La contrainte Dernière Heure Disponible est différente de la contrainte Aussi Tard Que Possible lorsque les critères suivants s’appliquent :

* Le projet est planifié à partir de la date de début.
* Les tâches du projet ont une relation antérieure.
* La tâche utlérieure présente une contrainte de tâche flexible.

Dans ce cas :

* **Dernière Heure Disponible :** l’utilisation de la contrainte Dernière Heure Disponible sur la tâche antérieure donne la priorité à la contrainte flexible de la tâche ultérieure.

  **Exemple :** par exemple, la tâche A est antérieure à la tâche B. La tâche A a la contrainte Dernière Heure Disponible et la tâche B la contrainte Aussi Tôt Que Possible. Dans ce cas, la tâche A est planifiée aussi près que possible du début du projet.

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **Aussi Tard Que Possible :** dans ce scénario, l’utilisation de la contrainte Aussi Tard Que Possible sur la tâche antérieure donne la priorité à la tâche antérieure.

  **Exemple :** par exemple, la tâche A est antérieure à la tâche B. La tâche A a la contrainte Aussi Tard Que Possible et la tâche B la contrainte Aussi Tôt Que Possible. Dans ce cas, la tâche A est planifiée aussi près que possible de la fin du projet.

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->
