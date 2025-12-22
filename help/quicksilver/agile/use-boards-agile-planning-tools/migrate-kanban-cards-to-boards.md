---
content-type: reference
navigation-topic: boards
title: Migrer les cartes Kanban de l’équipe Agile vers les tableaux Workfront
description: Vous pouvez migrer vos tâches d’un tableau Kanban d’équipe Agile vers un tableau Workfront nouveau ou existant.
author: Jenny
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 70%

---

# Migrer les cartes Kanban de l’équipe Agile vers les tableaux Workfront

Vous pouvez migrer vos tâches d’un tableau Kanban d’équipe Agile vers un tableau Workfront nouveau ou existant. Lorsque vous exécutez la migration, toutes les cartes du tableau Kanban sont copiées sur le tableau Workfront. Vous n’avez pas l’autorisation de choisir des cartes spécifiques.

Le placement des cartes sur le panorama Workfront est basé sur des politiques de colonnes. (Par exemple, une politique pourrait déplacer toutes les cartes ayant un statut « En cours » vers une colonne spécifique. Pour plus d’informations sur les politiques de colonnes, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) S’il n’existe aucune politique ou que les cartes ne correspondent pas aux politiques, les cartes sont placées dans la colonne la plus à gauche du panorama. Pour l’instant, les cartes de la colonne Liste d’attente du panorama hérité ne sont pas ajoutées au panorama Workfront.

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
   <p>Contributeur ou version ultérieure</p> 
   <p>Requête ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
