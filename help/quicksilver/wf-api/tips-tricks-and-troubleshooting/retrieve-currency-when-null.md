---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Récupérer les informations relatives à la devise d’un projet lorsque la devise est nulle.
description: Récupérer les informations relatives à la devise d’un projet lorsque la devise est nulle.
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
TQID: https://experienceleague.adobe.com/fWBcEeqoJFK6WzcEE2Ajqv6cdxk0J9IN1CiPPGU6pIg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 100%

---

# Récupérer les informations relatives à la devise d’un projet lorsque la devise est nulle (non attribuée)

L’objet de projet contenant le champ « devise » peut être récupéré à l’aide de la demande suivante :

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

Cela renverrait le corps de réponse suivant :

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

Si la devise n’est pas définie pour le projet, cette réponse inclura une devise ayant la valeur `null` :

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

Si vous avez besoin de la devise du projet (par exemple pour des calculs), vous pouvez récupérer la devise par défaut du client ou de la cliente :

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

La réponse comprend la devise que l’utilisateur ou l’utilisatrice a définie par défaut et qui sera utilisée par tous les projets de ce client ou de cette cliente dont la devise n’a pas été définie :

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
