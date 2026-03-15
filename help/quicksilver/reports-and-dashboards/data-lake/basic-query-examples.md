---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exemples de requête Data Connect
description: Exemples de requêtes permettant de se familiariser avec la syntaxe et la structure de types de requêtes spécifiques.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 1%

---

# Exemples de requête Workfront Data Connect

Pour vous aider à mieux utiliser vos données Workfront Data Connect, cette page contient des exemples de requêtes de base que vous pouvez utiliser pour vous familiariser avec la syntaxe et la structure de types de requêtes spécifiques.

## Requête de données personnalisée

Cet exemple montre comment créer une requête pour renvoyer vos données personnalisées dans Workfront, telles que des formulaires personnalisés et des champs personnalisés.

### Scénario

Votre organisation utilise un formulaire personnalisé appelé Intégration financière. Le formulaire est joint à chaque projet et contient les champs suivants :

* **Entité** : champ personnalisé qui contient une chaîne.
* **ProjectID** : champ personnalisé contenant une chaîne numérique.
* **Nom du projet développé** : champ de données personnalisé calculé qui concatène les valeurs Business Unit, ProjectID et le nom du projet Workfront natif dans une seule chaîne.

Vous devez inclure ces informations dans la réponse d&#39;une requête sur Data Connect. Les valeurs de données personnalisées d&#39;un enregistrement dans le lac de données sont contenues dans une colonne intitulée `parametervalues`. Cette colonne est stockée en tant qu’objet JSON.

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
* `Business Unit` : valeur de données personnalisée incluse dans l&#39;objet `parametervalues`.
* `Project ID` : valeur de données personnalisée incluse dans l&#39;objet `parametervalues`.
* `Expanded Project Name` : valeur de données personnalisée incluse dans l&#39;objet `parametervalues`.

### Explication

Lors de l&#39;interrogation de l&#39;objet JSON `parametervalues`, chaque champ de données personnalisé est accessible en tant que colonne à l&#39;aide des éléments suivants :

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` est le nom de l&#39;objet JSON dans la table interrogée. Dans le cas de données personnalisées, il s&#39;agira toujours de `parametervalues`.
* `<parameter_name>` est la chaîne `parametername` trouvée dans l&#39;outil de configuration de formulaire, bien qu&#39;elle ne corresponde pas toujours à cette valeur.

>[!NOTE]
>
>Si le nom du paramètre est modifié dans l’outil de configuration de formulaire Workfront, il est représenté sous la forme d’une nouvelle colonne dans l’objet JSON. Par conséquent, nous vous recommandons de ne pas modifier le nom d’une colonne une fois qu’elle est créée dans l’outil de configuration de formulaire. Cependant, le libellé peut être modifié sans affecter l’objet JSON.
>
>Si la chaîne de texte du nom de paramètre est incorrecte, la colonne renvoie une valeur NULL plutôt qu&#39;une erreur.

* `<data_type>` convertit la valeur renvoyée par l&#39;objet JSON en un type de données approprié pour le champ. Le choix d&#39;un type de données incompatible pour la valeur renvoyée entraînera une erreur d&#39;incompatibilité de type de données. Types de données possibles :

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (par exemple, `Number(32,4)` renvoie 1234.0987)
   * `date`
   * `timestamp`

* `<column_name>` est l&#39;étiquette que vous créez pour chaque colonne de données personnalisée.

>[!NOTE]
>
>Seuls les paramètres auxquels des valeurs sont affectées dans le formulaire seront inclus dans l’objet JSON. Si un champ de données personnalisé est vide dans le formulaire, il n’apparaît pas.

## Heure dans la requête d&#39;état

Cet exemple montre comment mesurer le temps passé par un projet dans des états précédemment attribués. Il peut être facilement adapté pour mesurer le temps de tâche ou de problème dans un état, ou il peut être adapté pour mesurer la durée pendant laquelle un autre attribut (y compris des valeurs de données personnalisées) a été appliqué à un objet.

### Scénario

La direction de votre entreprise estime que vous passez trop de temps à chaque étape de votre cycle de vie professionnelle. Avant de formuler des recommandations pour améliorer le processus, vous souhaitez créer une mesure de référence pour déterminer la fréquence à laquelle l&#39;état d&#39;un projet change au fil du temps et le nombre de jours qu&#39;un projet reste dans un état donné.

Vous allez utiliser la vue de données PROJECTS_EVENT pour extraire une liste de chaque changement d&#39;état par rapport à l&#39;objet du projet. Vous allez comparer le nouveau statut au statut précédent, saisir la plage de temps effective pour le statut précédemment attribué, puis calculer les jours passés dans ce statut.

À l&#39;aide de cette sortie brute du temps passé dans chaque état par projet, vous pouvez commencer à créer des visualisations ou agréger davantage les données pour créer des moyennes de durée d&#39;état par état, type de projet ou période de l&#39;année. Cette base de référence est ensuite utilisée pour établir un point de référence par rapport auquel vous pouvez vous mesurer pour répondre aux attentes de votre leadership.

La requête suivante utilise la vue de données PROJECTS_EVENTS de Data Connect pour comparer chaque événement de changement de statut de projet et afficher l&#39;heure dans le statut.

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

* `PROJECTID` : ID de projet Workfront associé à l&#39;événement de changement d&#39;état.
* `PROJECT_NAME` : nom du projet Workfront.
* `PREVIOUS_STATUS` : état du projet immédiatement avant la modification.
* `STATUS` : état du projet après la modification.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP` : horodatage de l&#39;événement de modification lorsque le statut précédent a été défini.
* `STATUS_END_EFFECTIVE_TIMESTAMP` : horodatage de l&#39;événement de modification lors de la définition de la valeur d&#39;état mise à jour.
* `STATUS_DURATION_DAYS` : différence (en jours) entre l&#39;horodatage effectif de fin et l&#39;horodatage effectif de début.

### Explication

La requête utilise les fonctionnalités de suivi des événements de modification de Data Connect.  Il détermine la date de déclenchement d&#39;un événement dont la nouvelle valeur d&#39;état était différente de l&#39;événement précédent. 

Examen de la requête de l’intérieur vers l’extérieur : 

1. Calculer les enregistrements dont le statut précédent est différent : 
   * Pour chaque événement de modification, utilisez la fonction lag() pour identifier la valeur précédente de status. 

2. Filtrer uniquement sur les enregistrements qui ont été modifiés : 

   * Sélectionner les enregistrements du calcul à l&#39;étape 1 où le statut précédent != état actuel. 

3. Calculer l’horodatage effectif de début/fin et la durée en jours : 

   * `<status_begin_effective_timestamp>` : calculé à l&#39;étape 2. 

   * `<status_end_effective_timestamp>` : calculé en fonction du suivant (lead()). `<status_begin_effective_timestamp>` : n&#39;affichez le statut que si `<status_begin_effective_timestamp>` n&#39;est PAS NULL. 
   * `<status_duration_days>` : différence de données entre `<status_begin_effective_timestamp>` et `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Il est recommandé d&#39;utiliser cette requête comme sa propre « Vue » dans PowerBI ou Tableau.  Si vous souhaitez importer d&#39;autres champs de `<object>_event view`, joignez la sortie de cette requête à `<object>_event view`.  Les champs de jointure sont les suivants : <br>
>Pour projects_event : 
>`From projects_event p`
>`Join <above query> c on c.projectid = p.projectid  `
>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
