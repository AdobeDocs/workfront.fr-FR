---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Présentation de "Can Start" pour les tâches
description: Lorsqu’une tâche est prête à démarrer, Adobe Workfront ajoute un indicateur Peut démarrer à la tâche pour identifier facilement qu’il est sans danger pour vous de commencer à travailler sur la tâche. Vous pouvez afficher cet indicateur dans la vue d'une liste de tâches ou d'un rapport.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 1%

---

# Vue d’ensemble de l’option « Peut démarrer » pour les tâches

Lorsqu’une tâche est prête à démarrer, Adobe Workfront ajoute un indicateur Peut démarrer à la tâche pour identifier facilement qu’il est sans danger pour vous de commencer à travailler sur la tâche. Vous pouvez afficher cet indicateur dans la vue d&#39;une liste de tâches ou d&#39;un rapport.

Lorsque la tâche est prête à être travaillée, le champ Peut démarrer sur la tâche est défini sur True.

## Comment Workfront marque une tâche comme &quot;Peut démarrer&quot;

Workfront recherche les éléments suivants avant d’attribuer la valeur True à une tâche pour le champ Début possible :

* Si la tâche possède un parent, elle vérifie si la valeur de Peut démarrer pour le parent qu’elle a défini sur True. Si la valeur du parent est False, toutes les sous-tâches ont également la valeur Can Start définie sur False. 
* Il vérifie également si les prédécesseurs de la tâche ainsi que les prédécesseurs de leurs parents sont complets. S’ils sont terminés, la valeur Can Start pour la tâche est définie sur True. Si l’un des prédécesseurs de la tâche ou les prédécesseurs de leurs parents ne sont pas terminés ou ont le statut Terminé en attente d’approbation, alors la valeur Peut commencer de la tâche est définie sur False. 

  Pour plus d’informations sur les prédécesseurs de tâches, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Observations relatives à l’identification des tâches prêtes à démarrer

* Si le type de dépendance entre une tâche et ses prédécesseurs est Début de début, le prédécesseur doit commencer avant que la relation précédente ne soit considérée comme résolue et que les tâches qui lui succèdent puissent commencer. Pour plus d’informations sur les types de dépendances, voir [Présentation des types de dépendances de tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Si une tâche a un prédécesseur multi-projet, la fin du prédécesseur ne déclenche pas automatiquement l’indicateur Début de la tâche à appliquer au successeur. Vous devez recalculer manuellement la chronologie du projet du successeur ou Workfront doit la recalculer automatiquement, avant que la tâche qui lui succède ne s’affiche sous la forme d’une tâche Peut démarrer . Pour plus d’informations sur le nouveau calcul des calendriers de projet, voir [Recalculer les chronologies de projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Pour plus d’informations sur les prédécesseurs sur plusieurs projets, voir [Création de prédécesseurs sur plusieurs projets](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
