---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Présentation De La Contrainte De Tâche : Commencer Au Plus Tard'
description: Commencer Au Plus Tard (SNLT) est une contrainte de tâche qui planifie le démarrage d’une tâche avant la date que vous spécifiez.
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 90%

---

# Vue d’ensemble de la contrainte de tâche : Commencer Au Plus Tard

Commencer Au Plus Tard (SNLT) est une contrainte de tâche qui planifie le démarrage d’une tâche avant la date que vous spécifiez.

Tenez compte des points suivants lorsque vous utilisez la contrainte SNLT :

* Utilisez la contrainte Commencer Au Plus Tard lorsque le projet est planifié à partir de la date d’achèvement. Dans ce cas, vous pouvez imposer une contrainte souple sur une tâche avant qu’elle ne force d’autres tâches dépendantes à s’afficher comme À risque.
* Débuter au plus tard est la contrainte par défaut si un projet utilise un mode de planification Planifier à partir de la date de fin et si la valeur par défaut du système ou du groupe pour la date de début d&#39;une tâche est Aujourd&#39;hui. Pour plus d’informations sur l’emplacement où définir la contrainte par défaut pour une nouvelle tâche, consultez la section [Configurer des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Lorsque vous utilisez la contrainte SNLT avec un projet dont la date de début est Planifier à partir de, Adobe Workfront planifie la tâche comme s’il s’agissait d’une tâche Aussi Tôt Que Possible.
* Lorsque vous déplacez ou copiez une tâche avec une contrainte SNLT vers un autre projet, la contrainte de la tâche ou les dates du projet peuvent changer en fonction des dates de contrainte et des dates de début et d’achèvement du projet. Les scénarios suivants sont possibles :

   * Lorsque le projet de destination est planifié à partir du début :

      * Lorsque la date de contrainte de la tâche est antérieure à la date de début prévue du projet, la contrainte de tâche passe à Aussi Tôt Que Possible.
      * Lorsque la date de contrainte de la tâche est postérieure à la date d’achèvement prévue du projet, la date d’achèvement prévue du projet est modifiée pour correspondre à la date de contrainte d’achèvement de la tâche.

      * Lorsque le projet de destination est planifié à partir de l’achèvement :

         * Lorsque la date de contrainte de la tâche est postérieure à la date d’achèvement du projet, la contrainte de la tâche passe à Aussi Tard Que Possible.
         * Lorsque la date de contrainte de la tâche est antérieure à la date de début prévue du projet, la date de début prévue du projet change pour correspondre à la date de contrainte de début de la tâche.

      * Quel que soit le planning du projet, lorsque la date de contrainte de la tâche se trouve entre les dates de début et d’achèvement du projet, aucune modification n’est apportée à la contrainte de tâche ou aux dates du projet.

  Pour plus d’informations sur le déplacement de tâches, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

  Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche, voir [Mettre à jour la contrainte de tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->
