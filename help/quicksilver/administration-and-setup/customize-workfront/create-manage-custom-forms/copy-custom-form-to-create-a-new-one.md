---
user-type: administrator
product-area: system-administration
keywords: créer,personnalisé,formulaire,copier,base,autre
navigation-topic: create-and-manage-custom-forms
title: Copier un formulaire personnalisé pour en créer un nouveau avec le créateur hérité
description: Vous pouvez créer un formulaire personnalisé basé sur un formulaire existant.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: ht
source-wordcount: '429'
ht-degree: 100%

---

# Copier un formulaire personnalisé pour en créer un nouveau avec le créateur hérité

Vous pouvez créer un formulaire personnalisé basé sur un formulaire existant.

## Conditions d’accès

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
   <td>
   <p>Nouvelle : standard</p>
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

## Copier un formulaire personnalisé pour en créer un nouveau

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés.**
1. Sélectionnez le formulaire personnalisé à utiliser comme base pour un nouveau formulaire personnalisé, puis cliquez sur l’![icône Copier](assets/copy-icon.png).
1. Dans la zone **Copie de formulaire personnalisée** qui s’affiche, saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du formulaire</td> 
      <td>Saisissez le nom du formulaire copié.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Types de formulaires </p> </td> 
      <td> <p>Dans la zone <b>Type de formulaire</b>, sélectionnez les types d’objets avec lesquels vous souhaitez que le formulaire personnalisé fonctionne, puis cliquez sur le X à côté des types que vous souhaitez retirer. Les types déjà associés au formulaire sont désactivés dans la liste.</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>Le formulaire doit être associé à au moins un type d’objet.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Copier**.

   Dans le formulaire d’origine, si des champs calculés font référence à des champs incompatibles avec un type d’objet que vous ajoutez au nouveau formulaire, un message vous invite à modifier les calculs dans ces champs.

   De la même manière, si une option d’accès pour un saut de section sur le formulaire d’origine n’est pas compatible avec un type d’objet que vous ajoutez au nouveau formulaire, un message vous invite à ajuster l’option.

1. Sélectionnez le formulaire que vous venez de copier, puis cliquez sur **Modifier**.
1. Apportez les modifications souhaitées au formulaire, comme expliqué dans les articles suivants :

   * [Copier un formulaire personnalisé pour en créer un nouveau avec le créateur de formulaires hérité](#Add2)
   * [Ajouter des données calculées dans un formulaire personnalisé avec le créateur de formulaires hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Positionner des champs personnalisés et des widgets dans un formulaire personnalisé avec le créateur de formulaires hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Ajouter ou modifier un widget de ressource dans un formulaire personnalisé avec le créateur de formulaires hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Réutiliser un champ personnalisé calculé existant dans un formulaire personnalisé avec le créateur de formulaires hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Ajouter une logique d’affichage et une logique de saut dans un formulaire personnalisé avec le créateur de formulaires hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Prévisualiser et remplir un formulaire personnalisé avec le créateur de formulaires hérité](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Facultatif) Après avoir cliqué sur **Enregistrer + Fermer**, joignez le formulaire à l’objet dans lequel vous souhaitez l’utiliser, comme décrit dans [Ajouter un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
