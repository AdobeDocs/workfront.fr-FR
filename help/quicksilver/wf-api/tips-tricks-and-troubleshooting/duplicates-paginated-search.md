---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Doublons renvoyés lors d’une recherche paginée de grande ampleur
description: Doublons renvoyés lors d’une recherche paginée de grande ampleur
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 100%

---

# Doublons renvoyés lors d’une recherche paginée de grande ampleur

## Problème

Lors d’une recherche paginée de grande ampleur d’un objet dans l’API, le client ou la cliente reçoit les entrées en double, ainsi que les enregistrements manquants.

## Solution

Lorsque l’ordre n’est pas formellement défini, l’ordre des lignes renvoyées par la base de données Oracle est fiable, mais celle-ci ne garantit aucun ordre prédéterminé. Par exemple, deux appels consécutifs avec la même requête peuvent renvoyer des lignes dans un ordre différent. De même, lorsque vous effectuez une pagination, les lignes peuvent être attribuées de manière aléatoire à différentes « pages », ce qui entraîne des doublons. La solution la plus simple peut être d’ajouter un tri par identifiant :

```
&ID_Sort=asc
```

