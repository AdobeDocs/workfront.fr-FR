---
title: Les affectations dans un objet supprimé apparaissent de manière inattendue dans les rapports affectés
description: Les affectations dans un objet supprimé apparaissent de manière inattendue dans les rapports affectés
author: Courtney
draft: Probably
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 100%
---
# Les affectations dans un objet supprimé apparaissent de manière inattendue dans les rapports affectés

## Problème

Après avoir supprimé un objet ayant une affectation, l’objet et l’affectation sont supprimés. Mais l’affectation peut encore apparaître dans certains rapports.

Par exemple, si vous supprimez une tâche affectée à un utilisateur ou une utilisatrice, l’affectation est également supprimée. Cependant, si vous exécutez par la suite un rapport de tâches filtré par cessionnaire, en spécifiant cet utilisateur ou cette utilisatrice, le rapport répertorie toujours la tâche supprimée si cette dernière se trouve toujours dans la corbeille.

## Cause

Cela est dû aux limites architecturales de la Corbeille. Il n’existe actuellement aucun plan sur la feuille de route pour résoudre ce problème à cause de l’ampleur de la refonte architecturale que cela impliquerait.
