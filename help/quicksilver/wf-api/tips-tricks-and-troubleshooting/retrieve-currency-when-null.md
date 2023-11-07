---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Récupération des informations de devise pour un projet lorsque la devise est nulle
description: Récupération des informations de devise pour un projet lorsque la devise est nulle
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# Récupération des informations de devise pour un projet lorsque la devise est nulle (non attribuée)

L’objet de projet avec le champ de devise peut être récupéré à l’aide de la requête suivante :

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Cela renverra le corps de réponse suivant :

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

Si la devise n’est pas définie pour le projet, cette réponse inclut une devise avec la valeur `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

Si vous avez besoin de la devise pour le projet (pour les calculs, par exemple), vous pouvez récupérer la devise par défaut du client :

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

La réponse inclut la devise que l’utilisateur a définie comme valeur par défaut, qui serait utilisée par tous les projets pour ce client dont la devise n’est pas définie :

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
