---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filtrage et recherche dans un panorama
description: Vous pouvez filtrer un panorama pour n’afficher que certaines cartes.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: 05cac2441474e0f6ecf18aa777a5a66fefb2dba8
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Filtrage et recherche dans un panorama

{{highlighted-preview}}

Vous pouvez filtrer un panorama pour afficher les éléments suivants :

* Cartes affectées à certaines personnes
* Cartes avec certaines balises
* Cartes avec un état spécifique
* Cartes arrivant à échéance dans une certaine période
* Cartes archivées
* Cartes connectées à un projet spécifique

<span class="preview">Le tri du panorama trie toutes les cartes des colonnes. Vous ne pouvez pas trier une seule colonne, et la colonne de journal ou d’entrée n’est pas triée.</span>

La recherche vous permet également de localiser une carte spécifique sur le panorama.

Lorsque des filtres sont appliqués, un indicateur s’affiche sur le panorama. ![Filtre appliqué au panorama](assets/boards-filterapplied-30x30.png). Cliquez sur **[!UICONTROL Effacer tout]** pour supprimer tous les filtres du panorama, cliquez sur **[!UICONTROL Masquer les filtres]** pour fermer le panneau de filtrage.

![Panneau Filtrer](assets/boards-all-filters-collapsed-1022.png)

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Filtrage d’un panorama par personne désignée

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Création ou modification d’un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur [!UICONTROL **Filtrer**], développez la variable [!UICONTROL Membres] et sélectionnez la ou les personnes dont vous souhaitez afficher les cartes. Vous pouvez également afficher les cartes non affectées.

   ![Filtrer par membre](assets/boards-filter-by-assignees-0822.png)

## Filtrage d’un panorama par balises

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la variable [!UICONTROL Balises] et sélectionnez les balises à afficher.

   ![Filtrage par balise](assets/boards-filter-by-tags-0822.png)

## Filtrage d’un panorama par statut

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la variable [!UICONTROL Statuts] et sélectionnez les types d’état à afficher.

   Vous pouvez également masquer les cartes terminées.

   ![Filtrage par statut](assets/boards-filter-by-status-0822.png)

## Filtrage d’un panorama par date d’échéance

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la variable [!UICONTROL Date d’échéance] et sélectionnez les options de date à afficher.

   Seules les cartes des périodes sélectionnées s’affichent.

   ![Filtrer par date d’échéance](assets/boards-filter-by-due-date-0822.png)

## Filtrage d’un panorama pour afficher les cartes archivées

Par défaut, seules les principales cartes sont affichées sur un panorama. Vous pouvez filtrer le panorama pour afficher également toutes les cartes archivées.

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la variable [!UICONTROL Cartes archivées] et sélectionnez **[!UICONTROL Cartes archivées]** pour afficher toutes les cartes archivées.

   Le filtre affiche le nombre de cartes archivées.

   ![Filtrage des cartes archivées](assets/boards-filter-by-archived-cards_0822.png)

1. Sélectionner **[!UICONTROL Cartes archivées]** pour effacer l’option et afficher uniquement les principales cartes.

## Filtrage d’un panorama par connexion

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Filtrer**], développez la variable [!UICONTROL Connexion] , puis sélectionnez la variable [!DNL Workfront] projets pour les cartes connectées que vous souhaitez afficher.

   Vous pouvez également afficher les cartes qui ne sont pas connectées à un projet.

   ![Filtrage par connexion](assets/boards-filter-by-connection.png)

<div class="preview">

## Tri sur un panorama

Lorsque vous sélectionnez une option de tri, toutes les colonnes sont triées. Vous ne pouvez pas trier une seule colonne, et la colonne de journal ou d’entrée n’est pas triée.

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Tri par**] et sélectionnez [!UICONTROL **Nom**], [!UICONTROL **Échéance**], [!UICONTROL **Estimation**], [!UICONTROL **État**] ou [!UICONTROL **Connexion**].

   La connexion (nom du projet) s’applique uniquement aux cartes connectées, et les autres options trient les cartes connectées et ad hoc dans les colonnes.

   L’option &quot;commande utilisateur&quot; renvoie les cartes dans l’ordre dans lequel elles ont été définies manuellement, avant toute autre option de tri. Il s’agit du tri par défaut des colonnes.

1. Sélectionner [!UICONTROL **Ordre inverse**] pour trier les colonnes dans l’ordre inverse de l’option de tri.

   La flèche sur l’icône de tri indique si les colonnes sont triées par ordre croissant ou décroissant.

   Lorsqu’un tri autre que le tri par défaut est appliqué, un indicateur s’affiche sur l’icône de tri. ![Tri appliqué](assets/sort-applied-boards.png).

   ![Tri par colonnes sur un panorama](assets/sort-by-columns-in-board.png)

</div>

## Recherche dans un panorama

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Rechercher**] et saisissez un terme de recherche. Ensuite, appuyez sur Entrée.

   Toutes les cartes qui contiennent le terme de recherche s’affichent.

   Cliquez sur le X pour effacer la recherche.

   ![Recherche de cartes dans un panorama](assets/boards-searchbox.png)
