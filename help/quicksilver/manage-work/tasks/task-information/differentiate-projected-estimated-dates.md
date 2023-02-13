---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Différence entre les dates prévues et estimées
description: Il existe plusieurs types de dates qui indiquent la chronologie des tâches entre le moment où elles peuvent démarrer et celui où elles peuvent se terminer.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# Différence entre les dates prévues et estimées

Il existe plusieurs types de dates qui indiquent la chronologie des tâches entre le moment où elles peuvent démarrer et celui où elles peuvent se terminer. 

Voici quelques dates qui affichent la chronologie des tâches :

* Dates de début et de fin planifiées
* Dates de début et de fin prévues
* Dates de début estimées et dates d’échéance estimées
* Dates de début et d’achèvement réelles

Cet article décrit les différences entre les dates estimées et projections pour les projets. Lorsque la tâche est créée pour la première fois, les dates prévues, prévues et estimées doivent généralement correspondre. Certaines exceptions existent. 

Pour plus d’informations sur le projet, la tâche et les dates de publication dans Adobe Workfront, voir [Présentation des dates de projet, de tâche et de publication dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Présentation des dates prévues

Les dates planifiées sont les dates que le propriétaire du projet définit comme les dates de début et de fin des tâches. 

Vous ou le propriétaire du projet pouvez modifier manuellement les dates planifiées d’une tâche.

## Présentation des dates réelles

Lorsqu’une tâche est créée pour la première fois, elle n’a pas de Dates réelles, car elle n’a pas encore commencé ni terminée.

## Présentation des dates prévues et estimées

Pendant la durée d’un projet, les dates prévues et estimées sont plus en phase avec la réalité du projet, car elles prennent en compte ce qui peut influencer le début et la fin d’une tâche. Cela les entraîne à changer par rapport aux dates prévues.

Tenez compte des points suivants lorsque vous utilisez des dates estimées et prévues pour les tâches :

* Vous ne pouvez pas modifier manuellement les Dates estimées ou projections des tâches. Elles sont toutes deux calculées par Adobe Workfront.
* Lorsque vous créez une tâche, les dates Prévue et Estimée doivent être identiques et elles doivent illustrer les temps réels pendant lesquels les tâches peuvent démarrer ou se terminer.\
   Certaines mises à jour apportées aux tâches affectent directement les valeurs des dates prévues et estimées. 

   Par exemple, si l’utilisateur démarre ou termine une tâche, la tâche affiche les dates de début et de fin réelles qui influencent les dates prévues et estimées de la tâche. En outre, si une personne désignée sur la tâche modifie la date de validation, cette date influence la date de projection de la tâche.

## Différence entre les dates prévues et estimées

La différence entre les dates prévues et estimées est la suivante :

* Les dates prévues sont affectées par un utilisateur qui effectue les mises à jour suivantes sur la tâche :

   * Ajout d’une date de contrainte en ajoutant une contrainte de tâche fixe
   * Ajout d’une date de validation

* Les dates estimées ne prennent en compte que la progression réelle d’une tâche à un moment donné.

**Exemple :** Si nous avons une tâche dont la date de début prévue est le 20 septembre et la date de fin prévue est le 24 septembre et qui doit se terminer sous contrainte, la date de fin prévue est le 24 septembre. Cette tâche a une durée de 4 jours.

La Date d’achèvement estimée est calculée en fonction de la progression actuelle du travail sur la tâche. Ainsi, si nous sommes aujourd’hui le 23 septembre et que la tâche n’a pas encore commencé, la date d’achèvement estimée est le 27 septembre (elle doit être terminée au bout de 4 jours, en supposant que le travail ait commencé aujourd’hui).

Si la tâche est terminée à 50 % aujourd’hui, la date d’achèvement estimée est le 25 septembre (elle doit être terminée au bout de 2 jours, soit la moitié de la durée de la tâche).

* [Comprendre quand les dates prévues mettent à jour les tâches](#understand-when-projected-dates-update-on-tasks)
* [Comprendre quand les dates estimées sont mises à jour pour les tâches](#understand-when-the-estimated-dates-update-on-tasks)

### Comprendre quand les dates prévues mettent à jour les tâches {#understand-when-projected-dates-update-on-tasks}

Les dates prévues peuvent correspondre à d’autres dates de tâche ou il s’agit d’un calcul effectué par Workfront qui prend en compte la progression réelle de la tâche.

La liste suivante répertorie plusieurs scénarios lorsque les dates prévues des tâches sont modifiées au cours de la vie d’un projet, selon ce qui se passe dans la vie réelle de la tâche :

* Lorsqu’une tâche est marquée comme terminée :

   *Dates prévues = Dates estimées = Dates réelles*

* Lorsqu’une tâche possède une Date de début réelle :

   *Date de début prévue = Date de début estimée = Date de début réelle*

* Lorsqu’une tâche ne comporte pas de date de début réelle, mais qu’une contrainte est imposée sur la date de début planifiée (qui doit être activée) qui se présente à l’avenir :

   *Date de début prévue = Date de contrainte*

   Pour plus d’informations sur la date de contrainte, voir [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Lorsqu’une tâche n’a pas de Date de début réelle et que la tâche n’a pas de date de contrainte forcée :

   *Date de début prévue = la prochaine date disponible dans le futur conforme au planning de travail*

* Lorsque la personne désignée met à jour la date de validation :

   *Date d’achèvement prévue = Date de validation*

   Pour plus d’informations sur la date de validation, voir [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Lorsque la date de validation de la tâche n’est pas mise à jour et que celle-ci est contrainte (à terminer le) pour la date d’achèvement planifiée qui se situe dans le futur :

   *Date d’achèvement prévue = date de contrainte*

* Lorsqu’une tâche ne dispose pas d’une date de validation mise à jour, d’une date de contrainte forcée à l’avenir ou qu’elle dispose d’une date de contrainte antérieure :

   *Date d’achèvement prévue = calcul système de la date d’achèvement en fonction de la progression actuelle et du travail à effectuer.*

### Comprendre quand les dates estimées sont mises à jour pour les tâches {#understand-when-the-estimated-dates-update-on-tasks}

En comparaison avec les scénarios décrits ci-dessus pour les dates prévues, les dates estimées reflètent toujours l’analyse réelle par Workfront du moment où la tâche va commencer ou se terminer, indépendamment des dates de contrainte ou de validation.

## Ce qui influence la chronologie d’une tâche

Voici quelques exemples de ce qui peut influencer la chronologie réelle d’une tâche : 

* progression de la tâche par rapport aux dates prévues et au jour en cours
* pourcentage d’achèvement de la tâche jusqu’à présent
* relation précédente
* état précédent
* affectation des utilisateurs

   >[!NOTE]
   >
   >L’affectation des utilisateurs peut influencer la Date estimée d’achèvement d’une tâche si elle affecte la vitesse à laquelle la tâche peut être terminée. Par exemple, si le type de durée de la tâche est piloté par l’effort, vous pouvez terminer la tâche plus tôt en ajoutant des personnes désignées. Par conséquent, la date d’achèvement estimée change.
