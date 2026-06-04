---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Vue D’Ensemble De La Contrainte De Tâche : Terminer Au Plus Tard'
description: Finir Au Plus Tard (Finish No Later Than, FNLT) est une contrainte de tâche qui planifie l’achèvement d’une tâche avant la date que vous avez spécifiée.
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
TQID: https://experienceleague.adobe.com/lNcQlOWhkCOl0keoOBLgyKVo3VmlOnEPXRmVGhHFHF8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 388
ht-degree: 98%

---

# Vue d’ensemble des contraintes de tâches : Terminer au plus tard

Finir Au Plus Tard (Finish No Later Than, FNLT) est une contrainte de tâche qui planifie l’achèvement d’une tâche avant la date que vous avez spécifiée.

## Vue d’ensemble de la contrainte Finir Au Plus Tard

Tenez compte de ce qui suit lorsque vous utilisez la contrainte Finir Au Plus Tard (FNLT) pour une tâche :

* Vous devez utiliser cette contrainte lorsque le projet est planifié à partir de la date de début. Dans ce cas, vous pouvez imposer une contrainte souple sur une tâche avant qu’elle ne force d’autres tâches dépendantes à s’afficher comme À risque.
* Lorsque vous utilisez la contrainte FNLT avec un projet Planifier à partir de la date d’achèvement, cette contrainte planifie la tâche comme une tâche Aussi Tard Que Possible.
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
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
