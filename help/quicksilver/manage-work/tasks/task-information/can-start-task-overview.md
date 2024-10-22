---
content-type: overview
product-area: projects
navigation-topic: task-information
title: « Vue d’ensemble des tâches "Peut démarrer" »
description: Lorsqu’une tâche peut être commencée, Adobe Workfront ajoute un indicateur « Peut démarrer » à la tâche afin d’indiquer clairement que vous pouvez commencer à travailler sur cette tâche. Vous pouvez visualiser cet indicateur dans la vue d’une liste de tâches ou d’un rapport.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 78%

---

# Vue d’ensemble de l’indicateur « Peut démarrer » pour les tâches

Lorsqu’une tâche peut être commencée, Adobe Workfront ajoute un indicateur « Peut démarrer » à la tâche afin d’indiquer clairement que vous pouvez commencer à travailler sur cette tâche. Vous pouvez visualiser cet indicateur dans la vue d’une liste de tâches ou d’un rapport.

Lorsque la tâche peut être commencée, le champ « Peut démarrer » de la tâche adopte la valeur « True ».

## Comment Workfront marque une tâche comme &quot;Peut démarrer&quot;

Workfront vérifie les éléments suivants avant de marquer une tâche comme « True » dans le champ « Peut démarrer » :

* Si la valeur de Peut démarrer pour le parent est définie sur True, si la tâche possède un parent. Si la valeur du parent est « False », l’indicateur « Peut démarrer » de toutes les sous-tâches est également défini sur « False ».
* Si les prédécesseurs de la tâche ainsi que les prédécesseurs de leurs parents sont terminés. Si elles sont terminées, la valeur « Peut démarrer » de la tâche est définie sur « True ». Si l’une des tâches antérieures à la tâche ou les tâches antérieures de leurs parents ne sont pas terminées ou ont un statut Terminé - En attente d’approbation, la valeur de « Peut démarrer » pour la tâche est définie sur « False ».
* Si le type de dépendance de tâche est Démarrage-Démarrage ou Démarrage-Terminaison. Si le type de dépendance est Démarrage-Démarrage ou Démarrage-Terminaison, l&#39;indicateur &quot;Peut démarrer&quot; de la tâche dépendante sera défini sur True une fois la tâche parent en cours (ou une fois le pourcentage d&#39;achèvement de la tâche parent supérieur à 1 %). <!--not sure if this should say PARENT or PREDECESSOR??; asking on the issue-->

  Pour plus d’informations sur les tâches antérieures, consultez la section [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Remarques sur l’identification des tâches prêtes à démarrer

* Si le type de dépendance entre une tâche et ses tâches antérieures est Démarrer-Démarrer, la tâche antérieure doit démarrer avant que la relation de tâche antérieure soit considérée comme résolue et que les tâches suivantes puissent démarrer. Pour plus d’informations sur les types de dépendance, voir [Vue d’ensemble des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Si une tâche a un projet transversal antérieur, l’achèvement du projet antérieur ne déclenche pas l’application automatique de l’indicateur « Peut démarrer » au projet ultérieur. Vous devez recalculer manuellement la chronologie du projet ultérieur au projet ou Workfront doit la recalculer automatiquement, avant que la tâche du projet ultérieur ne s’affiche comme une tâche pouvant démarrer. Pour plus d’informations sur le recalcul des chronologies d’un projet, consultez la section [Recalculer les chronologies d’un projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Pour plus d’informations sur les projets transversaux antérieurs, consultez la section [Créer des projets transversaux antérieurs](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
