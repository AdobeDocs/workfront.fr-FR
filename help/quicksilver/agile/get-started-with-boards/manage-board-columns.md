---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gestion des colonnes de panorama
description: Un nouveau panorama contient trois colonnes par défaut. Vous pouvez ajouter d’autres colonnes, modifier l’ordre des colonnes, renommer les colonnes et supprimer celles dont vous n’avez pas besoin.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 8097842fedb468d8f0e5c9eed94bf74d489edd2b
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# Gestion des colonnes de panorama

Un nouveau panorama contient trois colonnes par défaut. Vous pouvez ajouter d’autres colonnes, modifier l’ordre des colonnes, renommer les colonnes et supprimer celles dont vous n’avez pas besoin.

Les paramètres de colonne incluent des stratégies qui vous permettent de définir des options pour ce qui arrive à une carte lorsqu’elle est déplacée dans cette colonne.

Pour plus d’informations sur le tri des cartes en colonnes, voir [Filtrage et recherche dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

## Ajouter une colonne à un panorama

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Ajouter une colonne]** à droite des colonnes existantes.
1. Dans la nouvelle colonne, saisissez un nom, puis cliquez sur **[!UICONTROL Ajouter une colonne]**.

   ![Ajouter une nouvelle colonne](assets/boards-add-column.png)

>[!TIP]
>
>Pour ajouter une colonne d’ingestion, reportez-vous à la section [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Réorganiser les colonnes du panorama

1. Accédez au panorama.
1. Faites glisser et déposez les colonnes dans l’ordre approprié. Veillez à sélectionner le haut de la colonne avant de la faire glisser vers un autre emplacement.

   ![Glisser-déposer une colonne](assets/boards-dragdropcolumn.png)

## Renommer une colonne de panorama

1. Accédez au panorama.
1. Cliquez sur le nom de la colonne, saisissez le nouveau nom, puis appuyez sur Entrée.

   Ou

   Cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) dans la colonne et sélectionnez **[!UICONTROL Modifier]**. Dans la zone Paramètres , saisissez le nouveau nom dans la zone **[!UICONTROL Nom de la colonne]** puis cliquez sur **[!UICONTROL Fermer]**.

## Supprimer une colonne de panorama

Lorsque vous supprimez une colonne d’un panorama, elle ne peut pas être récupérée.

1. Accédez au panorama.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) dans la colonne , puis sélectionnez **[!UICONTROL Supprimer]**.

   >[!NOTE]
   >
   >Les colonnes contenant des cartes, y compris les cartes archivées, ne peuvent pas être supprimées. Si vous essayez de supprimer une colonne contenant des cartes, vous devez choisir une autre colonne pour ces cartes.

## Nombre de cartes d’affichage

Vous pouvez utiliser un paramètre de configuration pour afficher le nombre de cartes dans chaque colonne.

Si vous utilisez la limite de travaux en cours sur une colonne, aucun compteur de cartes distinct n’est ajouté. Pour plus d’informations sur les limites de travaux en cours, voir [Gérer les [!UICONTROL Travail en cours] Limite (en cours) sur un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Accédez au panorama.
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau Configurer .
1. Développer **[!UICONTROL Colonne]**.
1. Activer **[!UICONTROL Affichage d’un nombre de cartes de colonnes]**.

   ![Activer le compteur de cartes](assets/display-card-count.png)

   Le compteur de cartes s’affiche en haut de chaque colonne.

1. Cliquez sur **[!UICONTROL Masquer la configuration]** pour fermer la [!UICONTROL Configurer] du panneau.

## Définition des paramètres et des stratégies de colonne

1. Accédez au panorama.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) dans la colonne , puis sélectionnez **[!UICONTROL Modifier]**.

   La variable [!UICONTROL Paramètres] s’affiche. La variable **[!UICONTROL Nom de la colonne]** vous permet de savoir pour quelle colonne vous définissez les paramètres.

1. Activez la variable **[!UICONTROL Mettre à jour automatiquement les valeurs de champ]** pour modifier automatiquement certaines valeurs de champ lorsqu’une carte est déplacée vers cette colonne.

   ![Paramètres et stratégies de colonne](assets/boards-column-policies-enabled.png)

1. (Facultatif) Définissez une valeur pour l’état de la carte :

   1. Sélectionnez la variable **[!UICONTROL État]** .

   1. Sélectionnez l’état à appliquer à une carte lorsqu’elle est déplacée vers cette colonne.

      ![État des colonnes](assets/boards-column-status.png)

      Les options de traduction de l’état des cartes connectées s’affichent également. (La traduction de l’état ne s’applique pas aux cartes ad hoc.) Ces options déterminent l’état personnalisé appliqué à la tâche ou au problème dans [!DNL Workfront] lorsqu’une carte connectée est déplacée vers cette colonne.

   1. Sélectionnez une [!UICONTROL **Personnalisé**] à appliquer à la carte pour les tâches et les problèmes.

      Lorsqu’une carte est déplacée vers cette colonne, [!DNL Workfront] tente d’abord d’appliquer l’état personnalisé (par exemple, Résolu). Si l’état personnalisé sélectionné n’est pas disponible pour cette carte, vous êtes invité à choisir un autre état correspondant à l’état du système (à l’étape b ci-dessus). Pour plus d’informations sur les états, voir [Présentation des états](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      En outre, si l’état de la tâche ou du problème connecté est modifié dans l’état personnalisé ou système défini dans la stratégie de colonne, la carte est automatiquement déplacée dans la colonne.

1. (Facultatif) Définissez une valeur pour les personnes désignées par les cartes :

   1. Sélectionnez la variable **[!UICONTROL Assignation]** .
   1. Sélectionnez une action.

      * **[!UICONTROL Ajouter sur les personnes désignées]:** Les personnes désignées que vous sélectionnez sont ajoutées à la liste existante des personnes désignées sur une carte lorsqu’elle est déplacée vers cette colonne.
      * **[!UICONTROL Remplacer les personnes désignées]:** Les personnes désignées que vous sélectionnez remplacent toutes les autres personnes désignées et deviennent les seules personnes désignées sur une carte lorsqu’elle est déplacée vers cette colonne.

   1. Cliquez sur [!UICONTROL **Ajouter une affectation**] et recherchez un utilisateur. Sélectionnez les personnes désignées dans les résultats de la recherche. Tous les utilisateurs et équipes de Workfront sont disponibles pour effectuer un choix.

      ![Assignation de la colonne](assets/boards-column-assignees.png)

1. (Facultatif) Définissez une valeur pour les balises de carte :

   1. Sélectionnez la variable **[!UICONTROL Cartes]** .
   1. Sélectionnez une action.

      * **[!UICONTROL Ajouter sur les balises]:** Les balises que vous sélectionnez sont ajoutées à la liste des balises existantes sur une carte lorsqu’elles sont déplacées dans cette colonne.
      * **[!UICONTROL Remplacement des balises]:** Les balises que vous sélectionnez remplacent toutes les autres balises et deviennent les seules balises d’une carte lorsqu’elles sont déplacées dans cette colonne.

   1. Sélectionnez les balises dans la liste déroulante. Seules les balises déjà créées dans [!UICONTROL Gestionnaire de balises] sont disponibles. Pour plus d’informations sur l’ajout de nouvelles balises, voir [Ajout de balises](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Balises de colonne](assets/boards-column-tags.png)

1. Activez la variable **[!UICONTROL Limite de travail en cours]** pour limiter le nombre de cartes à ajouter à la colonne. Saisissez ensuite le nombre limite dans la variable **[!UICONTROL Définir la limite]** champ .

   ![Limite de travaux en cours pour la colonne](assets/boards-wip-limit-in-column.png)

   Pour plus d’informations, voir [Gestion de la limite de travail en cours sur un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Cliquez sur **[!UICONTROL Fermer]** pour quitter la zone Paramètres et afficher la colonne et ses cartes.
