---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Aperçu « Peut démarrer » pour les tâches
description: Lorsqu’une tâche peut être commencée, Adobe Workfront ajoute un indicateur « Peut démarrer » à la tâche afin d’indiquer clairement que vous pouvez commencer à travailler sur cette tâche. Vous pouvez visualiser cet indicateur dans la vue d’une liste de tâches ou d’un rapport.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 71%

---

# Vue d’ensemble de l’indicateur « Peut démarrer » pour les tâches

Lorsqu’une tâche peut être commencée, Adobe Workfront ajoute un indicateur « Peut démarrer » à la tâche afin d’indiquer clairement que vous pouvez commencer à travailler sur cette tâche. Vous pouvez visualiser cet indicateur dans la vue d’une liste de tâches ou d’un rapport.

Lorsque la tâche peut être commencée, le champ « Peut démarrer » de la tâche adopte la valeur « True ».

## Comment Workfront marque une tâche comme « Peut démarrer »

Workfront vérifie les éléments suivants avant de marquer une tâche comme « True » dans le champ « Peut démarrer » :

* Si la valeur de Peut démarrer pour le parent est définie sur True, si la tâche a un parent. Si la valeur du parent est « False », l’indicateur « Peut démarrer » de toutes les sous-tâches est également défini sur « False ».
* Indique si les prédécesseurs de la tâche, ainsi que les prédécesseurs de leurs parents, sont terminés. Si elles sont terminées, la valeur « Peut démarrer » de la tâche est définie sur « True ». Si l’une des tâches antérieures à la tâche ou les tâches antérieures de leurs parents ne sont pas terminées ou ont un statut Terminé - En attente d’approbation, la valeur de « Peut démarrer » pour la tâche est définie sur « False ».
* Indique si le type de dépendance de la tâche est Début-Début ou Début-Fin. Si le type de dépendance est Début-Début ou Début-Fin, l&#39;indicateur « Peut démarrer » est défini sur True pour la tâche dépendante une fois que la tâche antérieure est en cours (ou lorsque le pourcentage d&#39;achèvement de la tâche antérieure est supérieur à 1 %).

  Pour plus d’informations sur les tâches antérieures, consultez la section [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Remarques sur l’identification des tâches prêtes à démarrer

* Si le type de dépendance entre une tâche et ses tâches antérieures est Démarrer-Démarrer, la tâche antérieure doit démarrer avant que la relation de tâche antérieure soit considérée comme résolue et que les tâches suivantes puissent démarrer. Pour plus d’informations sur les types de dépendance, voir [Vue d’ensemble des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Si une tâche a un projet transversal antérieur, l’achèvement du projet antérieur ne déclenche pas l’application automatique de l’indicateur « Peut démarrer » au projet ultérieur. Vous devez recalculer manuellement la chronologie du projet du successeur ou Workfront doit la recalculer automatiquement, avant que la tâche du successeur ne s&#39;affiche comme une tâche Peut démarrer. Pour plus d’informations sur le recalcul des chronologies d’un projet, consultez la section [Recalculer les chronologies d’un projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Pour plus d’informations sur les projets transversaux antérieurs, consultez la section [Créer des projets transversaux antérieurs](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
