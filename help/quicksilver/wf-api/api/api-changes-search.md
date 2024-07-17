---
filename: api-changes-search
content-type: api
keywords: objet,status,search,best,practices,response
navigation-topic: api-navigation-topic
title: "Modifications de l’API principale : réponses de recherche d’état"
description: Modifications de la façon dont Workfront stocke les objets d’état.
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 2%

---

# Modifications principales de l’API : réponses à la recherche de statuts

Des modifications ont été apportées à la manière dont Workfront stocke les objets d’état. Ces modifications n’affectent pas la manière dont les demandes de recherche d’état sont effectuées, mais affectent la réponse renvoyée par les demandes d’API qui incluent une recherche d’objets d’état en renvoyant une liste incomplète d’états de groupe.

## Bonnes pratiques

Afin de récupérer de manière fiable la liste complète des statuts disponibles pour un groupe, les demandes suivantes sont considérées comme des bonnes pratiques.

>[!NOTE]
>
>Ces structures de requête sont recommandées pour tous les utilisateurs, que les modifications de recherche d’état aient été apportées ou non à votre grappe.

Pour l’état du groupe de projets :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Pour l’état du groupe de tâches :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Pour le statut du groupe de problèmes :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

Ces trois points de terminaison acceptent le paramètre **includeHidden=true** afin de récupérer les états de projet/tâche/problème masqués d&#39;un groupe donné. La modélisation de vos requêtes de recherche d’état après ces exemples de bonnes pratiques garantit que toutes les informations d’état de groupe sont incluses avec chaque réponse.

Voici un exemple de requête de recherche d’état effectuée vers un groupe de tâches qui inclut un état verrouillé au niveau du système **Custom_1** et un état déverrouillé **Custom_2** :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

L’utilisation de ce format permet de s’assurer que votre réponse comprend tous les éléments suivants :

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

## Comprendre les modifications apportées à la requête de recherche d’état héritée

Dans le système hérité, une requête de recherche d’état copierait tous les états système disponibles pour tous les groupes inclus dans une requête. La réponse héritée inclurait alors tous les états système et les états au niveau du groupe disponibles pour chaque groupe dans la requête.

Par exemple, cette requête (qui ne suit pas les bonnes pratiques actuellement recommandées) :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

La réponse suivante serait fournie sous l’ancien système, qui comprend tous les états d’objet :

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

Toutefois, suite aux mises à jour apportées à la manière dont les statuts sont stockés et utilisés, les statuts ne sont pas copiés pour les groupes et sont hérités par chaque groupe au niveau du système. Par conséquent, la requête de l’API de recherche lit uniquement les états qui sont directement associés à un groupe particulier. Par conséquent, la réponse inclut les états verrouillés et déverrouillés du système, mais uniquement pour les groupes qui ont été créés après l’ajout de l’état en question.

Si vous ne parvenez pas à utiliser les bonnes pratiques mises à jour pour effectuer des requêtes de recherche d’état après la mise à jour du système hérité, une liste incomplète des statuts de groupe sera renvoyée dans la réponse.

Voici un exemple de ce que cette structure de requête obsolète renvoie une fois que le système hérité a été mis à jour :

>**Exemple :**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

Notez que cette réponse inclut uniquement les états spécifiques au groupe et exclut les états déclarés au niveau du système :

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
