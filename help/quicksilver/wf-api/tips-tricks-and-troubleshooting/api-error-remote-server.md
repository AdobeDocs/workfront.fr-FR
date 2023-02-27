---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Message d’erreur d’API 400 Bad Request
description: Message d’erreur d’API 400 Bad Request
author: Becky
feature: Workfront API
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# Erreur API : &quot;Le serveur distant a renvoyé une erreur (400) Bad Request&quot;

## Problème

L’erreur suivante s’affiche lors de la tentative d’utilisation de l’API pour importer un champ personnalisé dans un problème :

`The remote server returned an error: (400) Bad Request`

## Cause

Cette erreur se produit lorsque vous essayez d’importer, via l’API, un champ personnalisé d’un projet pour lequel aucun formulaire personnalisé n’est associé à une rubrique de file d’attente.

## Solution

Ajoutez le formulaire personnalisé approprié à la rubrique File d’attente.

Pour en savoir plus sur les rubriques de la file d’attente, voir [Création de rubriques de file d’attente](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
