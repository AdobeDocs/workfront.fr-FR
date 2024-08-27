---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Configuration de l’abandon de carte
description: Vous pouvez configurer un panorama afin que les cartes soient archivées ou abandonnées selon un calendrier précis.
author: Lisa
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 38%

---

# Configurer le détachement des vignettes

Vous pouvez configurer un panorama afin que les cartes soient archivées ou &quot;tombent&quot; du panorama selon un calendrier précis. Vous pouvez définir des cartes dans une colonne spécifique pour qu’elles ne soient plus incluses dans le panorama au cours d’un certain nombre de jours ou de semaines.

Lorsqu’une carte tombe hors du panorama, elle est archivée. Vous pouvez afficher les cartes archivées avec un filtre. Pour plus d’informations, voir [Filtrer et rechercher dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

## Configurer le détachement des vignettes

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau Configurer.
1. Développez **[!UICONTROL Cartes]**.
1. Activez l’option **[!UICONTROL Archivage automatique des cartes du panorama]**.

   ![Paramètres de basculement de carte](assets/card-falloff-switch.png)

1. Sélectionnez le moment où archiver les cartes du panorama. Vous pouvez choisir jusqu’à 8 semaines ou jusqu’à 60 jours.

   La date est déterminée à partir de la dernière modification de la carte.

1. Sélectionnez la colonne dans laquelle vous souhaitez supprimer des cartes.
1. Cliquez sur **[!UICONTROL Enregistrer]** dans le message de confirmation.
1. Cliquez sur **[!UICONTROL Masquer la configuration]** pour fermer le panneau [!UICONTROL Configurer]. Les paramètres de configuration sont appliqués automatiquement lorsque vous actualisez le panorama.
