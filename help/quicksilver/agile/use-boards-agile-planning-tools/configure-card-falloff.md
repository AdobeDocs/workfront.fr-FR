---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Configuration des abandons de carte
description: Vous pouvez configurer un panorama afin que les cartes soient archivées ou abandonnées selon un calendrier précis.
author: Lisa
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Configuration des abandons de carte

Vous pouvez configurer un panorama afin que les cartes soient archivées ou &quot;tombent&quot; du panorama selon un calendrier précis. Vous pouvez définir des cartes dans une colonne spécifique pour qu’elles ne soient plus incluses dans le panorama au cours d’un certain nombre de jours ou de semaines.

Lorsqu’une carte tombe hors du panorama, elle est archivée. Vous pouvez afficher les cartes archivées avec un filtre. Pour plus d’informations, voir [Filtrage et recherche dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Configuration des abandons de carte

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau Configurer .
1. Développer **[!UICONTROL Cartes]**.
1. Activer **[!UICONTROL Archivage automatique des cartes du panorama]**.

   ![Paramètres de diffusion différée des cartes](assets/card-falloff-switch.png)

1. Sélectionnez le moment où archiver les cartes du panorama. Vous pouvez choisir jusqu’à 8 semaines ou jusqu’à 60 jours.

   La date est déterminée à partir de la dernière modification de la carte.

1. Sélectionnez la colonne dans laquelle vous souhaitez supprimer des cartes.
1. Cliquez sur **[!UICONTROL Enregistrer]** sur le message de confirmation.
1. Cliquez sur **[!UICONTROL Masquer la configuration]** pour fermer la [!UICONTROL Configurer] du panneau. Les paramètres de configuration sont appliqués automatiquement lorsque vous actualisez le panorama.
