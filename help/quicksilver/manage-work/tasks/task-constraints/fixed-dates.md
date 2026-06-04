---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D''Ensemble Des Contraintes De Tâche : Dates Fixes'
description: Vous pouvez utiliser la contrainte de tâche de dates fixes lorsque vous souhaitez de la précision quant à la date de début et à la date de fin exactes de vos tâches. Pour plus d’informations sur les contraintes de tâche, voir vue d’ensemble de la contrainte de tâche.
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
TQID: https://experienceleague.adobe.com/rVMjo1IgPBQpLatO8jufxGPYTn2W0qghce2v5O-zPRo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 98%

---

# Vue d’ensemble de la contrainte de tâche : dates fixes

Vous pouvez utiliser la contrainte de tâche de dates fixes lorsque vous souhaitez de la précision quant à la date de début et à la date de fin exactes de vos tâches. Pour plus d’informations sur les contraintes de tâche, voir [Vue d’ensemble de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

## Vue d’ensemble de la contrainte de dates fixes

Tenez compte des points suivants lors de l’utilisation de la contrainte de dates fixes :

* Lorsque vous sélectionnez la contrainte de tâche Dates fixes (FIXT), vous devez préciser la Date de début prévue et la Date d’achèvement prévue de la tâche. Dans ce cas, la relation antérieure de la tâche est ignorée.
* Le champ Durée de la tâche n’est pas modifiable lors de l’utilisation de la contrainte FIXT. La durée est calculée comme la différence entre les dates de début et d’achèvement prévues de la tâche.
* Si le Type de durée de la tâche est piloté par l’effort, le nombre de personnes affectées à la tâche a également un impact la Durée de la tâche.
* Lorsque vous déplacez ou copiez une tâche avec une contrainte FIXT vers un autre projet, la contrainte de la tâche ou les dates du projet peuvent changer en fonction des dates de contrainte et des dates de début et d’achèvement du projet. Les scénarios suivants sont possibles :

   * Lorsque le projet de destination est planifié à partir du début :

      * Lorsque les dates de contrainte de tâche sont antérieures à la date de début du projet, la contrainte de tâche passe à Aussi Tôt Que Possible.
      * Si l’une des dates de contrainte de tâche ou les deux sont postérieures à la date d’achèvement prévue du projet, la date d’achèvement prévue du projet change pour correspondre à la date de contrainte d’achèvement de la tâche.

   * Lorsque le projet de destination est planifié à partir de l’achèvement :

      * Lorsque les dates de contrainte de la tâche sont postérieures à la date d’achèvement du projet, la contrainte de tâche devient Aussi Tard Que possible.
      * Lorsque les dates de contrainte de tâche sont antérieures à la date de début prévue du projet, la date de début prévue du projet change pour correspondre à la date de contrainte de début de la tâche.

   * Quelle que soit le planning du projet, lorsque les dates de contrainte de la tâche sont comprises entre les dates de début et d’achèvement du projet, aucune modification n’est apportée à la contrainte de tâche ou aux dates du projet.

  Pour plus d’informations sur le déplacement de tâches, voir [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md). Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche, voir [Mettre à jour la contrainte de tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
