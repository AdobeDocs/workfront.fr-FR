---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Créer ou modifier un panorama
description: À partir du tableau de bord des [!UICONTROL Panoramas], vous pouvez créer un nouveau panorama ou modifier un panorama existant.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 91%

---

# Créer ou modifier un panorama

<!-- Audited: 12/2023 -->

À partir du tableau de bord des [!UICONTROL Panoramas], vous pouvez créer un nouveau panorama ou modifier un panorama existant.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou version ultérieure</p> 
   <p>Requête ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un panorama

{{step1-to-boards}}

1. Cliquez sur **[!UICONTROL Ajouter un panorama]**.

1. Sélectionnez un modèle pour le panorama.

   | Modèle | Description |
   |---------|----------|
   | Panorama de base | Trois colonnes par défaut sont fournies sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Trois colonnes par défaut sont fournies sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. |
   | Panorama Kanban | Les colonnes suivantes sont affichées sur le panorama : Liste d’attente, Nouveau, En cours, Terminé et Suspendu. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut.<p>Pour utiliser la liste d’attente, vous devez définir des filtres pour la colonne de saisie. Pour plus d’informations, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Pour revoir les politiques par défaut de chaque colonne, cliquez sur le menu [!UICONTROL **Plus** &#x200B;] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une ou l’autre de ces politiques prédéfinies. Pour plus d’informations, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Panorama rétrospectif | Les colonnes suivantes sont fournies dans le panorama : Points forts Améliorations possibles Qui devons-nous célébrer Que pouvons-nous faire pour aller plus vite Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune politique de colonne n’est appliquée. |
   | Panorama dynamique | Les colonnes suivantes sont fournies dans le panorama : Non sélectionné, Nouveau, En cours, Suspendu et Terminé. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. (La colonne Non sélectionné(e) peut être renommée mais pas supprimée. Cette colonne contient toutes les cartes dont le statut ne correspond à aucun des statuts des autres colonnes.) <p>Les politiques de colonne par défaut attribuent des cartes aux colonnes en fonction de leur statut. Pour plus d’informations, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Pour un panorama dynamique uniquement, suivez les étapes de l’assistant de configuration :

   1. Saisissez un nom pour le panorama et cliquez sur [!UICONTROL **Suivant**].
   1. Recherchez et sélectionnez les [!UICONTROL **Projets**] [!DNL Workfront] pour faire apparaître les tâches et les problèmes sur le panorama.
   1. Recherchez et sélectionnez les [!UICONTROL **Affectations**] pour faire apparaître les tâches et les problèmes sur le panorama.

      Tous les objets apparaissent sur le panorama sous forme de cartes connectées.

      Le compteur [!UICONTROL **Cartes ajoutées**] indique le nombre de cartes qui seront présentes sur le panorama. Par exemple, si vous sélectionnez un projet comportant 100 tâches et problèmes, le compteur affiche 100. Si vous ajoutez une affectation utilisateur ou utilisatrice et que cette personne est affectée à 5 tâches sur le projet, le compteur affiche 5.

      >[!NOTE]
      >
      >La limite de carte pour les panoramas dynamiques est de 700 tâches et de 700 problèmes, pour un total de 1 400 cartes. Un nombre élevé de cartes sur le tableau peut affecter les performances du tableau. Toutes les cartes archivées, à la fois masquées et visibles, sont prises en compte dans cette limite.

   1. (Facultatif) Sélectionnez [!UICONTROL **Ne pas archiver les cartes terminées**] pour faire apparaître les tâches et les problèmes terminés sur le panorama sous forme de cartes visibles dans la colonne Terminé. Si cette option n’est pas sélectionnée, les cartes terminées au moment de la création du panorama sont introduites dans le tableau en tant que cartes archivées.

      >[!NOTE]
      >
      >Par défaut, les cartes archivées ne sont pas affichées sur le panorama. Pour afficher les cartes archivées, vous devez activer un paramètre de configuration, puis filtrer le panorama pour afficher les cartes archivées. Pour plus d’informations, voir [Personnaliser les champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) et [Filtrer et rechercher dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Facultatif) Cliquez sur [!UICONTROL **Utiliser les filtres avancés**] pour afficher des options de filtrage supplémentaires.

      Il s’agit du même processus que la création d’un filtre sur une colonne d’entrée. Pour plus d’informations, voir [Ajouter une colonne d’entrée à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Si vous mettez à jour les filtres sur un panorama dynamique après sa création, les paramètres de carte qui ne font pas partie de la tâche ou du problème Workfront (comme les balises) sont réinitialisés.

   1. Après avoir ajouté les filtres, cliquez sur [!UICONTROL **Créer le panorama**].

1. Saisissez un nom pour le panorama dans le champ **[!UICONTROL Panorama]** et appuyez sur Entrée.
1. Configurez le panorama si nécessaire.

   Pour plus d’informations, voir [Ajouter ou supprimer des personnes membres d’un panorama](../../agile/get-started-with-boards/add-members-to-board.md), [Gérer les colonnes du panorama](../../agile/get-started-with-boards/manage-board-columns.md), [Ajouter une carte ad hoc à un panorama](../../agile/get-started-with-boards/add-card-to-board.md) et [Utiliser des cartes connectées sur des panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Cliquez sur **[!UICONTROL Tous les panoramas]** pour revenir au tableau de bord des panoramas.

   Vous pouvez également localiser le menu déroulant portant le nom du panorama actuel et cliquer dessus pour passer à un autre panorama.

   ![Liste des panoramas](assets/boards-button-list-of-boards-350x188.png)

## Modifier un panorama existant

{{step1-to-boards}}

1. Dans le tableau de bord, sélectionnez le panorama à ouvrir.
1. Modifier le panorama si nécessaire. Vous pouvez cliquer sur le nom du panorama pour le renommer.

   Pour synchroniser les cartes connectées avec Workfront et importer de nouvelles tâches et de nouveaux événements sur le panorama ou la colonne d’entrée, cliquez sur le menu **[!UICONTROL Plus]** ![[!UICONTROL Menu Plus]](assets/more-icon-spectrum.png) à côté du nom du panorama et sélectionnez **[!UICONTROL Synchroniser les éléments connectés]**.

   Pour plus d’informations, voir [Ajouter ou supprimer des personnes membres d’un panorama](../../agile/get-started-with-boards/add-members-to-board.md), [Gérer les colonnes d’un panorama](../../agile/get-started-with-boards/manage-board-columns.md) et [Ajouter une carte à un panorama](../../agile/get-started-with-boards/add-card-to-board.md).

1. Cliquez sur **[!UICONTROL Tous les panoramas]** pour revenir au tableau de bord des panoramas.

   Vous pouvez également localiser le menu déroulant portant le nom du panorama actuel et cliquer dessus pour passer à un autre panorama.

