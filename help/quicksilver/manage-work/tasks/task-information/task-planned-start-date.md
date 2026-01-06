---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Aperçu de la date de début prévue de la tâche
description: La date de début prévue d’une tâche est la date à laquelle vous, en tant que personne à l’origine de la tâche, décidez que le travail sur la tâche doit commencer. Les dates des tâches prévues influencent les dates et la chronologie du projet. Pour plus d’informations sur la date de début prévue du projet, consultez la section « Vue d’ensemble de la date de début prévue du projet ».
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 45%

---

# Vue d’ensemble de la Date de début prévue de la tâche

<!-- Audited: 6/2025 -->

La date de début prévue d’une tâche est la date à laquelle vous, en tant que personne à l’origine de la tâche, décidez que le travail sur la tâche doit commencer. Les dates des tâches prévues influencent les dates et la chronologie du projet. Pour plus d’informations sur la date de début prévue du projet, consultez la section [« Vue d’ensemble de la date de début prévue du projet »](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Date de début prévue d’une tâche

Vous pouvez indiquer la Date de début prévue de la tâche ou laisser à Adobe Workfront le soin de la calculer en fonction de certains critères.

* [Définir manuellement la date de début prévue d’une tâche](#manually-set-the-planned-start-date-of-a-task)
* [Calcul de la date de début prévue pour une tâche](#how-the-planned-start-date-is-calculated-for-a-task)

### Définir manuellement la date de début prévue d’une tâche {#manually-set-the-planned-start-date-of-a-task}

La définition de la date de début prévue d&#39;une tâche dépend du type de contrainte de tâche que vous affectez à la tâche.

Vous pouvez définir manuellement la Date de début prévue lors de la création d’une tâche. Pour plus d’informations, voir [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Vous pouvez spécifier manuellement la date de début prévue lorsque vous sélectionnez l&#39;une des contraintes de tâche suivantes :

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

* Le paramètre de préférence Date de début dans la zone Tâches et événements de la Configuration

  Votre administrateur Workfront ou de groupe peut déterminer si une nouvelle tâche commence à la même date que la date de début prévue du projet ou le jour où vous créez la tâche.

  Pour plus d’informations sur les préférences de tâches et d’événements, voir [Configurer les préférences de tâches et d’événements à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Contrainte de tâche

  Pour plus d&#39;informations sur les contraintes de tâche, voir [présentation des contraintes de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relation des tâches antérieures

  Pour plus d’informations sur les tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Date de début du projet, lorsque le projet est prévu à partir de la date de début.
* Planning des congés du cessionnaire de Principal de la tâche.

  Lorsque la personne désignée par Principal dispose de congés planifiés pendant la durée de la tâche, les dates planifiées de la tâche s’ajustent en conséquence lorsque le paramètre Prendre en compte les congés de l’utilisateur dans les durées de la tâche est sélectionné pour le champ Congés de l’utilisateur . Les nouveaux projets héritent de ce paramètre de la zone Préférences du projet , mais vous pouvez le modifier au niveau du projet.

  Par exemple, si une tâche assortie d&#39;une contrainte Dès Que Possible est planifiée pour commencer le 1er juin et se terminer le 3 juin et que le cessionnaire du Principal a marqué le 1er juin comme étant pour les congés, la date de début prévue de la tâche devient le 2 juin.

  Pour plus d’informations sur la préférence de Congés de l’utilisateur, voir [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Lorsqu’elle est définie automatiquement, la Date de début prévue est déterminée en fonction du calcul suivant :

```
Planned Start Date = Planned Completion Date - Task Duration
```

Par exemple, si votre tâche a une date d’achèvement fixée au 16 septembre et une durée de 10 jours, la date de début prévue est le 6 septembre.

>[!NOTE]
>
> Le type de mise à jour du projet doit également être défini sur Automatique et En cas de modification ou Automatiquement pour que les heures et la durée prévues soient automatiquement ajustées.\
>Pour plus d’informations sur le type de mise à jour, voir [Sélectionner le type de mise à jour du projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).
