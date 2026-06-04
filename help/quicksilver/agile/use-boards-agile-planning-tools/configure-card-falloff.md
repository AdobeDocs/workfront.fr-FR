---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Configurer l’abandon de carte
description: Vous pouvez configurer un panorama afin que les cartes soient archivées ou « tombent » du panorama selon un planning précis.
author: Courtney
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/iSsqfrcgbod28qez5XkHDP-nDSQO-UKDGm13zPeeBZ0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 228
ht-degree: 98%

---

# Configurer le détachement des vignettes

Vous pouvez configurer un panorama afin que les cartes soient archivées ou « tombent » du panorama selon un planning précis. Vous pouvez définir des cartes dans une colonne spécifique pour qu’elles tombent du panorama au cours d’un certain nombre de jours ou de semaines.

Lorsqu’une carte tombe du panorama, elle est archivée. Vous pouvez afficher les cartes archivées avec un filtre. Pour plus d’informations, voir [Filtrer et rechercher dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou supérieur</p> 
   <p>Requête ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer le détachement des vignettes

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau Configurer.
1. Développez **[!UICONTROL Cartes]**.
1. Activez **[!UICONTROL Archiver automatiquement les cartes du panorama]**.

   ![Paramètres du détachement des cartes](assets/card-falloff-switch.png)

1. Sélectionnez le moment où archiver les cartes du panorama. Vous pouvez choisir jusqu’à 8 semaines ou jusqu’à 60 jours.

   La date est déterminée à partir de la dernière modification de la carte.

1. Sélectionnez la colonne dans laquelle vous souhaitez supprimer des cartes.
1. Cliquez sur **[!UICONTROL Enregistrer]** sur le message de confirmation.
1. Cliquez sur **[!UICONTROL Masquer la configuration]** pour fermer le panneau [!UICONTROL Configurer]. Les paramètres de configuration sont appliqués automatiquement lorsque vous actualisez le panorama.
