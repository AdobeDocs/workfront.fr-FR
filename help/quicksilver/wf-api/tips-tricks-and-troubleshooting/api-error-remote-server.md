---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Message d’erreur d’API (400) Bad Request
description: Message d’erreur d’API (400) Bad Request
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 100%

---


# Erreur d’API : « Le serveur distant a renvoyé une erreur (400) Bad Request ».

## Problème

Vous obtenez l’erreur suivante lorsque vous tentez d’utiliser l’API pour importer un champ personnalisé dans un problème :

`The remote server returned an error: (400) Bad Request`

## Cause

Cette erreur se produit lorsque vous essayez d’importer, via l’API, un champ personnalisé à partir d’un projet qui n’a pas de formulaire personnalisé associé à une rubrique de la file d’attente.

## Solution

Ajoutez le formulaire personnalisé adéquat à la rubrique de la file d’attente.

Pour en savoir plus sur les rubriques de file d’attente, voir [Créer des rubriques de file d’attente](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
