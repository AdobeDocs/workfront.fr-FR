---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Vue d’ensemble des types de dépendances de tâches
description: Les types de dépendances se rapportent aux relations d’antériorité entre les tâches. Ils définissent le moment où la tâche dépendante peut commencer ou se terminer en fonction du début ou de la fin de sa tâche antérieure.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 100%

---

# Vue d’ensemble des types de dépendances de tâches

<!-- Audited: 12/2023 -->

Les types de dépendances se rapportent aux relations d’antériorité entre les tâches. Ils définissent le moment où la tâche dépendante peut commencer ou se terminer en fonction du début ou de la fin de sa tâche antérieure.

>[!IMPORTANT]
>
>Adobe Workfront n’empêche pas le démarrage ou la fin des tâches dépendantes en fonction des types de dépendances, sauf si les relations d’antériorité sont appliquées. Pour plus d’informations sur l’application des tâches antérieures, voir [Appliquer les tâches antérieures](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Vous devez spécifier le type de dépendance d’une relation d’antériorité lorsque vous établissez une telle relation entre vos tâches.

Pour plus d’informations sur les tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Voici les types de dépendances Workfront :

* **Terminer-Démarrer (FS)** : la tâche antérieure doit se terminer avant que la tâche dépendante puisse commencer. Il s’agit du type de dépendance par défaut, utilisé lorsqu’aucun autre type de dépendance n’est spécifié.
* **Terminer-Terminer (FF)** : la tâche antérieure doit se terminer avant que la tâche dépendante puisse se terminer.
* **Démarrer-Démarrer (SS)** : la tâche antérieure doit démarrer avant que la tâche dépendante puisse démarrer. Vous ne pouvez pas démarrer la tâche dépendante tant que la tâche antérieure n’a pas commencé.
* **Démarrer-Terminer (SF)** : la tâche antérieure doit commencer avant que la tâche dépendante puisse se terminer. Vous pouvez démarrer la tâche dépendante avant le début de la tâche antérieure, mais vous ne pouvez pas la terminer tant que la tâche antérieure n’a pas démarré.
* **Programmé-Démarrer (SD)** : cela planifie une tâche en suivant le modèle Terminer-Démarrer, mais le type appliqué est Terminer-Terminer. Lorsque vous utilisez ce type de dépendance, cela planifie le début de la tâche dépendante après la fin de la tâche antérieure. Toutefois, la méthode d’application fait en sorte que la tâche dépendante puisse démarrer à tout moment, mais celle-ci ne peut pas se terminer tant que la tâche antérieure n’est pas également terminée.

>[!NOTE]
>
>Les abréviations des types de dépendances sont utilisées dans les listes de tâches pour définir les relations d’antériorité. Pour plus d’informations, voir [Exemples de valeurs de tâches antérieures dans une liste de tâches](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) dans la [Vue d’ensemble des tâches antérieures](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

