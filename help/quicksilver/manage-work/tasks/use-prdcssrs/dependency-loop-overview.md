---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Vue d'ensemble de la boucle de dépendance de tâche
description: Lorsque vous ajoutez des relations antérieures aux tâches, vous pouvez rencontrer des boucles de dépendance. Pour plus d’informations sur les tâches antérieures, voir la section Vue d’ensemble des tâches antérieures.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
TQID: https://experienceleague.adobe.com/cQbPOUES-tmSgZTpXrft8lQby-ubPmI-TZ1PjdGURMc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 68%

---

# Vue d’ensemble de la boucle de dépendance des tâches

Lorsque vous ajoutez des relations antérieures aux tâches, vous pouvez rencontrer des boucles de dépendance. Pour plus d’informations sur les tâches antérieures, voir la section [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Vue d’ensemble des boucles de dépendance

Les boucles de dépendance se produisent lorsque vous avez deux tâches ou plus qui dépendent l&#39;une de l&#39;autre à terminer. Adobe Workfront ne vous permet pas de créer une relation de prédécesseur entre des tâches si une boucle de dépendance est créée.

**Exemple :** la tâche 2 est antérieure à la tâche 1, la tâche 2 doit donc être terminée avant que vous puissiez commencer à travailler sur la tâche 1.

Si vous essayez de rendre la tâche 1 antérieure à la tâche 2, vous obtenez une erreur de boucle de dépendance, car vous ne pouvez pas démarrer la tâche 1 tant que la tâche 2 n’est pas terminée, mais la tâche 2 ne peut pas être démarrée tant que la tâche 1 n’est pas terminée.

![Message d’erreur de boucle de dépendance](assets/dependency-loop-error-message-350x209.png)

![Boucle de dépendance dans la liste des tâches](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considérations sur les boucles de dépendance

* Les boucles de dépendance peuvent impliquer plus de deux tâches. Parfois, un certain nombre de parents des tâches que vous connectez avec une relation d’antériorité sont ceux qui créent la boucle de dépendance.
* Une boucle de dépendance peut également se produire si vous essayez de transformer un parent en tâche antérieure d’un enfant.
* Dans le cas d’une boucle de dépendance, vous ne pouvez sauvegarder ni les tâches ni le projet. Pour corriger la boucle de dépendance, vous devez réévaluer la relation de prédécesseur entre les tâches répertoriées dans le message d’erreur et supprimer les conflits avant de pouvoir enregistrer les tâches ou le projet.


