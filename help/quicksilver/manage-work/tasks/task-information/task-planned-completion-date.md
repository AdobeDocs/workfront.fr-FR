---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Vue d’ensemble de la Date d’achèvement prévue de la tâche
description: La date d’achèvement prévue d’une tâche est la date à laquelle la tâche doit être achevée.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 74%

---

# Vue d’ensemble de la Date d’achèvement prévue de la tâche

La date d’achèvement prévue d’une tâche est la date à laquelle la tâche doit être achevée.

Vous pouvez soit spécifier la date d’achèvement prévue d’une tâche, soit laisser Adobe Workfront la calculer en fonction de certains critères.

Les dates d’achèvement planifiées des tâches d’un projet déterminent la date d’achèvement planifiée d’un projet lorsque le projet est planifié à partir de la date de début. Pour plus d’informations sur la date d’achèvement prévue du projet, voir [Définition de la date d’achèvement prévu du projet](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>Les différences entre la date d’achèvement prévue d’une tâche et la date d’engagement de la tâche ou la date d’achèvement prévisionnelle de la tâche sont les suivantes :
>
>* La date de validation est la date à laquelle la personne affectée à la tâche estime manuellement qu’elle aura terminé la tâche. Pour plus d’informations, voir les articles suivants :
>
>   * [Vue d’ensemble de la date d’engagement](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interactions entre la date d’engagement et la date d’achèvement prévue](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md)
>
>* La date d’achèvement prévisionnelle est une date calculée par Workfront et prend en compte les retards de la tâche, la chronologie de la tâche ou des tâches antérieures, et d’autres facteurs pour déterminer une date réelle à laquelle la tâche peut être achevée de manière réaliste. Pour plus d’informations, voir [Vue d’ensemble de la date d’achèvement prévisionnelle pour les projets, les tâches et les problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Définir manuellement la date d’achèvement prévue d’une tâche

Vous devez disposer d’un accès en modification aux tâches et des autorisations de gestion sur la tâche pour pouvoir mettre à jour la date d’achèvement prévue de la tâche.

La définition de la date d’achèvement prévue d’une tâche dépend du type de contrainte que vous attribuez à la tâche.

Vous pouvez définir manuellement la date d’achèvement prévue dans les zones suivantes de Workfront :

* Dans la zone Modifier la tâche, lors de la création ou de la modification d’une tâche. Pour plus d’informations, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* Dans la zone Détails de la tâche. Pour plus d’informations, voir [Gérer les informations des tâches dans la zone Vue d’ensemble des détails de la tâche](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* Dans la zone Accueil , si la Date de fin planifiée s’affiche lors de l’affichage d’une tâche dans le panneau Résumé. Pour plus d’informations, voir [Mettre à jour ou modifier un élément de travail dans la zone d’accueil](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* Dans l’en-tête de la tâche. Pour plus d’informations, voir [Nouveaux en-têtes d’objets](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* Dans une liste de tâches ou un rapport, lorsque le champ Date d’achèvement prévue s’affiche dans la vue.

  Pour plus d’informations, voir [Modifier des tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

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
   <td> <p><span class="s1">La date de début prévue est ajustée pour que la durée reste inchangée.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dates fixes</p> </td> 
   <td> <p>La durée est ajustée pour que la date de début prévue reste inchangée.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Comment Workfront calcule automatiquement la date d’achèvement prévue pour une tâche

Lorsqu’elle est calculée automatiquement par le système, les éléments suivants peuvent influencer la date d’achèvement prévue d’une tâche :

* Contrainte de tâche

  Pour plus d’informations sur les contraintes de tâche, voir l’article [Vue d’ensemble des contraintes de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Relation des tâches antérieures

  Pour plus d’informations sur les tâches antérieures, voir l’article [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Date d’achèvement du projet, lorsque le projet est planifié à partir de la date d’achèvement.
* Le planning de désactivation du Principal cessionnaire de la tâche.

  Lorsque la personne cessionnaire principale prend des congés pendant la durée de la tâche, les dates prévues de la tâche sont ajustées en conséquence lorsque le paramètre **Prendre en compte les congés de l’utilisateur ou de l’utilisatrice dans la durée des tâches** est sélectionné pour le champ **Congés de l’utilisateur ou de l’utilisatrice**. Les nouveaux projets héritent de ce paramètre de la zone Préférences du projet, mais vous pouvez le modifier au niveau du projet.

  Par exemple, si une tâche avec une contrainte Aussi tôt que possible est planifiée pour commencer le 1er juin et se terminer le 3 juin, et que la personne cessionnaire principale a planifié un congé le 2 juin, la date d’achèvement prévue pour la tâche devient le 4 juin.

  Pour plus d’informations sur la préférence **Congés de l’utilisateur ou de l’utilisatrice**, voir les articles [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

* La durée associée aux paramètres d’approbation si la tâche est associée à une approbation. Pour plus d’informations, voir [Configurer les paramètres globaux d’approbation](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Lorsqu’elle est définie automatiquement, la date d’achèvement planifiée est déterminée selon le calcul suivant :

```
Planned Completion Date = Planned Start Date + Duration
```

Par exemple, si votre tâche a une date de début définie sur le 16 septembre et une durée de 10 jours, la date d’achèvement prévue est le 26 septembre.

>[!NOTE]
>
> Le type de mise à jour du projet doit être défini sur Automatique et Après changement ou Automatiquement pour que les heures et la durée planifiées soient automatiquement ajustées.\
>Pour plus d’informations sur le type de mise à jour, consultez l’article [Sélectionner le type de mise à jour du projet.](../../../manage-work/projects/manage-projects/select-project-update-type.md).
