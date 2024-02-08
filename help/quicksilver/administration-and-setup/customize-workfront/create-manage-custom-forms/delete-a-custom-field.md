---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Suppression d’un champ ou d’un widget personnalisé du système
description: Pour améliorer les performances du système et faciliter l’utilisation des formulaires pour les utilisateurs, vous pouvez supprimer des champs et des widgets personnalisés de votre système lorsqu’ils ne sont plus utilisés.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Suppression d’un champ ou d’un widget personnalisé du système

Pour améliorer les performances du système et faciliter l’utilisation des formulaires pour les utilisateurs, vous pouvez supprimer des champs et des widgets personnalisés de votre système lorsqu’ils ne sont plus utilisés.

>[!CAUTION]
>
>La suppression d’un champ personnalisé supprime également toutes les données personnalisées que les utilisateurs ont saisies dans le champ lors du remplissage de formulaires personnalisés associés à des objets. Les données supprimées ne peuvent pas être récupérées.
>
>Vous pouvez afficher tous les formulaires et rapports personnalisés qui utilisent un champ personnalisé que vous souhaitez supprimer afin d’évaluer les répercussions possibles. Pour plus d’informations, voir [Afficher tous les formulaires personnalisés qui utilisent un champ ou un widget personnalisé spécifique](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) et [Afficher tous les rapports qui utilisent un champ ou un widget personnalisé spécifique](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Ou, pour une solution de contournement, vous pouvez utiliser pour éviter de perdre des données dans les champs qui ne sont plus utilisés, voir [Supprimer un champ personnalisé sans perdre les données saisies par les utilisateurs](#remove-a-custom-field-without-losing-data-that-users-have-entered) dans cet article.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Suppression d’un champ ou d’un widget personnalisé du système

{{step-1-to-setup}}

1. Cliquez sur **Forms personnalisée.**
1. Cliquez sur **Champs** pour ouvrir la zone Champs .
1. Sélectionnez le champ personnalisé ou le widget, puis cliquez sur **Supprimer**.
1. Si vous souhaitez vraiment supprimer définitivement l’élément et (dans le cas d’un champ personnalisé) toutes les données associées sur les objets auxquels il a été associé, cliquez sur **Oui, la supprimer**.

## Supprimer un champ personnalisé sans perdre les données saisies par les utilisateurs {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>La suppression d’un champ personnalisé d’un formulaire personnalisé qui comporte plus de 500 champs et widgets ne peut pas être annulée. Si vous supprimez le champ, vous ne pouvez pas le rajouter tant que le formulaire ne comporte pas moins de 500 champs et widgets.

1. Déterminez les champs personnalisés à supprimer du formulaire personnalisé d’origine, mais ne les supprimez pas à ce stade.
1. Créez un formulaire personnalisé :

   1. Ajoutez les champs personnalisés au nouveau formulaire à supprimer du formulaire personnalisé d’origine.

      * Si vous utilisez le créateur de formulaires personnalisé, voir [Réutilisation d’un champ ou d’un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
      * Si vous utilisez le concepteur de formulaire, voir [Ajouter des champs nouveaux ou existants à votre formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form).

   1. Enregistrez le nouveau formulaire personnalisé.

1. Limitez l’accès au formulaire personnalisé aux seuls utilisateurs disposant d’un accès administratif, comme décrit dans la section [Partage d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Appliquez le nouveau formulaire personnalisé aux objets dans lesquels le formulaire personnalisé d’origine est déjà appliqué, comme décrit à la section [Ajout d’un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   L’application du nouveau formulaire personnalisé à ces objets garantit que les données de rapport historiques ne sont pas affectées.

1. Modifiez le formulaire personnalisé d’origine et supprimez les champs personnalisés que vous avez ajoutés au nouveau formulaire (à l’étape 2).

   Les champs que vous avez supprimés du formulaire personnalisé d’origine ne sont désormais disponibles que sur le nouveau formulaire personnalisé que vous avez créé. Les utilisateurs peuvent voir le formulaire personnalisé sur l’objet, mais les utilisateurs sans accès administrateur ne peuvent pas modifier le formulaire personnalisé.
