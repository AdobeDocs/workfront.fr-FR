---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D’Ensemble De La Contrainte De Tâche : Ne Pas Terminer Avant'
description: Finir Au Plus Tôt (Finish No Earlier Than, FNET) est une contrainte de tâche qui planifie l’achèvement d’une tâche après la date que vous avez spécifiée.
author: Alina
feature: Work Management
exl-id: b1dbf5c9-34b6-4c25-b582-ce9454501e03
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 98%

---

# Vue d’ensemble de la contrainte de tâche : Finir Au Plus Tôt

Finir Au Plus Tôt (Finish No Earlier Than, FNET) est une contrainte de tâche qui planifie l’achèvement d’une tâche après la date que vous avez spécifiée.

## Vue d’ensemble de la contrainte de tâche Finir Au Plus Tôt

Tenez compte des éléments suivants lorsque vous utilisez la contrainte « Finir Au Plus Tôt » (FNET) pour une tâche :

* Utilisez cette contrainte lorsque le projet est planifié à partir de la date d’achèvement. Dans ce cas, vous pouvez imposer une contrainte souple à la tâche avant de forcer d’autres tâches dépendantes à afficher « À risque ».
* Si vous utilisez FNET sur un projet planifié **À partir de la date de début**, la contrainte planifie la tâche comme si elle était définie comme Aussi Tôt Que Possible.
* Lorsque vous déplacez ou copiez une tâche avec une contrainte FNET vers un autre projet, la contrainte de la tâche ou les dates du projet peuvent changer en fonction des dates de la contrainte ainsi que des dates de début et de fin du projet. Les scénarios suivants sont possibles :

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
<h2>Use the Finish No Earlier Than constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Earlier Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>Finish No Earlier Than</strong>.</p> <p> <img src="assets/fnet-350x267.png" alt="FNET.png" style="width: 350;height: 267;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete no earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes.</strong> </li>
</ol>
</div>
-->
