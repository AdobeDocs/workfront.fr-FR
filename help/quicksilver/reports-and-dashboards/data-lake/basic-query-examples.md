---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exemples de requêtes Data Connect
description: Exemples de requêtes que vous pouvez utiliser pour vous familiariser avec la syntaxe et la structure de types de requêtes spécifiques.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Exemples de requêtes de connexion aux données Workfront

Pour mieux utiliser vos données Workfront Data Connect, cette page contient des exemples de requêtes de base que vous pouvez utiliser pour vous familiariser avec la syntaxe et la structure de types de requêtes spécifiques.

## Requête de données personnalisée

Cet exemple montre comment composer une requête pour renvoyer vos données personnalisées dans Workfront, telles que des formulaires personnalisés et des champs personnalisés.

### Scénario :

Votre entreprise, PeopleSoft, utilise un formulaire personnalisé nommé Intégration financière. Le formulaire est joint à chaque projet et contient les champs suivants :

* **PeopleSoft Business Unit** - Champ personnalisé contenant une chaîne.
* **PeopleSoft ProjectID** - Champ personnalisé contenant une chaîne numérique.
* **Nom de projet étendu** - Un champ de données personnalisé calculé qui concatène les valeurs de PeopleSoft Business Unit, PeopleSoft ProjectID et le nom de projet Workfront natif en une seule chaîne.

Vous devez inclure ces informations dans la réponse d’une requête sur Data Connect. Les valeurs de données personnalisées pour un enregistrement dans le lac de données sont contenues dans une colonne intitulée `parameterValues`. Cette colonne est stockée en tant qu’objet JSON.

### Requête :

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:PeopleSoft Business Unit" :: int as PeopleSoftBusinessUnit,
    parametervalues:"DE:PeopleSoft Project ID" :: int as PeopleSoftProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Réponse

La requête ci-dessus renvoie les données suivantes :

* `projectid` - ID de projet Workfront natif
* `parametervalues` : colonne stockant un objet JSON
* `name` - nom de projet Workfront natif
* `PeopleSoft Business Unit` : valeur de données personnalisée incluse dans l’objet `parametervalues`
* `PeopleSoft Project ID` : valeur de données personnalisée incluse dans l’objet `parametervalues`
* `Expanded Project Name` : valeur de données personnalisée incluse dans l’objet `parametervalues`

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
