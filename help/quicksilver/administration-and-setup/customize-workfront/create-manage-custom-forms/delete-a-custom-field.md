---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Suppression d’un champ ou d’un widget personnalisé du système
description: Pour améliorer les performances du système et faciliter l’utilisation des formulaires pour les utilisateurs, vous pouvez supprimer des champs et des widgets personnalisés de votre système lorsqu’ils ne sont plus utilisés.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '576'
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
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs de Workfront accordent cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Suppression d’un champ ou d’un widget personnalisé du système

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Forms personnalisée.**
1. Cliquez sur le bouton **Champs** .
1. Sélectionnez le champ personnalisé ou le widget, puis cliquez sur **Supprimer**.
1. Si vous êtes sûr de vouloir supprimer définitivement l’élément et (dans le cas d’un champ personnalisé) toutes les données associées sur les objets auxquels il a été associé, cliquez sur **Oui, la supprimer**.

## Supprimer un champ personnalisé sans perdre les données saisies par les utilisateurs {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>La suppression d’un champ personnalisé d’un formulaire personnalisé qui comporte plus de 500 champs et widgets ne peut pas être annulée. Si vous supprimez le champ, vous ne pouvez pas le rajouter tant que le formulaire ne comporte pas moins de 500 champs et widgets.

1. Déterminez les champs personnalisés à supprimer du formulaire personnalisé d’origine, mais ne les supprimez pas à ce stade.
1. Créez un formulaire personnalisé, comme décrit dans la section [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. Ajoutez les champs personnalisés au nouveau formulaire que vous souhaitez supprimer du formulaire personnalisé d’origine, comme décrit dans la section [Réutilisation d’un champ ou d’un widget personnalisé dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
   1. Enregistrez le nouveau formulaire personnalisé.

1. Limitez l’accès au formulaire personnalisé aux seuls utilisateurs disposant d’un accès administratif, comme décrit dans la section [Partage d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Appliquez le nouveau formulaire personnalisé aux objets dans lesquels le formulaire personnalisé d’origine est déjà appliqué, comme décrit à la section [Ajout d’un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   L’application du nouveau formulaire personnalisé à ces objets garantit que les données de rapport historiques ne sont pas affectées.

1. Modifiez le formulaire personnalisé d’origine et supprimez les champs personnalisés que vous avez ajoutés au nouveau formulaire (à l’étape 2).

   Les champs que vous avez supprimés du formulaire personnalisé d’origine ne sont désormais disponibles que sur le nouveau formulaire personnalisé que vous avez créé. Les utilisateurs peuvent voir le formulaire personnalisé sur l’objet, mais les utilisateurs sans accès administrateur ne peuvent pas modifier le formulaire personnalisé.
