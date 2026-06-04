---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Mettre à jour emailAddr ne met pas à jour username.
description: Mettre à jour emailAddr ne met pas à jour username.
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
TQID: https://experienceleague.adobe.com/dkceJuJ6WfaZTnbD6zdP6TsHR5bvkERD-EiBgVmrCck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 100%

---

# Mettre à jour emailAddr ne met pas à jour username.

## Problème

Normalement, `emailAddr` et `username` sont le même attribut. Par conséquent, si vous modifiez l’attribut `emailAddr` de l’utilisateur ou de l’utilisatrice, l’attribut `username` est automatiquement mis à jour pour correspondre.

Lorsque le `username` ne correspond pas à l’`emailAddr`, mettre à jour l’`emailAddr` ne met pas à jour le `username` automatiquement. C’est vrai pour les deux modifications `emailAddr` par le biais de l’interface d’utilisation et de l’API.

## Cause

La non-concordance peut être créée de plusieurs manières :

* Les utilisateurs et utilisatrices dont la création date d’avant l’existence de la règle de synchronisation. Il se peut que ces attributs ne soient pas synchronisés pour les comptes d’utilisateurs et d’utilisatrices très anciens.

* Les utilisateurs et utilisatrices dont la création a été effectuée via SSO à une époque où emailAddr dans Workfront était sensible à la casse. L’option de configuration automatique SSO exécute une vérification sensible à la casse pour les utilisateurs et utilisatrices en fonction des attributs d’utilisation du fournisseur d’identité. Lorsqu’il n’existait pas de correspondance exacte, les services d’affectation automatique créaient un nouvel utilisateur ou une nouvelle utilisatrice. Si un utilisateur ou une utilisatrice existait déjà, son nom et son `emailAddr` pouvaient ne pas avoir la même casse.

* Les utilisateurs et utilisatrices dont l’attribut `username` avait été mis à jour directement via l’API sans que leur `emailAddr` n’ait été mise à jour. Le `username` et l’`emailAddr` ne correspondent pas forcément.

## Solution

Utilisez l’API pour que le `username` corresponde à l’`emailAddr`. Après la synchronisation des attributs, toute mise à jour de l’`emailAddr` fera également correspondre le `username` (lorsque le champ nom d’utilisateur ou d’utilisatrice n’est pas inclus dans la mise à jour).
