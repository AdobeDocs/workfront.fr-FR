---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Présentation de la contrainte de tâche : Terminer au plus tard"
description: Finish No Later Than (FNLT) est une contrainte de tâche qui planifie l’achèvement d’une tâche avant la date que vous spécifiez.
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 2%

---

# Vue d’ensemble des contraintes de tâches : Terminer au plus tard

Finish No Later Than (FNLT) est une contrainte de tâche qui planifie l’achèvement d’une tâche avant la date que vous spécifiez.

## Présentation de la contrainte Terminer au plus tard

Tenez compte de ce qui suit lorsque vous utilisez la contrainte Terminer plus tard que (FNLT) pour une tâche :

* Vous devez utiliser cette contrainte lorsque le projet est planifié à partir de la date de début. Dans ce cas, vous pouvez fournir une contrainte souple sur une tâche avant qu’elle ne force d’autres tâches dépendantes à s’afficher comme En danger.
* Lorsque vous utilisez la contrainte FNLT avec un projet de date de fin de planification, cette contrainte planifie la tâche comme si elle était en retard.
* Lorsque vous déplacez ou copiez une tâche avec une contrainte FNET vers un autre projet, la contrainte de la tâche ou des dates du projet peut changer en fonction des dates de contrainte et des dates de début et de fin du projet. Les scénarios suivants sont possibles :

   * Lorsque le projet de destination est planifié à partir du début :

      * Lorsque la date de contrainte de la tâche est antérieure à la date de début prévue du projet, la contrainte de tâche passe à Dès que possible.
      * Lorsque la date de contrainte de la tâche est postérieure à la date de fin planifiée du projet, la date de fin prévue du projet est modifiée pour correspondre à la date de contrainte d’achèvement de la tâche.

      * Lorsque le projet de destination est planifié à partir de la fin :

         * Lorsque la date de contrainte de la tâche est postérieure à la date d’achèvement du projet, la contrainte de la tâche passe à Aussi tard que possible.
         * Lorsque la date de contrainte de la tâche est antérieure à la date de début planifiée du projet, la date de début planifiée du projet change pour correspondre à la date de contrainte de début de la tâche.

      * Quelle que soit la planification du projet, lorsque la date de contrainte de la tâche se trouve dans les dates de début et de fin du projet, aucune modification n’est apportée à la contrainte de tâche ou aux dates du projet.

  Pour plus d’informations sur le déplacement des tâches, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md). Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche sur une tâche, voir [Mise à jour de la contrainte de tâche d’une tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
