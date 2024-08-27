---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Gestion des workflows
description: Un flux de travail est un groupe configurable de panoramas et de cartes permettant de collaborer.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 99%

---

# Gérer les flux de travail

>[!IMPORTANT]
>
>Les flux de travail ne sont disponibles que pour un groupe spécifique de clientes et de clients.

Un flux de travail est un groupe configurable de panoramas et de cartes permettant de collaborer. Les flux de travail peuvent inclure différents types de panoramas créés à partir de modèles et une liste de cartes d’éléments de travail. Dans un flux de travail, vous pouvez effectuer le suivi du travail dans des itérations ou des sprints.

Pour plus d’informations, voir [Utiliser la liste des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) et [Créer une itération dans un flux de travail](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Les flux de travail apparaissent sur le tableau de bord avec des panoramas individuels auxquels vous avez accès et qui ne font pas partie d’un flux de travail. Pour plus d’informations sur le tableau de bord des panoramas, voir [Utiliser le tableau de bord des panoramas](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Vous pouvez cliquer sur le nom d’un panorama pour l’ouvrir.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> 
   <p>Nouvelle : [!UICONTROL Contributor] ou niveau supérieur</p> 
   <p>ou</p>
   <p>Actuel : [!UICONTROL Request] ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un flux de travail

{{step1-to-boards}}

1. Cliquez sur **[!UICONTROL Ajouter un flux de travail]** dans la zone [!UICONTROL Flux de travail] du tableau de bord.
1. Saisissez un nom pour remplacer **[!UICONTROL Flux de travail sans titre]** et appuyez sur Entrée.

   Vous pouvez ajouter des panoramas au flux de travail ou cliquer sur [!UICONTROL **Tous les panoramas**] pour revenir au tableau de bord.

## Créer un panorama dans un flux de travail

1. Si vous n’êtes pas déjà dans un flux de travail, cliquez sur [!UICONTROL **Afficher le flux de travail**] sur le tableau de bord pour ouvrir un flux de travail existant.
1. Cliquez sur **[!UICONTROL Ajouter un panorama]** sur l’onglet [!UICONTROL Panoramas] du flux de travail.
1. Sélectionnez un modèle pour le panorama.

| Modèle | Description |
|---------|----------|
| Panorama de base | Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune politique de colonne n’est appliquée. |
| Panorama Kanban | Les colonnes suivantes sont fournies sur le panorama : Liste d’attente, Nouveau, En cours, Terminé et En attente. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut.<p>Pour utiliser la liste d’attente, vous devez configurer des filtres pour la colonne de saisie. Pour plus d’informations, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Pour consulter les politiques par défaut pour chaque colonne, cliquez sur le menu Plus  sur une colonne et sélectionnez Modifier. [!UICONTROL ****][!UICONTROL ****] Vous pouvez modifier l’une de ces politiques prédéfinies. Pour plus d’informations, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Panorama rétrospectif | Les colonnes suivantes sont fournies sur le panorama : Qu’est-ce qui a bien fonctionné ? Qu’est-ce qui pourrait être amélioré ? Qui devons-nous célébrer ? Que pouvons-nous faire pour aller plus vite ? Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune politique de colonne n’est appliquée. |
| Processus d’itération | Il s’agit du panorama utilisé pour définir et exécuter une itération. <p>Les colonnes suivantes sont fournies sur le panorama : Liste d’attente, Nouveau, En cours, Terminé et En attente. Vous ne pouvez pas ajouter de colonnes au panorama. <p>Pour revoir les politiques par défaut de chaque colonne, cliquez sur le menu [!UICONTROL **Plus**] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces politiques prédéfinies. Pour plus d’informations, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Pour plus d’informations sur la configuration du panorama, consultez [Créer ou modifier un panorama](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrer la liste des panoramas sur un flux de travail

Lorsque des filtres autres que les valeurs par défaut sont appliqués sur la liste des panoramas, un indicateur s’affiche sur l’icône de filtrage ![Filtre appliqué](assets/boards-filterapplied-30x30.png). Cliquez sur [!UICONTROL **Effacer tout**] pour supprimer tous les filtres et cliquez sur [!UICONTROL **Masquer les filtres**] pour fermer le panneau de filtrage.

{{step1-to-boards}}

1. Dans le tableau de bord, cliquez sur [!UICONTROL **Afficher le flux de travail**] pour ouvrir un flux de travail.
1. Cliquez sur l’onglet [!UICONTROL **Panoramas**] s’il n’est pas déjà affiché.
1. Cliquez sur [!UICONTROL **Filtrer**].
1. Sélectionnez les panoramas que vous souhaitez voir par statut (panoramas archivés, panoramas actifs ou tous les panoramas).
1. Sélectionnez les panoramas que vous souhaitez voir par modèle.

## Ajouter des membres à un flux de travail

Les personnes et les équipes doivent être ajoutées au flux de travail en tant que membres avant de pouvoir afficher le flux de travail et son contenu. Une personne membre du flux de travail peut ajouter et supprimer des personnes membres dans le flux de travail et voir quels panoramas se trouvent dans le flux de travail.

>[!NOTE]
>
>Une personne membre du flux de travail ne peut pas ouvrir un panorama sur un flux de travail tant qu’elle n’a pas été ajoutée à ce panorama spécifique en tant que membre.

{{step1-to-boards}}

1. Dans le tableau de bord, cliquez sur [!UICONTROL **Afficher le flux de travail**] pour ouvrir un flux de travail.
1. Cliquez sur l’icône **[!UICONTROL Ajouter une personne membre]** ![Ajouter des membres](assets/boards-addmember-spectrum-25x25.png) pour ajouter des personnes membres et des équipes au flux de travail.

   Il s’agit du même processus que l’ajout de personnes membres à un panorama. Pour plus d’informations, voir [Ajouter ou supprimer des membres d’un panorama](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Ajouter des sources à un flux de travail

Une source détermine d’où viennent les cartes du flux de travail.

{{step1-to-boards}}

1. Cliquez sur l’icône [!UICONTROL **Sources**] ![Icône Sources](assets/sources-icon.png) pour définir une source permettant d’importer des cartes dans le flux de travail. Actuellement, la seule source disponible est [!DNL Adobe Workfront].
1. Ajoutez des filtres pour importer les tâches et les problèmes de Workfront sous forme de cartes.

   L’ajout de filtres pour les sources de flux de travail est identique à l’ajout de filtres avancés pour une colonne d’entrée sur un panorama de base ou un tableau Kanban. Pour plus d’informations, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Configurer le flux de travail

{{step1-to-boards}}

1. Dans le tableau de bord, cliquez sur [!UICONTROL **Afficher le flux de travail**] pour ouvrir un flux de travail.
1. Cliquez sur [!UICONTROL **Configurer**] pour ouvrir le panneau [!UICONTROL Configurer le flux de travail].
1. (Facultatif) Développez [!UICONTROL **Flux de travail**] et saisissez une description du flux de travail. Cette description s’affiche sur le tableau de bord.
1. (Facultatif) Développez [!UICONTROL **Itérations**] pour définir un processus d’itération pour ce flux de travail.

   Le nombre total de cartes, le nombre de cartes avec des points et le nombre d’itérations s’affichent dans la section Liste des cartes. Cliquez sur [!UICONTROL **Afficher la liste**] pour ouvrir la liste et ajouter des cartes. Pour plus d’informations, consultez [Utiliser la liste des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Si une itération a déjà été définie, sa date de début, le nombre de cartes et le nombre de points s’affichent. Cliquez sur [!UICONTROL **Afficher le panorama**] pour ouvrir le panorama d’itération. Pour plus d’informations, voir [Créer une itération dans un flux de travail](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Facultatif) Développez [!UICONTROL **Balises**] pour ajouter des balises au flux de travail. Recherchez une balise ou saisissez un nouveau nom dans la zone de recherche, puis appuyez sur Entrée pour la créer.
