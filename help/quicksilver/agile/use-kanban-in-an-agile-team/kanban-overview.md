---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Présentation De Kanban
description: Consultez cet article pour mieux comprendre le fonctionnement du tableau Kanban.
author: Jenny
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 88%

---

# Vue d’ensemble Kanban

<!-- Audited: 01/2024 -->

Les sections suivantes permettent de mieux comprendre le fonctionnement du panorama [!UICONTROL Kanban].

Pour une description de la méthodologie K[!UICONTROL anban], voir [Créer une équipe Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

Si vous souhaitez migrer d’une équipe agile [!UICONTROL tableau Kanban] vers des [!DNL Workfront] [!UICONTROL tableaux], consultez [Migrer les cartes de l’équipe agile [!UICONTROL Kanban] vers des  [!DNL Workfront] tableaux](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## Disposition et fonctions des panoramas [!UICONTROL Kanban]

Le panorama [!UICONTROL Kanban] se compose des éléments suivants :

**Colonne de liste d’attente** : affiche toutes les tâches actuellement en liste d’attente. Par défaut, cette colonne n’est pas affichée. Pour plus d’informations sur la liste d’attente, y compris sur son affichage sur le panorama [!UICONTROL Kanban], voir [Gérer la liste d’attente Agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**Statuts de story** : indique le déroulement d’une story en fonction de la colonne de statut dans laquelle elle se trouve.

Pour plus d’informations, voir la section [Mettre à jour le statut des histoires sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

Les statuts des histoires peuvent être personnalisés pour le projet en modifiant la vue agile, comme décrit dans la section [[!UICONTROL Créer ou personnaliser une vue Agile]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) dans [Créer ou modifier des vues dans  [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>Un maximum de cinquante cartes est affiché par défaut sur le tableau Kanban, mais vous pouvez cliquer sur **[!UICONTROL Afficher plus]** pour afficher d’autres cartes.

## Relation entre les sous-tâches et les histoires

Si une histoire contient des sous-tâches, vous ne pouvez mettre à jour aucune information sur l’histoire parent (comme les points/heures ou le pourcentage terminé). De plus, vous ne pouvez pas déplacer l’histoire sur le panorama [!UICONTROL Kanban] pour mettre à jour son statut. Au contraire, tout changement que vous apportez aux sous-tâches de l’histoire est reflété dans l’histoire. Les points ou les heures de l’histoire combinés pour toutes les sous-tâches déterminent les points ou les heures de l’histoire parent.

Par exemple, si une histoire ne comporte qu’une seule sous-tâche évaluée à 4 points, l’histoire elle-même comporte également 4 points. Si vous remplacez la valeur du point de sous-tâche sur 3, la valeur du point de l’histoire parent est aussi remplacée par 3. Si vous créez une autre sous-tâche sur la même histoire et que vous définissez la valeur du point de cette sous-tâche sur 4, la valeur du point de l’histoire est remplacée par 7 afin de refléter la valeur de point combinée pour les deux sous-tâches.

Cette même logique s’applique aux sous-tâches de deuxième niveau (sous-tâches de sous-tâches). Si une sous-tâche comporte une ou plusieurs sous-tâches de deuxième niveau, elle est calculée en fonction des sous-tâches de deuxième niveau.

## Fonctionnalités prises en charge

Vous pouvez effectuer les opérations suivantes lorsque vous utilisez le tableau Kanban :

* [Ajouter une sous-tâche à une histoire existante sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [Ajouter des tâches ou des problèmes existants au panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [Affecter des utilisateurs et utilisatrices à une histoire sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [Ajouter des histoires et des problèmes à partir du panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [Supprimer des histoires ou des problèmes du panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [Modifier les informations d’une histoire](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [Filtrer par utilisateur ou utilisatrice sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [Gérer la limite du travail en cours (WIP) sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [Réorganiser les histoires sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [Mettre à jour le statut des histoires sur le panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [Utiliser des indicateurs sur les histoires du panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [Ajouter la liste d’attente au panorama [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
