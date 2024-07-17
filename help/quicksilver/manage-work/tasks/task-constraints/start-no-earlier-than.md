---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: "Présentation de la contrainte de tâche : ne pas commencer avant"
description: Utilisez la contrainte de tâche Début avant (SNET) pour planifier le démarrage d’une tâche après la date que vous avez spécifiée.
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 2%

---

# Vue d’ensemble des contraintes de tâches : Commencer Au Plus Tôt

Utilisez la contrainte de tâche Début avant (SNET) pour planifier le démarrage d’une tâche après la date que vous avez spécifiée.

## Présentation de la contrainte Début non antérieur à la tâche

Tenez compte des points suivants lorsque vous utilisez la contrainte Début non plus tôt que Tâche :

* Vous devez utiliser la contrainte Ne pas commencer avant lorsque le projet est planifié à partir de la date de début. Dans ce cas, vous pouvez fournir une contrainte souple sur une tâche avant qu’elle ne force d’autres tâches dépendantes à s’afficher comme En danger.
* La contrainte par défaut Début non plus tôt est définie si un projet est planifié à partir de la date de début et si la date de début par défaut du système ou du groupe d’une nouvelle tâche est définie sur Aujourd’hui. Pour plus d’informations sur la configuration des paramètres par défaut pour les tâches, voir [Configuration des tâches à l’échelle du système et des préférences de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Si vous planifiez le projet à partir de la date de début et que la date de début par défaut du système d’une nouvelle tâche est définie sur Basé sur la date planifiée du projet, la contrainte par défaut d’une nouvelle tâche est Dès que possible.
* Si vous planifiez le projet à partir de la date de fin et que la date de début par défaut système d’une nouvelle tâche est définie sur Aujourd’hui, la contrainte Démarrer le plus tôt possible planifie la tâche, car elle serait aussi tardive que possible.
* Lorsque vous déplacez ou copiez une tâche avec une contrainte SNET vers un autre projet, la contrainte de la tâche ou des dates du projet peut changer en fonction des dates de contrainte et des dates de début et de fin du projet. Les scénarios suivants sont possibles :

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
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
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
