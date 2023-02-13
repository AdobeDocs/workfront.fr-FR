---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: La mise à jour vers emailAddr ne met pas à jour le nom d’utilisateur
description: La mise à jour vers emailAddr ne met pas à jour le nom d’utilisateur
author: John
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# La mise à jour vers emailAddr ne met pas à jour le nom d’utilisateur

## Problème

Normalement, `emailAddr` et `username` sont le même attribut. Par conséquent, si vous modifiez le `emailAddr` , l’attribut `username` est automatiquement mis à jour pour correspondre.

Lorsque la variable `username` ne correspond pas à la variable `emailAddr`, une mise à jour de la variable `emailAddr` ne met pas à jour la variable `username` automatiquement. C’est vrai pour les deux `emailAddr` change par le biais de l’interface utilisateur et de l’API.

## Cause

La discordance peut être créée de plusieurs manières :

* Utilisateurs créés avant l’existence de la règle de synchronisation. Les comptes utilisateur très anciens peuvent ne pas avoir ces attributs synchronisés.

* Utilisateurs créés via SSO à une époque où l’emailAddr dans Workfront était sensible à la casse. L’option de configuration automatique SSO exécute une vérification sensible à la casse pour les utilisateurs en fonction des attributs de l’utilisateur du fournisseur d’identité. Lorsqu’il n’existait pas de correspondance exacte, les services d’approvisionnement automatique créaient un nouvel utilisateur. Si un utilisateur existait déjà, le nom d’utilisateur et la variable `emailAddr` n’aurait pas la même casse.

* Les utilisateurs qui ont utilisé la variable `username` mis à jour directement via l’API et leurs `emailAddr` n’a pas été mis à jour. Le `username` et `emailAddr` ne correspondent peut-être pas.

## Solution

Utilisez l’API pour modifier la variable `username` pour être identique à l’attribut `emailAddr`. Après la synchronisation des attributs, toute mise à jour de la variable `emailAddr` mettra également à jour la variable `username` à faire correspondre (lorsque le champ nom d’utilisateur n’est pas inclus dans la mise à jour).
