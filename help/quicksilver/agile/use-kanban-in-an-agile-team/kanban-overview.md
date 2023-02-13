---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Présentation de Kanban
description: Consultez cet article pour mieux comprendre le fonctionnement de la carte Kanban.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: a478e5355db33e076b321a6219442198901f3252
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# Présentation de Kanban

Les sections suivantes vous permettent de mieux comprendre comment le [!UICONTROL Kanban] fonctions de panorama :

## [!UICONTROL Kanban] mise en page et fonctions de panorama

Le [!UICONTROL Kanban] Le panorama se compose des éléments suivants :

**Colonne de retard**: Affiche toutes les tâches actuellement en souffrance. Cette colonne n’est pas affichée par défaut. Pour plus d’informations sur le journal, y compris sur la manière de l’afficher sur le journal [!UICONTROL Kanban] panorama, voir [Gestion du journal en souffrance agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**États d’article**: Indique la progression d’un article en fonction de la colonne d’état dans laquelle se trouve l’article.

Pour plus d’informations, voir [Mettre à jour l’état des articles sur la variable [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Les statuts des articles peuvent être personnalisés pour le projet en modifiant la vue agile, comme décrit dans la section . [[!UICONTROL Création ou personnalisation d’une vue agile]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Présentation des vues dans [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Un maximum de cinquante cartes est affiché par défaut sur la carte Kanban, mais vous pouvez cliquer sur **[!UICONTROL Afficher plus]** pour afficher d’autres cartes.

## Relation entre les sous-tâches et les histoires

Si un article contient des sous-tâches, vous ne pouvez pas mettre à jour les informations sur l’article parent lui-même (comme les points/heures ou le pourcentage de fin). De plus, vous ne pouvez pas parcourir l’histoire [!UICONTROL Kanban] pour mettre à jour son état. Au contraire, tout changement que vous apportez aux sous-tâches de l&#39;histoire est reflété dans l&#39;histoire. Les points ou heures d’article combinés pour toutes les sous-tâches déterminent les points ou les heures de l’article parent.

Par exemple, si une histoire ne comporte qu’une seule sous-tâche évaluée à 4 points, l’histoire elle-même comporte également 4 points. Si vous définissez la valeur du point de sous-tâche sur 3, la valeur du point de l’article parent est remplacée par 3. Si vous créez une autre sous-tâche sur le même article et que vous définissez la valeur de point de cette sous-tâche sur 4, la valeur de point de l’article est remplacée par 7 afin de refléter la valeur de point combinée pour les deux sous-tâches.

Cette même logique s’applique aux sous-tâches de second niveau (sous-tâches de sous-tâches). Si une sous-tâche comporte une ou plusieurs sous-tâches de second niveau, la sous-tâche est calculée en fonction des sous-tâches de second niveau.

## Fonctionnalités prises en charge

Vous pouvez effectuer les opérations suivantes lors de l’utilisation du panorama Kanban :

* [Ajoutez une sous-tâche à un article existant sur la [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Ajoutez des tâches ou des problèmes existants au [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Affectez des utilisateurs à un article sur le [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Ajout d’articles et de problèmes à partir de [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Supprimer des articles ou des problèmes du [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Modifier les informations de l’article](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrage par utilisateur sur le [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Gérez la limite du travail en cours (WIP) sur la [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Réorganiser les articles sur la page [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Mettre à jour l’état des articles sur la variable [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Utilisez des indicateurs sur les articles de la [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Ajoutez le journal en souffrance au [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
