---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: La mise à jour d’emailAddr ne met pas à jour le nom d’utilisateur ou d’utilisatrice.
description: La mise à jour vers emailAddr ne met pas à jour le nom d’utilisateur
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 7%

---


# La mise à jour d’emailAddr ne met pas à jour le nom d’utilisateur ou d’utilisatrice.

## Problème

Normalement, `emailAddr` et `username` sont le même attribut. Par conséquent, si vous modifiez l’attribut `emailAddr` d’un utilisateur, l’attribut `username` est automatiquement mis à jour pour correspondre.

Lorsque `username` ne correspond pas à `emailAddr`, une mise à jour de `emailAddr` ne met pas automatiquement à jour le `username`. C’est le cas pour les modifications `emailAddr` effectuées par le biais de l’interface utilisateur et de l’API.

## Cause

La discordance peut être créée de plusieurs manières :

* Utilisateurs créés avant l’existence de la règle de synchronisation. Les comptes utilisateur très anciens peuvent ne pas avoir ces attributs synchronisés.

* Utilisateurs créés via SSO à une époque où l’adresse email dans Workfront était sensible à la casse. L’option de configuration automatique SSO exécute une vérification sensible à la casse pour les utilisateurs en fonction des attributs de l’utilisateur du fournisseur d’identité. Lorsqu’il n’existait pas de correspondance exacte, les services d’approvisionnement automatique créaient un nouvel utilisateur. Si un utilisateur existait déjà, il était possible que le nom d’utilisateur et `emailAddr` n’aient pas la même casse.

* Les utilisateurs qui ont eu l’attribut `username` mis à jour directement via l’API, et leur `emailAddr` n’a pas été mis à jour. Il est possible que les `username` et `emailAddr` ne correspondent pas.

## Solution

Utilisez l’API pour modifier l’attribut `username` afin qu’il soit identique à l’attribut `emailAddr`. Après la synchronisation des attributs, toute mise à jour de `emailAddr` mettra également à jour la correspondance `username` (lorsque le champ nom d’utilisateur n’est pas inclus dans la mise à jour).
