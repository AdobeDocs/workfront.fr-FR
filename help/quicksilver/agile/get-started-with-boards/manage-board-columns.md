---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gérer les colonnes de panorama
description: Un nouveau panorama contient trois colonnes par défaut. Vous pouvez ajouter d’autres colonnes, modifier l’ordre des colonnes, renommer les colonnes et supprimer celles dont vous n’avez pas besoin. Vous pouvez également définir des stratégies de colonne.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1149'
ht-degree: 9%

---

# Gérer les colonnes de panorama

<!-- Audited: 05/2024 -->

Un nouveau panorama contient trois colonnes par défaut. Vous pouvez ajouter d’autres colonnes, modifier l’ordre des colonnes, renommer les colonnes et supprimer celles dont vous n’avez pas besoin.

Les paramètres de colonne incluent des stratégies qui vous permettent de définir des options pour ce qui arrive à une carte lorsqu’elle est déplacée dans cette colonne.

Pour plus d’informations sur le tri des cartes dans les colonnes, voir [Filtrage et recherche dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : contributeur ou contributrice ou supérieure </p>
        <p>ou</p> 
        <p>Actuel : [!UICONTROL Request] ou supérieure </p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ajouter une colonne à un panorama

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Ajouter la colonne]** à droite des colonnes existantes.
1. Dans la nouvelle colonne, saisissez un nom et cliquez sur **[!UICONTROL Ajouter une colonne]**.

   ![Ajouter une nouvelle colonne](assets/boards-add-column.png)

>[!TIP]
>
>Pour ajouter une colonne d&#39;ingestion, voir [Ajout d&#39;une colonne d&#39;ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Réorganiser les colonnes du panorama

1. Accédez au panorama.
1. Faites glisser et déposez les colonnes dans l’ordre approprié. Veillez à sélectionner le haut de la colonne avant de la faire glisser vers un autre emplacement.

   ![Faire glisser et déposer la colonne](assets/boards-dragdropcolumn.png)

## Renommer une colonne de panorama

1. Accédez au panorama.
1. Cliquez sur le nom de la colonne, saisissez le nouveau nom, puis appuyez sur Entrée.

   Ou

   Cliquez sur le menu **[!UICONTROL Plus]** ![Plus de menu](assets/more-icon-spectrum.png) dans la colonne et sélectionnez **[!UICONTROL Modifier]**. Dans la zone Paramètres, saisissez le nouveau nom dans le champ **[!UICONTROL Nom de la colonne]**, puis cliquez sur **[!UICONTROL Fermer]**.

## Supprimer une colonne de panorama

Lorsque vous supprimez une colonne d’un panorama, elle ne peut pas être récupérée.

1. Accédez au panorama.
1. Cliquez sur le menu **[!UICONTROL Plus]** ![Plus de menu](assets/more-icon-spectrum.png) dans la colonne, puis sélectionnez **[!UICONTROL Supprimer]**.

   >[!NOTE]
   >
   >Les colonnes contenant des cartes, y compris les cartes archivées, ne peuvent pas être supprimées. Si vous essayez de supprimer une colonne contenant des cartes, vous devez choisir une autre colonne pour ces cartes.

## Nombre de cartes d’affichage

Vous pouvez utiliser un paramètre de configuration pour afficher le nombre de cartes dans chaque colonne.

Si vous utilisez la limite de travaux en cours sur une colonne, aucun compteur de cartes distinct n’est ajouté. Pour plus d’informations sur les limites de travaux en cours, voir [Gérer la limite de [!UICONTROL travail en cours] (travaux en cours) sur un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Accédez au panorama.
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau Configurer.
1. Développez **[!UICONTROL Column]**.
1. Activez **[!UICONTROL Afficher un nombre de cartes de colonnes]**.

   ![Activer le compteur de cartes](assets/display-card-count.png)

   Le compteur de cartes s’affiche en haut de chaque colonne.

1. Cliquez sur **[!UICONTROL Masquer la configuration]** pour fermer le panneau [!UICONTROL Configurer].

## Définition des paramètres et des stratégies de colonne

Les stratégies de colonne incluent la mise à jour automatique des valeurs de champ et la définition d’une limite de travail en cours.

La stratégie de mise à jour de l’état fonctionne automatiquement pour la carte et la colonne :

* Lorsqu’une carte est déplacée dans une colonne avec une stratégie, l’état de la carte est mis à jour vers l’état défini dans la stratégie. Cela s’applique aux cartes ad hoc et connectées.
* Lorsqu’un état de carte ad hoc ou connecté est mis à jour sur la carte pour correspondre à l’état de colonne dans la stratégie ou qu’un état de carte connecté est mis à jour ailleurs dans Workfront, la carte est automatiquement déplacée vers cette colonne. En outre, si un état personnalisé sur une carte correspond à l’état système affecté à la colonne, la carte est déplacée vers cette colonne.

Une carte reste dans une colonne où elle est placée si l’état de la carte ne correspond à aucun état défini dans les stratégies de colonne existantes.

>[!NOTE]
>
>Les panoramas dynamiques placent toujours dans la colonne des cartes qui correspondent à leur état, que les stratégies de colonnes soient activées ou désactivées. Lorsque vous actualisez le panorama, les cartes reviennent aux colonnes qui leur sont affectées.
> 
>En outre, pour tous les types de panoramas, si vous déplacez une carte d’une colonne à une autre avec le même état, la carte revient à la colonne d’origine lorsque vous actualisez le panorama.

1. Accédez au panorama.
1. Cliquez sur le menu **[!UICONTROL Plus]** ![Plus de menu](assets/more-icon-spectrum.png) dans la colonne, puis sélectionnez **[!UICONTROL Modifier]**.

   La zone [!UICONTROL Paramètres] s’affiche. Le **[!UICONTROL nom de colonne]** vous indique pour quelle colonne vous définissez les paramètres.

1. Activez la stratégie **[!UICONTROL Mettre à jour les valeurs de champ automatiquement]** pour modifier certaines valeurs de champ automatiquement lorsqu’une carte est déplacée vers cette colonne.

   ![ Paramètres et stratégies de colonne ](assets/boards-column-policies-enabled.png)

1. (Facultatif) Définissez une valeur pour l’état de la carte :

   1. Cochez la case **[!UICONTROL Status]** .

   1. Sélectionnez l’état à appliquer à une carte lorsqu’elle est déplacée vers cette colonne.

      ![État des colonnes](assets/boards-column-status.png)

      Les options de traduction de l’état des cartes connectées s’affichent également. (La traduction de l’état ne s’applique pas aux cartes ad hoc.) Ces options déterminent l’état personnalisé appliqué à la tâche ou au problème dans [!DNL Workfront] lorsqu’une carte connectée est déplacée vers cette colonne.

   1. Sélectionnez un état [!UICONTROL **Personnalisé**] à appliquer à la carte pour les tâches et les problèmes.

      Lorsqu’une carte est déplacée vers cette colonne, [!DNL Workfront] tente d’appliquer le statut personnalisé (par exemple, Résolu). Si l’état personnalisé sélectionné n’est pas disponible pour cette carte, vous êtes invité à choisir un autre état correspondant à l’état du système (à l’étape b ci-dessus). Pour plus d’informations sur les états, voir [Présentation des états](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      En outre, si le statut de la tâche ou du problème connecté passe au statut personnalisé ou système défini dans la politique de colonne, la carte est automatiquement déplacée dans la colonne.

1. (Facultatif) Définissez une valeur pour les personnes désignées par les cartes :

   1. Cochez la case **[!UICONTROL Assignation]** .
   1. Sélectionnez une action.

      * **[!UICONTROL Ajouter sur les personnes désignées] :** Les personnes désignées que vous sélectionnez sont ajoutées à la liste existante des personnes désignées sur une carte lorsqu’elle est déplacée vers cette colonne.
      * **[!UICONTROL Remplacer les personnes désignées] :** Les personnes désignées que vous sélectionnez remplacent toutes les autres personnes désignées et deviennent les seules personnes désignées sur une carte lorsqu’elle est déplacée vers cette colonne.

   1. Cliquez sur [!UICONTROL **Ajouter une affectation**] et recherchez un utilisateur. Sélectionnez les personnes désignées dans les résultats de la recherche. Tous les utilisateurs et équipes de Workfront sont disponibles pour effectuer un choix.

      ![Assignation de la colonne](assets/boards-column-assignees.png)

1. (Facultatif) Définissez une valeur pour les balises de carte :

   1. Cochez la case **[!UICONTROL Cartes]** .
   1. Sélectionnez une action.

      * **[!UICONTROL Ajouter sur les balises] :** Les balises sélectionnées sont ajoutées à la liste existante des balises sur une carte lorsqu’elles sont déplacées dans cette colonne.
      * **[!UICONTROL Remplacer les balises] :** Les balises que vous sélectionnez remplacent toutes les autres balises et deviennent les seules balises d’une carte lorsqu’elles sont déplacées dans cette colonne.

   1. Sélectionnez les balises dans la liste déroulante. Seules les balises déjà créées dans le [!UICONTROL Gestionnaire de balises] peuvent faire l’objet d’un choix. Pour plus d’informations sur l’ajout de nouvelles balises, voir [Ajout de balises](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Balises pour la colonne](assets/boards-column-tags.png)

1. Activez la stratégie **[!UICONTROL Limite de travail en cours]** pour limiter le nombre de cartes pouvant être ajoutées à la colonne. Saisissez ensuite le nombre limite dans le champ **[!UICONTROL Définir la limite]** .

   ![Limite de travail en cours pour la colonne](assets/boards-wip-limit-in-column.png)

   Pour plus d’informations, voir [Gestion de la limite de travail en cours sur un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Cliquez sur **[!UICONTROL Fermer]** pour quitter la zone Paramètres et afficher la colonne et ses cartes.
