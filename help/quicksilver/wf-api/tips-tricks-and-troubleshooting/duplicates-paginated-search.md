---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Doublons renvoyés lors d’une recherche paginée de grande ampleur
description: Doublons renvoyés lors d’une recherche paginée de grande ampleur
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
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

