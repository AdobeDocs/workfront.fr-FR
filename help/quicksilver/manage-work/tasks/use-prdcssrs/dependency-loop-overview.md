---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Vue d’ensemble de la boucle de dépendance des tâches
description: Lorsque vous ajoutez des relations de prédécesseur à des tâches, vous risquez de rencontrer des boucles de dépendance. Pour plus d’informations sur les prédécesseurs, voir Présentation des prédécesseurs de tâches.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 5%

---

# Présentation de la boucle de dépendance de tâche

Lorsque vous ajoutez des relations de prédécesseur à des tâches, vous risquez de rencontrer des boucles de dépendance. Pour plus d’informations sur les tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Présentation de la boucle de dépendance

Les boucles de dépendance se produisent lorsque deux tâches ou plus dépendent les unes des autres pour être terminées. Adobe Workfront ne vous permet pas de créer une relation de prédécesseur entre les tâches si cela crée une boucle de dépendance.

**Exemple :** La tâche 2 est un prédécesseur de la tâche 1, ce qui signifie que vous devez terminer la tâche 2 avant de pouvoir commencer à travailler sur la tâche 1.

Si vous essayez de faire de la tâche 1 un prédécesseur de la tâche 2, vous obtenez une erreur de boucle de dépendance car vous ne pouvez pas démarrer la tâche 1 tant que la tâche 2 n’a pas été terminée, mais la tâche 2 ne peut pas être lancée tant que la tâche 1 n’est pas terminée.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Considérations relatives aux boucles de dépendance

* Les boucles de dépendance peuvent impliquer plus de deux tâches. Parfois, n’importe quel nombre de parents des tâches que vous connectez à une relation précédente sont ceux qui créent la boucle de dépendance.
* Une boucle de dépendance peut également se produire si vous essayez de faire d’un parent le prédécesseur d’un enfant.
* Dans le cas d’une boucle de dépendance, vous ne pouvez pas enregistrer les tâches ou le projet. Pour corriger la boucle de dépendance, vous devez réévaluer la relation de prédécesseur entre les tâches répertoriées dans le message d’erreur et supprimer les conflits avant de pouvoir enregistrer les tâches ou le projet.

 
