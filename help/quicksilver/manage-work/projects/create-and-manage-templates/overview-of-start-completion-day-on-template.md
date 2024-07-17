---
product-area: templates
navigation-topic: templates-navigation-topic
title: Vue d’ensemble des jours de début et d’achèvement dans un modèle
description: Vous pouvez utiliser des modèles de projet pour capturer la plupart des processus, informations et paramètres répétables associés aux projets de votre entreprise. Bien que les projets comportent des dates de début et de fin spécifiques, les modèles ont des jours de début et de fin génériques comme indication de l’endroit où ces dates vont appartenir au projet, en fonction de la chronologie globale du projet.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 3%

---

# Vue d’ensemble des jours de début et d’achèvement dans un modèle

Vous pouvez utiliser des modèles de projet pour capturer la plupart des processus, informations et paramètres répétables associés aux projets de votre entreprise. Bien que les projets comportent des dates de début et de fin spécifiques, les modèles ont des jours de début et de fin génériques comme indication de l’endroit où ces dates vont appartenir au projet, en fonction de la chronologie globale du projet.

**Exemple :** Si la date de début d’un projet est le 1er avril et que vous souhaitez qu’une tâche démarre le 3 avril (deux jours après le début du projet), la tâche correspondante sur le modèle qui crée le projet doit commencer le jour 2 du modèle, où le premier jour du modèle est considéré comme le jour 0.

## Jour de début

Tenez compte des points suivants lorsque vous utilisez des modèles et des tâches de modèle :

* Par défaut, les modèles ont un Jour de début de 0 et les tâches du modèle et le modèle affichent un Jour de début de 0. Le Jour de début des tâches du modèle peut changer, mais cela ne modifie pas le Jour de début du modèle.
* Le jour de début d’une tâche de modèle représente le nombre de jours ouvrés que Workfront ajoute à la date de début planifiée de la tâche lorsqu’un projet est créé à partir du modèle. Par exemple, vous pouvez avoir un modèle avec une seule tâche et le Jour de début de la tâche de modèle est 4. Le jour de début du modèle est toujours 0. Lorsque vous créez un projet à partir de ce modèle dont le mode Planification du projet est Date de début et la Date de début planifiée du projet est le 1er novembre 2019, la tâche nouvellement créée ajoute 4 jours à cette date et définit sa valeur Date de début planifiée sur 5 novembre 2019.

Voici quelques actions qui peuvent modifier le Jour de début des tâches du modèle :

* Mettre à jour la durée des tâches du modèle précédent
* Mise à jour des contraintes de tâche

  Lorsque vous utilisez des contraintes de tâche basées sur la date, vous pouvez mettre à jour manuellement le jour de début des tâches du modèle. Certains exemples de contraintes de tâche basées sur des dates sont des dates fixes, ne pas commencer avant le, ne pas démarrer plus tard que, ne pas commencer plus tard.

* Mise à jour des prédécesseurs de tâches de modèle

## Jour d&#39;achèvement

Le jour de fin du modèle correspond au jour où la dernière tâche de modèle s’achève. Par défaut, toutes les tâches de modèle et le modèle affichent un jour de fin de 1, car Workfront suppose que toute tâche de modèle a une durée d’un jour. Le Jour de fin des tâches du modèle peut changer, ce qui modifie également le Jour de fin du modèle. Le jour d’achèvement du modèle devient la Date d’achèvement planifiée du futur projet et les Jours d’achèvement des tâches du modèle deviennent les Dates d’achèvement planifiées des futures tâches du projet.

Voici quelques actions qui peuvent modifier le jour de fin des tâches du modèle :

* Mettre à jour la durée des tâches du modèle
* Mise à jour des contraintes de tâche

  Lorsque vous utilisez des contraintes de tâche basées sur la date, vous pouvez mettre à jour manuellement le jour d’achèvement des tâches du modèle. Voici quelques exemples de contraintes de tâche basées sur des dates : Dates fixes, Terminer au plus tôt, Terminer au plus tard, Terminer au plus tard.

* Mise à jour des prédécesseurs de tâches de modèle

## Utilisation de modèles planifiés à partir de la fin

Vous pouvez planifier un modèle à partir du jour de fin. Pour plus d’informations, voir [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Tenez compte des points suivants lorsque vous utilisez des modèles planifiés à partir de la date d’achèvement :

* Si vous modifiez le Jour de début, la contrainte de tâche doit être activée.
* La modification du jour de fin définit la contrainte de tâche sur Doit se terminer.
* Lorsque le modèle est planifié à partir du jour de fin, le jour de contrainte de tâche est calculé à partir du jour de fin.

  **Exemple :** La durée de votre modèle est de 285 jours et vous avez une tâche de modèle de 60 jours. Si vous définissez la contrainte de tâche sur 120 et le jour de contrainte sur 120, vous aurez un jour de début 165 (285 à 120) et un jour de fin 225 (165 + 60). Ainsi, lorsque vous modifiez le Jour de début, il est en fait interprété comme Jour de contrainte.
