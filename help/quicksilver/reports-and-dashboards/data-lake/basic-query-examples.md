---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exemples de requêtes Data Connect
description: Exemples de requêtes que vous pouvez utiliser pour vous familiariser avec la syntaxe et la structure de types de requêtes spécifiques.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Exemples de requêtes de connexion aux données Workfront

Pour mieux utiliser vos données Workfront Data Connect, cette page contient des exemples de requêtes de base que vous pouvez utiliser pour vous familiariser avec la syntaxe et la structure de types de requêtes spécifiques.

## Requête de données personnalisée

Cet exemple montre comment composer une requête pour renvoyer vos données personnalisées dans Workfront, telles que des formulaires personnalisés et des champs personnalisés.

### Scénario :

Votre entreprise utilise un formulaire personnalisé nommé Intégration financière. Le formulaire est joint à chaque projet et contient les champs suivants :

* **Business Unit** - Champ personnalisé contenant une chaîne.
* **ProjectID** - Champ personnalisé contenant une chaîne numérique.
* **Nom de projet étendu** - Un champ de données personnalisé calculé qui concatène les valeurs de l’unité opérationnelle, de l’identifiant de projet et du nom de projet Workfront natif en une seule chaîne.

Vous devez inclure ces informations dans la réponse d’une requête sur Data Connect. Les valeurs de données personnalisées pour un enregistrement dans le lac de données sont contenues dans une colonne intitulée `parametervalues`. Cette colonne est stockée en tant qu’objet JSON.

### Requête :

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

### Réponse :

La requête ci-dessus renvoie les données suivantes :

* `projectid` - ID de projet Workfront natif
* `parametervalues` : colonne stockant un objet JSON
* `name` - nom de projet Workfront natif
* `Business Unit` : valeur de données personnalisée incluse dans l’objet `parametervalues`
* `Project ID` : valeur de données personnalisée incluse dans l’objet `parametervalues`
* `Expanded Project Name` : valeur de données personnalisée incluse dans l’objet `parametervalues`

### Explication :

Lors de l’interrogation de l’objet JSON `parametervalues`, chaque champ de données personnalisé est accessible sous la forme d’une colonne à l’aide des éléments suivants :

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` est le nom de l’objet JSON dans la table qui est interrogée. Dans le cas de données personnalisées, il s’agira toujours de `parametervalues`.
* `<parameter_name>` est la chaîne `parametername` trouvée dans l’outil de configuration de formulaire, bien qu’elle ne corresponde pas toujours à cette valeur.

>[!NOTE]
>
>Si le nom du paramètre est modifié dans l’outil de configuration de formulaire Workfront, il sera représenté sous la forme d’une nouvelle colonne dans l’objet JSON. Par conséquent, nous vous recommandons de ne pas modifier le nom d’une colonne une fois qu’elle a été créée dans l’outil de configuration de formulaire. Cependant, le libellé peut être modifié sans affecter l’objet JSON.
>
>Si la chaîne de texte du nom du paramètre est incorrecte, la colonne renvoie une valeur NULL, plutôt qu’une erreur.

* `<data_type>` convertit la valeur renvoyée par l’objet JSON en un type de données approprié pour le champ. Le choix d’un type de données incompatible pour la valeur renvoyée entraînera une erreur de discordance du type de données. Les types de données possibles sont les suivants :

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (par exemple, `Number(32,4)` renverrait 1234.0987)
   * `date`
   * `timestamp`

* `<column_name>` est le libellé que vous créez pour chaque colonne de données personnalisée.

>[!NOTE]
>
>Seuls les paramètres auxquels des valeurs sont affectées dans le formulaire seront inclus dans l’objet JSON. Si un champ de données personnalisé est vide sur le formulaire, il n’apparaîtra pas.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
