---
content-type: api
navigation-topic: wf-api
title: Obtention de l’API de temps disponible pour les utilisateurs
description: Obtention de l’API de temps disponible pour les utilisateurs
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 1%

---

# API de temps disponible pour les utilisateurs

**URI : task/api/v15.0/user/getUsersAvailableTime**

Le point de terminaison de l’heure disponible de l’utilisateur récupère les données sur l’heure disponible de l’utilisateur. Cela permet des intégrations pour l’agrégation des données en fonction des attributs utilisateur et des intervalles de temps.

## Exemple de requête

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Paramètres de requête

* **userIDs** : tableau de chaînes. Obligatoire. Exemple : `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate** : datetime. chaîne. Obligatoire. Exemple : `"2022-07-10T00:00:00"`.

* **toDate** : datetime. chaîne. Obligatoire. Exemple `"2022-07-20T23:59:59"`.

## Exemple de réponse :

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## Paramètres de réponse

* **AVL** : heures disponibles réelles. Tableau de nombres.
* **PAVL** : heures disponibles pures pour la planification qui n’incluent pas les jours non ouvrés ni le temps d’arrêt de l’utilisateur. Chaîne.
