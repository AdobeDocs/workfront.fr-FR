---
content-type: api
navigation-topic: wf-api
title: Obtenir l’API des heures disponibles pour les personnes
description: Obtenir l’API des heures disponibles pour les personnes
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 100%

---

# API des heures disponibles pour les personnes

**URI : attask/api/v15.0/user/getUsersAvailableTime**

Le point d’entrée des heures disponibles des personnes récupère les données sur les heures disponibles de la personne. Cela permet des intégrations pour l’agrégation des données en fonction des attributs de la personne et des intervalles de temps.

## Exemple de requête

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Paramètres de requête

* **userIDs** : séquence de chaînes de caractères. Requis. Exemple : `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate** : datetime. Chaîne de caractères. Requis. Exemple : `"2022-07-10T00:00:00"`.

* **toDate** : datetime. Chaîne de caractères. Requis. Exemple `"2022-07-20T23:59:59"`.

## Exemple de réponse :

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

* **AVL** : heures disponibles réelles. Tableau de nombres.
* **PAVL** : nombre d’heures pures disponibles pour la planification qui n’inclut pas les jours non ouvrés ni les jours de congé de la personne. Chaîne de caractères.
