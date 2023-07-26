---
title: Ajouter une logique d’affichage et ignorer la logique à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez choisir quelles sections d’un formulaire personnalisé doivent être affichées ou ignorées en fonction des choix que fait l’utilisateur lorsqu’il le remplit.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 1%

---

# Ajouter une logique d’affichage et ignorer la logique à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires

Vous pouvez choisir quelles sections d’un formulaire personnalisé doivent être affichées ou ignorées en fonction des choix que fait l’utilisateur lorsqu’il le remplit.

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

## Observations relatives à l’utilisation de la logique d’affichage et de la logique de saut

* Pour ajouter une logique d’affichage à un champ personnalisé, un widget ou un saut de section, au moins un champ à choix multiples (boutons radio, liste déroulante ou cases à cocher) doit être positionné avant cette logique sur le formulaire.

  Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Ajout d’un champ personnalisé à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) et [Ajout ou modification d’un widget de ressource dans un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Vous ne pouvez pas ajouter de logique de saut à un widget ou à un saut de section. Vous pouvez l’ajouter uniquement à plusieurs champs de choix (boutons radio, liste déroulante ou cases à cocher).

* Vous pouvez ajouter à la fois une logique d’affichage et une logique de saut à un champ personnalisé. Pour le champ personnalisé, tous les éléments suivants sont vrais :

   * Il s’agit d’un champ à choix multiples (boutons radio, liste déroulante ou cases à cocher).
   * Il est précédé d’un champ à choix multiples.
   * Il est suivi d’un autre champ personnalisé

* Lorsque vous copiez des formulaires avec une logique d’affichage ou ignorez la logique, celle-ci est copiée dans le nouveau formulaire personnalisé.
* Gardez ce qui suit à l’esprit lorsque vous créez une règle de logique d’affichage pour un formulaire personnalisé.

   * Les champs personnalisés non inclus dans une instruction de logique d’affichage s’affichent par défaut sur un formulaire personnalisé.
   * Vous pouvez créer des instructions logiques d’affichage à champs multiples.

* Lorsque vous modifiez des objets en bloc, tous les champs personnalisés s’affichent dans la zone Modifier les objets , y compris les champs qui sont ignorés ou masqués.

## Création d’un exemple de formulaire personnalisé avec une logique d’affichage et de saut

La meilleure façon d’apprendre à ajouter une logique d’affichage et d’exclusion à un formulaire personnalisé est de suivre l’exemple pratique décrit dans les deux sections suivantes :

* [Logique d’affichage](#display-logic)
* [Logique de saut](#skip-logic)

### Logique d’affichage {#display-logic}

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Forms personnalisée** ![](assets/custom-forms-icon.png).

1. Créez l’exemple de formulaire personnalisé :

   1. Cliquez sur **Nouveau formulaire personnalisé**, puis cliquez sur **Projet** dans la liste déroulante.

   1. Dans le **Titre du formulaire** box, type **Exemple de formulaire personnalisé : apprentissage de la logique d’affichage et de la logique de saut**.

   1. Cliquez sur **Ajouter un champ** dans le coin supérieur gauche.
   1. Ajoutez un champ de liste déroulante appelé *Champ de problème* en cliquant **Liste déroulante**, puis en tapant **Champ de problème** dans le **Libellé** de la boîte.

   1. Sous **Choix**, ajoutez les options suivantes dans les zones de texte :

      La recherche nécessaire

      Plus de recherche

   1. Cliquez sur **Enregistrer + Fermer** dans le coin inférieur gauche.

1. Sélectionnez la nouvelle **Exemple de formulaire personnalisé : apprentissage de la logique d’affichage et de la logique de saut** formulaire personnalisé, puis cliquez sur **Modifier**.

1. Ajoutez un nouveau champ de texte d’une seule ligne appelé *Autres recherches* en cliquant **Champ de texte d’une seule ligne**, puis en tapant **Autres recherches** dans le **Libellé** de la boîte.

1. Cliquez sur **Ajouter une logique** près du côté inférieur gauche du **Modifier le formulaire personnalisé** écran.

1. Dans la zone qui s’affiche, avec la fonction **Logique d’affichage** ouvrez l’onglet , configurez la logique pour le moment où la variable **Autres recherches** apparaît sur le formulaire en cliquant sur **Champ de problème** dans la première liste déroulante, **Recherche nécessaire** dans la deuxième liste déroulante, et **Sélectionné** dans la troisième liste déroulante.
1. Cliquez sur **Enregistrer** pour fermer la **Logique du champ** , puis cliquez sur **Terminé** dans le **Paramètres des champs** zone.

   Maintenant, lorsqu’une personne sélectionne **Recherche nécessaire** dans le **Champ de problème** , la variable **Autres recherches** s’affiche.

1. Cliquez sur **Aperçu** pour vous assurer que la logique s’affiche comme vous le souhaitez sur le formulaire.
1. Cliquez sur **Aperçu de la fin** lorsque vous constatez que la logique fonctionne comme prévu.
1. Cliquez sur **Enregistrer + Fermer** sur le **Modifier le formulaire personnalisé** pour enregistrer le formulaire, puis passez à [Ignorer la logique](#skip-logic) ci-dessous

### Logique de saut {#skip-logic}

Ignorer la logique fonctionne de la même manière que pour afficher la logique, mais agit comme l’inverse : au lieu de faire apparaître des champs personnalisés à choix multiples spécifiques en fonction de sélections spécifiques, vous déterminez ceux qui doivent être ignorés en fonction des sélections des utilisateurs.

Pour en savoir plus, continuez à travailler sur l’exemple de formulaire personnalisé que vous avez créé dans la section . [Logique d’affichage](#display-logic) dans cet article :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Forms personnalisée**.
1. Sélectionner le formulaire **Exemple de formulaire personnalisé : apprentissage de la logique d’affichage et de la logique de saut** que vous avez créé lors des étapes ci-dessus, puis cliquez sur **Modifier**.

1. Sélectionnez le champ déroulant que vous avez créé nommé *Champ de problème*.
1. Cliquez sur le bouton **Ajouter une logique** dans le **Paramètres des champs** barre latérale.

1. Dans le **Logique du champ** , assurez-vous que la variable **Ignorer la logique** est sélectionné.

1. Définissez la première liste déroulante sur **Plus de recherche** et la deuxième liste déroulante de **Sélectionné**.

1. Dans le **Puis, passez à** , sélectionnez **Fin de formulaire.**

   Maintenant, lorsqu’une personne sélectionne **Plus de recherche** dans le **Champ de problème** , le formulaire passe directement à la fin du formulaire sans afficher le champ **Autres recherches** champ .

1. Cliquer sur **Enregistrer**.
1. Cliquez sur **Aperçu**  pour vous assurer que la logique s’applique comme vous le souhaitez.
1. Cliquez sur **Terminé** dans le coin inférieur gauche du formulaire.
