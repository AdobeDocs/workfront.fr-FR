---
product-area: projects;user-management
keywords: modifier, formulaires, texte enrichi, spécial, format, champs, personalisé, informations, personnaliser, objets
navigation-topic: work-with-custom-forms
title: Modifier les informations dans les champs des formulaire personnalisés
description: Vous pouvez modifier les informations d’un formulaire personnalisé après l’avoir joint à un objet. Pour plus d’informations sur l’ajout de formulaires personnalisés aux objets, voir Ajouter un formulaire personnalisé à un objet.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 96%

---

# Modifier les informations dans les champs des formulaire personnalisés

Vous pouvez modifier les informations d’un formulaire personnalisé après l’avoir joint à un objet. Pour plus d’informations sur l’ajout de formulaires personnalisés aux objets, voir [Ajouter un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Équipe ou supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licences Adobe Workfront*</p> </td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Accédez à l’objet pour lequel vous souhaitez modifier des informations sur le formulaire personnalisé.</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> 
    <ul> 
     <li> <p>Autorisation de contribution ou supérieure sur l’objet dont vous souhaitez modifier le formulaire personnalisé.</p> </li> 
     <li>Afficher les autorisations sur les champs que vous souhaitez modifier. Pour plus d’informations sur le partage des autorisations pour les champs personnalisés, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configuration du partage pour les champs et widgets personnalisés</a>.</li> 
     <li> <p>Autorisations de modification pour les sections du formulaire qui contiennent les champs à modifier.</p> </li> 
    </ul> <p>Pour plus d’informations sur la demande d’accès supplémentaire aux objets, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Conditions préalables

* L’équipe d’administration Workfront ou l’utilisateur ou utilisatrice Plan ayant accès à des formulaires personnalisés doit créer des formulaires personnalisés dans votre environnement. Pour plus d’informations, voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
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

   Pour plus d’informations sur tous les types de champ, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
>En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lors du recalcul en bloc des champs personnalisés calculés afin de garantir des performances optimales. Un projet peut être trop complexe s’il comporte de multiples dépendances ou affectations ou un grand nombre de champs personnalisés.
>
>Pour recalculer en bloc des expressions personnalisées à partir d’une liste de projets :
>
>1. Accédez à une liste de projets ou à un rapport et sélectionnez un ou plusieurs projets.
>1. Cliquez sur le menu **Plus** ![](assets/more-icon.png), puis cliquez sur **Recalculer les expressions personnalisées**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront calcule tous les champs personnalisés pour tous les projets sélectionnés.
