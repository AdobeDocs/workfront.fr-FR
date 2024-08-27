---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Gestion de la limite de travail en cours sur un panorama
description: Vous pouvez configurer une limite de travail en cours pour chaque colonne d’un panorama.
author: Lisa
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 26%

---

# Gérer la limite de [!UICONTROL travail en cours] (travail en cours) sur un panorama

Vous pouvez configurer une limite de [!UICONTROL travail en cours] pour chaque colonne d’un panorama.

La limite de travaux en cours est simplement un avertissement visuel et ne vous empêche pas d’avoir plus d’éléments dans chaque colonne que la limite que vous avez définie.

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

## Définition de la limite de travail en cours sur une colonne

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Recherchez la colonne à laquelle vous souhaitez ajouter la limite de travaux en cours.

   Pour ajouter une nouvelle colonne, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

1. Cliquez sur le menu **[!UICONTROL Plus]** de la colonne, puis sélectionnez **[!UICONTROL Modifier]** pour ouvrir la zone Paramètres.
1. Sous [!UICONTROL Stratégies de colonne], activez la stratégie **[!UICONTROL Travail en cours] limite** pour limiter le nombre de cartes pouvant être ajoutées à la colonne.
1. Saisissez le nombre limite dans le champ **[!UICONTROL Définir la limite]** .

   ![Limite du travail en cours pour la colonne](assets/boards-wip-limit-in-column.png)

   Le nombre de cartes et la limite s’affichent en haut de la colonne. Si la colonne contient plus de cartes que la limite, le compteur devient rouge.

   ![Compteur limite de travail](assets/boards-wip-limit-counter.png)

1. Cliquez sur **[!UICONTROL Fermer]** pour quitter la zone [!UICONTROL Paramètres] et afficher la colonne et ses cartes.
