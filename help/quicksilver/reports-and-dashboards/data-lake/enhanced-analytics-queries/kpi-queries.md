---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Requêtes relatives aux indicateurs de performance clés
description: Requêtes Analytics améliorées
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: eccecaece64b78aa19444407b182ea80b2115a63
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 73%

---


# Requêtes relatives aux indicateurs de performance clés

Vous pouvez utiliser les requêtes de cet article pour créer des visualisations de données similaires à celles d’Enhanced Analytics.

>[!IMPORTANT]
>
>Les requêtes produisent des résultats similaires à ceux affichés dans Enhanced Analytics, mais ils peuvent ne pas correspondre exactement.


## Conditions préalables

Avant de commencer, vous devez

1. Établissez une connexion avec votre outil Business Intelligence (BI) :
   1. [Créer un compte de lecteur ou une connexion pour Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Établir une connexion à Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

Une fois la connexion établie, vous pouvez utiliser les requêtes de cet article pour extraire et visualiser des données.

## Projets terminés

Le KPI « Projets terminés » indique le nombre de projets terminés sur une période filtrée, ainsi que l’augmentation ou la diminution du pourcentage depuis la période précédente. Vous trouverez ci-dessous le nombre de projets terminés au cours de la période précédente ainsi que le nombre de jours de la période précédente.

![ Projets d’indicateurs de performance clés terminés ](assets/kpi-projects-completed-350x182.png)

### Requête

```
WITH completedProjectsInRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
SELECT (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
SELECT  
CASE 
WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
a.PROJECT_COUNT, 
b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
c.CHANGE_FROM_PREVIOUS_PERIOD, 
d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d
```

## Projets terminés dans les délais

Le KPI « Projets terminés dans les délais » indique le pourcentage de projets terminés dans les délais au cours de la période filtrée, ainsi que l’augmentation ou la diminution du pourcentage depuis la période précédente. Vous trouverez ci-dessous le pourcentage de projets terminés dans les délais au cours de la période précédente, ainsi que le nombre de jours de la période précédente.

![Projets d’indicateurs de performance clés terminés dans les délais](assets/kpi-projects-completed-on-time-350x180.png)

## Durée moy. du projet

Le KPI « Durée moy.du projet » indique la durée moyenne d’achèvement des projets (en jours, semaines ou années) avec des dates de fin effectives au cours de la période filtrée, ainsi que l’augmentation ou la diminution du pourcentage depuis la période précédente. En dessous de ces chiffres, vous pouvez voir la durée moyenne d’achèvement des projets avec des dates de fin effectives dans la période précédente, ainsi que le nombre de jours dans la période précédente.

![Durée moyenne du projet basée sur les KPI](assets/kpi-avg.-project-duration-350x168.png)

## Nombre moyen de tâches par projet

Le KPI « Tâches moy. par projet » indique le nombre moyen de tâches affectées aux projets au cours de la période filtrée, ainsi que l’augmentation ou la diminution du pourcentage depuis la période précédente. Vous trouverez ci-dessous le nombre moyen de tâches affectées aux projets au cours de la période précédente, ainsi que le nombre de jours de la période précédente.

![KPI moyen des tâches par projet](assets/kpi-average-tasks-per-project-350x179.png)