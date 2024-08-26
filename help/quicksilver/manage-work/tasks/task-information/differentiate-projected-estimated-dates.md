---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Présentation des dates prévues et estimées
description: Il existe plusieurs types de dates qui indiquent la chronologie des tâches entre le moment où elles peuvent commencer et le moment où elles peuvent s’achever.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 90%

---

# Présentation des dates prévues et estimées

<!--Audited: 07/2024-->

Il existe plusieurs types de dates qui indiquent la chronologie des tâches entre le moment où elles peuvent commencer et le moment où elles peuvent s’achever. Voici quelques dates qui affichent la chronologie des tâches :

* Dates de début et d’achèvement prévues
* Dates de début et d’achèvement prévisionnelles
* Dates de début et d’achèvement estimées
* Dates de début et d’achèvement réelles

Cet article décrit les différences entre les dates estimées et les dates prévisionnelles pour les projets.

Lors de la création de la tâche, les dates prévues, prévisionnelles et estimées doivent normalement correspondre. Il existe quelques exceptions.

Pour plus d’informations sur les dates du projet, de la tâche et du problème dans Adobe Workfront, voir [Vue d’ensemble des dates du projet, de la tâche et du problème dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Vue d’ensemble des dates prévues

Les dates prévues sont les dates que la personne propriétaire du projet définit comme les dates de début et de fin des tâches. Vous (ou la personne propriétaire) pouvez modifier manuellement les dates prévues d’une tâche.

## Vue d’ensemble des dates effectives

Lorsqu’une tâche est créée, elle n’a pas de dates effectives, car elle n’a pas encore commencé ni terminé.

## Présentation des dates prévues et estimées

Au cours de la vie d’un projet, les dates prévisionnelles et estimées sont plus conformes à la réalité du projet, car elles prennent en compte ce qui peut influencer le début et la fin effectifs d’une tâche. Cela entraîne une modification des dates prévues.

Tenez compte des points suivants lorsque vous utilisez des dates prévisionnelles et estimées pour des tâches :

* Vous ne pouvez pas modifier manuellement les dates estimées ou prévisionnelles des tâches. Elles sont toutes les deux calculées par Adobe Workfront.
* Lorsque vous créez une tâche, les dates prévisionnelles et estimées doivent être identiques et illustrer les dates réelles auxquelles les tâches peuvent commencer ou se terminer.\
  Certaines mises à jour que vous apportez aux tâches affectent directement les valeurs des dates prévisionnelles et estimées.

  Par exemple, si l’utilisateur ou l’utilisatrice commence ou termine une tâche, celle-ci affiche les dates de début et d’achèvement effectives qui influencent les dates prévisionnelles et estimées de la tâche. De plus, si une personne cessionnaire sur la tâche modifie la date d’engagement, cette date influence la date prévisionnelle de la tâche.

## Différence entre les dates prévisionnelles et les dates estimées

La différence entre les dates prévisionnelles et les dates estimées est la suivante :

* Les dates prévisionnelles sont affectées par les mises à jour suivantes effectuées par l’utilisateur ou l’utilisatrice sur la tâche :

   * Ajouter une date de contrainte en ajoutant une contrainte de tâche fixe
   * Ajouter une date d’engagement

* Les dates estimées ne tiennent compte que de la progression réelle d’une tâche à un moment donné.

**Exemple :** si nous avons une tâche dont la date de début prévue est le 20 septembre et la date d’achèvement prévue est le 24 septembre, et qu’elle est soumise à la contrainte « Il Faut Finir Le », la date d’achèvement prévisionnelle est le 24 septembre. Cette tâche a une durée de 4 jours.

La date d’achèvement estimée est calculée sur la base de la progression actuelle du travail sur la tâche. Ainsi, si nous sommes le 23 septembre et que la tâche n’a pas encore commencé, la date d’achèvement estimée est le 27 septembre (elle devrait être terminée après 4 jours, en supposant que le travail soit commencé aujourd’hui).

Si la tâche est achevée à 50 % aujourd’hui, la date d’achèvement estimée est le 25 septembre (elle devrait être achevée après 2 jours, ce qui correspond à la moitié de la durée de la tâche).


### Comprendre quand les dates prévisionnelles sont mises à jour sur les tâches {#understand-when-projected-dates-update-on-tasks}

Les dates prévues peuvent correspondre à d’autres dates de tâche ou il s’agit d’un calcul effectué par Workfront qui prend en compte la progression réelle de la tâche.

La liste suivante présente plusieurs scénarios dans lesquels les dates prévisionnelles des tâches sont modifiées pendant la durée d’un projet en fonction de ce qui se passe dans la vie réelle de la tâche :

* Lorsqu’une tâche est marquée comme terminée :

  `Projected Dates = Estimated Dates = Actual Dates`

* Lorsqu’une tâche a une date de début effective :

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* Lorsqu’une tâche n’a pas de date de début effective, mais qu’il existe une contrainte forcée sur la date de début prévue (Doit commencer le) future :

  `Projected Start Date = Constraint Date`

  Pour plus d’informations sur la date de contrainte, voir [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Lorsqu’une tâche n’a pas de date de début effectif et que la tâche n’a pas de date de contrainte forcée :

  `Projected Start Date = the next available date in the future that falls within working schedule`

* Lorsque la personne cessionnaire met à jour la date d’engagement :

  `Projected Completion Date = Commit Date`

  Pour plus d’informations sur la date d’engagement, consultez [Vue d’ensemble de la date d’engagement](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Lorsque la tâche n’a pas de date d’engagement mise à jour et que la tâche a une contrainte forcée (Doit se terminer le) pour la date d’achèvement prévue qui est dans le futur :

  `Projected Completion Date = Constraint Date`

* Lorsqu’une tâche n’a pas de date d’engagement mise à jour, de date de contrainte forcée dans le futur, ou qu’elle a une date de contrainte dans le passé :

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### Comprendre quand les dates estimées sont mises à jour pour les tâches {#understand-when-the-estimated-dates-update-on-tasks}

Par rapport aux scénarios décrits ci-dessus pour les dates prévisionnelles, les dates estimées reflètent toujours l’analyse réelle de Workfront quant à la date de début ou de fin de la tâche, indépendamment des dates de contrainte ou d’engagement.

## Qu’est-ce qui influence la chronologie d’une tâche ?

Voici quelques exemples de ce qui peut influencer la chronologie réelle d’une tâche :

* Progression de la tâche par rapport aux dates prévues et à la date du jour
* Pourcentage terminé de la tâche jusqu’à présent
* Relation d’antériorité
* Progression de la tâche antérieure
* Affectation des utilisateurs et utilisatrices

  >[!NOTE]
  >
  >L’affectation des utilisateurs peut influencer la Date estimée d’achèvement d’une tâche si elle affecte la vitesse à laquelle la tâche peut être terminée. Par exemple, si le type de durée de la tâche est Piloté par l’effort, vous pouvez accélérer l’achèvement de la tâche en ajoutant des personnes cessionnaires. La date d’achèvement estimée change en conséquence.
