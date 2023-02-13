---
title: Les affectations dans un objet supprimé apparaissent de manière inattendue dans les rapports attribués
description: Les affectations dans un objet supprimé apparaissent de manière inattendue dans les rapports attribués
author: Nolan
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Les affectations dans un objet supprimé apparaissent de manière inattendue dans les rapports attribués

## Problème

Après avoir supprimé un objet ayant une affectation, l’objet et l’affectation sont supprimés. Mais la mission peut encore apparaître dans certains rapports.

Par exemple, si vous supprimez une tâche qui a été affectée à un utilisateur, l’affectation à l’utilisateur est également supprimée. Cependant, si vous exécutez par la suite un rapport de tâches filtré par personne désignée, cet utilisateur étant spécifié, le rapport répertorie toujours la tâche supprimée si la tâche se trouve toujours dans la corbeille.

## Cause

Cela est dû aux limitations architecturales de la Corbeille. Il n&#39;existe actuellement aucun plan de route pour résoudre ce problème à cause de l&#39;ampleur de la refonte de l&#39;architecture qui serait nécessaire.
