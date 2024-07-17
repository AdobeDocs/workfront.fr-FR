---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filtrer et rechercher dans un panorama
description: Vous pouvez filtrer un panorama pour n’afficher que certaines cartes.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: b6a824ac6248c86043f7f21866c8a14a6c97602f
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 12%

---

# Filtrer et rechercher dans un panorama

Vous pouvez filtrer un panorama pour afficher les éléments suivants :

* Cartes affectées à certaines personnes
* Cartes avec certaines balises
* Cartes avec un état spécifique
* Cartes arrivant à échéance dans une certaine période
* Cartes archivées
* Cartes connectées à un projet spécifique

Le tri du panorama trie toutes les cartes des colonnes. Vous ne pouvez pas trier une seule colonne, et la colonne de journal ou d’entrée n’est pas triée.

La recherche vous permet également de localiser une carte spécifique sur le panorama.

Lorsque des filtres sont appliqués, un indicateur s’affiche sur le panorama ![Filtre appliqué au panorama](assets/boards-filterapplied-30x30.png). Cliquez sur **[!UICONTROL Effacer tout]** pour supprimer tous les filtres du panorama, puis cliquez sur l’icône Réduire pour fermer le panneau de filtrage.

![Panneau de filtrage](assets/boards-all-filters-collapsed-0823.png)

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Filtrage d’un panorama par personne désignée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur [!UICONTROL **Filtrer**], développez la section [!UICONTROL Membres] et sélectionnez la ou les personnes dont vous souhaitez afficher les cartes. Vous pouvez également afficher les cartes non affectées.

   ![Filtre par membre](assets/boards-filter-by-assignees-0822.png)

## Filtrage d’un panorama par balises

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la section [!UICONTROL Balises] et sélectionnez les balises à afficher.

   ![Filtrer par balise](assets/boards-filter-by-tags-0822.png)

## Filtrage d’un panorama par statut

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la section [!UICONTROL Statuts] et sélectionnez les types d’état que vous souhaitez afficher.

   Vous pouvez également masquer les cartes terminées.

   ![Filtrer par statut](assets/boards-filter-by-status-0822.png)

## Filtrage d’un panorama par date d’échéance

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la section [!UICONTROL Date d’échéance] et sélectionnez les options de date à afficher.

   Seules les cartes des périodes sélectionnées s’affichent.

   ![Filtrer par date d’échéance](assets/boards-filter-by-due-date-0822.png)

## Filtrage d’un panorama pour afficher les cartes archivées

Par défaut, seules les cartes actives sont affichées sur un panorama. Vous pouvez filtrer le panorama pour afficher également toutes les cartes archivées.

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Configurer**] à droite du panorama pour ouvrir le panneau Configurer.
1. Développez [!UICONTROL **Cartes**].
1. Activez [!UICONTROL **Afficher les cartes archivées sur le panorama**].
1. Cliquez sur [!UICONTROL **Filtrer**], développez la section [!UICONTROL Cartes archivées] et sélectionnez **[!UICONTROL Cartes archivées]** pour afficher toutes les cartes archivées.

   Le filtre affiche le nombre de cartes archivées.

   ![Filtrer les cartes archivées](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >La section [!UICONTROL Cartes archivées] n’est pas disponible dans le filtre si vous n’avez pas activé le paramètre de configuration pour afficher les cartes archivées. Pour plus d’informations, voir [Personnaliser des champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Sélectionnez à nouveau **[!UICONTROL Cartes archivées]** pour effacer l’option et afficher uniquement les cartes actives.

## Filtrage d’un panorama par connexion

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la section [!UICONTROL Connexion] et sélectionnez les projets [!DNL Workfront] pour les cartes connectées que vous souhaitez voir.

   Vous pouvez également afficher les cartes qui ne sont pas connectées à un projet.

   ![Filtrer par connexion](assets/boards-filter-by-connection.png)

## Tri sur un panorama

Lorsque vous sélectionnez une option de tri, toutes les colonnes sont triées. Vous ne pouvez pas trier une seule colonne, et la colonne de journal ou d’entrée n’est pas triée.

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Trier par**] et sélectionnez [!UICONTROL **Nom**], [!UICONTROL **Date d’échéance**], [!UICONTROL **Estimation**], [!UICONTROL **État**] ou [!UICONTROL **Connexion**].

   La connexion (nom du projet) s’applique uniquement aux cartes connectées, et les autres options trient les cartes connectées et les cartes ad hoc dans les colonnes.

   L’option &quot;commande utilisateur&quot; renvoie les cartes dans l’ordre dans lequel elles ont été définies manuellement, avant toute autre option de tri. Il s’agit du tri par défaut des colonnes.

1. Sélectionnez [!UICONTROL **Ordre inverse**] pour trier les colonnes dans l’ordre inverse de l’option de tri.

   La flèche sur l’icône de tri indique si les colonnes sont triées par ordre croissant ou décroissant.

   Lorsqu’un tri autre que le tri par défaut est appliqué, un indicateur s’affiche sur l’icône de tri ![Tri appliqué](assets/sort-applied-boards.png).

   ![Tri par colonnes sur un panorama](assets/sort-by-columns-in-board.png)

## Recherche dans un panorama

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Rechercher**] et saisissez un terme de recherche. Ensuite, appuyez sur Entrée.

   Toutes les cartes qui contiennent le terme de recherche s’affichent.

   Cliquez sur le X pour effacer la recherche.

   ![Recherche de cartes dans un panorama](assets/boards-searchbox.png)
