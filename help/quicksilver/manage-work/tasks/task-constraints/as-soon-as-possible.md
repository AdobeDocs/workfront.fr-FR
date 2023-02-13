---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Présentation de la contrainte de tâche : Dès Que Possible'''
description: Dès que possible, une contrainte de tâche place l’heure de début de la tâche aussi près que possible du début du projet.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Présentation de la contrainte de tâche : Dès Que Possible

Dès que possible, une contrainte de tâche place l’heure de début de la tâche aussi près que possible du début du projet.

## Observations relatives à l’utilisation de la contrainte Dès que possible

* Dès que possible, la contrainte par défaut est définie si un projet utilise un mode de planification de la planification à partir de la date de début et si la date de début par défaut du système pour une nouvelle tâche est définie sur Basé sur la date planifiée du projet.

* Si un projet utilise un mode de planification de Planification à partir de la date de début et si la date de début par défaut du système ou du groupe d’une nouvelle tâche est définie sur Aujourd’hui, alors la contrainte de tâche par défaut est Début au plus tôt.

   Pour plus d’informations sur l’emplacement où définir la contrainte par défaut pour une nouvelle tâche, reportez-vous à la section [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche sur une tâche, voir [Mettre à jour la contrainte de tâche d’une tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Différence entre le plus tôt temps disponible et le plus tôt possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

La contrainte Heure disponible la plus ancienne diffère de la contrainte Dès que possible lorsque tous les critères suivants existent :

* Le projet est planifié à partir de la fin.
* Les tâches du projet ont une relation de prédécesseur.
* La tâche du prédécesseur présente une contrainte de tâche flexible.

Dans ce cas :

* **Heure disponible la plus récente :** L’utilisation de la contrainte de la première heure disponible sur la tâche qui lui succède donne la priorité à la contrainte flexible du prédécesseur.

   Supposons, par exemple, que la tâche A soit un prédécesseur de la tâche B. La tâche B a la contrainte Temps disponible la plus ancienne et la tâche A la contrainte Aussi tardive que possible. Dans ce cas, la tâche est planifiée aussi près que possible de la fin du projet.

* **Dès Que Possible :** Dans ce scénario, l’utilisation de la contrainte Dès que possible sur la tâche qui lui succède donne la priorité à la tâche qui lui succède.

   Supposons, par exemple, que la tâche A soit un prédécesseur de la tâche B. La tâche B a la contrainte Dès que possible et la tâche A la contrainte Aussi tardive que possible. Dans ce cas, la tâche est planifiée aussi près que possible du début du projet.
