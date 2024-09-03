---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Vue d’ensemble de la Date de début prévue de la tâche
description: La date de début prévue d’une tâche est la date à laquelle vous, en tant que personne à l’origine de la tâche, décidez que le travail sur la tâche doit commencer. Les dates des tâches prévues influencent les dates et la chronologie du projet. Pour plus d’informations sur la date de début prévue du projet, consultez la section « Vue d’ensemble de la date de début prévue du projet ».
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 100%

---

# Vue d’ensemble de la Date de début prévue de la tâche

La date de début prévue d’une tâche est la date à laquelle vous, en tant que personne à l’origine de la tâche, décidez que le travail sur la tâche doit commencer. Les dates des tâches prévues influencent les dates et la chronologie du projet. Pour plus d’informations sur la date de début prévue du projet, consultez la section [« Vue d’ensemble de la date de début prévue du projet »](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Date de début prévue d’une tâche

Vous pouvez spécifier la date de début prévue d’une tâche ou laisser Adobe Workfront la calculer en fonction de certains critères. 

* [Définir manuellement la date de début prévue d’une tâche](#manually-set-the-planned-start-date-of-a-task)
* [Calcul de la date de début prévue pour une tâche](#how-the-planned-start-date-is-calculated-for-a-task)

### Définir manuellement la date de début prévue d’une tâche {#manually-set-the-planned-start-date-of-a-task}

La définition de la date de début prévue d’une tâche dépend du type de contrainte de tâche que vous affectez à la tâche. 

Vous pouvez définir manuellement la date de début prévue lors de la création d’une tâche, comme décrit dans l’article [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Vous pouvez spécifier manuellement la date de début prévue lorsque vous sélectionnez l’une des contraintes de tâche suivantes :

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Type de contrainte de tâche</strong> </p> </th> 
   <th> <p><strong>Effet de la modification manuelle de la date d’achèvement prévue</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Il Faut Commencer Le</p> <p>Commencer Au Plus Tôt</p> <p>Commencer Au Plus Tard</p> </td> 
   <td> <p><span class="s1">La date d’achèvement prévue est ajustée afin de conserver la même durée.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dates fixes</p> </td> 
   <td> <p>La durée est ajustée afin de conserver la date d’achèvement prévue identique.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calcul de la date de début prévue pour une tâche {#how-the-planned-start-date-is-calculated-for-a-task}

Lorsqu’elle est calculée automatiquement par le système, les éléments suivants peuvent influencer la date de début prévue d’une tâche :

* Paramètres de préférence de la date de début dans la zone des tâches et des problèmes de la configuration

  Votre administrateur ou votre administratrice Workfront ou de groupes peut déterminer si une nouvelle tâche commence à la même date que la date de début prévue du projet ou le jour où vous créez la tâche.

  Pour plus d’informations sur les préférences relatives aux tâches et aux problèmes, consultez la section [Configurer les préférences des tâches et des problèmes à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Contrainte de tâche

  Pour plus d’informations sur les contraintes de tâches, consultez l’article [Vue d’ensemble des contraintes de tâches.](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* Relation des tâches antérieures

  Pour plus d’informations sur les tâches antérieures, consultez l’article [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Date de début du projet, lorsque le projet est prévu à partir de la date de début.
* Les congés planifiés de la personne cessionnaire principale de la tâche.

  Lorsque la personne cessionnaire principale prend des congés pendant la durée de la tâche, les dates prévues de la tâche sont ajustées en conséquence lorsque le paramètre **Prendre en compte les congés de l’utilisateur ou de l’utilisatrice dans la durée des tâches** est sélectionné pour le champ **Congés de l’utilisateur ou de l’utilisatrice**. Les nouveaux projets héritent de ce paramètre depuis la zone Préférences du projet, mais vous pouvez modifier ce paramètre au niveau du projet.

  Par exemple, si une tâche avec une contrainte « Aussi Tôt Que Possible » est programmée pour commencer le 1er juin et se terminer le 3 juin, et que la personne cessionnaire principale a marqué le 1er juin comme date de congé, la date de début prévue de la tâche devient le 2 juin.

  Pour plus d’informations sur la préférence **Congés des utilisateurs et des utilisatrices**, consultez les articles [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Lorsqu’elle est définie automatiquement, la date de début prévue est déterminée selon le calcul suivant :

```
Planned Start Date = Planned Completion Date - Task Duration
```

Par exemple, si votre tâche a une date d’achèvement fixée au 16 septembre et une durée de 10 jours, la date de début prévue est le 6 septembre.

>[!NOTE]
>
>Le type de mise à jour du projet doit également être défini sur « Automatique et En cas de modification » ou « Automatiquement » pour que le nombre d’heures prévues et la durée soient automatiquement ajustés.\
>Pour plus d’informations sur le type de mise à jour, consultez l’article [Sélectionner le type de mise à jour du projet.](../../../manage-work/projects/manage-projects/select-project-update-type.md).
