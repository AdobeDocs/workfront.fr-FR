---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Requêtes d'activité par équipe
description: Requêtes Analytics améliorées
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 6f07e52b-b813-4b3a-9333-0c9300e051ca
source-git-commit: da5c7197b3826855bae5dd3d3bf2ba9d07d7f188
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 3%

---

# Requêtes d&#39;activité par équipe

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

## Événements de connexion des utilisateurs des équipes locales 

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM users_current uc 
    INNER JOIN userlogins ul ON uc.userid = ul.userid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, TO_DATE(ul.lastlogindate) 
```

### Événements de connexion des utilisateurs des équipes locales : analyse en profondeur

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM users_current uc 
    INNER JOIN userlogins ul ON uc.userid = ul.userid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(ul.lastlogindate)
```

## Événements de connexion des utilisateurs des équipes

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    tmc.teamid, 
    TO_DATE(ul.lastlogindate), 
    count(*) 
FROM teammembers_current tmc 
    inner join teams_current tc on tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    inner join userlogins ul on tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(ul.lastlogindate)
```

### Événements de connexion des utilisateurs des équipes : analyse en profondeur

```
WITH userlogins as ( 
    SELECT userid, lastlogindate 
    FROM ( 
        SELECT userid, lastlogindate, lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid  ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT tmc.teamid, tmc.userid, TO_DATE(ul.lastlogindate), count(*) 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN userlogins ul ON tmc.userid = ul.userid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, tmc.userid, TO_DATE(ul.lastlogindate)
```



## Événements de changement de statut de la tâche des utilisateurs des équipes internes 

```
WITH task_status_changes as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    ) 
    WHERE status != previous_status 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid 
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid,  TO_DATE(tsc.begin_effective_timestamp)
```

### Événements de changement de statut de la tâche des utilisateurs des équipes internes : analyser en profondeur

```
WITH task_status_changes as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    ) 
    WHERE status != previous_status 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid 
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid 
WHERE hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(tsc.begin_effective_timestamp)
```

## Événements de changement de statut de la tâche des utilisateurs des équipes

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
    WHERE status != previous_status  
) 

SELECT tmc.teamid,  TO_DATE(tsc.begin_effective_timestamp), count(tsc.taskid) as task_status_updates  
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN task_status_changes tsc ON ac.taskid = tsc.taskid  
WHERE tmc.teamid is not null  
GROUP BY tmc.teamid,  TO_DATE(tsc.begin_effective_timestamp) 
```

### Événements de changement de statut de la tâche des utilisateurs des équipes : analyse en profondeur

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
WHERE status != previous_status  
) 
 
SELECT 
    tmc.teamid, 
    tmc.userid, 
    TO_DATE(tsc.begin_effective_timestamp), 
    count(tsc.taskid) as task_status_updates  
FROM teammembers_current tmc 
    inner join teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    inner join assignments_current ac ON tmc.userid = ac.assignedtoid  
    inner join task_status_changes tsc ON ac.taskid = tsc.taskid  
WHERE tmc.teamid is not null  
GROUP BY tmc.teamid, tmc.userid, TO_DATE(tsc.begin_effective_timestamp) 
```

## Événements d’achèvement de tâche des utilisateurs de l’équipe interne

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    uc.hometeamid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE uc.hometeamid is not null 
GROUP BY uc.hometeamid, TO_DATE(tasks_done.task_completion_date)
```

### Événements d’achèvement de tâche des utilisateurs des équipes locales : analyse en profondeur

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    uc.hometeamid, 
    uc.userid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM users_current uc 
    INNER JOIN assignments_current ac ON uc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        ) 
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE uc.hometeamid is not null 
GROUP BY uc.hometeamid, uc.userid, TO_DATE(tasks_done.task_completion_date) 
```

## Événements d’achèvement de tâche des utilisateurs des équipes

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT 
        taskid, 
        actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    tmc.teamid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid and tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, TO_DATE(tasks_done.task_completion_date) 
```

### Événements d’achèvement de tâche des utilisateurs et utilisatrices des équipes : analyse en profondeur

```
WITH task_status_done as ( 
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event te 
        WHERE status = 'CPL' 
    ) 
    WHERE status != previous_status 
), task_percentage_done as ( 
    SELECT 
        taskid, 
        percentcomplete, 
        begin_effective_timestamp 
    FROM ( 
        SELECT 
            taskid, 
            percentcomplete, 
            begin_effective_timestamp, 
            lag(percentcomplete, 1, '0') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_percent_complete 
        FROM tasks_event 
        WHERE TO_NUMBER(percentcomplete) = 100 
    ) 
    WHERE percentcomplete != previous_percent_complete 
), task_completion_date_exists as ( 
    SELECT taskid, actualcompletiondate 
    FROM tasks_event 
    WHERE actualcompletiondate is not null 
) 
 
SELECT 
    tmc.teamid, 
    tmc.userid, 
    TO_DATE(tasks_done.task_completion_date), 
    count(tasks_done.taskid) as task_completed 
FROM teammembers_current tmc 
    INNER JOIN teams_current tc ON tc.teamid = tmc.teamid AND tc.teamtype != 'PROJECT' 
    INNER JOIN assignments_current ac ON tmc.userid = ac.assignedtoid  
    INNER JOIN ( 
        SELECT distinct taskid, task_completion_date 
        FROM ( 
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_status_done 
            UNION  
            SELECT taskid, TO_DATE(begin_effective_timestamp) as task_completion_date 
            FROM task_percentage_done 
            UNION 
            SELECT taskid, TO_DATE(actualcompletiondate) as task_completion_date 
            FROM task_completion_date_exists 
        )  
    ) tasks_done ON ac.taskid = tasks_done.taskid 
WHERE tmc.teamid is not null 
GROUP BY tmc.teamid, tmc.userid, TO_DATE(tasks_done.task_completion_date) 
```
