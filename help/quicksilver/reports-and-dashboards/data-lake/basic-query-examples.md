---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exemples de requêtes Data Connect
description: Exemples de requêtes que vous pouvez utiliser pour vous familiariser avec la syntaxe et la structure de types de requêtes spécifiques.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
ht-degree: 1%

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

La requête utilise les fonctionnalités de suivi des événements de modification de Data Connect. Elle détermine la date de déclenchement d&#39;un événement dont la nouvelle valeur de statut était différente de celle de l&#39;événement précédent. 

Examiner la requête de l’intérieur vers l’extérieur : 

1. Calculer les enregistrements dont le statut précédent est différent : 
   * Pour chaque événement de modification, utilisez la fonction lag() pour identifier la valeur précédente de status. 

2. Filtrez uniquement les enregistrements qui ont été modifiés : 

   * Sélectionnez les enregistrements du calcul de l’étape 1 où le statut précédent != le statut actuel. 

3. Calculer la date et l’heure effectives de début et de fin en jours : 

   * `<status_begin_effective_timestamp>` : calculé à l’étape 2. 

   * `<status_end_effective_timestamp>` : calculé en fonction du suivant (lead()). `<status_begin_effective_timestamp>` : n&#39;afficher le statut que si `<status_begin_effective_timestamp>` n&#39;est PAS NULL. 
   * `<status_duration_days>` : différence de données entre `<status_begin_effective_timestamp>` et `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>Il est recommandé d&#39;utiliser cette requête comme sa propre « Vue » dans PowerBI ou Tableau. Si vous souhaitez importer d&#39;autres champs du `<object>_event view`, rejoignez la sortie de cette requête dans le `<object>_event view`. Les champs de jointure seraient les suivants : <br>
>Pour projects_event : 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## Planification : requête de type enregistrement unique

Cet exemple montre comment interroger les données Workfront Planning pour un type d’enregistrement unique stocké dans le lac de données Data Connect.

### Scénario

Votre entreprise utilise Workfront Planning pour effectuer le suivi des campagnes. Chaque enregistrement de campagne comprend un nom, un statut, une date de début, une date de fin et un propriétaire. Vous souhaitez extraire une liste de toutes les campagnes actives et leurs détails clés pour les utiliser dans un tableau de bord.

* Les données de type d&#39;enregistrement Planning sont stockées dans la vue PLANNINGRECORD_CURRENT.
* Chaque ligne représente un seul enregistrement et toutes les valeurs de champ sont stockées dans une colonne JSON nommée FIELD_VALUES.
* Le type d’enregistrement est identifié par la colonne RECORDTYPEID .
* L&#39;espace de travail de l&#39;enregistrement est identifié par la colonne WORKSPACEID (ou la colonne WORKSPACENAME pour un filtre lisible par l&#39;utilisateur).

### Requête

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### Réponse

La requête ci-dessus renvoie les données suivantes :

* **recordid** : ID d’enregistrement Planning unique pour la campagne.
* **nom_campagne** : nom de la campagne, extrait de l’objet JSON FIELD_VALUES.
* **campaign_status** : statut actuel de la campagne.
* **start_date** : date de début de la campagne, convertie en un type de données de date.
* **end_date** : date de fin de la campagne, convertie en données de type date.
* **propriétaire** : nom de l’utilisateur ou de l’équipe affecté(e) comme propriétaire de la campagne.

### Explication

Les enregistrements Planning dans Data Connect partagent une structure de table unique, quel que soit le type d&#39;enregistrement. La colonne RECORDTYPEID permet d’étendre la requête à un type d’enregistrement spécifique (dans ce cas, Campagnes). Remplacez `<your_campaign_record_type_id>` par l&#39;ID du type d&#39;enregistrement que vous souhaitez interroger, qui se trouve dans les paramètres de type d&#39;enregistrement Workfront Planning ou en interrogeant RECORDTYPE_CURRENT.

Les valeurs de champ sont stockées sous la forme d’un objet JSON dans la colonne FIELD_VALUES et sont accessibles en utilisant la même syntaxe avec deux points que celle utilisée pour les données de formulaire personnalisé :

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

Les références au nom du champ doivent correspondre exactement au nom du champ défini dans la configuration du champ de type d&#39;enregistrement Planning, y compris les majuscules, l&#39;espacement et les émoticônes.

>[!NOTE]
>
>Les identifiants de type d’enregistrement Planning se trouvent dans l’URL lors de l’affichage d’un type d’enregistrement dans Workfront Planning. Il s’agit du chemin de l’URL qui commence par « Rt... ». Vous pouvez également trouver des types d’enregistrement avec l’appel SQL suivant dans Data Connect :
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planning : requête sur les types d&#39;enregistrements connectés

Cet exemple montre comment interroger les données de deux types d&#39;enregistrements Planning connectés : un type d&#39;enregistrement parent et un type d&#39;enregistrement auquel il est connecté.

### Scénario

Votre entreprise connecte les enregistrements Campaign aux enregistrements Tactiques dans Workfront Planning. Vous souhaitez générer un rapport qui présente chaque campagne avec les détails clés des tactiques associées. Ils veulent en particulier montrer le nom de la tactique, la priorité stratégique et l&#39;allocation budgétaire afin que la direction puisse examiner l&#39;activité de campagne organisée par tactique.

Dans Data Connect, les connexions entre les types d&#39;enregistrements Planning natifs sont stockées directement dans la colonne FIELD_VALUES_RAW de PLANNINGRECORD_CURRENT. Pour un champ de référence nommé « Tactiques », la valeur est un tableau JSON d’objets d’enregistrement connectés, chacun contenant une propriété id avec le RECORDID de l’enregistrement connecté. Utilisez l’APLATISSEMENT LATÉRAL Snowflake pour développer ce tableau en lignes et le joindre au type d’enregistrement connecté.

### Requête

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### Réponse

La requête ci-dessus renvoie les données suivantes :

* **campaign_id** : ID d’enregistrement Planning unique pour la campagne.
* **campaign_name** : nom de l’enregistrement de la campagne.
* **campaign_status** : statut actuel de la campagne.
* **tactic_name** : nom de l’enregistrement tactique connecté.
* **strategy_priority** : valeur du champ Priorité stratégique de l’enregistrement Tactique connecté.
* **budget_allocation** : valeur du champ Affectation budgétaire de l’enregistrement Tactique connecté, convertie en flottant.

### Explication - KP modifié

Les connexions entre les types d&#39;enregistrements Planning natifs sont stockées dans une table de jointure REFERENCE_CURRENT.  La table de jointure REFERENCE_CURRENT est utilisée pour les jointures entre RecordType.   Lors de la jonction entre RecordType, le champ TO_RECORDID doit être utilisé.

La colonne REFERENCE_ID de la vue PLANNINGRECORD contient la liste de tous les champs REFERENCEID applicables à cet enregistrement de planification. Vous pouvez accéder à l’identifiant en utilisant la même notation JSON qu’une valeur_champ.

```
<reference_ids>:"<reference_name>"::text
```

La vue REFERENCE_CURRENT contient un ou plusieurs enregistrements dans lesquels TO_RECORDID pointe vers d&#39;autres champs de `recordId` de planification dans les vues PLANNINGRECORD_*.

Pour joindre un autre champ REFERENCE à d&#39;autres enregistrements de planification, le même modèle de jointure à REFERENCE_CURRENT et à PLANNINGRECORD_* des vues sont ajoutés à la requête ci-dessus.


## Planification : type d’enregistrement joint à la requête de données de workflow Workfront

Cet exemple montre comment joindre un type d&#39;enregistrement Workfront Planning à un objet de workflow Workfront natif (dans ce cas, un projet) à l&#39;aide de la fonction de connexion native de Planning, qui stocke les références d&#39;objet externes dans la vue REFERENCE_CURRENT.

### Scénario

Votre entreprise connecte les enregistrements Campaign dans Workfront Planning aux projets Workfront à l&#39;aide de la fonctionnalité de connexion native de Planning. Vous souhaitez produire un rapport combiné présentant les détails de la campagne ainsi que les données d&#39;exécution en direct du projet lié, en particulier le pourcentage achevé actuel du projet, la date d&#39;achèvement prévue et le propriétaire du projet affecté, afin que les responsables de la campagne puissent suivre la progression de la diffusion sans quitter leur contexte d&#39;espace de travail Planning.

### Requête

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### Réponse

La requête ci-dessus renvoie les données suivantes :

* **campaign_id** : ID d’enregistrement Planning unique pour la campagne.
* **campaign_name** : nom de l’enregistrement de la campagne.
* **campaign_status** : statut actuel de la campagne, à partir de Planning.
* **linked_project_id** : ID de projet Workfront provenant de REFERENCE_CURRENT.TO_EXTERNALID, identifiant le projet Workfront connecté.
* **project_name** : nom natif du projet Workfront provenant de PROJECTS_CURRENT.
* **project_percent_complete** : valeur actuelle du projet en pourcentage d’achèvement.
* **project_scheduled_completion** : date d’achèvement prévue du projet Workfront lié.
* **project_owner_id** : ID utilisateur Workfront du propriétaire du projet.
* **project_owner_name** : nom d’affichage du propriétaire du projet, résolu en joignant à USERS_CURRENT.

### Explication

Les connexions d&#39;un type d&#39;enregistrement Planning à un objet de workflow Workfront natif sont stockées dans REFERENCE_CURRENT. Chaque ligne de cette vue représente un lien directionnel : TO_EXTERNALID contient l’identifiant de l’objet Workfront connecté. Les lignes représentant les connexions Workfront sont identifiées par `TO_EXTERNALCONNECTIONNAME = 'workfront'` et une valeur TO_EXTERNALOBJECTNAME correspondant au code API du type d’objet Workfront, par exemple PROJ pour les projets.

La colonne REFERENCE_ID des tables PLANNINGRECORD contient la liste de tous les champs REFERENCEID qui s&#39;appliquent à cet enregistrement.  Vous pouvez accéder à l’identifiant en utilisant la même notation JSON qu’une valeur_champ.\
Un ID REFERENCE_ID unique dans PLANNINGRECORD_CURRENT peut contenir un ou plusieurs liens de référence dans la table REFERENCE_CURRENT qui sont liés à des objets d&#39;un type d&#39;objet spécifique dans la table Workfront.

```
<reference_ids>:"<reference_name>"::text
```

Notez que les vues Planning (PLANNINGRECORD_CURRENT, REFERENCE_CURRENT) résident dans le schéma WORKFRONT.PLANNING, tandis que les vues de workflow Workfront natives (PROJECTS_CURRENT, USERS_CURRENT, etc.) résident dans le schéma WORKFRONT.WF ; Les jointures entre schémas nécessitent des noms de table entièrement qualifiés.

La requête effectue trois jointures :

1. **Enregistrements Planning dans la table des références :** REFERENCE_CURRENT est joint sur `TO_RECORDID = c.RECORDID` pour rechercher toutes les connexions provenant de chaque enregistrement Campaign. Les filtres sur `TO_EXTERNALCONNECTIONNAME = 'workfront'` et `TO_EXTERNALOBJECTNAME = 'PROJ'` limitent les résultats aux lignes qui représentent spécifiquement les connexions aux projets Workfront.
1. **Tableau de références aux projets Workfront :** TO_EXTERNALID contient l’ID de projet Workfront natif pour le projet connecté. Il est joint directement à `PROJECTS_CURRENT.projectid` pour récupérer les données de projet actives.
1. **Projets pour les utilisateurs :** une JOINTURE À GAUCHE pour USERS_CURRENT résout la clé étrangère ownerid sur le projet en un nom lisible par l’utilisateur. Une JOINTURE À GAUCHE est utilisée ici afin que les projets sans propriétaire affecté soient toujours inclus dans les résultats.

>[!NOTE]
>
>Lors de la jointure à des tables externes à Planning, N&#39;utilisez PAS le champ TO_RECORDID dans la requête.  Elle n&#39;est pas nécessaire lors de la jonction à des tables externes.
>
>Ce modèle peut être appliqué à tout objet de processus Workfront auquel Planning prend en charge la connexion, comme les projets, les portfolios ou les programmes, en modifiant le filtre TO_EXTERNALOBJECTNAME sur le code d&#39;API d&#39;objet approprié (par exemple, PORT pour les portfolios ou PRGM pour les programmes) et en joignant le tableau WORKFRONT.WF correspondant. Reportez-vous au dictionnaire de données de Workfront Data Connect pour connaître les noms de table et de colonne d’ID corrects pour chaque type d’objet.

Pour joindre un autre champ REFERENCE à des enregistrements externes supplémentaires, ajoutez le même modèle de jointure à REFERENCE_CURRENT et les vues de workflow Workfront à la requête ci-dessus.

Les valeurs des enregistrements External et Planningrecord peuvent être jointes dans la même requête en joignant plusieurs fois la table REFERENCE_CURRENT et en utilisant le modèle de jointure approprié.


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
