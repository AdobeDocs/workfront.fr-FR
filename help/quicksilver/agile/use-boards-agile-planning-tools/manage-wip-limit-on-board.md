---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Gérer la limite de travail en cours (WIP) sur un tableau
description: Vous pouvez configurer une limite de travail en cours (WIP) pour chaque colonne d’un panorama.
author: Courtney
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jOCQTCkNgEZfE8O4-KyKVjEluncwWx0vh5NdrKHC9vg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 95%

---

# Gérer la limite de [!UICONTROL travail en cours] (WIP) sur un panorama

Vous pouvez configurer une limite de [!UICONTROL travail en cours] (WIP) pour chaque colonne d’un panorama.

La limite WIP est simplement un avertissement visuel et ne vous empêche pas d’avoir plus d’éléments dans chaque colonne que la limite que vous avez définie.

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
