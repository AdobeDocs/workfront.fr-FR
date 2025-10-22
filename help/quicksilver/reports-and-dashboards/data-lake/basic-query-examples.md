---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exemples de requêtes Data Connect
description: Exemples de requêtes que vous pouvez utiliser pour vous familiariser avec la syntaxe et la structure de types de requêtes spécifiques.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Exemples de requête Workfront Data Connect

Pour vous aider à mieux utiliser vos données Workfront Data Connect, cette page contient des exemples de requêtes de base que vous pouvez utiliser pour vous familiariser avec la syntaxe et la structure de types de requêtes spécifiques.

## Requête de données personnalisées

Cet exemple montre comment composer une requête pour renvoyer vos données personnalisées dans Workfront, telles que les formulaires personnalisés et les champs personnalisés.

### Scénario

Votre entreprise utilise un formulaire personnalisé nommé Finance Integration. Le formulaire est joint à chaque projet et contient les champs suivants :

* **Unité opérationnelle** : champ personnalisé contenant une chaîne.
* **ProjectID** : champ personnalisé contenant une chaîne numérique.
* **Nom du projet développé** : champ de données personnalisé calculé qui concatène les valeurs de l’entité professionnelle, de l’ID de projet et du nom du projet Workfront natif en une seule chaîne.

Vous devez inclure ces informations dans la réponse à une requête sur Data Connect. Les valeurs de données personnalisées d’un enregistrement du lac de données se trouvent dans une colonne intitulée `parametervalues`. Cette colonne est stockée en tant qu’objet JSON.

### Requête

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Réponse

La requête ci-dessus renvoie les données suivantes :

* `projectid` : ID de projet Workfront natif.
* `parametervalues` : colonne stockant un objet JSON.
* `name` : nom du projet Workfront natif.
* `Business Unit` : valeur de données personnalisée incluse dans l’objet `parametervalues`.
* `Project ID` : valeur de données personnalisée incluse dans l’objet `parametervalues`.
* `Expanded Project Name` : valeur de données personnalisée incluse dans l’objet `parametervalues`.

### Explication

Lors de l’interrogation de l’objet JSON `parametervalues`, chaque champ de données personnalisé est accessible sous la forme d’une colonne à l’aide des éléments suivants :

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` est le nom de l’objet JSON dans la table interrogée. Dans le cas de données personnalisées, cela sera toujours `parametervalues`.
* `<parameter_name>` est la chaîne `parametername` qui se trouve dans l’outil de configuration de formulaire, bien qu’elle ne corresponde pas toujours à cette valeur.

>[!NOTE]
>
>Si le nom du paramètre est modifié dans l’outil de configuration des formulaires Workfront, il est représenté sous la forme d’une nouvelle colonne dans l’objet JSON. Par conséquent, nous vous recommandons de ne pas modifier le nom d’une colonne une fois qu’elle a été créée dans l’outil de configuration de formulaire. Cependant, le libellé peut être modifié sans affecter l’objet JSON.
>
>Si la chaîne de texte du nom du paramètre est incorrecte, la colonne renvoie une valeur NULL plutôt qu’une erreur.

* `<data_type>` convertit la valeur renvoyée par l’objet JSON en un type de données approprié pour le champ. Le choix d’un type de données incompatible pour la valeur renvoyée entraîne une erreur de correspondance de type de données. Les types de données possibles sont les suivants :

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (par exemple, `Number(32,4)` renvoie 1 234,0987)
   * `date`
   * `timestamp`

* `<column_name>` est le libellé que vous créez pour chaque colonne de données personnalisée.

>[!NOTE]
>
>Seuls les paramètres auxquels des valeurs sont affectées dans le formulaire seront inclus dans l’objet JSON. Si un champ de données personnalisé est vide dans le formulaire, il n’apparaît pas.

## Durée dans la requête de statut

Cet exemple montre comment mesurer le temps passé par un projet dans des statuts précédemment attribués. Il peut être facilement adapté pour mesurer le temps passé sur une tâche ou un événement dans un statut, ou il peut être adapté pour mesurer la durée pendant laquelle un autre attribut (y compris des valeurs de données personnalisées) a été appliqué à un objet.

### Scénario

La direction de votre entreprise estime que vous passez trop de temps à chaque étape de votre cycle de vie professionnelle. Avant de faire des recommandations pour améliorer le processus, vous souhaitez créer une mesure de référence de la fréquence à laquelle le statut d&#39;un projet change au fil du temps et du nombre de jours qu&#39;un projet reste dans un statut donné.

Vous allez utiliser la vue de données PROJECTS_EVENT pour extraire une liste de chaque changement de statut par rapport à l&#39;objet du projet. Vous allez comparer le nouveau statut au statut précédent, saisir la période effective pour le statut précédemment attribué, puis calculer les jours passés dans ce statut.

Grâce à cette sortie brute de temps passé dans chaque statut par projet, vous pouvez commencer à créer des visualisations ou agréger les données pour créer des moyennes de durée de statut par statut, type de projet ou période de l’année. Cette ligne de base est ensuite utilisée pour établir un point de référence par rapport auquel vous pouvez effectuer des mesures afin de répondre aux attentes de votre direction.

La requête suivante utilise la vue de données PROJECTS_EVENTS de Data Connect pour comparer chaque événement de changement de statut de projet et afficher l’heure dans le statut.

### Requête

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### Réponse

La requête ci-dessus renvoie les données suivantes :

* `PROJECTID` : ID de projet Workfront associé à l’événement de changement de statut.
* `PROJECT_NAME` : nom du projet Workfront.
* `PREVIOUS_STATUS` : statut du projet immédiatement avant la modification.
* `STATUS` : statut du projet après la modification.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP` : la date et l’heure de l’événement de modification lorsque le statut précédent a été défini.
* `STATUS_END_EFFECTIVE_TIMESTAMP` : la date et l’heure de l’événement de modification lorsque la valeur de statut mise à jour a été définie.
* `STATUS_DURATION_DAYS` : différence (en jours) entre l’horodatage de fin effective et l’horodatage de début effective.

### Explication

La requête utilise les fonctionnalités de suivi des événements de modification de Data Connect.  Il détermine la date de déclenchement d’un événement dont la nouvelle valeur de statut était différente de celle de l’événement précédent. 

Examiner la requête de l’intérieur vers l’extérieur : 

1. Calculer les enregistrements dont le statut précédent est différent : 
   * Pour chaque événement de modification, utilisez la fonction lag() pour identifier la valeur précédente de status. 

2. Filtrez uniquement les enregistrements qui ont été modifiés : 

   * Sélectionnez les enregistrements du calcul de l’étape 1 où le statut précédent != statut actuel. 

3. Calculer la date et l’heure effectives de début et de fin en jours : 

   * `<status_begin_effective_timestamp>` : calculé à l’étape 2. 

   * `<status_end_effective_timestamp>` : calculé en fonction du suivant (lead()). `<status_begin_effective_timestamp>` : n&#39;afficher le statut que si `<status_begin_effective_timestamp>` n&#39;est PAS NULL. 
   * `<status_duration_days>` : différence de données entre `<status_begin_effective_timestamp>` et `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Il est recommandé d&#39;utiliser cette requête comme sa propre « Vue » dans PowerBI ou Tableau.  Si vous souhaitez importer d’autres champs du `<object>_event view`, rejoignez la sortie de cette requête sur le `<object>_event view` .  Les champs de jointure seraient les suivants : <br>
>>Pour projects_event : 
>>`From projects_event p`
>>`Join <above query> c on c.projectid = p.projectid  `
>>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
