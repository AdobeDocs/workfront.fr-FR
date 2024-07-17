---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Vue d’ensemble de la date de début prévue de la tâche
description: La Date de début planifiée d’une tâche est la date à laquelle, en tant que créateur de la tâche, vous décidez que le travail sur la tâche doit commencer. Les dates des tâches planifiées influent sur les dates et la chronologie du projet. Pour plus d’informations sur la date de début prévue du projet, voir Présentation de la date de début prévue du projet.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 4%

---

# Vue d’ensemble de la date de début prévue de la tâche

La Date de début planifiée d’une tâche est la date à laquelle, en tant que créateur de la tâche, vous décidez que le travail sur la tâche doit commencer. Les dates des tâches planifiées influent sur les dates et la chronologie du projet. Pour plus d’informations sur la date de début planifiée du projet, voir [Présentation de la date de début planifiée du projet](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## Date de début planifiée d’une tâche

Vous pouvez indiquer la Date de début planifiée d&#39;une tâche ou laisser Adobe Workfront en charge de la calculer selon certains critères. 

* [Définition manuelle de la date de début planifiée d’une tâche](#manually-set-the-planned-start-date-of-a-task)
* [Méthode de calcul de la date de début planifiée pour une tâche](#how-the-planned-start-date-is-calculated-for-a-task)

### Définir manuellement la date de début planifiée d’une tâche {#manually-set-the-planned-start-date-of-a-task}

La définition de la date de début planifiée d’une tâche dépend du type de contrainte de tâche que vous lui affectez. 

Vous pouvez définir manuellement la date de début planifiée lors de la création d’une tâche, comme décrit dans l’article [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Vous pouvez spécifier manuellement la date de début planifiée lorsque vous sélectionnez l’une des contraintes de tâche suivantes : 

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
   <td> <p>La durée est ajustée afin de conserver la date d’achèvement planifiée identique.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Méthode de calcul de la date de début planifiée pour une tâche {#how-the-planned-start-date-is-calculated-for-a-task}

Lorsqu&#39;il est calculé automatiquement par le système, les éléments suivants peuvent influencer la Date de début planifiée d&#39;une tâche :

* Paramètre de préférence Date de début dans la zone Tâches et problèmes de la configuration.

  L’administrateur de Workfront ou de groupe peut déterminer si une nouvelle tâche commence à la même date que la date de début planifiée du projet ou le jour où vous créez la tâche.

  Pour plus d’informations sur les préférences Tâches et problèmes, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Contrainte de tâche

  Pour plus d’informations sur les contraintes de tâche, consultez l’article [Présentation de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* Relation de prédécesseur de tâche

  Pour plus d’informations sur les prédécesseurs de tâches, consultez l’article [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Date de début du projet, lorsque le projet est planifié à partir de la date de début.
* Le planning de désactivation du Principal cessionnaire de la tâche.

  Lorsque le Principal cessionnaire a un délai d’expiration planifié pendant la durée de la tâche, les dates planifiées de la tâche s’ajustent en conséquence lorsque le paramètre **Prendre en compte le temps d’arrêt de l’utilisateur dans les durées de la tâche** est sélectionné pour le champ **Durée d’expiration de l’utilisateur** . Les nouveaux projets héritent de ce paramètre de la zone Préférences du projet, mais vous pouvez le modifier au niveau du projet.

  Par exemple, si une tâche dont la contrainte est définie sur Dès que possible doit commencer le 1er juin et se terminer le 3 juin, et que la personne désignée par le Principal a marqué le 1er juin pour un délai de pause, la date de début planifiée de la tâche devient le 2 juin.

  Pour plus d’informations sur la préférence **User Time Off**, reportez-vous aux articles [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Lorsqu&#39;elle est définie automatiquement, la Date de début planifiée est déterminée selon le calcul suivant : 

```
Planned Start Date = Planned Completion Date - Task Duration
```

Par exemple, si votre tâche a une date de fin du 16 septembre et une durée de 10 jours, la date de début planifiée est le 6 septembre.

>[!NOTE]
>
> Le type de mise à jour du projet doit également être défini sur &quot;Automatique et En Changement&quot; ou &quot;Automatiquement&quot; pour que les Heures et Durée Planifiées soient automatiquement ajustées.\
>Pour plus d’informations sur le type de mise à jour, consultez l’article [Sélectionner le type de mise à jour du projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).
