---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personnalisation des champs affichés sur une carte
description: Vous pouvez personnaliser les champs qui s’affichent sur une carte en désactivant un champ afin qu’il ne s’affiche pas dans le mode Carte complète ou condensé, ou en masquant un champ dans le mode Carte condensée.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 17%

---

# Personnaliser les champs affichés sur une carte

Par défaut, tous les champs disponibles sont affichés sur une carte, à la fois dans l’affichage complet lorsque la carte est ouverte et dans l’affichage condensé de la carte sur le panorama. Vous pouvez personnaliser les champs affichés en procédant comme suit :

* Désactivation d’un champ afin qu’il ne s’affiche dans aucune vue
* Masquage d’un champ en mode Carte condensée

Si un champ contient une valeur et que vous la désactivez, la valeur est conservée si vous la réactivez ultérieurement.

Les sections (qui s’affichent comme les options de navigation de gauche sur les détails de la carte) peuvent également s’afficher et se masquer.

Vous pouvez également afficher les champs personnalisés qui ont été créés précédemment. Vous ne pouvez pas concevoir et créer de nouveaux champs personnalisés dans un panorama.

>[!NOTE]
>
>Toutes les personnalisations de champ que vous effectuez s’appliquent uniquement au panorama dans lequel vous travaillez.

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

## Configuration des cartes {#configure-cards}

{{step1-to-boards}}

1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur [!UICONTROL **Configurer**] à droite du panorama pour ouvrir le panneau Configurer.
1. Développez [!UICONTROL **Cartes**].

   La plupart des champs et des sections sont activés par défaut.

1. Désactivez un champ ou une section pour le désactiver en mode Carte.
1. Cliquez sur l’icône Masquer ![Icône Masquer](assets/eye-hide-icon.png) en regard d’un champ ou d’une section pour le masquer sur l’affichage condensé.
1. Pour afficher tous les champs et sections des deux vues, cliquez sur [!UICONTROL **Restaurer tous les champs par défaut**].
1. Cliquez sur [!UICONTROL **Masquer la configuration**] pour fermer le panneau Configurer.

## Ajout de champs personnalisés aux cartes

Les champs personnalisés sont disponibles sur les cartes connectées. Elles ne sont visibles que sur le mode Carte complète, et non sur l’affichage condensé du panorama.

Les données des champs personnalisés sont modifiables sur la carte, bien que certains éléments personnalisés puissent uniquement être disponibles pour modification sur le champ d’origine et non sur la carte.

1. Accédez à un panorama et cliquez sur [!UICONTROL **Configurer**] pour ouvrir le panneau Configurer.
1. Développez [!UICONTROL **Cartes**].
1. Sous [!UICONTROL Card Fields], cliquez sur [!UICONTROL **Ajouter un champ personnalisé**].
1. Sélectionnez [!UICONTROL **Tâche**] ou [!UICONTROL **Problème**].

   Les catégories de champs disponibles pour les tâches ou les problèmes apparaissent. Développez une catégorie pour afficher tous les champs. Vous pouvez également rechercher un champ.

   ![Rechercher un champ personnalisé](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Les types de champs suivants ne peuvent pas être ajoutés aux cartes : Adobe XD, Image, PDF, Vidéo.

1. Sélectionnez le nom du champ.
1. (Facultatif) Cliquez dans le champ **[!UICONTROL Valeur du champ]** pour remplacer ce champ personnalisé par un autre.
1. (Facultatif) Remplacez le **[!UICONTROL libellé du champ]** par le nom du champ que vous souhaitez afficher sur les cartes.
1. Lorsque vous avez terminé d’apporter des modifications, cliquez sur [!UICONTROL **Enregistrer le champ**].

   ![Valeur de champ personnalisé et libellé](assets/save-custom-field-value-label.png)

   Le champ personnalisé est ajouté à la liste des champs disponibles et est activé par défaut. Vous pouvez désactiver le champ personnalisé en suivant les étapes de la section [Configurer les cartes](customize-fields-on-card.md#configure-cards) ci-dessus, modifier le champ ou le supprimer de toutes les cartes.

>[!NOTE]
>
>Si vous renommez ultérieurement le champ personnalisé dans Workfront, vous devez modifier le libellé du champ dans le panneau Configurer pour qu’il corresponde, sinon le champ ne s’affichera pas sur les cartes.

## Affichage ou masquage des cartes archivées

Vous devez activer un paramètre de configuration pour afficher les cartes archivées sur un panorama.

1. Accédez à un panorama et cliquez sur [!UICONTROL **Configurer**] pour ouvrir le panneau Configurer.
1. Développez [!UICONTROL **Cartes**].
1. Activez [!UICONTROL **Afficher les cartes archivées sur le panorama**].

   Vous pouvez désormais filtrer le panorama pour afficher toutes les cartes qui ont été archivées. Pour plus d’informations, voir [Filtrage et recherche dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

1. Cliquez sur [!UICONTROL **Masquer la configuration**] pour fermer le panneau Configurer.

## Configurer le détachement des vignettes

Pour supprimer automatiquement les cartes du panorama après un certain temps, voir [Configuration de l’abandon de carte](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).
