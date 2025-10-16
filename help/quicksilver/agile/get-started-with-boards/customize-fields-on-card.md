---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personnaliser les champs affichés sur une carte
description: Vous pouvez personnaliser les champs affichés sur une carte en désactivant un champ pour qu’il ne soit pas affiché dans la carte complète ou dans l’affichage condensé, ou en masquant un champ dans l’affichage condensé de la carte.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 97%

---

# Personnaliser les champs affichés sur une carte

Par défaut, tous les champs disponibles sont affichés sur une carte, à la fois dans l’affichage complet lorsque la carte est ouverte et dans l’affichage condensé de la carte sur le panorama. Vous pouvez personnaliser les champs affichés des manières suivantes :

* Désactiver un champ pour qu’il ne s’affiche dans aucune des deux vues
* Masquer un champ dans l’affichage condensé de la carte

Si un champ contient une valeur et que vous désactivez le champ, la valeur est conservée si vous réactivez le champ ultérieurement.

Il est également possible d’afficher ou de masquer les sections, qui apparaissent comme les options de navigation de gauche sur les détails de la carte.

Vous pouvez également afficher les champs personnalisés qui ont été créés précédemment. Vous ne pouvez pas concevoir et créer de nouveaux champs personnalisés dans un panorama.

>[!NOTE]
>
>Toutes les personnalisations de champs que vous effectuez ne s’appliquent qu’au panorama dans lequel vous travaillez.

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

## Configurer les cartes {#configure-cards}

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur [!UICONTROL **Configurer**] à droite de la carte pour ouvrir le panneau de configuration.
1. Développez [!UICONTROL **Cartes**].

   La plupart des champs et sections sont activés par défaut.

1. Désactivez un champ ou une section pour désactiver l’élément dans les deux affichages de carte.
1. Cliquez sur l’![icône Masquer](assets/eye-hide-icon.png) en regard d’un champ ou d’une section pour le masquer dans la vue condensée.
1. Pour afficher tous les champs et toutes les sections dans les deux affichages, cliquez sur [!UICONTROL **Restaurer tous les champs par défaut**].
1. Cliquez sur [!UICONTROL **Masquer la configuration**] pour fermer le panneau de configuration.

## Ajouter des champs personnalisés aux cartes

Les champs personnalisés sont disponibles sur les cartes connectées. Ils ne sont visibles que sur l’affichage de carte complet, et non sur l’affichage de carte condensé.

Les données des champs personnalisés sont modifiables sur la carte, bien que certains éléments personnalisés ne puissent être modifiés que sur le champ d’origine et non sur la carte.

1. Accédez à un panorama et cliquez sur [!UICONTROL **Configurer**] pour ouvrir le panneau de configuration.
1. Développez [!UICONTROL **Cartes**].
1. Sous [!UICONTROL Champs de carte], cliquez sur [!UICONTROL **Ajouter un champ personnalisé**].
1. Sélectionnez [!UICONTROL **Tâche**] ou [!UICONTROL **Problème**].

   Les catégories de champs disponibles pour les tâches ou les problèmes apparaissent. Développez une catégorie pour afficher tous les champs. Vous pouvez également rechercher un champ.

   ![Recherche d’un champ personnalisé](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Les types de champs suivants ne peuvent pas être ajoutés aux cartes : Adobe XD, Image, PDF, Vidéo.

1. Sélectionnez le nom de champ.
1. (Facultatif) Cliquez sur le champ **[!UICONTROL Valeur de champ]** pour remplacer ce champ personnalisé par un autre.
1. (Facultatif) Remplacez le **[!UICONTROL libellé de champ]** par le nom de champ que vous souhaitez voir apparaître sur les cartes.
1. Lorsque vous avez terminé vos modifications, cliquez sur [!UICONTROL **Enregistrer le champ**].

   ![Valeur et libellé du champ personnalisé](assets/save-custom-field-value-label.png)

   Le champ personnalisé est ajouté à la liste des champs disponibles et est activé par défaut. Vous pouvez désactiver le champ personnalisé en suivant les étapes de la section [Configurer les cartes](customize-fields-on-card.md#configure-cards) ci-dessus, modifier le champ ou le supprimer de toutes les cartes.

>[!NOTE]
>
>Si vous renommez ultérieurement le champ personnalisé dans Workfront, vous devez modifier le libellé du champ dans le panneau de configuration pour qu’il corresponde, sinon le champ ne s’affichera pas sur les cartes.

## Afficher ou masquer les cartes archivées

Vous devez activer un paramètre de configuration pour afficher les cartes archivées sur un panorama.

1. Accédez à un panorama et cliquez sur [!UICONTROL **Configurer**] pour ouvrir le panneau de configuration.
1. Développez [!UICONTROL **Cartes**].
1. Activez [!UICONTROL **Afficher les cartes archivées sur le panorama**].

   Vous pouvez désormais filtrer le panorama pour afficher les cartes qui ont été archivées. Pour plus de détails, voir [Filtrer et rechercher dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

1. Cliquez sur [!UICONTROL **Masquer la configuration**] pour fermer le panneau de configuration.

## Configurer le détachement des vignettes

Pour retirer automatiquement les cartes du panorama après un certain temps, voir [Configurer le détachement des vignettes](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).
