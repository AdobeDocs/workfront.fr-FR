---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Vue d’ensemble de Kanban
description: Consultez cet article pour mieux comprendre le fonctionnement de la carte Kanban.
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: fa499d74df891441e729c32188e9b2f74e4ef5c0
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Vue d’ensemble de Kanban

<!-- Audited: 01/2024 -->

Les sections suivantes vous permettent de mieux comprendre le fonctionnement de la carte [!UICONTROL Kanban].

Pour une description de la méthodologie K[!UICONTROL anban], voir [Création d’une équipe agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Si vous souhaitez migrer d’un panorama [!UICONTROL Kanban] vers [!DNL Workfront] [!UICONTROL Panoramas], reportez-vous à la section [Migration de l’équipe agile [!UICONTROL Kanban] vers [!DNL Workfront] panoramas](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] présentation et fonctions du panorama

La carte [!UICONTROL Kanban] se compose des éléments suivants :

**Colonne de Backlog** : affiche toutes les tâches actuellement en souffrance. Cette colonne n’est pas affichée par défaut. Pour plus d’informations sur le journal, y compris sur la façon de l’afficher sur le panorama [!UICONTROL Kanban], voir [Gérer le journal agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**États d’article** : indique l’état d’un article en fonction de la colonne d’état dans laquelle se trouve l’article.

Pour plus d’informations, voir [Mise à jour de l’état des articles sur le [!UICONTROL panorama Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Les statuts des articles peuvent être personnalisés pour le projet en modifiant la vue agile, comme décrit dans la section [[!UICONTROL Créer ou personnaliser une vue agile]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) dans [Créer ou modifier des vues dans [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>Par défaut, le panorama Kanban affiche un maximum de cinquante cartes, mais vous pouvez cliquer sur **[!UICONTROL Afficher plus]** pour afficher d’autres cartes.

## Relation entre les sous-tâches et les histoires

Si un article contient des sous-tâches, vous ne pouvez pas mettre à jour les informations sur l’article parent lui-même (comme les points/heures ou le pourcentage de fin). De plus, vous ne pouvez pas déplacer l&#39;histoire sur le panorama [!UICONTROL Kanban] pour mettre à jour son statut. Au contraire, tout changement que vous apportez aux sous-tâches de l&#39;histoire est reflété dans l&#39;histoire. Les points ou heures d’article combinés pour toutes les sous-tâches déterminent les points ou les heures de l’article parent.

Par exemple, si une histoire ne comporte qu’une seule sous-tâche évaluée à 4 points, l’histoire elle-même comporte également 4 points. Si vous définissez la valeur du point de sous-tâche sur 3, la valeur du point de l’article parent est remplacée par 3. Si vous créez une autre sous-tâche sur le même article et que vous définissez la valeur de point de cette sous-tâche sur 4, la valeur de point de l’article est changée sur 7 afin de refléter la valeur de point combinée pour les deux sous-tâches.

Cette même logique s’applique aux sous-tâches de second niveau (sous-tâches de sous-tâches). Si une sous-tâche comporte une ou plusieurs sous-tâches de second niveau, la sous-tâche est calculée en fonction des sous-tâches de second niveau.

## Fonctionnalités prises en charge

Vous pouvez effectuer les opérations suivantes lors de l’utilisation du panorama Kanban :

* [Ajoutez une sous-tâche à un article existant sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Ajoutez des tâches ou des problèmes existants au panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Affectez des utilisateurs à un article sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Ajout d’articles et de problèmes sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Supprimer des articles ou des problèmes du panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Modifier les informations sur la story](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrage par utilisateur sur la carte [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Gérer la limite de travail en cours sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Réorganiser les articles sur la carte [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Mettez à jour l&#39;état des articles sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Utilisez des indicateurs sur les articles sur la carte [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Ajoutez le journal en souffrance à la carte [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
