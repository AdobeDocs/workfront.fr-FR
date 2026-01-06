---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D''Ensemble Des Contraintes De Tâche : Dès Que Possible'
description: Aussi tôt que possible est une contrainte de tâche qui place l’heure de début de la tâche aussi près que possible du début du projet.
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 98%

---

# Vue d’ensemble des contraintes de tâche : Aussi tôt que possible

Aussi tôt que possible est une contrainte de tâche qui place l’heure de début de la tâche aussi près que possible du début du projet.

## Remarques relatives à l’utilisation de la contrainte Aussi tôt que possible

* Aussi tôt que possible est la contrainte par défaut si un projet utilise un mode de planification à partir de la date de début et si la date de début par défaut du système pour une nouvelle tâche est définie sur Basée sur la date prévue du projet.

* Si un projet utilise un mode de planification à partir de la date de début et si la date de début par défaut du système ou du groupe pour une nouvelle tâche est définie sur Aujourd’hui, alors la contrainte de tâche par défaut est Commencer au plus tôt.

  Pour plus d’informations sur l’emplacement où définir la contrainte par défaut pour une nouvelle tâche, consultez la section [Configurer des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche, voir [Mettre à jour la contrainte de tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## Différence entre Première heure disponible et Aussi tôt que possible

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"]) </p>
-->

La contrainte Première heure disponible diffère de la contrainte Aussi tôt que possible lorsque tous les critères suivants sont remplis :

* Le projet est planifié à partir de la fin.
* Les tâches du projet ont une relation de tâche antérieure.
* La tâche antérieure a une contrainte de tâche flexible.

Dans ce cas :

* **Première heure disponible :** l’utilisation de la contrainte Première heure disponible sur la tâche ultérieure donne la priorité à la contrainte flexible de la tâche antérieure.

  Supposons, par exemple, que la tâche A soit antérieure à la tâche B. La tâche B a la contrainte Première heure disponible et la tâche A la contrainte Aussi tard que possible. Dans ce cas, la tâche est planifiée aussi près que possible de l’achèvement du projet.

* **Aussi tôt que possible :** dans ce scénario, l’utilisation de la contrainte Aussi tôt que possible sur la tâche ultérieure lui donne la priorité.

  Supposons, par exemple, que la tâche A soit antérieure à la tâche B. La tâche B a la contrainte Aussi tôt que possible et la tâche A la contrainte Aussi tard que possible. Dans ce cas, la tâche est planifiée aussi près que possible du début du projet.
