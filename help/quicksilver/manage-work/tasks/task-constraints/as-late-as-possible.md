---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Présentation de la contrainte de tâche : aussi tard que possible"
description: Dans la mesure du possible (ALAP), une contrainte de tâche Adobe Workfront est définie. Elle place le temps d’achèvement de la tâche aussi près que possible de la fin du projet.
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Présentation de la contrainte de tâche : aussi tard que possible

Dans la mesure du possible (ALAP), une contrainte de tâche Adobe Workfront est définie. Elle place le temps d’achèvement de la tâche aussi près que possible de la fin du projet.

L’utilisation de cette contrainte peut entraîner la replanification des tâches dépendantes ou précédentes.

Pour plus d’informations sur les relations de prédécesseur, voir [Utilisation des prédécesseurs de tâche](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md).

La contrainte par défaut est aussi tardive que possible si un projet utilise un mode de planification de la date de fin et que la valeur par défaut système ou groupe de la date de début d’une tâche est Basée sur la date planifiée du projet.

Pour plus d’informations sur l’emplacement où définir la contrainte par défaut pour une nouvelle tâche, reportez-vous à la section [Configuration de la tâche à l’échelle du système et préférences de publication](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche sur une tâche, voir [Mise à jour de la contrainte de tâche d’une tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## Différence entre la dernière heure disponible et aussi tardive que possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

La dernière contrainte Heure disponible diffère de la contrainte Dès que possible lorsqu’il existe les critères suivants :

* Le projet est planifié à partir de la date de début
* Les tâches du projet ont une relation de prédécesseur
* La tâche qui lui succède présente une contrainte de tâche flexible.

Dans ce cas :

* **Dernière heure disponible :** L’utilisation de la dernière contrainte de temps disponible sur la tâche du prédécesseur donne la priorité à la contrainte flexible du successeur.

  **Exemple :** Par exemple, la tâche A est un prédécesseur de la tâche B. La tâche A a la contrainte de temps disponible la plus récente et la tâche B a la contrainte de temps aussi tôt que possible. Dans ce cas, la tâche A est planifiée aussi près que possible du début du projet.

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **Aussi tard que possible :** Dans ce scénario, l’utilisation de la contrainte Aussi tard que possible sur la tâche du prédécesseur donne la priorité à la tâche du prédécesseur.

  **Exemple :** Par exemple, la tâche A est un prédécesseur de la tâche B. La tâche A a la contrainte Aussi tardive que possible et la tâche B la contrainte Dès que possible. Dans ce cas, la tâche A est planifiée aussi près que possible de la fin du projet.

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
