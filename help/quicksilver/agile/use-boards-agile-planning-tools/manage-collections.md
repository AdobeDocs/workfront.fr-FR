---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Gestion des workflows
description: Un flux de travail est un groupe configurable de panoramas et de cartes pour collaborer sur le travail.
author: Lisa
feature: Agile
source-git-commit: 16e96d55932116cb475eecbe8b6ebfd4661eb494
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# Gestion des workflows

{{highlighted-preview}}

>[!NOTE]
>
>Les flux de travail sont disponibles dans l’environnement Aperçu et dans Production par le biais de l’accord préalable à la fonctionnalité pour [!UICONTROL [!DNL Workfront] Panoramas]. Pour plus d’informations, voir [Inclusion anticipée des fonctionnalités pour les panoramas Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

Un flux de travail est un groupe configurable de panoramas et de cartes pour collaborer sur le travail. Les flux de travail peuvent inclure différents types de panoramas créés à partir de modèles, <span class="preview">et une liste de cartes des tâches. Dans un flux de travail, vous pouvez effectuer le suivi du travail dans les itérations ou les empreintes.</span>

<span class="preview">Pour plus d’informations, voir [Utiliser la liste des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) et [Créer une itération](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).</span>

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

1. Cliquez sur **[!UICONTROL Ajouter un workflow]** dans le [!UICONTROL Workflows] du tableau de bord.
1. Saisissez un nom à remplacer. **[!UICONTROL Processus sans titre]** et appuyez sur Entrée.

   Vous pouvez ajouter des panoramas au processus ou cliquer sur [!UICONTROL **Toutes les panoramas**] pour revenir au tableau de bord.

## Création d’un panorama dans un workflow

1. Si vous n’êtes pas déjà dans un flux de travail, cliquez sur [!UICONTROL **Afficher le flux de travail**] sur le tableau de bord pour ouvrir un flux de travail existant.
1. Cliquez sur **[!UICONTROL Ajouter un panorama]** sur le [!UICONTROL Panoramas] de workflows.
1. Sélectionnez un modèle pour le panorama.

| Modèle | Description |
|---------|----------|
| Panorama de base | Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune stratégie de colonne n’est appliquée. |
| Panorama Kanban | Les colonnes suivantes sont fournies sur le panorama : En attente, nouveauté, En cours, Terminé et En attente. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut.<p>Pour utiliser le journal des logs, vous devez configurer des filtres pour la colonne d&#39;ingestion. Pour plus d’informations, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Pour consulter les stratégies par défaut pour chaque colonne, cliquez sur le bouton [!UICONTROL **Plus** menu] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces stratégies prédéfinies. Pour plus d’informations, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Panorama rétrospectif | Les colonnes suivantes sont fournies sur le panorama : Qu&#39;est-ce qui s&#39;est bien passé ? Améliorations possibles? Qui devons-nous célébrer? Que pouvons-nous faire pour aller plus vite? Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune stratégie de colonne n’est appliquée. |
| <span class="preview">Processus d’itération</span> | <span class="preview">Il s’agit du panorama utilisé pour définir et exécuter une itération. <p>Les colonnes suivantes sont fournies sur le panorama : En attente, nouveauté, En cours, Terminé et En attente. Vous ne pouvez pas ajouter de colonnes au panorama. <p>Pour consulter les stratégies par défaut pour chaque colonne, cliquez sur le bouton [!UICONTROL **Plus**] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces stratégies prédéfinies. Pour plus d’informations, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

Pour plus d’informations sur la configuration du panorama, voir [Création ou modification d’un panorama](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrage de la liste des panoramas sur un workflow

Lorsque des filtres autres que les valeurs par défaut sont appliqués sur la liste des panoramas, un indicateur s’affiche sur l’icône de filtrage. ![Filtre appliqué](assets/boards-filterapplied-30x30.png). Cliquez sur [!UICONTROL **Effacer tout**] pour supprimer tous les filtres, cliquez sur [!UICONTROL **Masquer les filtres**] pour fermer le panneau de filtrage.

{{step1-to-boards}}

1. Dans le tableau de bord, cliquez sur [!UICONTROL **Afficher le flux de travail**] pour ouvrir un workflow.
1. Cliquez sur le bouton [!UICONTROL **Panoramas**] s’il n’est pas déjà affiché.
1. Cliquez sur [!UICONTROL **Filtrer**].
1. Sélectionnez les panoramas que vous souhaitez voir par statut (panoramas archivés, principaux panoramas ou tous panoramas).
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

<div class="preview">

## Configuration d’un flux de travail

{{step1-to-boards}}

1. Dans le tableau de bord, cliquez sur [!UICONTROL **Afficher le flux de travail**] pour ouvrir un workflow.
1. Cliquez sur [!UICONTROL **Configurer**] pour ouvrir le [!UICONTROL Configuration de Workstream] du panneau.
1. (Facultatif) Saisissez une description du processus. Cette description s’affiche sur le tableau de bord.

   Le nombre total de cartes, le nombre de cartes pointées et le nombre d’itérations s’affichent dans la section Liste de cartes . Cliquez sur [!UICONTROL **Afficher la liste**] pour ouvrir la liste et ajouter des cartes. Pour plus d’informations, voir [Utiliser la liste des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Si une itération a été définie, sa date de début, le nombre de cartes et le nombre de points s’affichent. Cliquez sur [!UICONTROL **Afficher le panorama d’itération**] pour ouvrir le panorama. Pour plus d’informations, voir [Créer une itération](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).

1. Cliquez sur [!UICONTROL **Ajouter une source**] pour définir une source permettant d’importer des cartes dans le workflow. Actuellement, la seule source disponible est [!DNL Adobe Workfront].
1. Ajoutez des filtres pour importer les tâches et les problèmes de Workfront sous forme de cartes.

   L’ajout de filtres pour les sources de workflows est identique à l’ajout de filtres pour une colonne d’entrée sur un panorama de base ou un panorama Kanban. Pour plus d’informations, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

</div>
