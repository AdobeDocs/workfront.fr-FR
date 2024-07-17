---
product-area: projects
navigation-topic: issue-information
title: Vue d’ensemble de la date d’achèvement prévue du problème
description: La date d’achèvement prévue d’une publication est la date à laquelle le problème doit se terminer.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 2%

---

# Vue d’ensemble de la date d’achèvement prévue du problème

La date d’achèvement prévue d’une publication est la date à laquelle le problème doit se terminer.

Vous pouvez indiquer la date d’achèvement prévue d’une publication ou laisser Adobe Workfront en charge de son calcul selon certains critères. 

Les dates d’achèvement prévues des problèmes n’ont aucune incidence sur la date d’achèvement prévue du projet. Seules les dates d’achèvement prévues des tâches affectent la date d’achèvement prévue du projet. Pour plus d’informations sur la date d’achèvement prévue du projet, voir [Définition de la date d’achèvement prévu du projet](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>La date d’achèvement prévue d’une publication diffère de la date de validation de la publication ou de la date d’achèvement prévue de la publication de la manière suivante :
>
>* La date de validation est la date à laquelle la personne affectée au problème estime manuellement qu’elle aura terminé le problème. Pour plus d’informations, voir les articles suivants :
>
>   * [Vue d’ensemble des dates d’engagement](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [Interactions entre la date de validation et la date d’achèvement planifiée](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* La date d’achèvement prévue est une date calculée par Workfront qui prend en compte des facteurs externes pour déterminer une date de réalisation réelle du problème. Pour plus d’informations, voir [Présentation de la date d’achèvement prévue pour les projets, les tâches et les problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Définition manuelle de la date d’achèvement planifiée d’un problème

Pour pouvoir mettre à jour la date d’achèvement prévue du problème, vous devez disposer de l’accès Modifier aux problèmes et des autorisations Gérer sur le problème.

Vous pouvez définir manuellement la date d’achèvement planifiée d’un problème dans les zones suivantes de Workfront :

* Dans la zone Modifier le problème ou dans la zone Détails du problème lors de la création ou de la modification d’un problème. Pour plus d’informations, voir [Modification des problèmes](../../../manage-work/issues/manage-issues/edit-issues.md).
* Dans la zone Accueil , si la date de fin planifiée s’affiche lors de l’affichage d’un problème. Pour plus d’informations, voir [Mise à jour ou modification d’un élément de travail dans la zone d’accueil](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* Dans l’en-tête du problème. Pour plus d’informations, voir [Nouveaux en-têtes d’objet](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* Dans une liste de problèmes ou un rapport lorsque le champ Date d’achèvement planifiée s’affiche dans la vue.

  Pour plus d’informations, voir [Modification des problèmes dans une liste](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Comment Workfront calcule automatiquement la date d’achèvement planifiée d’un problème

Lorsque Workfront calcule automatiquement la date d’achèvement planifiée d’un problème, les éléments suivants peuvent influer sur la date :

* Date de début planifiée

  La Date d’entrée et la Date de début planifiée doivent correspondre pour un problème lors de la première création du problème.

* Durée par défaut telle que configurée dans la section Détails de la file d’attente du projet. Pour plus d’informations, voir [Création d’une file d’attente de requêtes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

  Si la durée par défaut est de 0 jour, la date de fin planifiée correspond à la date de début planifiée de l’émission.

* Planification du projet

Lorsqu’elle est définie automatiquement, la date d’achèvement planifiée est déterminée selon le calcul suivant : 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Exemple :** Par exemple, si votre tâche a une date de début du vendredi 14 janvier et que la durée par défaut est de 5 jours, la date d’achèvement planifiée est le vendredi 21 janvier, si la planification du projet est du lundi au vendredi pour 8 heures par jour.

Les situations suivantes se présentent :

* Si le projet ne comporte pas de planification, la planification par défaut de votre système Workfront est prise en compte. Pour plus d’informations, voir [Aperçu des planifications](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Si la planification est du lundi au vendredi de 9 h à 13 h (4 heures par jour) et que le nombre d’heures par jour de travail standard de votre système Workfront est de 8 heures, la date d’achèvement planifiée est le 27 janvier.

>[!TIP]
>
>Workfront prend en compte les exceptions aux planifications comme les jours fériés et les week-ends lors du calcul des dates d’achèvement planifiées.

 
