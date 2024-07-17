---
content-type: reference
navigation-topic: boards
title: Migrer les cartes Kanban de l’équipe agile vers les panoramas Workfront
description: Vous pouvez migrer vos tâches d’un panorama Kanban d’équipe agile vers un panorama Workfront nouveau ou existant.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 13%

---

# Migrer les cartes Kanban de l’équipe agile vers les panoramas Workfront

Vous pouvez migrer vos tâches d’un panorama Kanban d’équipe agile vers un panorama Workfront nouveau ou existant. Lorsque vous exécutez la migration, toutes les cartes du panorama Kanban sont copiées dans le panorama Workfront. Vous n’êtes pas autorisé à choisir des cartes spécifiques.

Le positionnement des cartes sur le panorama Workfront est basé sur des stratégies de colonnes. (Par exemple, une stratégie peut déplacer toutes les cartes dont l’état est &quot;En cours&quot; vers une colonne spécifique. Pour plus d’informations sur les stratégies de colonnes, voir [Gestion des colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) S’il n’existe aucune stratégie ou si les cartes ne correspondent pas aux stratégies, elles sont placées dans la colonne la plus à gauche du panorama. Pour l’instant, les cartes de la colonne Backlog du panorama hérité ne sont pas ajoutées au panorama Workfront.

Les cartes ne sont pas supprimées du panorama Kanban de l’équipe agile, et les modifications d’état des cartes sont synchronisées avec les deux panoramas. Vous pouvez conserver les deux panoramas actifs jusqu’à ce que vous soyez prêt à passer aux panoramas Workfront.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td>
   <td> <p>N’importe quelle</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td>
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td>
  </tr>
 </tbody>
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Migration de cartes Kanban vers un nouveau panorama

{{step1-to-team}}

1. Accédez à un panorama Kanban.
1. Cliquez sur [!UICONTROL **Ajouter aux panoramas**] et sélectionnez [!UICONTROL **Nouveau panorama**].
1. Dans la boîte de dialogue [!UICONTROL Ajouter au nouveau panorama], saisissez le nom du nouveau panorama (le nom du panorama [!UICONTROL Kanban] actuel s’affiche automatiquement) et cliquez sur [!UICONTROL **Ajouter**].

   ![Ajouter des cartes Kanban à un nouveau panorama](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Facultatif) Dans le message de réussite qui s’affiche, cliquez sur le lien pour ouvrir le nouveau panorama.

## Migration de cartes Kanban vers un panorama existant

{{step1-to-team}}

1. Accédez à un panorama Kanban.
1. Cliquez sur [!UICONTROL **Ajouter aux panoramas**] et sélectionnez [!UICONTROL **Panorama existant**].
1. Dans la boîte de dialogue [!UICONTROL Ajouter au panorama existant] , recherchez et sélectionnez le panorama vers lequel migrer les cartes. Cliquez ensuite sur [!UICONTROL **Ajouter**].

   ![Ajouter des cartes Kanban à la carte existante](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Facultatif) Dans le message de réussite qui s’affiche, cliquez sur le lien pour ouvrir le panorama.
