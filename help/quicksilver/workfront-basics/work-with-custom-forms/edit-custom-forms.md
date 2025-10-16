---
product-area: projects;user-management
keywords: modifier, formulaires, texte enrichi, spécial, format, champs, personalisé, informations, personnaliser, objets
navigation-topic: work-with-custom-forms
title: Modifier les informations dans les champs des formulaire personnalisés
description: Vous pouvez modifier les informations d’un formulaire personnalisé après l’avoir joint à un objet. Pour plus d’informations sur l’ajout de formulaires personnalisés aux objets, voir Ajouter un formulaire personnalisé à un objet.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 93%

---

# Modifier les informations dans les champs des formulaire personnalisés

<!--Audited: 10/2025-->

Vous pouvez modifier les informations d’un formulaire personnalisé après l’avoir joint à un objet. Pour plus d’informations sur l’ajout de formulaires personnalisés aux objets, voir [Ajouter un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Package Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licence Adobe Workfront</p> </td> 
   <td> <p>Contributeur ou version ultérieure</p> 
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accédez à l’objet pour lequel vous souhaitez modifier des informations sur le formulaire personnalisé.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> 
    <ul> 
     <li> <p>Autorisation de contribution ou supérieure sur l’objet dont vous souhaitez modifier le formulaire personnalisé.</p> </li> 
     <li><p>Autorisations d’affichage des champs que vous souhaitez modifier.</p></li> 
     <li><p>Autorisations de modification pour les sections du formulaire qui contiennent les champs à modifier.</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Conditions préalables

* L’équipe d’administration Workfront ou l’utilisateur ou utilisatrice Plan ayant accès à des formulaires personnalisés doit créer des formulaires personnalisés dans votre environnement. Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Vous devez avoir des formulaires personnalisés joints à un objet.

  Pour plus d’informations sur l’application de formulaires personnalisés à un objet, voir [Ajouter un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Modifier les informations d’un formulaire personnalisé

La modification des informations sur un formulaire personnalisé joint à un objet est identique pour tous les objets. Pour plus d’informations sur les objets pouvant avoir un formulaire personnalisé, voir [Vue d’ensemble des formulaires personnalisés](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Accédez à l’objet pour lequel vous souhaitez modifier des informations sur le formulaire personnalisé.
1. Cliquez sur **`<Object type>`Détails** dans le panneau de gauche.

   Par exemple, lorsque vous modifiez les informations d’un formulaire personnalisé de projet, cliquez sur **Détails du projet**.

1. Faites défiler jusqu’au formulaire personnalisé. Lorsqu’un formulaire personnalisé est joint à l’objet, le nom du formulaire s’affiche comme une zone de la section Détails.
1. Si nécessaire, cliquez sur la flèche ![](assets/expand-arrow-right.png) à gauche du nom du formulaire personnalisé pour la développer.
1. Dans le coin supérieur droit de la page, cliquez sur l’icône Modifier ![](assets/edit-icon.png).
1. Commencez à saisir des informations dans les champs auxquels vous avez accès.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   Ou

   Si aucune information n’a encore été saisie dans le formulaire, cliquez sur **Ajouter+** pour les champs auxquels vous avez accès et commencez à saisir des informations.

   ![](assets/plus-add-to-edit-info-350x180.png)

   Si plusieurs formulaires personnalisés sont joints à l’objet, vous pouvez le faire pour chaque formulaire.

   Selon le type de champ dans lequel vous travaillez, tenez compte des éléments suivants :

   * Vous ne pouvez sélectionner qu’une seule option pour les champs à cases d’option.
   * Vous pouvez sélectionner une ou plusieurs options dans un champ à cases à cocher, selon la manière dont le créateur ou la créatrice du formulaire a configuré le champ.
   * Vous pouvez sélectionner une ou plusieurs options dans un champ déroulant à sélection multiple, en fonction de la manière dont le créateur ou la créatrice du formulaire a configuré le champ.
   * Vous ne pouvez formater les champs de texte (gras, italique ou souligné) que si la personne qui a créé le formulaire les a configurés en tant que type de champ Champ de texte avec formatage. Les types Champs de texte à ligne simple et Champs de texte de paragraphe ne peuvent pas être formatés.
   * Vous pouvez mettre à jour l’heure dans un champ de type de champ Date uniquement si la personne qui a créé le formulaire l’a indiqué lors de la création du champ.

   Pour plus d’informations sur tous les types de champ, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur **Enregistrer les modifications**.

   >[!IMPORTANT]
   >
   >Vous devez remplir tous les champs obligatoires du formulaire avant de pouvoir l’enregistrer. Le nom d’un champ obligatoire est suivi d’un astérisque.
   >
   >![](assets/nwe-required-custom-field.png)

   Lorsque quelqu’un modifie des données dans un autre objet qui est référencé par des champs personnalisés calculés dans votre objet, les modifications ne sont pas reflétées automatiquement dans votre objet. Pour plus d’informations sur la mise à jour manuelle de tous les champs personnalisés calculés dans votre objet, voir [Recalculer tous les champs personnalisés calculés pour un objet](#recalculate-all-calculated-custom-fields-for-an-object) dans cet article.

   Lorsque les champs dépendants de la page sont modifiés, les champs calculés du formulaire personnalisé sont recalculés dynamiquement en temps réel. Vous pouvez voir la nouvelle valeur du champ calculé sans enregistrer le formulaire, mais elle n’est pas réellement appliquée au formulaire et à l’objet tant que vous n’avez pas enregistré les modifications. Cela s’applique aux champs calculés des formulaires par défaut et des formulaires personnalisés.

   Vous pouvez également mettre à jour manuellement tous les champs personnalisés calculés pour un objet lorsque vous modifiez l’objet en bloc avec d’autres objets dans une liste. Pour les instructions, voir [Recalculer tous les champs personnalisés calculés pour plusieurs objets d’une liste lors de la modification des objets](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) dans cet article.

## Recalculer tous les champs personnalisés calculés pour un objet  {#recalculate-all-calculated-custom-fields-for-an-object}

1. Accédez à la page principale de l’objet dont vous souhaitez recalculer les champs personnalisés.
1. Cliquez sur le menu **Plus** ![](assets/more-icon.png) à droite du nom de l’objet, puis cliquez sur **Recalculer les expressions**.

   Cela permet de recalculer tous les champs personnalisés du formulaire de l’objet.

## Recalculer tous les champs personnalisés calculés pour plusieurs objets d’une liste lors de la modification des objets {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

Vous pouvez recalculer manuellement les champs personnalisés de plusieurs objets en les modifiant en bloc à partir d’une liste ou d’un rapport.

1. Accédez à une liste d’objets contenant des formulaires personnalisés avec des champs calculés.
1. Sélectionnez les objets dont vous souhaitez mettre à jour les champs personnalisés calculés.
1. Cliquez sur l’**icône Modifier**.
1. Cliquez sur **Formulaires personnalisés** dans le menu de gauche, puis sélectionnez **Recalculer les expressions personnalisées**.
1. Cliquez sur **Enregistrer** **les modifications**.

   Workfront calcule tous les champs personnalisés pour tous les objets sélectionnés.

>[!TIP]
>
>Vous pouvez également recalculer des expressions personnalisées à partir d’une liste d’objets. Par exemple, pour recalculer des expressions personnalisées en bloc à partir d’une liste de projets :
>
>1. Accédez à une liste de projets ou à un rapport et sélectionnez un ou plusieurs projets.
>1. Cliquez sur le menu **Plus** ![](assets/more-icon.png), puis cliquez sur **Recalculer les expressions personnalisées**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront calcule tous les champs personnalisés pour tous les projets sélectionnés.
>>Toutes les listes de tous les objets ne disposent pas de cette fonctionnalité.
>
>En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lors du recalcul en bloc des champs personnalisés calculés afin de garantir des performances optimales. Un projet peut être trop complexe s’il comporte de multiples dépendances ou affectations ou un grand nombre de champs personnalisés.

