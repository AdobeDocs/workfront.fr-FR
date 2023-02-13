---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Présentation de la contrainte de tâche : Doit démarrer le"'
description: Utilisez la contrainte de tâche Doit démarrer le (MSO) pour planifier le démarrage exact d’une tâche à une date spécifique.
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Présentation de la contrainte de tâche : Doit démarrer le

Utilisez la contrainte de tâche Doit démarrer le (MSO) pour planifier le démarrage exact d’une tâche à une date spécifique.

La contrainte Doit commencer à planifie une tâche pour qu’elle commence exactement à l’heure et à la date spécifiées dans la variable **Date de début planifiée** champ .

>[!TIP]
>
>La mise à jour manuelle de la Date de début planifiée d’une tâche modifie la contrainte de la tâche à Sur laquelle la tâche doit commencer.

## Présentation de la contrainte de tâche Doit démarrer sur

Tenez compte de ce qui suit lors de la planification d’une tâche avec une contrainte Doit démarrer sur :

* Les relations avec le prédécesseur ne forcent pas cette tâche à replanifier. Workfront ignore essentiellement les relations précédentes de la tâche avec cette contrainte.
* La tâche n’affiche pas **À risque** si les prédécesseurs commencent à courir en retard ou en retard.

* Lorsque vous déplacez ou copiez une tâche avec une contrainte MSO vers un autre projet, la contrainte de la tâche ou des dates du projet peut changer en fonction des dates de contrainte et des dates de début et de fin du projet. Les scénarios suivants existent :

   * Lorsque le projet de destination est planifié à partir du début :

      * Lorsque la date de contrainte de la tâche est antérieure à la date de début prévue du projet, la contrainte de tâche passe à Dès que possible.
      * Lorsque la date de contrainte de la tâche est postérieure à la date de fin planifiée du projet, la date de fin prévue du projet est modifiée pour correspondre à la date de contrainte d’achèvement de la tâche.

      * Lorsque le projet de destination est planifié à partir de la fin :

         * Lorsque la date de contrainte de la tâche est postérieure à la date d’achèvement du projet, la contrainte de la tâche passe à Aussi tard que possible.
         * Lorsque la date de contrainte de la tâche est antérieure à la date de début planifiée du projet, la date de début planifiée du projet change pour correspondre à la date de contrainte de début de la tâche.
      * Quelle que soit la planification du projet, lorsque la date de contrainte de la tâche se trouve dans les dates de début et de fin du projet, aucune modification n’est apportée à la contrainte de tâche ou aux dates du projet.

   Pour plus d’informations sur le déplacement des tâches, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md). Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur la mise à jour de la contrainte de tâche sur une tâche, voir [Mettre à jour la contrainte de tâche d’une tâche](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
