---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Doublons renvoyés lors d’une recherche paginée de grande envergure
description: Doublons renvoyés lors d’une recherche paginée de grande envergure
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 20%

---


# Doublons renvoyés lors d’une recherche paginée de grande envergure

## Problème

Lors d’une grande recherche paginée dans l’API pour un objet, le client reçoit des entrées en double et des enregistrements manquants.

## Solution

Lorsque la commande n&#39;est pas formellement définie, l&#39;ordre des lignes renvoyé par la base de données Oracle est fiable, ce qui ne garantit aucun ordre déterministe. Par exemple, deux appels consécutifs avec la même requête peuvent renvoyer des lignes dans un ordre différent. De même, lorsque vous effectuez une pagination, les lignes peuvent être attribuées de manière aléatoire à différentes &quot;pages&quot;, ce qui entraîne des doublons. La solution la plus simple peut être d’ajouter un tri par identifiant :

```
&ID_Sort=asc
```

