---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Requêtes sur l’arborescence de projets
description: Requêtes relatives à l’analytique améliorée
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 3943703a-0d0b-46d3-a708-52987d330523
TQID: 'https://experienceleague.adobe.com/tukTMDDsdNPEaS5mPafVJ0ajIVQFQ7sLs9xBQ04uQ2w'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 21%
---
# Requêtes sur l’arborescence de projets

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

## Heures planifiées des projets retirées

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Heures planifiées des projets retirées : avancement

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

## Durée prévue des projets retirés 

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Durée prévue des projets retirés : avancement

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```
