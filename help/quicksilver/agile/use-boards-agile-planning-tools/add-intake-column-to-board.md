---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Ajout d’une colonne d’entrée à un panorama
description: Vous pouvez éventuellement ajouter une colonne d’entrée à votre panorama qui extrait automatiquement les tâches et les problèmes en tant que cartes connectées lorsqu’ils sont ajoutés dans Workfront, en fonction des filtres que vous définissez.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 0c0c1f538cfd12e18c504fcb42ee424789d1cde8
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 96%

---

# Ajouter une colonne d’entrée à un panorama

Vous pouvez éventuellement ajouter une colonne d’entrée à votre panorama qui extrait automatiquement les tâches et les problèmes en tant que cartes connectées lorsqu’ils sont ajoutés dans [!DNL Workfront], en fonction des filtres que vous définissez. La colonne de saisie peut servir de colonne de liste d’attente pour une équipe Kanban, d’emplacement de saisie pour une équipe d’assistance afin de voir les problèmes au fur et à mesure qu’ils sont ajoutés à une file d’attente des demandes, ou pour toute autre raison dont vous avez besoin.

Une seule colonne de saisie est autorisée sur un panorama et apparaît toujours comme la colonne à l’extrémité gauche.

La colonne de saisie n’est pas disponible sur un panorama dynamique. Vous pouvez toutefois mettre à jour les filtres qui définissent les cartes qui sont importées sur un panorama dynamique. Lorsque vous modifiez ces filtres sur un panorama dynamique, les paramètres de carte qui ne font pas partie de la tâche ou du problème Workfront (comme les balises) sont réinitialisés.

>[!NOTE]
>
>Pour des raisons de sécurité, seule la personne propriétaire d’un panorama peut modifier les filtres du panorama dans le panneau Configurer.

La colonne d’entrée est limitée à 300 tâches et 300 problèmes. L’ordre par défaut des éléments dans la colonne d’entrée est le suivant :

Tâches :

* Ordre principal : nom du projet
* Ordre secondaire : structure de répartition du travail

Problèmes :

* Ordre principal : nom du projet
* Ordre secondaire : numéro de référence

>[!IMPORTANT]
>
>Il est recommandé d’actualiser fréquemment le panorama si plusieurs personnes y travaillent simultanément. L’actualisation de la page permet de maintenir les modifications visuelles sur le panorama à jour et d’éviter des problèmes tels que les cartes en double qui sont déplacées sur le panorama à partir de la colonne de saisie.
>
>Pour vous synchroniser avec Workfront et faire apparaître de nouvelles tâches et problèmes sur le panorama ou la colonne d’accueil, cliquez sur le menu **[!UICONTROL Plus]** ![[!UICONTROL Plus de menu]](assets/more-icon-spectrum.png) en regard du nom du panorama et sélectionnez **[!UICONTROL Synchroniser les éléments connectés]**.

Pour plus d’informations sur les colonnes, voir [Gérer des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Pour plus d’informations sur les cartes connectées, voir [Utiliser des cartes connectées sur des panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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

## Créer une colonne d’entrée à l’aide de filtres simples

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau de configuration.
1. Développez **[!UICONTROL Panorama]**.
1. Activez **[!UICONTROL Ajout dynamique d’objets au panorama]**.

   ![Options de filtrage simple des colonnes d’entrée](assets/intake-column-simple-filters.png)

   La colonne d’entrée est ajoutée à gauche du panorama. Elle reste vide jusqu’à ce que vous y appliquiez des filtres.

1. (Facultatif) Recherchez et sélectionnez [!UICONTROL **Projets**] [!DNL Workfront].
1. (Facultatif) Recherchez et sélectionnez des [!UICONTROL **Affectations**] de personne ou d’équipe.
1. Sélectionnez [!UICONTROL **Inclure le travail terminé**] pour afficher les tâches et les problèmes dont le statut est Terminé dans la colonne d’entrée.

   >[!NOTE]
   >
   >Si cette option n’est pas sélectionnée, lorsque les cartes portant d’autres statuts sont marquées comme étant terminées, elles « tombent » du panorama et ne s’affichent plus.

1. Cliquez sur [!UICONTROL **Appliquer**].

   Tous les objets apparaissent dans la colonne d’entrée du panorama sous la forme de cartes connectées.

   ![Colonne d’entrée](assets/intake-column-added3.png)

## Créer une colonne d’entrée à l’aide de filtres avancés

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Configurer]** à droite du panorama pour ouvrir le panneau de configuration.
1. Développez **[!UICONTROL Panorama]**.
1. Activez **[!UICONTROL Ajout dynamique d’objets au panorama]**.

   La colonne d’entrée est ajoutée à gauche du panorama. Elle reste vide jusqu’à ce que vous y appliquiez des filtres.

1. Cliquez sur [!UICONTROL **Utiliser des filtres avancés**].
1. Cliquez sur **[!UICONTROL Ajouter des sources de filtre]** et sélectionnez **[!UICONTROL Tâche]** ou **[!UICONTROL Problèmes]**.

   ![Options de filtrage avancées de la colonne d’entrée](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >Vous pouvez filtrer la colonne d’entrée pour inclure à la fois les tâches et les problèmes, mais vous devez configurer les filtres séparément pour chaque type d’objet.
   >
   >Vous pouvez également sélectionner des filtres enregistrés et des filtres par défaut du système.

1. Dans le panneau de filtres, cliquez sur **[!UICONTROL Nouveau filtre]** pour commencer.

   ![Clic sur Nouveau filtre](assets/intake-filter-dialog5.png)

1. Créez votre filtre et cliquez sur **[!UICONTROL Enregistrer comme nouveau]**.

   ![Créateur de filtres](assets/intake-filter-dialog6.png)

   Cet exemple affiche un filtre pour les tâches d’un projet spécifique qui sont au statut [!UICONTROL Nouveau] ou [!UICONTROL En cours].

   >[!NOTE]
   >
   >Il est recommandé de ne pas utiliser le caractère générique « Moi » (personne connectée) sur un filtre de panorama, car il n’est pas garanti que la personne connectée affiche toujours les tâches ou les problèmes. Une fois le panorama configuré avec les tâches et problèmes appropriés, vous pouvez le filtrer pour afficher les éléments d’une personne cessionnaire spécifique. Pour plus d’informations, consultez l’article [Filtres et recherche dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   Pour plus d’informations sur la création d’un filtre, consultez la section « Création ou modification d’un filtre dans le créateur standard » de l’article [Création ou modification de filtres dans  [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Nommez le filtre, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![Saisie du nom du filtre](assets/intake-filter-dialog7.png)

   Vous pourrez rechercher le filtre ultérieurement en lui donnant un nom unique.

1. Le filtre apparaît dans votre liste de filtres enregistrés et est automatiquement appliqué à la colonne d’entrée. Cliquez sur le X en haut du panneau de filtre pour le fermer.

   ![Filtre enregistré](assets/intake-filter-dialog8.png)

1. (Facultatif) Pour partager le filtre avec d’autres personnes, pointez sur le filtre enregistré, cliquez sur le menu **[!UICONTROL Plus]** ![Icône de menu Plus](assets/more-icon-spectrum.png), puis sélectionnez **[!UICONTROL Partager]**. Sélectionnez les utilisateurs et utilisatrices ou les équipes à partager dans la zone Partage des filtres. Pour plus d’informations, voir [Partager un filtre, une vue ou un regroupement](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Facultatif) Pour inclure les tâches et les problèmes dans la colonne d’entrée, cliquez sur **[!UICONTROL Sources de filtre]** et sélectionnez l’autre objet pour créer un autre filtre.
1. Lorsque vous avez terminé d’ajouter des filtres, passez en revue la colonne d’entrée pour vérifier que les tâches et problèmes corrects apparaissent.

   ![Colonne d’entrée](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Vous pouvez à tout moment mettre à jour les filtres en ouvrant le panneau Configurer, en cliquant sur **[!UICONTROL Sources de filtre]** et en sélectionnant **[!UICONTROL Tâche]** ou **[!UICONTROL Problèmes]**.

## Utiliser la colonne d’entrée

Les cartes de la colonne d’entrée ne peuvent pas être modifiées tant que vous ne les déplacez pas dans d’autres colonnes du panorama. Vous pouvez cliquer sur la carte pour l’ouvrir en lecture seule ou cliquer sur ![Ouvrir une tâche ou un problème](assets/boards-launch-icon.png) pour les ouvrir dans un nouvel onglet du navigateur.

Vous pouvez réorganiser manuellement les éléments de la colonne d’entrée.

Les icônes situées en haut à droite de la colonne d’entrée indiquent le nombre de cartes actuellement présentes dans la colonne et le nombre de filtres appliqués.

1. (Facultatif) Pour rechercher un élément dans la colonne d’entrée, cliquez sur l’![icône Rechercher](assets/search-icon.png) sur la colonne.
1. (Facultatif) Pour déplacer une carte de la colonne d’entrée vers une autre colonne, faites-la glisser et déposez-la à l’emplacement où elle doit apparaître.

   Ou

   Cliquez sur le menu **[!UICONTROL Plus]** ![icône de menu Plus](assets/more-icon-spectrum.png) sur la carte, puis sélectionnez **[!UICONTROL Déplacer]**. Ensuite, dans la zone **[!UICONTROL Déplacer un élément]**, choisissez une autre colonne et sélectionnez **[!UICONTROL Déplacer]**.

1. (Facultatif) Pour supprimer la colonne d’entrée, cliquez sur le menu **[!UICONTROL Plus]** ![Icône de menu Plus](assets/more-icon-spectrum.png), puis sélectionnez **[!UICONTROL Supprimer]**.
