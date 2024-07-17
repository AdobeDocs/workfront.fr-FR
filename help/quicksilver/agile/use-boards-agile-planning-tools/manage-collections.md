---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Gérer les flux de travail
description: Un flux de travail est un groupe configurable de panoramas et de cartes pour collaborer sur le travail.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 24%

---

# Gérer les flux de travail

>[!IMPORTANT]
>
>Les flux de travail ne sont disponibles que pour un groupe spécifique de clients.

Un flux de travail est un groupe configurable de panoramas et de cartes pour collaborer sur le travail. Les flux de travail peuvent inclure différents types de panoramas créés à partir de modèles et une liste de cartes d’éléments de travail. Dans un flux de travail, vous pouvez effectuer le suivi du travail dans les itérations ou les empreintes.

Pour plus d’informations, voir [Utilisation de la liste de cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) et [Création d’une itération dans un workflow](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Les flux de travail apparaissent sur le tableau de bord avec les panoramas individuels auxquels vous avez accès et qui ne font pas partie d’un flux de travail. Pour plus d’informations sur le tableau de bord des panoramas, voir [Utilisation du tableau de bord des panoramas](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Vous pouvez cliquer sur le nom d’un panorama pour l’ouvrir.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Création d’un flux de travail

{{step1-to-boards}}

1. Cliquez sur **[!UICONTROL Ajouter un flux de travail]** dans la zone [!UICONTROL Flux de travail] du tableau de bord.
1. Saisissez un nom pour remplacer **[!UICONTROL Untitled Workstream]** et appuyez sur Entrée.

   Vous pouvez ajouter des panoramas au processus ou cliquer sur [!UICONTROL **Toutes les panoramas**] pour revenir au tableau de bord.

## Création d’un panorama dans un workflow

1. Si vous n’êtes pas déjà dans un flux de travail, cliquez sur [!UICONTROL **Afficher le flux de travail**] dans le tableau de bord pour ouvrir un flux de travail existant.
1. Cliquez sur **[!UICONTROL Ajouter un panorama]** dans l’onglet [!UICONTROL Panoramas] du processus.
1. Sélectionnez un modèle pour le panorama.

| Modèle | Description |
|---------|----------|
| Panorama de base | Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune politique de colonne n’est appliquée. |
| Panorama Kanban | Les colonnes suivantes sont fournies sur le panorama : Liste d’attente, Nouveau, En cours, Terminé et En attente. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut.<p>Pour utiliser la liste d’attente, vous devez configurer des filtres pour la colonne de saisie. Pour plus d’informations, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Pour consulter les politiques par défaut pour chaque colonne, cliquez sur le menu [!UICONTROL **Plus** ] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces politiques prédéfinies. Pour plus d’informations, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Panorama rétrospectif | Les colonnes suivantes sont fournies sur le panorama : Qu’est-ce qui a bien fonctionné ? Qu’est-ce qui pourrait être amélioré ? Qui devons-nous célébrer ? Que pouvons-nous faire pour aller plus vite ? Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune politique de colonne n’est appliquée. |
| Processus d’itération | Il s’agit du panorama utilisé pour définir et exécuter une itération. <p>Les colonnes suivantes sont fournies sur le panorama : Liste d’attente, Nouveau, En cours, Terminé et En attente. Vous ne pouvez pas ajouter de colonnes au panorama. <p>Pour passer en revue les stratégies par défaut pour chaque colonne, cliquez sur le menu [!UICONTROL **Plus**] d’une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces politiques prédéfinies. Pour plus d’informations, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Pour plus d’informations sur la configuration du panorama, voir [Création ou modification d’un panorama](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrage de la liste des panoramas sur un workflow

Lorsque des filtres autres que les valeurs par défaut sont appliqués sur la liste du panorama, un indicateur s’affiche sur l’icône de filtre ![Filtre appliqué](assets/boards-filterapplied-30x30.png). Cliquez sur [!UICONTROL **Effacer tout**] pour supprimer tous les filtres, puis sur [!UICONTROL **Masquer les filtres**] pour fermer le panneau des filtres.

{{step1-to-boards}}

1. Sur le tableau de bord, cliquez sur [!UICONTROL **Afficher le processus**] pour ouvrir un processus.
1. Cliquez sur l’onglet [!UICONTROL **Panoramas**] s’il n’est pas déjà affiché.
1. Cliquez sur [!UICONTROL **Filter**].
1. Sélectionnez les panoramas que vous souhaitez voir par statut (panoramas archivés, panoramas actifs ou tous panoramas).
1. Sélectionnez les panoramas que vous souhaitez voir par modèle.

## Ajout de membres à un workflow

Les personnes et les équipes doivent être ajoutées au workflow en tant que membres avant de pouvoir afficher le workflow et son contenu. Un membre du workflow peut ajouter et supprimer des membres dans le workflow et voir quels panoramas se trouvent dans le workflow.

>[!NOTE]
>
>Un membre du workflow ne peut pas ouvrir un panorama sur un workflow tant qu’il n’a pas été ajouté à ce panorama spécifique en tant que membre.

{{step1-to-boards}}

1. Sur le tableau de bord, cliquez sur [!UICONTROL **Afficher le processus**] pour ouvrir un processus.
1. Cliquez sur l&#39;icône **[!UICONTROL Ajouter un membre]** ![Ajouter des membres](assets/boards-addmember-spectrum-25x25.png) pour ajouter des membres et des équipes au workflow.

   Il s’agit du même processus que l’ajout de membres à un panorama. Pour plus d’informations, voir [Ajout ou suppression de membres d’un panorama](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Ajout de sources à un workflow

Une source détermine d’où viennent les cartes du processus.

{{step1-to-boards}}

1. Cliquez sur l&#39;icône [!UICONTROL **Sources**] ![Icône Sources](assets/sources-icon.png) pour définir une source permettant d&#39;importer des cartes dans le workflow. Actuellement, la seule source disponible est [!DNL Adobe Workfront].
1. Ajoutez des filtres pour importer les tâches et les problèmes de Workfront sous forme de cartes.

   L’ajout de filtres pour les sources de workflows est identique à l’ajout de filtres avancés pour une colonne d’entrée sur un panorama de base ou un panorama Kanban. Pour plus d’informations, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Configuration d’un workflow

{{step1-to-boards}}

1. Sur le tableau de bord, cliquez sur [!UICONTROL **Afficher le processus**] pour ouvrir un processus.
1. Cliquez sur [!UICONTROL **Configurer**] pour ouvrir le panneau [!UICONTROL Configurer le flux de travail].
1. (Facultatif) Développez [!UICONTROL **Workstream**] et saisissez une description du workflow. Cette description s’affiche sur le tableau de bord.
1. (Facultatif) Développez [!UICONTROL **Itérations**] pour définir un processus d’itération pour ce flux de travail.

   Le nombre total de cartes, le nombre de cartes pointées et le nombre d’itérations s’affichent dans la section Liste de cartes . Cliquez sur [!UICONTROL **Afficher la liste**] pour ouvrir la liste et ajouter des cartes. Pour plus d’informations, voir [Utilisation de la liste de cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Si une itération a déjà été définie, sa date de début, le nombre de cartes et le nombre de points s’affichent. Cliquez sur [!UICONTROL **Afficher le panorama**] pour ouvrir le panorama d’itération. Pour plus d’informations, voir [Création d’une itération dans un workflow](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Facultatif) Développez [!UICONTROL **Balises**] pour ajouter des balises au processus. Recherchez une balise ou saisissez un nouveau nom dans la zone de recherche, puis appuyez sur Entrée pour la créer.
