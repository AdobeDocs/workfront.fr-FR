---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D''Ensemble Des Contraintes De Tâche : Aussi Tard Que Possible'
description: Aussi Tard Que Possible (ALAP) est une contrainte de tâche Adobe Workfront qui place la date d’achèvement de la tâche aussi près que possible de la fin du projet.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 77%

---

# Vue d’ensemble des contraintes de tâches : Aussi tard que possible

Aussi Tard Que Possible (ALAP) est une contrainte de tâche Adobe Workfront qui place la date d’achèvement de la tâche aussi près que possible de la fin du projet.

L&#39;utilisation de cette contrainte peut entraîner la replanification de tâches antérieures ou dépendantes.

Pour plus d&#39;informations sur les relations des prédécesseurs, voir [Utiliser les prédécesseurs de tâche : index d&#39;article](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

Le plus tard possible est la contrainte par défaut si un projet utilise le mode de planification Planifier à partir de la date de fin et si les valeurs système ou de groupe par défaut pour la date de début d&#39;une tâche sont basées sur la date prévue du projet.

Pour plus d’informations sur l’emplacement où définir la contrainte par défaut pour une nouvelle tâche, consultez la section [Configurer des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche, voir [Mettre à jour la contrainte de tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## La différence entre Dernière Heure Disponible et Aussi Tard Que Possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

La contrainte Dernière Heure Disponible est différente de la contrainte Aussi Tard Que Possible lorsque les critères suivants s’appliquent :

* Le projet est planifié à partir de la date de début.
* Les tâches du projet ont une relation antérieure.
* La tâche utlérieure présente une contrainte de tâche flexible.

Dans ce cas :

* **Dernière Heure Disponible :** l’utilisation de la contrainte Dernière Heure Disponible sur la tâche antérieure donne la priorité à la contrainte flexible de la tâche ultérieure.

  **Exemple :** par exemple, la tâche A est antérieure à la tâche B. La tâche A a la contrainte Dernière Heure Disponible et la tâche B la contrainte Aussi Tôt Que Possible. Dans ce cas, la tâche A est planifiée aussi près que possible du début du projet.

  ![Dernière contrainte de tâche de temps disponible](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **Aussi Tard Que Possible :** dans ce scénario, l’utilisation de la contrainte Aussi Tard Que Possible sur la tâche antérieure donne la priorité à la tâche antérieure.

  **Exemple :** par exemple, la tâche A est antérieure à la tâche B. La tâche A a la contrainte Aussi Tard Que Possible et la tâche B la contrainte Aussi Tôt Que Possible. Dans ce cas, la tâche A est planifiée aussi près que possible de la fin du projet.

  ![Contrainte de tâche aussi tardive que possible dans une liste de tâches](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)



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
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
