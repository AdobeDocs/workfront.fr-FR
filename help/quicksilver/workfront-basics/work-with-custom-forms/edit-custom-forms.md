---
product-area: projects;user-management
keywords: edit,forms,rich,text,special,format,fields,custom,information,customize,object
navigation-topic: work-with-custom-forms
title: Modifier les informations dans les champs de formulaire personnalisés
description: Vous pouvez modifier les informations d’un formulaire personnalisé une fois le formulaire joint à un objet. Pour plus d’informations sur l’ajout de formulaires personnalisés à des objets, voir Ajout d’un formulaire personnalisé à un objet.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: b2bb5d1292291cb6632cc5d1b1fb32ce37e594a6
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Modifier les informations dans les champs de formulaire personnalisés

{{preview-and-fast-release}}

Vous pouvez modifier les informations d’un formulaire personnalisé une fois le formulaire joint à un objet. Pour plus d’informations sur l’ajout de formulaires personnalisés à des objets, voir [Ajout d’un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Equipe ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licences Adobe Workfront*</p> </td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès à l’objet pour lequel vous souhaitez modifier le formulaire personnalisé</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribuez à l’objet pour lequel vous souhaitez modifier le formulaire personnalisé avec des autorisations supérieures.</p> </li> 
     <li>Afficher les autorisations sur les champs que vous souhaitez modifier. Pour plus d’informations sur le partage des autorisations pour les champs personnalisés, voir <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configuration du partage pour les champs et widgets personnalisés</a>.</li> 
     <li> <p>Modifier les autorisations pour les sections du formulaire où se trouvent les champs que vous souhaitez modifier</p> </li> 
    </ul> <p>Pour plus d’informations sur la demande d’accès supplémentaire aux objets, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

* L’administrateur Workfront ou l’utilisateur Plan ayant accès à des formulaires personnalisés doit créer des formulaires personnalisés dans votre environnement. Pour plus d’informations, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* Des formulaires personnalisés doivent être associés à un objet.

  Pour plus d’informations sur l’application de formulaires personnalisés à un objet, voir [Ajout d’un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Modifier les informations d’un formulaire personnalisé

La modification des informations d’un formulaire personnalisé associé à un objet est identique pour tous les objets. Pour plus d’informations sur les objets pouvant avoir un formulaire personnalisé, voir [Aperçu des formulaires personnalisés](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Accédez à un objet pour lequel vous souhaitez modifier des informations sur le formulaire personnalisé.
1. Cliquez sur **`<Object type>`Détails** dans le panneau de gauche.

   Par exemple, lorsque vous modifiez des informations sur un formulaire personnalisé de projet, cliquez sur **Détails du projet**.

1. Accédez au formulaire personnalisé. Lorsqu’un formulaire personnalisé est associé à l’objet, son nom s’affiche sous la forme d’une zone dans la section Détails.
1. Si nécessaire, cliquez sur la flèche ![](assets/expand-arrow-right.png) à gauche du nom du formulaire personnalisé pour le développer.
1. Dans le coin supérieur droit de la page, cliquez sur l’icône Modifier ![](assets/edit-icon.png).
1. Commencez à saisir des informations dans les champs auxquels vous avez accès.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   Ou

   Si aucune information n’a encore été saisie sur le formulaire, cliquez sur **Ajouter+** pour tout champ auquel vous avez accès et commencez à saisir des informations.

   ![](assets/plus-add-to-edit-info-350x180.png)

   Si plusieurs formulaires personnalisés sont associés à l’objet, vous pouvez le faire pour chaque formulaire.

   En fonction du type de champ dans lequel vous travaillez, tenez compte des points suivants :

   * Vous ne pouvez sélectionner qu’une seule option pour les champs de bouton radio.
   * Vous pouvez sélectionner une ou plusieurs options dans un champ de case à cocher, selon la manière dont l’auteur du formulaire a configuré le champ.
   * Vous pouvez sélectionner une ou plusieurs options dans un champ déroulant à sélection multiple, en fonction de la configuration du champ par l’auteur du formulaire.
   * Vous ne pouvez mettre en forme les champs de texte (gras, italique ou souligné) que si l’utilisateur qui a créé le formulaire les a configurés en tant que champ de texte avec un type de champ Formatage . Les champs de texte d’une seule ligne et les champs de texte de paragraphe ne peuvent pas être formatés.
   * Vous ne pouvez mettre à jour l’heure dans un type de champ Date que si l’utilisateur qui a créé le formulaire l’a incluse lors de la création du champ.

   Pour plus d’informations sur tous les types de champ, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Cliquez sur **Enregistrer les modifications**.

   >[!IMPORTANT]
   >
   >Vous devez remplir tous les champs requis du formulaire avant de pouvoir l’enregistrer. Le nom d’un champ obligatoire est suivi d’un astérisque.
   >
   >![](assets/nwe-required-custom-field.png)

   Lorsqu’une personne modifie des données dans un autre objet référencé par des champs personnalisés calculés de votre objet, les modifications ne sont pas répercutées automatiquement dans votre objet. Pour plus d’informations sur la mise à jour manuelle de tous les champs personnalisés calculés de votre objet, voir [Recalculer tous les champs personnalisés calculés d’un objet](#recalculate-all-calculated-custom-fields-for-an-object) dans cet article.

   <span class="preview">Lorsque des champs dépendants de la page sont modifiés, les champs calculés du formulaire personnalisé sont recalculés dynamiquement en temps réel. Vous pouvez voir la nouvelle valeur du champ calculé sans enregistrer le formulaire, mais elle n’est pas appliquée au formulaire et à l’objet tant que vous n’avez pas enregistré les modifications. Cela s’applique aux champs calculés sur les formulaires par défaut et aux formulaires personnalisés.</span>

   Vous pouvez également mettre à jour manuellement tous les champs personnalisés calculés d’un objet lorsque vous modifiez l’objet en masse avec d’autres objets d’une liste. Pour obtenir des instructions, voir [Recalculer tous les champs personnalisés calculés de plusieurs objets dans une liste lors de la modification des objets](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) dans cet article.

## Recalculer tous les champs personnalisés calculés d’un objet  {#recalculate-all-calculated-custom-fields-for-an-object}

1. Accédez à la page principale de l’objet dont vous souhaitez recalculer les champs personnalisés.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) à droite du nom de l’objet, puis cliquez sur **Recalculer les expressions**.

   Cela recalcule tous les champs personnalisés du formulaire de l’objet.

## Recalculer tous les champs personnalisés calculés de plusieurs objets dans une liste lors de la modification des objets {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

Vous pouvez recalculer manuellement les champs personnalisés de plusieurs objets en les modifiant en masse à partir d&#39;une liste ou d&#39;un rapport.

1. Accédez à la liste des objets qui contiennent des formulaires personnalisés avec des champs calculés.
1. Sélectionnez les objets dont vous souhaitez mettre à jour les champs personnalisés calculés.
1. Cliquez sur le bouton **Icône Modifier**.
1. Cliquez sur **Forms personnalisée** dans le menu de gauche, puis sélectionnez **Recalculer des expressions personnalisées**.
1. Cliquez sur **Enregistrer** **Modifications**.

   Workfront calcule tous les champs personnalisés pour tous les objets sélectionnés.

>[!TIP]
>
>En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lors du recalculage en masse des champs personnalisés calculés pour garantir des performances optimales. Certaines choses qui peuvent rendre un projet trop complexe peuvent être des dépendances ou des affectations multiples ou un grand nombre de champs personnalisés.
>
>Pour recalculer les expressions personnalisées en bloc à partir d’une liste de projets :
>
>1. Accédez à une liste de projets ou à un rapport et sélectionnez un ou plusieurs projets.
>1. Cliquez sur le bouton **Plus** menu ![](assets/more-icon.png), puis cliquez sur **Recalculer des expressions personnalisées**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront calcule tous les champs personnalisés pour tous les projets sélectionnés.
