---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Vue d’ensemble de la date d’achèvement prévue de la tâche
description: La date d’achèvement planifiée d’une tâche est la date à laquelle la tâche est configurée pour se terminer.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 4%

---

# Vue d’ensemble de la date d’achèvement prévue de la tâche

La date d’achèvement planifiée d’une tâche est la date à laquelle la tâche est configurée pour se terminer.

Vous pouvez indiquer la Date d’achèvement planifiée d’une tâche ou laisser Adobe Workfront en charge de son calcul selon certains critères. 

Les dates d’achèvement planifiées des tâches d’un projet déterminent la date d’achèvement planifiée d’un projet lorsque le projet est planifié à partir de la date de début. Pour plus d’informations sur la date d’achèvement prévue du projet, voir [Définition de la date d’achèvement prévu du projet](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La date d’achèvement planifiée d’une tâche diffère de la date de validation de la tâche ou de la date d’achèvement prévue de la tâche de la manière suivante :
>
>* La date de validation est la date à laquelle la personne affectée à la tâche estime manuellement qu’elle aura terminé la tâche. Pour plus d’informations, voir les articles suivants :
>
>   * [Vue d’ensemble des dates d’engagement](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interactions entre la date de validation et la date d’achèvement planifiée](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* La date de fin prévue est une date calculée par Workfront qui prend en compte les délais de la tâche, les calendriers de la tâche ou de ses prédécesseurs, ainsi que d’autres facteurs pour déterminer une date de vie réelle à laquelle la tâche peut être réalisablement terminée. Pour plus d’informations, voir [Présentation de la date d’achèvement prévue pour les projets, les tâches et les problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Définition manuelle de la date d’achèvement planifiée d’une tâche

Pour pouvoir mettre à jour la date d’achèvement planifiée de la tâche, vous devez disposer des autorisations Modifier pour les tâches et Gérer la tâche.

La définition de la date d’achèvement planifiée d’une tâche dépend du type de contrainte de tâche que vous affectez à la tâche. 

Vous pouvez définir manuellement la date d’achèvement prévue dans les zones suivantes de Workfront :

* Dans la zone Modifier la tâche, lors de la création ou de la modification d’une tâche. Pour plus d’informations, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Dans la zone Détails de la tâche. Pour plus d’informations, voir [Gérer les informations de tâche dans la zone Task Details Overview](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* Dans la zone Accueil , si la Date de fin planifiée s’affiche lors de l’affichage d’une tâche. Pour plus d’informations, voir [Mise à jour ou modification d’un élément de travail dans la zone d’accueil](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* Dans l’en-tête de la tâche. Pour plus d’informations, voir [Nouveaux en-têtes d’objet](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* Dans une liste de tâches ou un rapport lorsque le champ Date d’achèvement planifiée s’affiche dans la vue.

  Pour plus d’informations, voir [Modifier les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Vous pouvez spécifier manuellement la date d’achèvement planifiée lorsque vous sélectionnez l’une des contraintes de tâche suivantes : 

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
   <td> <p>Il Faut Finir Le</p> <p>Finir Au Plus Tard</p> <p>Finir Au Plus Tôt</p> </td> 
   <td> <p><span class="s1">La date de début planifiée est ajustée afin de conserver la même durée.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dates fixes</p> </td> 
   <td> <p>La durée est ajustée afin de conserver la date de début planifiée identique.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Comment Workfront calcule automatiquement la date d’achèvement planifiée d’une tâche

Lorsqu’il est calculé automatiquement par le système, les éléments suivants peuvent influencer la Date d’achèvement planifiée d’une tâche :

* Contrainte de tâche

  Pour plus d’informations sur les contraintes de tâche, consultez l’article [Présentation de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relation de prédécesseur de tâche

  Pour plus d’informations sur les prédécesseurs de tâches, consultez l’article [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Date de fin du projet, lorsque le projet est planifié à partir de la date de fin.
* Le planning de désactivation du Principal cessionnaire de la tâche.

  Lorsque le Principal cessionnaire a un délai d’expiration planifié pendant la durée de la tâche, les dates planifiées de la tâche s’ajustent en conséquence lorsque le paramètre **Prendre en compte le temps d’arrêt de l’utilisateur dans les durées de la tâche** est sélectionné pour le champ **Durée d’expiration de l’utilisateur** . Les nouveaux projets héritent de ce paramètre de la zone Préférences du projet, mais vous pouvez le modifier au niveau du projet.

  Par exemple, si une tâche dont la contrainte est définie sur Dès que possible doit commencer le 1er juin et se terminer le 3 juin, et que le Principal cessionnaire a été marqué le 2 juin pour un délai dépassé, la date d’achèvement prévue de la tâche devient le 4 juin.

  Pour plus d’informations sur la préférence **User Time Off**, reportez-vous aux articles [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

* La durée associée aux paramètres d’approbation si la tâche est associée à une validation. Pour plus d’informations, voir [Configuration des paramètres d’approbation globale](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Lorsqu’elle est définie automatiquement, la date d’achèvement planifiée est déterminée selon le calcul suivant : 

```
Planned Completion Date = Planned Start Date + Duration
```

Par exemple, si votre tâche a une date de début du 16 septembre et une durée de 10 jours, la date d’achèvement planifiée est le 26 septembre.

>[!NOTE]
>
> Le type de mise à jour du projet doit être défini sur Automatique et Après changement ou Automatiquement pour que les heures et la durée planifiées soient automatiquement ajustées.\
>Pour plus d’informations sur le type de mise à jour, consultez l’article [Sélectionner le type de mise à jour du projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).
