---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcul du coût du travail planifié
description: Lorsque vous planifiez le travail sur vos projets, Adobe Workfront calcule le coût de main-d’oeuvre planifié pour les rôles et les utilisateurs affectés à ce travail en fonction de leurs valeurs Coût par heure.
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Calcul du coût du travail planifié

Lorsque vous planifiez le travail sur vos projets, Adobe Workfront calcule le coût de main-d’oeuvre planifié pour les rôles et les utilisateurs affectés à ce travail en fonction de leurs valeurs Coût par heure.

Le coût du travail planifié d’un projet est un calcul entre le coût associé aux rôles de travail ou les utilisateurs affectés pour terminer le travail sur le projet et le nombre d’heures planifiées (heures planifiées) qui peuvent nécessiter chaque rôle ou utilisateur pour terminer ce travail.

## Présentation du coût du travail planifié

Le **Coût du travail planifié** La partie d’un projet est calculée en ajoutant tous les coûts de main-d’oeuvre planifiés de toutes les tâches du projet.

>[!TIP]
>
>Aucun coût de main-d’oeuvre planifié n’est associé aux problèmes ou au projet lui-même.

Workfront calcule le coût du travail planifié d’un projet à l’aide de la formule suivante :

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

Le coût du travail planifié de la tâche est calculé en fonction des éléments suivants :

* Le nombre de ressources de la tâche et leur allocation individuelle à la tâche
* Type de coût de la tâche.

Le coût de la main-d’oeuvre planifiée de la tâche est calculé à l’aide de la formule suivante :

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Pour plus d’informations sur la façon dont Workfront calcule le coût de main-d’oeuvre planifié pour les tâches, en fonction de l’affectation des tâches et du type de coût, voir la section &quot;Modifier les types de coûts pour les tâches individuelles&quot; de l’article. [Suivi des coûts](../../../manage-work/projects/project-finances/track-costs.md).

## Localisation du coût du travail planifié

Vous pouvez localiser le coût du travail planifié d’un projet dans les zones suivantes de Workfront :

* Rapport Projet
* Liste des projets
* Rapport de ligne de base dans lequel vous pouvez effectuer un suivi dans le temps.
* Via l’API

Pour plus d’informations sur la création de rapports et l’utilisation de l’API Workfront, reportez-vous aux articles suivants :

* [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Bases d’API](../../../wf-api/general/api-basics.md)
