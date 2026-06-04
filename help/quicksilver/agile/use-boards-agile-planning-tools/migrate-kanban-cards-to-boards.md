---
content-type: reference
navigation-topic: boards
title: Migrer les cartes Kanban de l’équipe Agile vers les tableaux Workfront
description: Vous pouvez migrer vos tâches d’un tableau Kanban d’équipe Agile vers un tableau Workfront nouveau ou existant.
author: Courtney
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/RXk7PYF6JsdF71pRVwEA-Wk23h-UqbgLPXSyNR7VX5Y
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
source-wordcount: 360
ht-degree: 72%

---

# Migrer les cartes Kanban de l’équipe Agile vers les panoramas Workfront

Vous pouvez migrer vos tâches d’un tableau Kanban d’équipe Agile vers un tableau Workfront nouveau ou existant. Lorsque vous exécutez la migration, toutes les cartes du tableau Kanban sont copiées sur le tableau Workfront. Vous n’avez pas l’autorisation de choisir des cartes spécifiques.

Le placement des cartes sur le panorama Workfront est basé sur des politiques de colonnes. (Par exemple, une politique pourrait déplacer toutes les cartes ayant un statut « En cours » vers une colonne spécifique. Pour plus d’informations sur les politiques de colonne, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) S’il n’existe aucune stratégie ou si les cartes ne correspondent pas aux stratégies, les cartes sont placées dans la colonne la plus à gauche du panorama. Pour l’instant, les cartes de la colonne Liste d’attente du panorama hérité ne sont pas ajoutées au panorama Workfront.

Les cartes ne sont pas supprimées du tableau Kanban de l’équipe Agile et les modifications du statut des cartes sont synchronisées avec les deux tableaux. Vous pouvez conserver les deux tableaux actifs jusqu’à ce que vous soyez en mesure de passer aux panoramas Workfront.

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

## Migrer les cartes Kanban vers un nouveau tableau

{{step1-to-team}}

1. Accédez à un tableau Kanban.
1. Cliquez sur [!UICONTROL **Ajouter aux tableaux**] et sélectionnez [!UICONTROL **Nouveau tableau**].
1. Dans la boîte de dialogue [!UICONTROL Ajouter au nouveau tableau], saisissez un nom pour le nouveau tableau (le nom du tableau [!UICONTROL Kanban] actuel est automatiquement affiché) et cliquez sur [!UICONTROL **Ajouter**].

   ![Ajouter des cartes Kanban à un nouveau tableau](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Facultatif) Dans le message de réussite qui s’affiche, cliquez sur le lien pour ouvrir le nouveau tableau.

## Migrer des cartes Kanban vers un tableau existant

{{step1-to-team}}

1. Accédez à un tableau Kanban.
1. Cliquez sur [!UICONTROL **Ajouter aux tableaux**] et sélectionnez [!UICONTROL **Tableau existant**].
1. Dans la boîte de dialogue [!UICONTROL Ajouter au tableau existant], recherchez et sélectionnez le tableau vers lequel migrer les cartes. Cliquez ensuite sur [!UICONTROL **Ajouter**].

   ![Ajouter des cartes Kanban à un tableau existant](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Facultatif) Dans le message de réussite qui s’affiche, cliquez sur le lien pour ouvrir le tableau.
