---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Suppression ou archivage d’une carte d’un panorama
description: Lorsque vous supprimez une carte d’un panorama, elle est supprimée définitivement et ne peut pas être restaurée. L’archivage d’une carte l’envoie dans les archives et vous pouvez la restaurer dans le panorama ultérieurement.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 98%

---

# Supprimer ou archiver une carte d’un panorama

Lorsque vous supprimez une carte ad hoc d’un panorama, elle est supprimée définitivement et ne peut pas être restaurée. Une fois supprimées, les cartes connectées peuvent être réajoutées manuellement à un panorama.

Si vous supprimez une carte connectée d’un panorama dynamique, elle réapparaît lorsque vous actualisez le panorama, car ce type de panorama extrait toutes les tâches et tous les problèmes d’un projet spécifique. Pour supprimer la carte, vous devez supprimer la tâche ou le problème connecté du projet Workfront.

Lorsque vous supprimez une carte connectée d’un autre type de panorama comportant une colonne de saisie, la carte réapparaît dans la colonne de saisie lorsque vous actualisez le panorama si la tâche ou le problème connecté n’est pas encore marqué comme terminé. Pour plus d’informations sur les colonnes de saisie, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

L’archivage d’une carte l’envoie dans les archives et vous pouvez la restaurer dans le panorama ultérieurement.

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

## Supprimer une carte d’un panorama

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur le menu **[!UICONTROL Plus]** ![Menu Plus](assets/more-icon-spectrum.png) de la carte et sélectionnez **[!UICONTROL Supprimer]**.
1. Cliquez sur **[!UICONTROL Supprimer]** dans le message de confirmation.

## Archiver une carte à partir d’un panorama

1. Accédez au panorama.
1. Cliquez sur le menu **[!UICONTROL Plus]** ![Menu Plus](assets/more-icon-spectrum.png) de la carte et sélectionnez **[!UICONTROL Archiver]**.

   Les cartes archivées sont masquées dans le panorama à moins que vous n’appliquiez un filtre pour les afficher. Pour plus d’informations, consultez dans cet article la section [Filtrer un panorama pour afficher les cartes archivées](#filter-a-board-to-show-archived-cards).

   Une icône [!UICONTROL Archiver] ![Archiver](assets/archive-icon-spectrum-25x20.png) apparaît sur les cartes archivées. Vous ne pouvez pas modifier une carte archivée, mais vous pouvez la supprimer ou la déplacer vers une autre colonne.

1. Pour restaurer une carte archivée, cliquez sur le menu **[!UICONTROL Plus]** ![Menu Plus](assets/more-icon-spectrum.png) sur la carte et sélectionnez **[!UICONTROL Restaurer]**.

## Filtrer un panorama pour afficher les cartes archivées {#filter-a-board-to-show-archived-cards}

Par défaut, seules les cartes actives sont affichées sur un panorama. Le panorama peut être également filtré pour afficher les cartes archivées.

1. Accédez au panorama.
1. Cliquez sur [!UICONTROL **Configurer**] à droite du panorama pour ouvrir le panneau Configurer.
1. Développez [!UICONTROL **Cartes**].
1. Activez [!UICONTROL **Afficher les cartes archivées sur le panorama**].
1. Cliquez sur [!UICONTROL **Filtrer**], développez la section [!UICONTROL Cartes archivées] et sélectionnez **[!UICONTROL Cartes archivées]** pour afficher toutes les cartes archivées.

   Le filtre indique le nombre de cartes archivées.

   ![Filtrer les cartes archivées](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >La section [!UICONTROL Cartes archivées] n’est pas disponible dans le filtre si vous n’avez pas activé le paramètre de configuration permettant d’afficher les cartes archivées. Pour plus d’informations, voir [Personnaliser des champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Sélectionnez à nouveau **[!UICONTROL Cartes archivées]** pour effacer l’option et n’afficher que les cartes actives.
