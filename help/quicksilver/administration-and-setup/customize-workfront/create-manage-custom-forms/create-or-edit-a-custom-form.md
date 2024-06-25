---
title: Créer ou modifier un formulaire personnalisé avec le créateur de formulaire hérité
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez créer ou modifier un formulaire personnalisé.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 98%

---

# Créer ou modifier un formulaire personnalisé avec le créateur de formulaire hérité

<!--Audited: 01/2024-->

{{form-designer-default}}

Vous pouvez créer un formulaire personnalisé ou modifier un formulaire existant. Les deux tâches sont expliquées dans cet article.

Pour plus d’informations sur la création d’un formulaire personnalisé à partir d’un formulaire existant, voir [Copier un formulaire personnalisé pour en créer un nouveau avec le créateur de formulaire hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

Cet article décrit comment créer un formulaire personnalisé à l’aide du créateur de formulaire hérité. Pour plus d’informations sur la création d’un formulaire personnalisé à l’aide du créateur de formulaire, voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Forfait Adobe Workfront</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouvelle : standard</p>
   <p>ou</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Commencer à créer un formulaire personnalisé

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés** dans le panneau de gauche.

   Les formulaires personnalisés s’affichent dans une liste. Vous pouvez passer en revue tous les formulaires et champs personnalisés créés pour votre entreprise. Vous pouvez également voir qui a créé chaque formulaire, les objets qui lui sont associés et s’il est actif.

1. Cliquez sur **Nouveau formulaire personnalisé**.
1. Sélectionnez au moins un type d’objet à associer au formulaire personnalisé, puis cliquez sur **Continuer**.

   ![](assets/choose-object-type.jpg)

1. Dans l’onglet **Paramètres du formulaire** qui s’ouvre, saisissez un **Titre du formulaire** et une **Description** facultative pour le formulaire personnalisé.

1. (Facultatif) Si vous souhaitez ajouter d’autres types d’objets au formulaire afin de pouvoir les joindre à d’autres objets, cliquez sur le signe **plus** après **Types d’objets**, puis sélectionnez le type d’objet souhaité dans le menu qui s’affiche.

   Vous pouvez répéter cette opération pour ajouter autant de types d’objet que vous le souhaitez.

1. (Facultatif) Cliquez sur **X** sur un type d’objet pour le supprimer du formulaire.

   Pour plus d’informations sur la suppression de types d’objets d’un formulaire personnalisé que vous avez déjà enregistré, voir [Supprimer de types d’objets sur un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Cliquez sur **Terminé** dans le coin inférieur gauche de l’écran.

   >[!TIP]
   >
   >Vous pouvez cliquer sur **Appliquer** à tout moment de la création d’un formulaire personnalisé pour enregistrer vos modifications et garder le formulaire ouvert.

1. Si vous souhaitez ajouter un nouveau champ personnalisé au formulaire, passez à [Ajouter un champ personnalisé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) ou à [Réutiliser un champ ou un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)

   Ou

   Si vous souhaitez continuer à créer votre formulaire personnalisé d’une autre manière, consultez les articles suivants :


   * [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Placer des champs et des widgets personnalisés dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajouter un saut de section à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Ajouter des données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Réutiliser un champ personnalisé calculé existant dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Ajouter une logique d’affichage et une logique de saut à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Commencer à modifier un formulaire personnalisé

Vous pouvez modifier un formulaire personnalisé à tout moment après sa création.

>[!CAUTION]
>
>Pour plus d’informations sur la suppression de champs d’un formulaire personnalisé sans perdre les données saisies par les utilisateurs et les utilisatrices dans ces champs, voir la section [Supprimer un champ personnalisé sans perdre les données saisies par les utilisateurs et utilisatrices](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) dans l’article [Supprimer un champ ou un widget personnalisé du système](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>En règle générale, il est recommandé de réduire au minimum le nombre de fois où vous modifiez un formulaire personnalisé déjà utilisé. Il n’existe pas de système de notification pour informer les personnes qui utilisent le formulaire personnalisé de vos modifications.

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés** dans le panneau de gauche.

   Les formulaires personnalisés s’affichent dans une liste. Vous pouvez passer en revue tous les formulaires et champs personnalisés créés pour votre entreprise. Vous pouvez également voir qui a créé chaque formulaire, les objets qui lui sont associés et s’il est actif.

1. Sélectionnez le formulaire personnalisé à modifier, puis cliquez sur l’![icône Modifier](assets/edit-icon.png).
1. (Facultatif) Pour modifier le titre et la description du formulaire personnalisé, cliquez sur l’onglet **Paramètres du formulaire**, puis saisissez le **Titre du formulaire** et une **Description**.

1. (Facultatif) Si vous souhaitez ajouter d’autres types d’objets au formulaire afin de pouvoir les joindre à d’autres objets, cliquez sur le signe + après **Types d’objet**, puis sélectionnez le type souhaité dans le menu qui s’affiche.

   ![](assets/add-object-type-existing-form.png)

   Vous pouvez répéter cette opération pour ajouter autant de types d’objet que vous le souhaitez.

   Vous pouvez également cliquer sur le bouton X d’un type d’objet pour le supprimer du formulaire. Procédez avec prudence lorsque vous souhaitez supprimer un type d’objet d’un formulaire personnalisé déjà enregistré. Pour plus d’informations, consultez la section [Supprimer les types d’objet sur un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Cliquez sur **Terminé**.

   >[!TIP]
   >
   >Cliquez sur **Appliquer** lorsque vous créez un formulaire personnalisé pour enregistrer vos modifications et garder le formulaire ouvert.

1. Si vous souhaitez ajouter un nouveau champ personnalisé au formulaire, passez à [Ajouter un champ personnalisé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) ou à [Réutiliser un champ ou un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)

   Ou

   Si vous souhaitez continuer à créer votre formulaire personnalisé d’une autre manière, consultez les articles suivants :


   * [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Placer des champs et des widgets personnalisés dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajouter un saut de section à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Ajouter des données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Réutiliser un champ personnalisé calculé existant dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Ajouter une logique d’affichage et une logique de saut à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
