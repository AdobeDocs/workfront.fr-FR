---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Vue d’ensemble du statut de la progression de la tâche
description: Adobe Workfront détermine l’état d’avancement d’une tâche en examinant l’avancement de celle-ci dans sa chronologie. Vous pouvez configurer Workfront pour déterminer la condition d’un projet en fonction de la valeur de l’état de progression des tâches. Pour plus d’informations sur la configuration de la condition du projet, consultez l’article Présentation de la condition et du type de condition du projet .
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# Vue d’ensemble du statut de la progression de la tâche

<!-- Audited: 1/2024 -->

Adobe Workfront détermine l’état d’avancement d’une tâche en examinant l’avancement de celle-ci dans sa chronologie. Vous pouvez configurer Workfront pour déterminer la condition d’un projet en fonction de la valeur de l’état de progression des tâches. Pour plus d’informations sur la configuration de la condition du projet, consultez l’article [Présentation de la condition et du type de condition du projet](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Critères qui déterminent l’état d’avancement des tâches

Pour plus d’informations sur l’état de progression d’un projet, voir [Aperçu de l’état de progression du projet](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Pour plus d’informations sur le suivi de la progression de vos tâches, voir [Présentation du mode de suivi des tâches](../../../manage-work/tasks/task-information/task-tracking-mode.md).

Les critères suivants déterminent l’état d’avancement d’une tâche :

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Statut de progression</strong> </p> </th> 
   <th> <p><strong>Détermination des critères</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>Heure d’activation</strong> </p> </td> 
   <td scope="col"> <p>Une tâche est considérée comme <strong> à l’heure </strong> lorsque toutes les dates planifiées correspondent aux dates prévues. Cet état d’avancement peut également signifier que le projet est en avance sur le calendrier et que les dates prévues peuvent être antérieures aux dates prévues.</p> <p>Pour plus d’informations sur les dates prévues, voir <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Présentation de la date d’achèvement prévue pour les projets, les tâches et les problèmes</a>.</p> <p>Pour plus d’informations sur la date d’achèvement prévue de la tâche, voir les articles suivants :</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Présentation de la tâche Date de début planifiée</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Présentation de la tâche Date d’achèvement prévue</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>En danger</strong> </p> </td> 
   <td><p>Une tâche est considérée <strong>à risque</strong> lorsque la date d’achèvement estimée est supérieure à la date d’achèvement prévue et supérieure à la date d’achèvement prévue. Cela peut se produire lorsqu’une tâche a une contrainte de <strong>Doit se terminer le </strong> ou <strong>Doit commencer le</strong>, mais que le pourcentage de réalisation ou les relations de prédécesseur de la tâche montrent qu’elle ne peut pas se terminer ou commencer aux dates spécifiées. </p><p> Si vous définissez la contrainte de tâche sur <strong>Doit se terminer le </strong>, la date d’achèvement planifiée est définie manuellement sur une date spécifique. Dans ce cas, la date de fin prévue correspond à la date de fin planifiée. Dans le cas de cette contrainte, Workfront analyse la tâche pour calculer à quel moment elle se terminera en fonction du pourcentage d’achèvement. Ce calcul est stocké en tant que Date d’échéance estimée. Si la date d’échéance estimée est postérieure à la date d’achèvement prévue, la tâche risque d’être en retard. </p> <p> Si vous définissez la contrainte de tâche sur <strong>Doit démarrer le </strong>, la date de début planifiée est définie manuellement sur une date spécifique. Dans ce cas, la Date de début prévue correspond à la Date de début planifiée. Dans le cas de cette contrainte, Workfront analyse la tâche à calculer à quel moment elle commencera en fonction des relations de son prédécesseur. Ce calcul est stocké en tant que Date de début estimée. Si un prédécesseur appliqué ne permet pas à la tâche de commencer à la date de début spécifiée, la date de début estimée peut être postérieure à la date de fin prévue. La tâche est considérée comme susceptible d'être en retard. </p> <p>Remarque : En règle générale, les dates estimées correspondent aux dates projetées, à l’exception des cas où <strong>Doit démarrer le</strong> ou <strong>Doit se terminer le</strong> sont utilisés. Dans ce cas, les dates estimées continuent à être calculées en fonction du pourcentage de données complètes et d’autres facteurs (relations précédentes), tandis que les dates prévues sont obligées de correspondre aux dates planifiées qui ont été définies manuellement.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Derrière </strong> </p> </td> 
   <td> <p>Une tâche est considérée comme <strong>Derrière</strong> lorsque la date d’achèvement estimée est supérieure ou égale à la date d’achèvement planifiée et inférieure à la date d’achèvement prévue.</p> <p>La date de fin prévue est une vue en temps réel du moment où la tâche sera terminée en fonction de la progression précédente. Bien que la tâche ait été lancée tardivement, elle n’est pas encore considérée comme en retard, car les dates d’achèvement prévues et prévues sont toujours à l’avenir et la tâche peut encore être terminée à temps.</p> <p>Remarque : Les états de progression <strong>Derrière </strong> et <strong>À risque</strong> sont presque identiques. Cependant, <strong>Au risque</strong> indique qu’il existe des contraintes de tâche forcées (Doit se terminer, Doit commencer, dates fixes) sur l’une ou les deux dates planifiées. S’il n’y a aucune contrainte sur la tâche, les Dates projetées sont les mêmes que les Dates estimées et reflètent le calcul système de la Date de fin en fonction de la progression actuelle de la tâche. La tâche n’est pas encore considérée en retard, car les dates de fin prévues et prévues sont toujours à l’avenir et la tâche peut encore être terminée à temps.<br>Pour plus d’informations sur les dates prévues et estimées, consultez la <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Présentation des dates projetées et estimées </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>En retard</strong> </p> </td> 
   <td> <p>Une tâche est <strong>En retard</strong> lorsque la date d’achèvement planifiée est antérieure à la date d’aujourd’hui.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![](assets/on-time-progress-status-350x233.png)

* At Risk

  ![](assets/at-risk-progress-status-350x233.png)

* Behind

  ![](assets/behind-progress-status-350x233.png)

* Late

  ![](assets/late-progress-status-350x233.png)

-->