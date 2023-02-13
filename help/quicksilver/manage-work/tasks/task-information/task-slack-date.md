---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Présentation de la date du Slack de tâches
description: Les tâches peuvent parfois démarrer et se terminer tard sans affecter la date d’achèvement du projet.
author: Alina
feature: Work Management
exl-id: ccdaa27d-e212-45dc-afca-08539f2b4001
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Présentation de la date du Slack de tâches

Les tâches peuvent parfois démarrer et se terminer tard sans affecter la date d’achèvement du projet.

La date du Slack affiche la date exacte à laquelle une tâche peut avoir une incidence définitive sur la date de fin du projet.

## Présentation de la date du Slack

La date du Slack est différente de la date d’achèvement prévue, car les relations précédentes et les contraintes de tâche augmentent le temps d’attente.

Tenez compte des scénarios suivants, selon qu’une tâche se trouve ou non sur le chemin critique d’un projet :

* Pour les tâches qui se trouvent sur le chemin critique du projet ou qui ont des successeurs sur le chemin critique, la date du Slack correspond à la date d’achèvement prévue de la tâche, sauf si l’état de progression de la tâche est déjà En retard ou En arrière-plan.

   Pour plus d’informations sur le chemin critique, voir [Présentation du projet Chemin critique](../../../manage-work/tasks/manage-tasks/critical-path.md).

   Pour plus d’informations sur l’état d’avancement des tâches, voir [Présentation de l’état de progression de la tâche](../../../manage-work/tasks/task-information/task-progress-status.md).

* Pour les tâches qui ne se trouvent pas sur le chemin critique, le temps de relâchement augmente plus tôt la planification de la tâche. Pour ces tâches, la date du Slack reste à l’avenir jusqu’à ce que les tâches deviennent tellement en retard qu’elles commencent à avoir une incidence sur la date d’achèvement du projet.

## Localisation de la date du Slack d’une tâche

Pour afficher la date du Slack d’une tâche, vous pouvez ajouter le champ Date du Slack à une vue de tâche ou à un rapport.

Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
