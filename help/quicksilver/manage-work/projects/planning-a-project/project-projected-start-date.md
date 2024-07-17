---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la date de début prévisionnelle du projet
description: La date de début prévue est une date en temps réel du début du projet, basée sur la date de début prévue de la première tâche sur le projet.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 3%

---

# Vue d’ensemble de la date de début prévisionnelle du projet

## Présentation de la date de début prévue pour les projets et les tâches

La date de début prévue est une date en temps réel du début du projet, basée sur la date de début prévue de la première tâche sur le projet. 

Lorsque vous planifiez un projet pour la première fois, la Date de début planifiée et la Date de début prévue des tâches et du projet sont identiques. Comme des retards peuvent se produire ou que des tâches peuvent être terminées plus tôt, la Date de début prévue peut devenir différente de la Date de début planifiée. 

Les modifications apportées à la Date de début prévue de la première tâche sur le projet déclenchent des modifications à la Date de début prévue du projet. 

## Modification de la date de début prévue d’une tâche

La Date de début prévue d’un projet ou d’une tâche est un calcul effectué par Adobe Workfront et ne peut pas être modifiée manuellement. 

Les événements suivants peuvent déclencher une modification dans la Date de début prévue d’une tâche :

* Lorsque vous commencez à travailler sur une tâche, la Date de début réelle de la tâche devient sa Date de début prévue.
* Si la Date de début planifiée d’une tâche est transmise, la Date de début prévue se déplace dans le futur, indiquant la date la plus proche disponible pour que la tâche démarre.\
  Workfront prend en compte le nombre d’heures planifiées de la tâche, ainsi que le planning du projet ou de l’utilisateur affecté à la tâche lors du calcul de la date la plus proche possible pour que la tâche démarre. 
* Les tâches précédentes en cours d’exécution ont un impact sur la date de début prévue de leurs tâches dépendantes. La Date de début prévue des tâches dépendantes se déplace selon le Type de dépendance de la relation précédente et selon les Dates prévues des prédécesseurs. 

Si l’une de ces tâches est la première tâche d’un projet, la Date de début prévue du projet change pour correspondre à la Date de début prévue de cette tâche. 

## Localisation de la date de début prévue d’un projet ou d’une tâche

Vous pouvez localiser la date de début prévue d’un projet ou d’une tâche dans les zones suivantes de Workfront :

* Vous pouvez l’ajouter à un projet ou à un rapport ou à une vue de tâche.

  Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Dans la section Détails du projet d’un projet ou la section Détails de la tâche d’une tâche.
