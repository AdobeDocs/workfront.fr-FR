---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble du statut de progression du projet
description: Adobe Workfront détermine l’état d’avancement d’un projet en examinant l’avancement du projet dans sa chronologie. Vous pouvez configurer Workfront pour déterminer la condition d’un projet en fonction de la valeur de l’état de progression des tâches. Pour en savoir plus sur l’état d’avancement du projet, consultez cet article .
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 4%

---

# Vue d’ensemble du statut de progression du projet

<!--Audited: 12/2023-->

Adobe Workfront détermine l’état d’avancement d’un projet en examinant l’avancement du projet dans sa chronologie. Vous pouvez configurer Workfront pour déterminer la condition d’un projet en fonction de la valeur de l’état de progression des tâches. Pour plus d’informations sur la configuration de la condition du projet, consultez l’article [Présentation de la condition et du type de condition du projet](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Vous trouverez ci-dessous les états d’avancement des projets dans Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>À l’heure</td> 
   <td> L’état de progression d’un projet est <strong>À l’heure d’activation</strong> si :<ul><li>Si les dates de fin prévues et estimées sont antérieures ou égales à la date de fin prévue du projet</li></ul> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>En danger</td> 
   <td> L'état d'avancement d'un projet est <strong>En danger</strong> si <strong>tous</strong> des cas suivants sont vrais :<ul><li>Les dates d’achèvement estimées et prévues sont dans le futur.</li><li> Les dates de fin estimées et prévues sont postérieures à la date de fin planifiée.</li><li> La date de fin estimée est postérieure à la date de fin prévue</li></ul><p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>En retard</td> 
   <td> L’état d’avancement d’un projet est <strong>Derrière</strong> si <strong>tous</strong> des éléments suivants sont vrais :<ul><li>Les dates d’achèvement estimées et prévues sont dans le futur.</li><li> Les dates de fin estimées et prévues sont postérieures à la date de fin planifiée du projet.</li><li> La date d’achèvement estimée n’est pas postérieure à la date d’achèvement prévue</li></ul> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>En retard</td> 
   <td> 
     L’état de progression d’un projet est <strong>En retard</strong> si <strong>l’un des </strong> des éléments suivants est vrai :<ul><li>Le projet est terminé et la date d’achèvement réelle est postérieure à la date d’achèvement planifiée <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Le projet n’est pas terminé et la date d’achèvement prévue du projet se situe dans le passé <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants :

* La date d’achèvement prévue du projet est gérée par la tâche sur le chemin critique avec la dernière date d’achèvement prévue.
* La date d’achèvement estimée du projet est générée par la tâche sur le chemin critique avec la dernière date d’achèvement estimée.

Pour plus d’informations sur le projet Chemin critique, voir [Présentation du projet Chemin critique](../../../manage-work/tasks/manage-tasks/critical-path.md).

Pour plus d’informations sur les dates de fin prévues, voir [Présentation de la date de fin prévue pour les projets, les tâches et les problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
