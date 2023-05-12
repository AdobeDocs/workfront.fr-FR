---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Création ou modification d’un panorama
description: Dans la [!UICONTROL panoramas] tableau de bord, vous pouvez créer un panorama ou en modifier un existant.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 5e73603b695ff7456216ca7a4e15ce527b01559d
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 3%

---

# Création ou modification d’un panorama

Dans la [!UICONTROL panoramas] tableau de bord, vous pouvez créer un panorama ou en modifier un existant.

Pour ajouter un panorama à un flux de travail, reportez-vous à la section [Gestion des workflows](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

## Création d’un panorama

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Panoramas]**.
1. Pour créer un panorama autonome, cliquez sur **[!UICONTROL Ajouter un panorama]** dans le [!UICONTROL Panoramas] zone. Pour ajouter un panorama à un flux de travail, reportez-vous à la section [Gestion des workflows](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

1. Sélectionnez un modèle pour le panorama.

   | Modèle | Description |
   |---------|----------|
   | Panorama de base | Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Trois colonnes sont fournies par défaut sur le panorama. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. |
   | Panorama Kanban | Les colonnes suivantes sont fournies sur le panorama : En attente, nouveauté, En cours, Terminé et En attente. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut.<p>Pour utiliser le journal des logs, vous devez configurer des filtres pour la colonne d&#39;ingestion. Pour plus d’informations, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Pour consulter les stratégies par défaut pour chaque colonne, cliquez sur le bouton [!UICONTROL **Plus** menu] sur une colonne et sélectionnez [!UICONTROL **Modifier**]. Vous pouvez modifier l’une de ces stratégies prédéfinies. Pour plus d’informations, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Panorama rétrospectif | Les colonnes suivantes sont fournies sur le panorama : Qu&#39;est-ce qui s&#39;est bien passé ? Améliorations possibles? Qui devons-nous célébrer? Que pouvons-nous faire pour aller plus vite? Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. <p>Aucune stratégie de colonne n’est appliquée. |
   | Panorama dynamique | Les colonnes suivantes sont fournies sur le panorama : Non sélectionné, Nouveau, En cours, En attente et Terminé. Vous pouvez ajouter de nouvelles colonnes et renommer ou supprimer les colonnes par défaut. (La colonne Non sélectionné peut être renommée mais pas supprimée. Cette colonne contient toutes les cartes dont l’état ne correspond à aucun des autres états de colonne.) <p>Les stratégies de colonne par défaut attribuent des cartes aux colonnes en fonction de leur état. Pour plus d’informations, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). <p>**REMARQUE :** Le panorama dynamique n’est disponible que par le biais de l’accord préalable aux fonctionnalités des panoramas Workfront. |

1. Pour une carte dynamique uniquement, suivez les étapes de l&#39;assistant de configuration :

   1. Recherchez et sélectionnez [!DNL Workfront] [!UICONTROL **Projets**] pour intégrer des tâches et des problèmes au tableau.
   1. Recherchez et sélectionnez [!UICONTROL **Affectations**] pour intégrer des tâches et des problèmes au tableau.

      Tous les objets apparaissent sur le panorama sous forme de cartes connectées.

      Le [!UICONTROL **Cartes ajoutées**] compteur indique le nombre de cartes qui seront sur le panorama. Par exemple, si vous sélectionnez un projet comportant 100 tâches et problèmes, le compteur affiche 100. Si vous ajoutez une affectation utilisateur et que cette personne est affectée à 5 tâches sur le projet, le compteur affiche 5.

   1. (Facultatif) Sélectionnez [!UICONTROL **Inclure le travail terminé**] pour inclure les cartes complétées sur le panorama.

      >[!NOTE]
      >
      >Si cette option n’est pas sélectionnée, lorsque les cartes dans d’autres états sont marquées comme étant terminées, elles &quot;tombent&quot; du panorama et ne s’affichent plus.

   1. (Facultatif) Cliquez sur [!UICONTROL **Utilisation de filtres avancés**] pour afficher d’autres options de filtrage.

      Il s’agit du même processus que la création d’un filtre sur une colonne d’entrée. Pour plus d’informations, voir [Ajout d’une colonne d’ingestion à un panorama](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. Après avoir ajouté les filtres, cliquez sur [!UICONTROL **Créer un panorama**].

1. Saisissez le nom du panorama dans la zone **[!UICONTROL Panorama]** et appuyez sur Entrée.
1. Configurez le panorama suivant vos besoins.

   Pour plus d’informations, voir [Ajout ou suppression de membres d’un panorama](../../agile/get-started-with-boards/add-members-to-board.md), [Gestion des colonnes de panorama](../../agile/get-started-with-boards/manage-board-columns.md), [Ajout d’une carte ad hoc à un panorama](../../agile/get-started-with-boards/add-card-to-board.md), et [Utilisation de cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Cliquez sur **[!UICONTROL Toutes les panoramas]** pour revenir au tableau de bord des panoramas.

   Vous pouvez également localiser le menu déroulant intitulé &quot;nom du panorama actuel&quot;, puis cliquer dessus pour passer à un autre panorama.

   ![Liste des panoramas](assets/boards-button-list-of-boards-350x188.png)

## Modification d’un panorama existant

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Panoramas]**.
1. Dans le tableau de bord, sélectionnez le panorama à ouvrir.
1. Modifiez le panorama si nécessaire. Vous pouvez cliquer sur le nom du panorama pour le renommer.

   Pour plus d’informations, voir [Ajout ou suppression de membres d’un panorama](../../agile/get-started-with-boards/add-members-to-board.md), [Gestion des colonnes de panorama](../../agile/get-started-with-boards/manage-board-columns.md), et [Ajout d’une carte à un panorama](../../agile/get-started-with-boards/add-card-to-board.md).

1. Cliquez sur **[!UICONTROL Toutes les panoramas]** pour revenir au tableau de bord des panoramas.

   Vous pouvez également localiser le menu déroulant intitulé &quot;nom du panorama actuel&quot;, puis cliquer dessus pour passer à un autre panorama.
