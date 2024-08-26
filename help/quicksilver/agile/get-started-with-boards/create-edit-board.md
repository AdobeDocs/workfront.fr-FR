---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Création ou modification d’un panorama
description: Dans le tableau de bord [!UICONTROL Panoramas], vous pouvez créer un panorama ou en modifier un existant.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: efe636e14964cc8705839c9f534a9947327803d7
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 96%

---

# Créer ou modifier un panorama

<!-- Audited: 12/2023 -->

Dans le tableau de bord [!UICONTROL Panoramas], vous pouvez créer un panorama ou en modifier un existant.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : contributeur ou contributrice ou supérieure </p>
 <p>ou</p> 
<p>Actuel : [!UICONTROL Request] ou supérieure </p> 
</td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un panorama

{{step1-to-boards}}

1. Cliquez sur **[!UICONTROL Ajouter un panorama]**.

1. Sélectionnez un modèle pour le panorama.

   | Modèle | Description |
   |---------|----------|
   | Panorama de base | Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. |
   | Panorama Kanban | Les colonnes suivantes sont fournies sur le panorama : Liste d’attente, Nouveau, En cours, Terminé et En attente. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut.<p>Pour utiliser la liste d’attente, vous devez configurer des filtres pour la colonne de saisie. Pour plus d’informations, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Pour consulter les politiques par défaut pour chaque colonne, cliquez sur le menu Plus  sur une colonne et sélectionnez Modifier. [!UICONTROL ****][!UICONTROL ****] Vous pouvez modifier l’une de ces politiques prédéfinies. Pour plus d’informations, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Panorama rétrospectif | Les colonnes suivantes sont fournies sur le panorama : Qu’est-ce qui a bien fonctionné ? Qu’est-ce qui pourrait être amélioré ? Qui devons-nous célébrer ? Que pouvons-nous faire pour aller plus vite ? Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune politique de colonne n’est appliquée. |
   | Panorama dynamique | Les colonnes suivantes sont fournies sur le panorama : Non sélectionné, Nouveau, En cours, En attente et Terminé. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. (La colonne Non sélectionné peut être renommée mais pas supprimée. Cette colonne contient toutes les cartes dont le statut ne correspond à aucun des autres statuts de colonne.) <p>Les politiques de colonne par défaut attribuent des cartes aux colonnes en fonction de leur statut. Pour plus d’informations, voir [Gérer les colonnes du panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Pour un panorama dynamique uniquement, suivez les étapes de l’assistant de configuration :

   1. Saisissez un nom pour le panorama et cliquez sur [!UICONTROL **Suivant**].
   1. Recherchez et sélectionnez des [!UICONTROL **Projets**] [!DNL Workfront] pour intégrer des tâches et des problèmes au panorama.
   1. Recherchez et sélectionnez des [!UICONTROL **Affectations**] pour intégrer des tâches et des problèmes au panorama.

      Tous les objets apparaissent sur le panorama sous forme de cartes connectées.

      Le compteur Cartes en cours d’ajout indique le nombre de cartes qui seront sur le panorama. [!UICONTROL ****] Par exemple, si vous sélectionnez un projet comportant 100 tâches et problèmes, le compteur affiche 100. Si vous ajoutez une affectation utilisateur ou utilisatrice et que cette personne est affectée à 5 tâches sur le projet, le compteur affiche 5.

      >[!NOTE]
      >
      >La limite de carte pour les panoramas dynamiques est de 700 tâches et de 700 problèmes, pour un total de 1 400 cartes. Un nombre élevé de cartes sur le panorama peut affecter les performances du panorama. Toutes les cartes archivées, qu’elles soient masquées ou visibles, sont comptabilisées dans cette limite.

   1. (Facultatif) Sélectionnez Ne pas archiver les cartes terminées pour afficher les tâches et les problèmes terminés sur le panorama sous la forme de cartes visibles dans la colonne Terminé. [!UICONTROL ****] Lorsque cette option n’est pas sélectionnée, les cartes terminées au moment de la création du panorama sont importées sous la forme de cartes archivées.

      >[!NOTE]
      >
      >Par défaut, les cartes archivées ne s’affichent pas sur le panorama. Pour afficher les cartes archivées, vous devez activer un paramètre de configuration, puis filtrer le panorama afin d’afficher les cartes archivées. Pour plus d’informations, voir [Personnaliser les champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) et [Filtrer et rechercher dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Facultatif) Cliquez sur [!UICONTROL **Utiliser des filtres avancés**] pour afficher d’autres options de filtre.

      Il s’agit du même processus que la création d’un filtre sur une colonne de saisie. Pour plus d’informations, voir [Ajouter une colonne de saisie à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Si vous mettez à jour les filtres sur un panorama dynamique après sa création, les paramètres de carte qui ne font pas partie de la tâche ou du problème Workfront (comme les balises) sont réinitialisés.

   1. Après avoir ajouté les filtres, cliquez sur [!UICONTROL **Créer un panorama**].

1. Saisissez un nom pour panorama dans la zone **[!UICONTROL Panorama]** et appuyez sur Entrée.
1. Configurez le panorama selon vos besoins.

   Pour plus d’informations, voir [Ajouter ou supprimer des membres d’un panorama](../../agile/get-started-with-boards/add-members-to-board.md), [Gérer les colonnes du panorama](../../agile/get-started-with-boards/manage-board-columns.md), [Ajouter une carte ad hoc à un panorama](../../agile/get-started-with-boards/add-card-to-board.md) et [Utiliser des cartes connectées sur des panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Cliquez sur **[!UICONTROL Tous les panoramas]** pour revenir au tableau de bord des panoramas.

   Vous pouvez également localiser le menu déroulant portant le nom du panorama actuel, puis cliquer dessus pour passer à un autre panorama.

   ![Liste des panoramas](assets/boards-button-list-of-boards-350x188.png)

## Modifier un panorama existant

{{step1-to-boards}}

1. Dans le tableau de bord, sélectionnez le panorama à ouvrir.
1. Modifiez le panorama selon vos besoins. Vous pouvez cliquer sur le nom du panorama pour le renommer.

   Pour plus d’informations, voir [Ajouter ou supprimer des membres d’un panorama](../../agile/get-started-with-boards/add-members-to-board.md), [Gérer les colonnes du panorama](../../agile/get-started-with-boards/manage-board-columns.md) et [Ajouter une carte à un panorama](../../agile/get-started-with-boards/add-card-to-board.md).

1. Cliquez sur **[!UICONTROL Tous les panoramas]** pour revenir au tableau de bord des panoramas.

   Vous pouvez également localiser le menu déroulant portant le nom du panorama actuel, puis cliquer dessus pour passer à un autre panorama.

