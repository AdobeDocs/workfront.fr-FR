---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Suppression d’un champ ou d’un widget personnalisé du système
description: Afin d’améliorer les performances du système et de faciliter l’utilisation des formulaires pour les utilisateurs et les utilisatrices, vous pouvez supprimer des widgets et des champs personnalisés de votre système lorsqu’ils ne sont plus utilisés.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 8dac7959919014d7bfbbbd39d193d026ca31c4b2
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 93%

---

# Supprimer un champ ou un widget personnalisé du système

Afin d’améliorer les performances du système et de faciliter l’utilisation des formulaires pour les utilisateurs et les utilisatrices, vous pouvez supprimer des widgets et des champs personnalisés de votre système lorsqu’ils ne sont plus utilisés.

>[!CAUTION]
>
>La suppression d’un champ personnalisé entraîne celle de toutes les données personnalisées que les utilisateurs et les utilisatrices ont entrées dans ce champ lors du remplissage de formulaires associés à des objets. Les données supprimées ne peuvent pas être récupérées. En outre, il n’existe aucun système de notification pour avertir les personnes qui utilisent le formulaire personnalisé qu’il a été supprimé.
>
>Il est possible d’afficher tous les formulaires et rapports personnalisés utilisant un champ personnalisé que vous envisagez de supprimer, afin d’évaluer les conséquences potentielles. Pour plus d’informations, consultez les sections [Afficher tous les formulaires personnalisés qui utilisent un champ personnalisé ou un widget particulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) et [Afficher tous les rapports qui utilisent un champ personnalisé ou un widget particulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Ou, pour une solution de contournement que vous pouvez utiliser pour éviter de perdre des données dans les champs qui ne sont plus utilisés, consultez dans cet article la section [Supprimer un champ personnalisé sans perdre les données saisies par les utilisateurs et les utilisatrices](#remove-a-custom-field-without-losing-data-that-users-have-entered).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Supprimer un champ ou un widget personnalisé du système

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés.**
1. Cliquez sur **Champs** pour ouvrir la zone de champs.
1. Sélectionnez le champ personnalisé ou le widget, puis cliquez sur **Supprimer**.
1. Si vous souhaitez vraiment supprimer définitivement l’élément et (dans le cas d’un champ personnalisé) toutes les données associées sur les objets auxquels il a été associé, cliquez sur **Oui, supprimer**.

## Supprimer un champ personnalisé sans perdre les données saisies par les utilisateurs et les utilisatrices {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>La suppression d’un champ personnalisé d’un formulaire personnalisé comportant plus de 500 champs et widgets ne peut pas être annulée. Si vous supprimez le champ, vous ne pouvez pas le rajouter tant que le formulaire ne comporte pas moins de 500 champs et widgets.

1. Déterminez les champs personnalisés à supprimer du formulaire personnalisé d’origine, mais ne les supprimez pas à ce stade.
1. Créez un nouveau formulaire personnalisé :

   1. Ajoutez les champs personnalisés au nouveau formulaire à supprimer du formulaire personnalisé d’origine.

      Pour plus d’informations, reportez-vous à la section [Ajout de champs nouveaux ou existants à votre formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form) dans [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   1. Enregistrez le nouveau formulaire personnalisé.

1. Limitez l’accès au formulaire personnalisé aux seules personnes disposant d’un accès administratif, comme décrit dans la section [Partager un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Appliquez le nouveau formulaire personnalisé aux objets dans lesquels le formulaire personnalisé d’origine est déjà appliqué, comme décrit à la section [Ajouter un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   L’application du nouveau formulaire personnalisé à ces objets garantit que les données de rapport historiques ne sont pas affectées.

1. Modifiez le formulaire personnalisé d’origine et supprimez les champs personnalisés que vous avez ajoutés au nouveau formulaire (à l’étape 2).

   Les champs que vous avez supprimés du formulaire personnalisé d’origine ne sont désormais disponibles que sur le nouveau formulaire personnalisé que vous avez créé. Les utilisateurs et les utilisatrices peuvent voir le formulaire personnalisé sur l’objet, mais les personnes qui ne disposent pas d’un accès d’administration ne peuvent pas modifier le formulaire personnalisé.
