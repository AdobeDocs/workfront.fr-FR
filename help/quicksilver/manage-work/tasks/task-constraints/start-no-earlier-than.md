---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D’Ensemble De La Contrainte De Tâche : Commencer Au Plus Tôt'
description: Utilisez la contrainte de tâche Commencer Au Plus Tôt (SNET) pour planifier le démarrage d’une tâche après la date que vous avez spécifiée.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 98%

---

# Vue d’ensemble de la contrainte de tâche : Commencer Au Plus Tôt

Utilisez la contrainte de tâche Commencer Au Plus Tôt (SNET) pour planifier le démarrage d’une tâche après la date que vous avez spécifiée.

## Vue d’ensemble de la contrainte de tâche Commencer Au Plus Tôt

Prenez en compte les points suivants lorsque vous utilisez la contrainte Commencer Au Plus Tôt :

* Vous devez utiliser la contrainte Commencer Au Plus Tôt lorsque le projet est planifié à partir de la date de début. Dans ce cas, vous pouvez imposer une contrainte souple sur une tâche avant qu’elle ne force d’autres tâches dépendantes à s’afficher comme À risque.
* La contrainte Commencer Au Plus Tôt est celle par défaut si un projet est planifié à partir de la date de début et si la date de début par défaut du système ou du groupe d’une nouvelle tâche est définie sur Aujourd’hui. Pour plus d’informations sur la configuration des paramètres par défaut des tâches, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Si vous planifiez le projet à partir de la date de début et que la date de début par défaut du système d’une nouvelle tâche est définie sur Basé sur la date prévue du projet, la contrainte par défaut d’une nouvelle tâche est Aussi Tôt Que Possible.
* Si vous planifiez le projet à partir de la date d’achèvement et que la date de début par défaut du système d’une nouvelle tâche est définie sur Aujourd’hui, la contrainte Commencer Au Plus Tôt planifie la tâche, de la même manière qu’une tâche Aussi Tard Que Possible.
* Lorsque vous déplacez ou copiez une tâche avec une contrainte SNET vers un autre projet, la contrainte de la tâche ou des dates du projet peut changer en fonction des dates de contrainte et des dates de début et d’achèvement du projet. Les scénarios suivants sont possibles :

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
