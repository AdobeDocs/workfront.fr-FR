---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Créer ou modifier un panorama
description: Dans la [!UICONTROL panoramas] vous pouvez créer un panorama ou en modifier un existant.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: d593d288546abb4a674646519c6245563673b938
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Créer ou modifier un panorama

<!-- Audited: 12/2023 -->

Dans la [!UICONTROL panoramas] vous pouvez créer un panorama ou en modifier un existant.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>Nouveau : contributeur ou version ultérieure </p>
 <p>ou</p> 
<p>Actuel : [!UICONTROL Request] ou version ultérieure </p> 
</td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Création d’un panorama

{{step1-to-boards}}

1. Cliquez sur **[!UICONTROL Ajouter un panorama]**.

1. Sélectionnez un modèle pour le panorama.

   | Modèle | Description |
   |---------|----------|
   | Panorama de base | Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. |
   | Panorama Kanban | Les colonnes suivantes sont fournies sur le tableau : Backlog, New, In Progress, Complete et On hold. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut.<p>Pour utiliser le journal des logs, vous devez configurer des filtres pour la colonne d&#39;ingestion. Pour plus d’informations, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Pour consulter les stratégies par défaut pour chaque colonne, cliquez sur le bouton [!UICONTROL **Plus** menu] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces stratégies prédéfinies. Pour plus d’informations, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Panorama rétrospectif | Les colonnes suivantes sont fournies sur le tableau : Qu’est-ce qui s’est bien passé ? Qu&#39;est-ce qui pourrait être amélioré ? Qui devrions-nous célébrer ? Que pouvons-nous faire pour aller plus vite ? Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune stratégie de colonne n’est appliquée. |
   | Panorama dynamique | Les colonnes suivantes sont fournies sur le panorama : Non sélectionné, Nouveau, En cours, En attente et Terminé. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. (La colonne Non sélectionné peut être renommée mais pas supprimée. Cette colonne contient toutes les cartes dont l’état ne correspond à aucun des autres états de colonne.) <p>Les stratégies de colonne par défaut attribuent des cartes aux colonnes en fonction de leur état. Pour plus d’informations, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Pour une carte dynamique uniquement, suivez les étapes de l&#39;assistant de configuration :

   1. Saisissez le nom du panorama, puis cliquez sur [!UICONTROL **Suivant**].
   1. Recherchez et sélectionnez [!DNL Workfront] [!UICONTROL **Projets**] pour intégrer des tâches et des problèmes au tableau.
   1. Recherchez et sélectionnez [!UICONTROL **Affectations**] pour intégrer des tâches et des problèmes au tableau.

      Tous les objets apparaissent sur le panorama sous forme de cartes connectées.

      La variable [!UICONTROL **Cartes ajoutées**] compteur indique le nombre de cartes qui seront sur le panorama. Par exemple, si vous sélectionnez un projet comportant 100 tâches et problèmes, le compteur affiche 100. Si vous ajoutez une affectation utilisateur et que cette personne est affectée à 5 tâches sur le projet, le compteur affiche 5.

      >[!NOTE]
      >
      >La limite de carte pour les panoramas dynamiques est de 700 tâches et de 700 problèmes, pour un total de 1 400 cartes. Un nombre élevé de cartes sur le panorama peut affecter les performances du panorama.

   1. (Facultatif) Sélectionnez [!UICONTROL **Ne pas archiver les cartes terminées**] pour afficher les tâches terminées et les problèmes sur le panorama sous forme de cartes visibles dans la colonne Terminé . Lorsque cette option n’est pas sélectionnée, les cartes terminées au moment de la création du panorama sont importées sous forme de cartes archivées.

      >[!NOTE]
      >
      >Par défaut, les cartes archivées ne s’affichent pas sur le panorama. Pour afficher les cartes archivées, vous devez activer un paramètre de configuration, puis filtrer le panorama afin d’afficher les cartes archivées. Pour plus d’informations, voir [Personnalisation des champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) et [Filtrage et recherche dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Facultatif) Cliquez sur [!UICONTROL **Utilisation de filtres avancés**] pour afficher d’autres options de filtrage.

      Il s’agit du même processus que la création d’un filtre sur une colonne d’entrée. Pour plus d’informations, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Si vous mettez à jour les filtres sur un panorama dynamique après sa création, les paramètres de carte qui ne font pas partie de la tâche ou du problème Workfront (comme les balises) sont réinitialisés.

   1. Après avoir ajouté les filtres, cliquez sur [!UICONTROL **Créer un panorama**].

1. Saisissez le nom du panorama dans la zone **[!UICONTROL board]** et appuyez sur Entrée.
1. Configurez le panorama suivant vos besoins.

   Pour plus d’informations, voir [Ajout ou suppression de membres d’un panorama](../../agile/get-started-with-boards/add-members-to-board.md), [Gestion des colonnes de panorama](../../agile/get-started-with-boards/manage-board-columns.md), [Ajouter une carte ad hoc à un panorama](../../agile/get-started-with-boards/add-card-to-board.md), et [Utilisation de cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Cliquez sur **[!UICONTROL Toutes les panoramas]** pour revenir au tableau de bord des panoramas.

   Vous pouvez également localiser le menu déroulant intitulé &quot;nom du panorama actuel&quot;, puis cliquer dessus pour passer à un autre panorama.

   ![Liste des panoramas](assets/boards-button-list-of-boards-350x188.png)

## Modifier un panorama existant

{{step1-to-boards}}

1. Dans le tableau de bord, sélectionnez le panorama à ouvrir.
1. Modifiez le panorama si nécessaire. Cliquez sur le nom du panorama pour le renommer.

   Pour plus d’informations, voir [Ajout ou suppression de membres d’un panorama](../../agile/get-started-with-boards/add-members-to-board.md), [Gestion des colonnes de panorama](../../agile/get-started-with-boards/manage-board-columns.md), et [Ajouter une carte à un panorama](../../agile/get-started-with-boards/add-card-to-board.md).

1. Cliquez sur **[!UICONTROL Toutes les panoramas]** pour revenir au tableau de bord des panoramas.

   Vous pouvez également localiser le menu déroulant intitulé &quot;nom du panorama actuel&quot;, puis cliquer dessus pour passer à un autre panorama.
