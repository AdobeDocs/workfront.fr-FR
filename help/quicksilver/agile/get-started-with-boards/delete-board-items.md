---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Suppression ou archivage d’une carte d’un panorama
description: Lorsque vous supprimez une carte d’un panorama, elle est définitivement supprimée et ne peut pas être restaurée. L’archivage d’une carte l’envoie à l’archive et vous pouvez la restaurer ultérieurement sur le panorama.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: b6a824ac6248c86043f7f21866c8a14a6c97602f
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Suppression ou archivage d’une carte d’un panorama

Lorsque vous supprimez une carte d’un panorama, elle est définitivement supprimée et ne peut pas être restaurée. L’archivage d’une carte l’envoie à l’archive et vous pouvez la restaurer ultérieurement sur le panorama.

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

## Supprimer une carte d’un panorama

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) sur la carte, puis sélectionnez **[!UICONTROL Supprimer]**.
1. Cliquez sur **[!UICONTROL Supprimer]** sur le message de confirmation.

## Archiver une carte à partir d’un panorama

1. Accédez au panorama.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) sur la carte, puis sélectionnez **[!UICONTROL Archiver]**.

   Les cartes archivées sont masquées sur le panorama, sauf si vous appliquez un filtre pour les afficher. Pour plus d’informations, voir [Filtrage d’un panorama pour afficher les cartes archivées](#filter-a-board-to-show-archived-cards) dans cet article.

   Un [!UICONTROL Archiver] icon ![Archiver](assets/archive-icon-spectrum-25x20.png) s’affiche sur les cartes archivées. Vous ne pouvez pas modifier une carte archivée, mais vous pouvez la supprimer ou la déplacer vers une autre colonne.

1. Pour restaurer une carte archivée, cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) sur la carte et sélectionnez **[!UICONTROL Restaurer]**.

## Filtrage d’un panorama pour afficher les cartes archivées {#filter-a-board-to-show-archived-cards}

Par défaut, seules les cartes actives sont affichées sur un panorama. Vous pouvez filtrer le panorama pour afficher également toutes les cartes archivées.

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Configurer**] à droite du panorama pour ouvrir le panneau Configurer .
1. Développer [!UICONTROL **Cartes**].
1. Activer [!UICONTROL **Afficher les cartes archivées sur le panorama**].
1. Cliquez sur [!UICONTROL **Filtrer**], développez la variable [!UICONTROL Cartes archivées] et sélectionnez **[!UICONTROL Cartes archivées]** pour afficher toutes les cartes archivées.

   Le filtre affiche le nombre de cartes archivées.

   ![Filtrage des cartes archivées](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >La variable [!UICONTROL Cartes archivées] n’est pas disponible dans le filtre si vous n’avez pas activé le paramètre de configuration pour afficher les cartes archivées. Pour plus d’informations, voir [Personnalisation des champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Sélectionner **[!UICONTROL Cartes archivées]** pour effacer l’option et afficher uniquement les cartes actives.
