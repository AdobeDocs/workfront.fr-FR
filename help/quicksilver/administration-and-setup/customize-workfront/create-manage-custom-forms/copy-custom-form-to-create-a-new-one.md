---
user-type: administrator
product-area: system-administration
keywords: create,custom,form,copy,base,another
navigation-topic: create-and-manage-custom-forms
title: Copier un formulaire personnalisé pour en créer un nouveau avec le créateur hérité
description: Vous pouvez créer un formulaire personnalisé basé sur un formulaire existant.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Copier un formulaire personnalisé pour en créer un nouveau avec le créateur hérité

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients ou dans l’environnement Production pour les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Présentation de la version du deuxième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Vous pouvez créer un formulaire personnalisé basé sur un formulaire existant.

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

## Copier un formulaire personnalisé pour en créer un nouveau

{{step-1-to-setup}}

1. Cliquez sur **Forms personnalisée.**
1. Sélectionnez le formulaire personnalisé à utiliser comme base pour un nouveau formulaire personnalisé, puis cliquez sur **Copier** <span class="preview">ou ![Icône Copier](assets/copy-icon.png).</span>
1. Dans le **Copie de formulaire personnalisée** dans la zone qui s’affiche, saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du formulaire</td> 
      <td>Saisissez le nom du formulaire copié.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Types de formulaire </p> </td> 
      <td> <p>Dans le <b>Type de formulaire</b> , sélectionnez les types d’objets avec lesquels vous souhaitez que le formulaire personnalisé fonctionne, puis cliquez sur le X en regard des types à supprimer. Les types déjà associés au formulaire sont désactivés dans la liste.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>Le formulaire doit être associé à au moins un type d’objet.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Copier le formulaire**.

   Dans le formulaire d’origine, si des champs calculés font référence à des champs incompatibles avec un type d’objet que vous ajoutez au nouveau formulaire, un message vous invite à modifier les calculs dans ces champs.

   De même, si une option d’accès pour un saut de section sur le formulaire d’origine n’est pas compatible avec un type d’objet que vous ajoutez au nouveau, un message vous invite à ajuster l’option.

1. Sélectionnez le formulaire à copier, puis cliquez sur **Modifier**.
1. Apportez toute modification au formulaire, comme expliqué dans les articles suivants :

   * [Copier un formulaire personnalisé pour en créer un nouveau avec l’ancien créateur de formulaires](#Add2)
   * [Ajout de données calculées à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Placement de champs et de widgets personnalisés dans un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajout ou modification d’un widget de ressource dans un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Réutilisation d’un champ personnalisé calculé existant dans un formulaire personnalisé avec l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Ajouter une logique d’affichage et ignorer la logique à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Aperçu et remplissage d’un formulaire personnalisé avec le créateur de formulaires hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Facultatif) Après avoir cliqué sur **Enregistrer + Fermer**, joignez le formulaire à l’objet dans lequel vous souhaitez l’utiliser, comme décrit à la section [Ajout d’un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
