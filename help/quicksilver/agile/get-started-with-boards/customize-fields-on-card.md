---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personnalisation des champs affichés sur une carte
description: Vous pouvez personnaliser les champs qui s’affichent sur une carte en désactivant un champ afin qu’il ne s’affiche pas dans le mode Carte complète ou condensé, ou en masquant un champ dans le mode Carte condensée.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 0beb96dc3869e6f913d87f699aa9a51c5aaa8f79
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# Personnalisation des champs affichés sur une carte

Par défaut, tous les champs disponibles sont affichés sur une carte, à la fois dans l’affichage complet lorsque la carte est ouverte et dans l’affichage condensé de la carte sur le panorama. Vous pouvez personnaliser les champs affichés en procédant comme suit :

* Désactivation d’un champ afin qu’il ne s’affiche dans aucune vue
* Masquage d’un champ en mode Carte condensée

Si un champ contient une valeur et que vous la désactivez, la valeur est conservée si vous la réactivez ultérieurement.

Les sections (qui s’affichent comme les options de navigation de gauche sur les détails de la carte) peuvent également s’afficher et se masquer.

Vous pouvez également afficher les champs personnalisés qui ont été créés précédemment. Vous ne pouvez pas concevoir et créer de nouveaux champs personnalisés dans un panorama.

>[!NOTE]
>
>Toutes les personnalisations de champ que vous effectuez s’appliquent uniquement au panorama dans lequel vous travaillez.

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

## Configuration des cartes {#configure-cards}

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur [!UICONTROL **Configurer**] à droite du panorama pour ouvrir le panneau Configurer .
1. Développer [!UICONTROL **Cartes**].

   La plupart des champs et des sections sont activés par défaut.

1. Désactivez un champ ou une section pour le désactiver en mode Carte.
1. Cliquez sur l’icône Masquer . ![Icône Masquer](assets/eye-hide-icon.png) en regard d’un champ ou d’une section pour le masquer sur l’affichage condensé.
1. Pour afficher tous les champs et sections des deux modes, cliquez sur [!UICONTROL **Restaurer tous les champs par défaut**].
1. Cliquez sur [!UICONTROL **Masquer la configuration**] pour fermer le panneau Configurer .

## Ajout de champs personnalisés aux cartes

Les champs personnalisés sont disponibles sur les cartes connectées. Elles ne sont visibles que sur le mode Carte complète, et non sur l’affichage condensé du panorama.

>[!NOTE]
>
>Lorsque vous ajoutez un champ personnalisé à vos cartes, les données qu’elle contient sont en lecture seule.

1. Accédez à un panorama, puis cliquez sur [!UICONTROL **Configurer**] pour ouvrir le panneau Configurer .
1. Développer [!UICONTROL **Cartes**].
1. Sous [!UICONTROL Champs de carte], cliquez sur [!UICONTROL **Ajouter un champ personnalisé**].
1. Sélectionner [!UICONTROL **Tâche**] ou [!UICONTROL **Problème**].

   Les catégories de champs disponibles pour les tâches ou les problèmes apparaissent. Développez une catégorie pour afficher tous les champs. Vous pouvez également rechercher un champ.

   ![Recherche d’un champ personnalisé](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Les types de champs suivants ne peuvent pas être ajoutés aux cartes : Adobe XD, Image, PDF, Vidéo.

1. Sélectionnez le nom du champ.
1. (Facultatif) Cliquez sur le bouton **[!UICONTROL Valeur du champ]** pour remplacer ce champ personnalisé par un autre.
1. (Facultatif) Modifiez la variable **[!UICONTROL Libellé du champ]** au nom du champ que vous souhaitez voir apparaître sur les cartes.
1. Une fois les modifications effectuées, cliquez sur [!UICONTROL **Champ Enregistrer**].

   ![Valeur et libellé de champ personnalisés](assets/save-custom-field-value-label.png)

   Le champ personnalisé est ajouté à la liste des champs disponibles et est activé par défaut. Vous pouvez désactiver le champ personnalisé en suivant les étapes de la section [Configuration des cartes](customize-fields-on-card.md#configure-cards) ci-dessus, modifiez le champ ou supprimez-le de toutes les cartes.

>[!NOTE]
>
>Si vous renommez ultérieurement le champ personnalisé dans Workfront, vous devez modifier le libellé du champ dans le panneau Configurer pour qu’il corresponde, sinon le champ ne s’affichera pas sur les cartes.
