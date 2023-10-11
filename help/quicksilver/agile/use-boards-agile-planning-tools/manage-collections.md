---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Gestion des workflows
description: Un flux de travail est un groupe configurable de panoramas et de cartes pour collaborer sur le travail.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 2%

---

# Gestion des workflows

>[!IMPORTANT]
>
>Les flux de travail ne sont disponibles que pour un groupe spécifique de clients.

Un flux de travail est un groupe configurable de panoramas et de cartes pour collaborer sur le travail. Les flux de travail peuvent inclure différents types de panoramas créés à partir de modèles et une liste de cartes d’éléments de travail. Dans un flux de travail, vous pouvez effectuer le suivi du travail dans les itérations ou les empreintes.

Pour plus d’informations, voir [Utiliser la liste des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) et [Création d’une itération dans un workflow](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Les flux de travail apparaissent sur le tableau de bord avec les panoramas individuels auxquels vous avez accès et qui ne font pas partie d’un flux de travail. Pour plus d’informations sur le tableau de bord des panoramas, voir [Utilisation du tableau de bord des panoramas](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Vous pouvez cliquer sur le nom d’un panorama pour l’ouvrir.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

## Création d’un flux de travail

{{step1-to-boards}}

1. Cliquez sur **[!UICONTROL Ajout d’un workflow]** dans le [!UICONTROL Workflows] du tableau de bord.
1. Saisissez un nom à remplacer. **[!UICONTROL Processus sans titre]** et appuyez sur Entrée.

   Vous pouvez ajouter des panoramas au processus ou cliquer sur [!UICONTROL **Toutes les panoramas**] pour revenir au tableau de bord.

## Création d’un panorama dans un workflow

1. Si vous n’êtes pas déjà dans un workflow, cliquez sur [!UICONTROL **Afficher le flux de travail**] sur le tableau de bord pour ouvrir un flux de travail existant.
1. Cliquez sur **[!UICONTROL Ajouter un panorama]** sur le [!UICONTROL Panoramas] de workflows.
1. Sélectionnez un modèle pour le panorama.

| Modèle | Description |
|---------|----------|
| Panorama de base | Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune stratégie de colonne n’est appliquée. |
| Panorama Kanban | Les colonnes suivantes sont fournies sur le tableau : Backlog, New, In Progress, Complete et On hold. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut.<p>Pour utiliser le journal des logs, vous devez configurer des filtres pour la colonne d&#39;ingestion. Pour plus d’informations, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Pour consulter les stratégies par défaut pour chaque colonne, cliquez sur le bouton [!UICONTROL **Plus** menu] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces stratégies prédéfinies. Pour plus d’informations, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Panorama rétrospectif | Les colonnes suivantes sont fournies sur le tableau : Qu’est-ce qui s’est bien passé ? Améliorations possibles? Qui devons-nous célébrer? Que pouvons-nous faire pour aller plus vite? Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune stratégie de colonne n’est appliquée. |
| Processus d’itération | Il s’agit du panorama utilisé pour définir et exécuter une itération. <p>Les colonnes suivantes sont fournies sur le tableau : Backlog, New, In Progress, Complete et On hold. Vous ne pouvez pas ajouter de colonnes au panorama. <p>Pour consulter les stratégies par défaut pour chaque colonne, cliquez sur le bouton [!UICONTROL **Plus**] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces stratégies prédéfinies. Pour plus d’informations, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Pour plus d’informations sur la configuration du panorama, voir [Créer ou modifier un panorama](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrage de la liste des panoramas sur un workflow

Lorsque des filtres autres que les valeurs par défaut sont appliqués sur la liste des panoramas, un indicateur s’affiche sur l’icône de filtrage. ![Filtre appliqué](assets/boards-filterapplied-30x30.png). Cliquez sur [!UICONTROL **Effacer tout**] pour supprimer tous les filtres, cliquez sur [!UICONTROL **Masquer les filtres**] pour fermer le panneau de filtrage.

{{step1-to-boards}}

1. Dans le tableau de bord, cliquez sur [!UICONTROL **Afficher le flux de travail**] pour ouvrir un workflow.
1. Cliquez sur le bouton [!UICONTROL **Panoramas**] s’il n’est pas déjà affiché.
1. Cliquez sur [!UICONTROL **Filtrer**].
1. Sélectionnez les panoramas que vous souhaitez voir par statut (panoramas archivés, panoramas actifs ou tous panoramas).
1. Sélectionnez les panoramas que vous souhaitez voir par modèle.

## Ajout de membres à un workflow

Les personnes et les équipes doivent être ajoutées au workflow en tant que membres avant de pouvoir afficher le workflow et son contenu. Un membre du workflow peut ajouter et supprimer des membres dans le workflow et voir quels panoramas se trouvent dans le workflow.

>[!NOTE]
>
>Un membre du workflow ne peut pas ouvrir un panorama sur un workflow tant qu’il n’a pas été ajouté à ce panorama spécifique en tant que membre.

{{step1-to-boards}}

1. Dans le tableau de bord, cliquez sur [!UICONTROL **Afficher le flux de travail**] pour ouvrir un workflow.
1. Cliquez sur le bouton **[!UICONTROL Ajouter un membre]** icon ![Ajouter des membres](assets/boards-addmember-spectrum-25x25.png) pour ajouter des membres et des équipes au workflow.

   Il s’agit du même processus que l’ajout de membres à un panorama. Pour plus d’informations, voir [Ajout ou suppression de membres d’un panorama](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Ajout de sources à un workflow

Une source détermine d’où viennent les cartes du processus.

{{step1-to-boards}}

1. Cliquez sur le bouton [!UICONTROL **Sources**] icon ![Icône Sources](assets/sources-icon.png) pour définir une source permettant d’importer des cartes dans le workflow. Actuellement, la seule source disponible est [!DNL Adobe Workfront].
1. Ajoutez des filtres pour importer les tâches et les problèmes de Workfront sous forme de cartes.

   L’ajout de filtres pour les sources de workflows est identique à l’ajout de filtres avancés pour une colonne d’entrée sur un panorama de base ou un panorama Kanban. Pour plus d’informations, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Configuration d’un workflow

{{step1-to-boards}}

1. Dans le tableau de bord, cliquez sur [!UICONTROL **Afficher le flux de travail**] pour ouvrir un workflow.
1. Cliquez sur [!UICONTROL **Configurer**] pour ouvrir le [!UICONTROL Configuration du flux de travail] du panneau.
1. (Facultatif) Développez [!UICONTROL **Workflows**] et saisissez une description du processus. Cette description s’affiche sur le tableau de bord.
1. (Facultatif) Développez [!UICONTROL **Itérations**] pour définir un processus d’itération pour ce workflow.

   Le nombre total de cartes, le nombre de cartes pointées et le nombre d’itérations s’affichent dans la section Liste de cartes . Cliquez sur [!UICONTROL **Afficher la liste**] pour ouvrir la liste et ajouter des cartes. Pour plus d’informations, voir [Utiliser la liste des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Si une itération a déjà été définie, sa date de début, le nombre de cartes et le nombre de points s’affichent. Cliquez sur [!UICONTROL **Afficher le panorama**] pour ouvrir le panorama d’itération. Pour plus d’informations, voir [Création d’une itération dans un workflow](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Facultatif) Développez [!UICONTROL **Balises**] pour ajouter des balises au workflow. Recherchez une balise ou saisissez un nouveau nom dans la zone de recherche, puis appuyez sur Entrée pour la créer.
