---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: État d’avancement du projet - Aperçu
description: Adobe Workfront détermine l’état d’avancement d’un projet en examinant l’avancement du projet dans sa chronologie. Vous pouvez configurer Workfront pour déterminer la condition d’un projet en fonction de la valeur de l’état de progression des tâches. Pour plus d’informations sur la configuration de la condition du projet, consultez l’article Présentation de la condition et du type de condition du projet .
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# État d’avancement du projet - Aperçu

Adobe Workfront détermine l’état d’avancement d’un projet en examinant l’avancement du projet dans sa chronologie. Vous pouvez configurer Workfront pour déterminer la condition d’un projet en fonction de la valeur de l’état de progression des tâches. Pour plus d’informations sur la configuration de la condition du projet, consultez l’article . [Présentation de la condition et du type de condition du projet](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Vous trouverez ci-dessous les états d’avancement des projets dans Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Heure d’activation</td> 
   <td> <p>Si les dates d’achèvement prévues et estimées sont antérieures ou égales à la date d’achèvement prévue du projet, l’état d’avancement du projet est <strong>Heure d’activation</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>En danger</td> 
   <td> <p>Lorsque les dates d’achèvement estimées et prévues sont dans le futur mais postérieures à la date d’achèvement planifiée du projet et que la date d’achèvement estimée est postérieure à la date d’achèvement prévue, l’état d’avancement du projet est <strong>À risque</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>En retard</td> 
   <td> <p>Lorsque les dates d’achèvement estimées et prévues sont dans le futur mais postérieures à la date d’achèvement planifiée du projet, mais que la date d’achèvement estimée n’est pas supérieure à la date d’achèvement prévue, l’état d’avancement du projet est <strong>Derrière</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>En retard</td> 
   <td> 
    <ul> 
     <li> <p>Si le projet est terminé et que la date d’achèvement réelle est postérieure à la date d’achèvement planifiée, l’état d’avancement du projet est <strong>Tard</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Si le projet n’est pas terminé et que la date d’achèvement planifiée du projet se situe dans le passé, l’état d’avancement du projet est <strong>Tard</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants :

* La date d’achèvement prévue du projet est gérée par la tâche sur le chemin critique avec la dernière date d’achèvement prévue.
* La date d’achèvement estimée du projet est générée par la tâche sur le chemin critique avec la dernière date d’achèvement estimée.

Pour plus d’informations sur le projet Chemin critique, voir [Présentation du projet Chemin critique](../../../manage-work/tasks/manage-tasks/critical-path.md).

Pour plus d’informations sur les dates d’achèvement prévues, voir [Présentation de la date d’achèvement prévue pour les projets, tâches et problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
