---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Ajouter une colonne de saisie à un panorama
description: Vous pouvez éventuellement ajouter une colonne d’entrée à votre panorama qui extrait automatiquement les tâches et les problèmes en tant que cartes connectées lorsqu’elles sont ajoutées dans Workfront, en fonction des filtres que vous définissez.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 14448432922ec1fa478b805dead2ba1e6c211e86
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 9%

---

# Ajouter une colonne de saisie à un panorama

Vous pouvez éventuellement ajouter une colonne d’entrée à votre panorama qui extrait automatiquement les tâches et les problèmes en tant que cartes connectées lorsqu’elles sont ajoutées dans [!DNL Workfront], en fonction des filtres que vous définissez. La colonne d’entrée peut servir de colonne de journal pour une équipe Kanban, un emplacement d’entrée pour une équipe d’assistance afin de voir les problèmes lorsqu’ils sont ajoutés à une file d’attente de demandes ou tout autre objectif dont vous avez besoin.

Une seule colonne d’entrée est autorisée sur un panorama et apparaît toujours comme la colonne la plus à gauche.

La colonne d’ingestion n’est pas disponible sur un panorama dynamique. Vous pouvez toutefois mettre à jour les filtres qui définissent les cartes qui sont importées sur un panorama dynamique. Lorsque vous modifiez ces filtres sur un panorama dynamique, les paramètres de carte qui ne font pas partie de la tâche ou du problème Workfront (comme les balises) sont réinitialisés.

>[!NOTE]
>
>Pour des raisons de sécurité, seule la personne propriétaire d’un panorama peut modifier les filtres du panorama dans le panneau Configurer.

La colonne d’admission est limitée à 300 tâches et 300 numéros. L&#39;ordre par défaut des éléments dans la colonne d&#39;entrée est le suivant :

Tâches :

* Ordre principal : nom du projet
* Ordre secondaire : structure de répartition du travail

Problèmes :

* Ordre principal : nom du projet
* Ordre secondaire : numéro de référence

>[!IMPORTANT]
>
>Il est recommandé d’actualiser fréquemment le panorama si plusieurs utilisateurs y travaillent simultanément. L’actualisation de la page permet de maintenir les modifications visuelles sur le panorama à jour et d’éviter des problèmes tels que les cartes en double qui sont déplacées sur le panorama à partir de la colonne d’ingestion.

Pour plus d’informations sur les colonnes, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Pour plus d’informations sur les cartes connectées, voir [Utilisation de cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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
   <td> <p>[!DNL Request] ou supérieur</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Création d’une colonne d’entrée à l’aide de filtres simples

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau Configurer.
1. Développez **[!UICONTROL Board]**.
1. Activez l’option **[!UICONTROL Réception dynamique d’éléments sur le panorama]**.

   ![Options de filtre simple de colonne d’entrée](assets/intake-column-simple-filters.png)

   La colonne d’ingestion est ajoutée à gauche du panorama. Il reste vide jusqu’à ce que vous lui appliquiez des filtres.

1. (Facultatif) Recherchez et sélectionnez [!DNL Workfront] [!UICONTROL **Projets**].
1. (Facultatif) Recherchez et sélectionnez l’utilisateur ou l’équipe [!UICONTROL **Affectations**].
1. Sélectionnez [!UICONTROL **Inclure le travail terminé**] pour afficher les tâches et les problèmes dont l’état est Complet dans la colonne d’admission.

   >[!NOTE]
   >
   >Si cette option n’est pas sélectionnée, lorsque les cartes dans d’autres états sont marquées comme étant terminées, elles &quot;tombent&quot; du panorama et ne s’affichent plus.

1. Cliquez sur [!UICONTROL **Appliquer**].

   Tous les objets apparaissent dans la colonne d’entrée du panorama sous la forme de cartes connectées.

   ![Colonne d’ingestion](assets/intake-column-added3.png)

## Création d’une colonne d’entrée à l’aide de filtres avancés

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau Configurer.
1. Développez **[!UICONTROL Board]**.
1. Activez l’option **[!UICONTROL Réception dynamique d’éléments sur le panorama]**.

   La colonne d’ingestion est ajoutée à gauche du panorama. Il reste vide jusqu’à ce que vous lui appliquiez des filtres.

1. Cliquez sur [!UICONTROL **Utiliser des filtres avancés**].
1. Cliquez sur **[!UICONTROL Ajouter des sources de filtre]** et sélectionnez **[!UICONTROL Tâches]** ou **[!UICONTROL Problèmes]**.

   ![Options de filtre avancé de colonne d’entrée](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >Vous pouvez filtrer la colonne d’ingestion pour inclure à la fois les tâches et les problèmes, mais vous devez configurer les filtres séparément pour chaque type d’objet.
   >
   >Vous pouvez également sélectionner des filtres enregistrés et des filtres par défaut du système.

1. Dans le panneau de filtrage, cliquez sur **[!UICONTROL Nouveau filtre]** pour commencer.

   ![Cliquez sur Nouveau filtre](assets/intake-filter-dialog5.png)

1. Créez votre filtre et cliquez sur **[!UICONTROL Enregistrer comme nouveau]**.

   ![Créateur de filtres](assets/intake-filter-dialog6.png)

   Cet exemple illustre un filtre pour les tâches d’un projet spécifique qui ont l’état [!UICONTROL Nouveau] ou [!UICONTROL En cours].

   >[!NOTE]
   >
   >Il est recommandé de ne pas utiliser le caractère générique &quot;Moi&quot; (utilisateur connecté) sur un filtre de panorama, car il n’est pas garanti que l’utilisateur connecté affiche toujours les tâches ou les problèmes. Une fois le panorama configuré avec les tâches et problèmes appropriés, vous pouvez le filtrer pour afficher les éléments d’une personne désignée spécifique. Pour plus d’informations, voir [Filtrage et recherche dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   Pour plus d’informations sur la création d’un filtre, reportez-vous à la section &quot;Création ou modification d’un filtre dans le créateur standard&quot; dans l’article [Créer ou modifier des filtres dans [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Nommez le filtre et cliquez sur **[!UICONTROL Enregistrer]**.

   ![Saisissez un nom pour le filtre](assets/intake-filter-dialog7.png)

   En attribuant au filtre un nom unique, vous pouvez le rechercher ultérieurement.

1. Le filtre apparaît dans votre liste de filtres enregistrés et est automatiquement appliqué à la colonne d’entrée. Cliquez sur le X en haut du panneau de filtrage pour le fermer.

   ![Filtre enregistré](assets/intake-filter-dialog8.png)

1. (Facultatif) Pour partager le filtre avec d’autres utilisateurs, passez la souris sur le filtre enregistré, cliquez sur le menu **[!UICONTROL Plus]** ![Icône Plus de menu](assets/more-icon-spectrum.png), puis sélectionnez **[!UICONTROL Partager]**. Sélectionnez les utilisateurs ou les équipes à partager dans la boîte Partage des filtres . Pour plus d’informations, voir [Partage d’un filtre, d’une vue ou d’un regroupement](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Facultatif) Pour inclure à la fois les tâches et les problèmes dans la colonne d’ingestion, cliquez sur **[!UICONTROL Filtrer les sources]** et sélectionnez l’autre objet pour créer un autre filtre.
1. Lorsque vous avez terminé d’ajouter des filtres, passez en revue la colonne d’ingestion pour vérifier que les tâches et problèmes corrects apparaissent.

   ![Colonne d’ingestion](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Vous pouvez à tout moment mettre à jour les filtres en ouvrant le panneau Configurer, en cliquant sur **[!UICONTROL Filtrer les sources]** et en sélectionnant **[!UICONTROL Tâches]** ou **[!UICONTROL Problèmes]**.

## Utiliser la colonne d&#39;ingestion

Les cartes de la colonne d’entrée ne peuvent pas être modifiées tant que vous ne les déplacez pas dans d’autres colonnes de la carte. Vous pouvez cliquer sur la carte pour l’ouvrir en lecture seule, ou cliquer sur ![Ouvrir la tâche ou le problème](assets/boards-launch-icon.png) pour ouvrir la tâche ou le problème dans un nouvel onglet du navigateur.

Vous pouvez réorganiser manuellement les éléments de la colonne d’ingestion.

Les icônes situées en haut à droite de la colonne d’entrée indiquent le nombre de cartes actuellement présentes dans la colonne et le nombre de filtres appliqués.

1. (Facultatif) Pour rechercher un élément dans la colonne d’ingestion, cliquez sur ![Icône de recherche](assets/search-icon.png) dans la colonne.
1. (Facultatif) Pour déplacer une carte de la colonne d’entrée vers une autre colonne, faites-la glisser et déposez-la à l’emplacement où elle doit apparaître.

   Ou

   Cliquez sur l’icône **[!UICONTROL Plus]** du menu ![Icône Plus de menu](assets/more-icon-spectrum.png) sur la carte, puis sélectionnez **[!UICONTROL Déplacer]**. Ensuite, dans la zone **[!UICONTROL Déplacer l’élément]**, choisissez une autre colonne et sélectionnez **[!UICONTROL Déplacer]**.

1. (Facultatif) Pour supprimer la colonne d’ingestion, cliquez sur le menu **[!UICONTROL Plus]** ![Icône Plus de menu](assets/more-icon-spectrum.png) et sélectionnez **[!UICONTROL Supprimer]**.
