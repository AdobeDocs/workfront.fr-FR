---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer le coût prévu de main-d’œuvre
description: Lorsque vous planifiez le travail sur vos projets, Adobe Workfront calcule le coût prévu de main-d’œuvre pour les fonctions et les utilisateurs et utilisatrices affectés à ce travail en fonction de leurs valeurs Coûts par heure.
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 100%

---

# Calculer le coût prévu de main-d’œuvre

Lorsque vous planifiez le travail sur vos projets, Adobe Workfront calcule le coût prévu de main-d’œuvre pour les fonctions et les utilisateurs et utilisatrices affectés à ce travail en fonction de leurs valeurs Coûts par heure.

Le coût prévu de main d’œuvre d’un projet résulte du calcul entre le coût associé aux fonctions ou aux utilisateurs et utilisatrices affectés pour terminer le travail sur le projet et la quantité d’heures prévues (Nombre d’heures prévues) dont chaque fonction ou utilisateur ou utilisatrice pourrait avoir besoin pour terminer ce travail.

## Vue d’ensemble du coût prévu de main d’œuvre

Le **Coût prévu de main d’œuvre** d’un projet est calculé en ajoutant tous les coûts prévus de main-d’œuvre de toutes les tâches du projet.

>[!TIP]
>
>Aucun coût prévu de main-d’œuvre n’est associé aux problèmes ou au projet lui-même.

Workfront calcule le coût prévu de main d’œuvre d’un projet à l’aide de la formule suivante :

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

Le coût prévu de main-d’œuvre de la tâche est calculé en fonction des éléments suivants :

* Nombre de ressources de la tâche et leur affectation individuelle à la tâche.
* Type de coût de la tâche.

Le coût prévu de main-d’œuvre de la tâche est calculé à l’aide de la formule suivante :

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Pour plus d’informations sur la façon dont Workfront calcule le coût prévu de main-d’œuvre pour les tâches, en fonction des affectations de tâches et du type de coût, voir la section « Modifier les types de coûts pour les tâches individuelles » de l’article [Suivi des coûts](../../../manage-work/projects/project-finances/track-costs.md).

## Localiser le coût prévu de main d’œuvre

Vous pouvez localiser le coût prévu de main d’œuvre d’un projet dans les zones suivantes de Workfront :

* Rapport du projet.
* Liste de projets.
* Rapport de niveau de référence dans lequel vous pouvez effectuer un suivi dans le temps.
* Via l’API.

Pour plus d’informations sur la création de rapports et l’utilisation de l’API Workfront, reportez-vous aux articles suivants :

* [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [Bases d’API](../../../wf-api/general/api-basics.md)
