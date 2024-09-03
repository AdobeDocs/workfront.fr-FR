---
filename: api-changes-search
content-type: api
keywords: objet,statut,recherche,bonnes,pratiques,réponse
navigation-topic: api-navigation-topic
title: '« Modifications principales de l’API : réponses à la recherche de statuts »'
description: Modifications de la façon dont Workfront stocke les statuts des objets.
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 100%

---

# Modifications principales de l’API : réponses à la recherche de statuts

Des modifications ont été apportées à la manière dont Workfront stocke les statuts des objets. Ces modifications n’affectent pas la manière dont les demandes de recherche de statut sont effectuées, mais elles affecteront la réponse renvoyée par les demandes API qui incluent une recherche de statut des objets en renvoyant une liste incomplète de statuts de groupe.

## Bonnes pratiques

Afin de récupérer de manière fiable la liste complète des statuts disponibles pour un groupe, les requêtes suivantes sont considérées comme des bonnes pratiques.

>[!NOTE]
>
>Ces structures de requête sont recommandées pour tous les utilisateurs et toutes les utilisatrices, que les modifications de recherche de statut aient été apportées ou non à votre cluster.

Pour le statut du groupe de projets :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Pour le statut du groupe de tâches :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Pour le statut du groupe de problèmes :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Ces trois points d’entrée acceptent le paramètre **includeHidden=true** pour récupérer les statuts masqués de projet/tâche/problème d’un groupe donné. En vous inspirant de ces exemples de bonnes pratiques pour vos requêtes de recherche de statut, vous vous assurez que toutes les informations relatives au statut du groupe sont incluses dans chaque réponse.

Voici un exemple de requête de recherche de statut envoyée à un groupe de tâches qui inclut un statut verrouillé **Custom_1** et un statut déverrouillé **Custom_2** au niveau du système :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

Utiliser ce format permet de s’assurer que votre réponse comprend tous les éléments suivants :

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## Comprendre les modifications apportées à la requête de statut héritée

Dans le système hérité, une requête de statut copiait tous les statuts système disponibles pour tous les groupes inclus dans une requête. La réponse héritée incluait alors tous les statuts système et les statuts au niveau du groupe disponibles pour chaque groupe dans la requête.

Par exemple, cette requête (qui ne suit pas les bonnes pratiques actuellement recommandées) :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

La réponse suivante serait obtenue dans le cadre du système hérité, qui comprend tous les statuts d’objets :

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

Toutefois, suite aux mises à jour apportées à la manière dont les statuts sont stockés et utilisés, les statuts ne sont pas copiés pour les groupes et sont hérités par chaque groupe au niveau du système. Par conséquent, la requête API de recherche ne lit que les statuts qui sont directement associés à un groupe particulier, de sorte que la réponse inclut les statuts verrouillés et déverrouillés, mais uniquement pour les groupes qui ont été créés après l’ajout du statut en question.

Si vous ne parvenez pas à utiliser les bonnes pratiques mises à jour pour effectuer des requêtes de statut après la mise à jour du système hérité, une liste incomplète des statuts de groupe sera renvoyée dans la réponse.

Voici un exemple de ce que cette structure de requête obsolète renvoie une fois que le système hérité a été mis à jour :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Notez que cette réponse inclut uniquement les statuts spécifiques au groupe et exclut les statuts déclarés au niveau du système :

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
