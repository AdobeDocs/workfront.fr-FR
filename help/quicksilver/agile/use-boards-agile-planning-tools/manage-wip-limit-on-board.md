---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Gestion de la limite de travail en cours sur un panorama
description: Vous pouvez configurer une limite de travail en cours (WIP) pour chaque colonne d’un panorama.
author: Lisa
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 96%

---

# Gérer la limite de [!UICONTROL travail en cours] (WIP) sur un panorama

Vous pouvez configurer une limite de [!UICONTROL travail en cours] (WIP) pour chaque colonne d’un panorama.

La limite WIP est simplement un avertissement visuel et ne vous empêche pas d’avoir plus d’éléments dans chaque colonne que la limite que vous avez définie.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> 
   <p>Nouvelle : [!UICONTROL Contributor] ou niveau supérieur</p> 
   <p>ou</p>
   <p>Actuelle : [!UICONTROL Request] ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Définir la limite WIP sur une colonne

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Localisez la colonne à laquelle vous souhaitez ajouter la limite WIP.

   Pour ajouter une colonne, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

1. Cliquez sur le menu **[!UICONTROL Plus]** dans la colonne et sélectionnez **[!UICONTROL Modifier]** pour ouvrir la zone Paramètres.
1. Sous [!UICONTROL Politiques des colonnes], activez la politique de limite de **[!UICONTROL travail en cours]** pour limiter le nombre de cartes pouvant être ajoutées à la colonne.
1. Saisissez le numéro de la limite dans le champ **[!UICONTROL Définir la limite]**.

   ![Limite WIP de la colonne](assets/boards-wip-limit-in-column.png)

   Le nombre de cartes et la limite s’affichent en haut de la colonne. Si la colonne contient plus de cartes que la limite, le compteur devient rouge.

   ![Compteur de limite WIP](assets/boards-wip-limit-counter.png)

1. Cliquez sur **[!UICONTROL Fermer]** pour quitter la zone [!UICONTROL Paramètres] et afficher la colonne et ses cartes.
