---
product-area: templates
navigation-topic: templates-navigation-topic
title: Vue d’ensemble des jours de début et d’achèvement dans un modèle
description: Vous pouvez utiliser des modèles de projet pour capturer la plupart des processus, informations et paramètres reproductibles associés aux projets de votre organisation. Bien que les projets comportent des dates de début et d’achèvement spécifiques, les modèles ont des jours de début et d’achèvement génériques comme indication de l’endroit où ces dates vont appartenir au projet, en fonction de la chronologie globale du projet.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 87%

---

# Vue d’ensemble des jours de début et d’achèvement dans un modèle

Vous pouvez utiliser des modèles de projet pour capturer la plupart des processus, informations et paramètres reproductibles associés aux projets de votre organisation. Bien que les projets comportent des dates de début et d’achèvement spécifiques, les modèles ont des jours de début et d’achèvement génériques comme indication de l’endroit où ces dates vont appartenir au projet, en fonction de la chronologie globale du projet.

**Exemple :** si la date de début d’un projet est le 1er avril et que vous souhaitez qu’une tâche commence le 3 avril (deux jours après le début du projet), la tâche correspondante sur le modèle qui crée le projet doit commencer le Jour 2 du modèle, où le premier jour du modèle est considéré comme le Jour 0.

## Jour de début

Tenez compte des points suivants lorsque vous utilisez des modèles et des tâches de modèle :

* Par défaut, les modèles ont un jour de début 0 et les tâches de modèle et le modèle affichent un jour de début 0. Le jour de début des tâches de modèle peut changer, mais cela ne modifie pas le jour de début du modèle.
* Le jour de début d’une tâche de modèle représente le nombre de jours ouvrés que Workfront ajoute à la date de début prévue de la tâche lorsqu’un projet est créé à partir du modèle. Par exemple, vous pouvez avoir un modèle avec une seule tâche et le jour de début de la tâche de modèle est 4. Le jour de début du modèle est toujours 0. Lorsque vous créez un projet à partir de ce modèle dont le mode horaire du projet est Date de début et que la date de début prévue du projet est le 1er novembre 2019, la tâche nouvellement créée ajoute 4 jours à cette date et définit sa valeur Date de début prévue sur le 5 novembre 2019.

Les actions suivantes peuvent modifier le jour de début des tâches de modèle :

* Mettre à jour la durée des tâches de modèle antérieures
* Mettre à jour les contraintes de tâche

  Lorsque vous utilisez des contraintes de tâche basées sur la date, vous pouvez mettre à jour manuellement le jour de début des tâches de modèle. Certains exemples de contraintes de tâche basées sur la date sont : Dates fixes, Commencer Au Plus Tôt, Commencer Au Plus Tard, Il Faut Commencer Le.

* Mettre à jour des tâches de modèle antérieures

## Jour d&#39;achèvement

Le jour d’achèvement du modèle correspond au jour où la dernière tâche de modèle s’achève. Par défaut, toutes les tâches de modèle et le modèle affichent un jour d’achèvement de 1, car Workfront suppose que toute tâche de modèle a une durée d’un jour. Le jour d’achèvement des tâches de modèle peut changer, ce qui modifie également le jour d’achèvement du modèle. Le jour d’achèvement du modèle devient la date d’achèvement prévue du futur projet et les jours d’achèvement des tâches du modèle deviennent les dates d’achèvement prévues des futures tâches du projet.

Les actions suivantes peuvent modifier le jour d’achèvement des tâches de modèle :

* Mettre à jour la durée des tâches de modèle
* Mettre à jour les contraintes de tâche

  Lorsque vous utilisez des contraintes de tâche basées sur la date, vous pouvez mettre à jour manuellement le jour d’achèvement des tâches de modèle. Voici quelques exemples de contraintes de tâche basées sur la date : Dates fixes, Finir Au Plus Tôt, Finir Au Plus Tard, Il Faut Finir Le.

* Mettre à jour des tâches de modèle antérieures

## Utiliser des modèles planifiés à partir de la date d’achèvement

Vous pouvez planifier un modèle à partir du jour d’achèvement. Pour plus d’informations, consultez [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Tenez compte des points suivants lorsque vous utilisez des modèles planifiés à partir de la date d’achèvement :

* Si vous modifiez le jour de début, la contrainte de tâche doit être définie sur Il Faut Commencer Le.
* La modification du jour d’achèvement définit la contrainte de tâche sur Il Faut Finir Le.
* Lorsque le modèle est planifié à partir du Jour d&#39;achèvement, le Jour de contrainte de tâche est calculé à partir du Jour d&#39;achèvement.

  **Exemple :** la durée de votre modèle est de 285 jours et vous disposez d’une tâche de modèle de 60 jours. Si vous définissez la contrainte de tâche sur Il Faut Commencer Le et le jour de contrainte sur 120, vous aurez un jour de début de 165 (285 - 120) et un jour d’achèvement de 225 (165 + 60). Ainsi, lorsque vous modifiez le Jour de début, il est en fait interprété comme un Jour de contrainte.
