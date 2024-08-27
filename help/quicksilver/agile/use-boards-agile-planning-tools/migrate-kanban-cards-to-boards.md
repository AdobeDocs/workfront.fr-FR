---
content-type: reference
navigation-topic: boards
title: Migration des cartes Kanban de l’équipe agile vers les panoramas Workfront
description: Vous pouvez migrer vos tâches d’un panorama Kanban d’équipe agile vers un panorama Workfront nouveau ou existant.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 16%

---

# Migrer les cartes Kanban de l’équipe agile vers les panoramas Workfront

Vous pouvez migrer vos tâches d’un panorama Kanban d’équipe agile vers un panorama Workfront nouveau ou existant. Lorsque vous exécutez la migration, toutes les cartes du panorama Kanban sont copiées dans le panorama Workfront. Vous n’êtes pas autorisé à choisir des cartes spécifiques.

Le positionnement des cartes sur le panorama Workfront est basé sur des stratégies de colonnes. (Par exemple, une stratégie peut déplacer toutes les cartes dont l’état est &quot;En cours&quot; vers une colonne spécifique. Pour plus d’informations sur les stratégies de colonnes, voir [Gestion des colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) S’il n’existe aucune stratégie ou si les cartes ne correspondent pas aux stratégies, elles sont placées dans la colonne la plus à gauche du panorama. Pour l’instant, les cartes de la colonne Backlog du panorama hérité ne sont pas ajoutées au panorama Workfront.

Les cartes ne sont pas supprimées du panorama Kanban de l’équipe agile, et les modifications d’état des cartes sont synchronisées avec les deux panoramas. Vous pouvez conserver les deux panoramas actifs jusqu’à ce que vous soyez prêt à passer aux panoramas Workfront.

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
