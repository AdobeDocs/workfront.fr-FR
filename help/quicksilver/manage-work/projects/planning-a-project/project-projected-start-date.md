---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la Date de début prévisionnelle du projet
description: La date de début prévisionnelle est une date en temps réel du début du projet, basée sur la date de début prévisionnelle de la première tâche du projet.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 96%

---

# Vue d’ensemble de la Date de début prévisionnelle du projet

## Vue d’ensemble de la date de début prévisionnelle pour les projets et les tâches

La date de début prévisionnelle est une date en temps réel du début du projet, basée sur la date de début prévisionnelle de la première tâche du projet.

Lorsque vous planifiez un projet pour la première fois, la Date de début prévue et la Date de début prévisionnelle des tâches et du projet sont identiques. Comme des retards peuvent se produire ou que des tâches peuvent être terminées plus tôt, la Date de début prévisionnelle peut devenir différente de la Date de début prévue.

Les modifications apportées à la Date de début prévisionnelle de la première tâche du projet déclenchent des modifications de la Date de début prévisionnelle du projet.

## Modifier la Date de début prévisionnelle d’une tâche

La Date de début prévisionnelle d’un projet ou d’une tâche est un calcul effectué par Adobe Workfront et ne peut pas être modifiée manuellement.

Les événements suivants peuvent déclencher une modification dans la Date de début prévisionnelle d’une tâche :

* Lorsque vous commencez à travailler sur une tâche, la Date de début effective de la tâche devient sa Date de début prévisionnelle.
* Si la Date de début prévue d’une tâche est dépassée, la Date de début prévisionnelle est déplacée dans le futur et indique la date la plus proche disponible pour que la tâche démarre.\
  Workfront prend en compte le nombre d’heures prévues de la tâche, ainsi que le planning du projet ou de la personne affectée à la tâche lors du calcul de la date la plus proche possible pour que la tâche démarre.
* Les tâches antérieures en cours d’exécution ont un impact sur la date de début prévisionnelle de leurs tâches dépendantes. La Date de début prévisionnelle des tâches dépendantes se déplace selon le Type de dépendance de la relation d’antériorité et selon les Dates prévisionnelles des tâches antérieures.

Si l’une de ces tâches est la première tâche d’un projet, la Date de début prévisionnelle du projet change pour correspondre à la Date de début prévisionnelle de cette tâche.

## Localiser la date de début prévisionnelle d’un projet ou d’une tâche

Vous pouvez localiser la date de début prévisonnelle d’un projet ou d’une tâche dans les zones suivantes de Workfront :

* Vous pouvez l’ajouter à un projet ou à un rapport ou à une vue de tâche.

  Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Dans la section Détails du projet d’un projet ou la section Détails de la tâche d’une tâche.
