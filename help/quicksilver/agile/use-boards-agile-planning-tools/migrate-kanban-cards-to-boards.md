---
content-type: reference
navigation-topic: boards
title: Migration de cartes Kanban d’équipe agile vers des panoramas Workfront
description: Vous pouvez migrer vos tâches d’un panorama Kanban d’équipe agile vers un panorama Workfront nouveau ou existant.
author: Lisa
feature: Agile
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Migration de cartes Kanban d’équipe agile vers des panoramas Workfront

Vous pouvez migrer vos tâches d’un panorama Kanban d’équipe agile vers un panorama Workfront nouveau ou existant. Lorsque vous exécutez la migration, toutes les cartes du panorama Kanban sont copiées dans le panorama Workfront. Vous n’êtes pas autorisé à choisir des cartes spécifiques.

Le positionnement des cartes sur le panorama Workfront est basé sur des stratégies de colonnes. (Par exemple, une stratégie peut déplacer toutes les cartes dont l’état est &quot;En cours&quot; vers une colonne spécifique. Pour plus d’informations sur les stratégies de colonne, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) S’il n’existe aucune stratégie ou si les cartes ne correspondent pas aux stratégies, elles sont placées dans la colonne la plus à gauche du panorama. Pour l’instant, les cartes de la colonne Backlog du panorama hérité ne sont pas ajoutées au panorama Workfront.

Les cartes ne sont pas supprimées du panorama Kanban de l’équipe agile, et les modifications d’état des cartes sont synchronisées avec les deux panoramas. Vous pouvez garder les deux panoramas principaux jusqu’à ce que vous soyez prêt à passer aux panoramas Workfront.

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

## Migration de cartes Kanban vers un nouveau panorama

{{step1-to-team}}

1. Accédez à un panorama Kanban.
1. Cliquez sur [!UICONTROL **Ajout à des panoramas**] et sélectionnez [!UICONTROL **Nouveau panorama**].
1. Sur le [!UICONTROL Ajouter au nouveau panorama] Entrez le nom du nouveau panorama (nom de la boîte de dialogue active). [!UICONTROL Kanban] le panorama s’affiche automatiquement) et cliquez sur [!UICONTROL **Ajouter**].

   ![Ajout de cartes Kanban à un nouveau panorama](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Facultatif) Dans le message de réussite qui s’affiche, cliquez sur le lien pour ouvrir le nouveau panorama.

## Migration de cartes Kanban vers un panorama existant

{{step1-to-team}}

1. Accédez à un panorama Kanban.
1. Cliquez sur [!UICONTROL **Ajout à des panoramas**] et sélectionnez [!UICONTROL **Panorama existant**].
1. Sur le [!UICONTROL Ajouter à un panorama existant] , recherchez et sélectionnez le panorama vers lequel les cartes doivent être migrées. Cliquez ensuite sur [!UICONTROL **Ajouter**].

   ![Ajout de cartes Kanban à un panorama existant](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Facultatif) Dans le message de réussite qui s’affiche, cliquez sur le lien pour ouvrir le panorama.
