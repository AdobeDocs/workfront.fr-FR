---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Supprimer ou archiver une carte d’un panorama
description: Lorsque vous supprimez une carte d’un panorama, elle est définitivement supprimée et ne peut pas être restaurée. L’archivage d’une carte l’envoie à l’archive et vous pouvez la restaurer ultérieurement sur le panorama.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 6%

---

# Supprimer ou archiver une carte d’un panorama

Lorsque vous supprimez une carte ad hoc d’un panorama, elle est définitivement supprimée et ne peut pas être restaurée. Une fois supprimées, les cartes connectées peuvent être ajoutées manuellement à un panorama.

Si vous supprimez une carte connectée d’un panorama dynamique, elle réapparaîtra lorsque vous l’actualiserez, car ce type de panorama extrait toutes les tâches et tous les problèmes d’un projet spécifique. Pour supprimer la carte, vous devez supprimer la tâche ou le problème connecté du projet Workfront.

Lorsque vous supprimez une carte connectée d’un autre type de carte comportant une colonne d’entrée, la carte réapparaît dans la colonne d’entrée lorsque vous actualisez le panorama si la tâche ou le problème connecté n’est pas encore marqué comme terminé. Pour plus d’informations sur les colonnes d’ingestion, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

L’archivage d’une carte l’envoie à l’archive et vous pouvez la restaurer ultérieurement sur le panorama.

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
