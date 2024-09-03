---
content-type: reference
navigation-topic: boards
title: Migration des cartes Kanban de l’équipe agile vers les panoramas Workfront
description: Vous pouvez migrer vos éléments de travail d’un tableau Kanban d’une équipe agile vers un tableau Workfront nouveau ou existant.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 97%

---

# Migrer des cartes Kanban d’équipe Agile vers des panoramas Workfront

Vous pouvez migrer vos éléments de travail d’un tableau Kanban d’une équipe agile vers un tableau Workfront nouveau ou existant. Lorsque vous exécutez la migration, toutes les cartes du tableau Kanban sont copiées sur le tableau Workfront. Vous n’avez pas l’autorisation de choisir des cartes spécifiques.

Le placement des cartes sur le panorama Workfront est basé sur des politiques de colonnes. (Par exemple, une politique pourrait déplacer toutes les cartes ayant un statut « En cours » vers une colonne spécifique. Pour plus d’informations sur les politiques des colonnes, voir [Gérer les colonnes du tableau](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)). S’il n’y a pas de politiques ou si les cartes ne correspondent pas aux politiques, les cartes sont placées dans la colonne la plus à gauche du tableau. Pour l’instant, les cartes de la colonne Liste d’attente du panorama hérité ne sont pas ajoutées au panorama Workfront.

Les cartes ne sont pas supprimées du tableau Kanban de l’équipe Agile et les modifications du statut des cartes sont synchronisées avec les deux tableaux. Vous pouvez conserver les deux tableaux actifs jusqu’à ce que vous soyez en mesure de passer aux panoramas Workfront.

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
