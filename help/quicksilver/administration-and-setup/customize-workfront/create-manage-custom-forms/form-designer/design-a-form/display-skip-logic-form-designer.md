---
title: Ajouter une logique d’affichage et ignorer la logique dans un formulaire
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez choisir quelles sections d’un formulaire personnalisé doivent être affichées ou ignorées en fonction des choix que fait la personne qui le remplit.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 98%

---

# Ajouter une logique d’affichage et ignorer la logique dans un formulaire

Vous pouvez choisir quelles sections d’un formulaire personnalisé doivent être affichées ou ignorées en fonction des choix que fait la personne qui le remplit.

>[!NOTE]
>
>La logique s’applique uniquement à un formulaire et ne peut pas être basée sur des sélections d’un autre formulaire.

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Forfait Adobe Workfront </td> 
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
   <td>Accès administratif aux formulaires personnalisés </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Icônes Logique d’affichage et Logique de saut

Les formulaires personnalisés affichent des icônes pour indiquer la logique appliquée à certains champs. Les icônes d’un champ dans le créateur de formulaire indiquent que la logique est appliquée au champ.

| Icône | Emplacement sur le champ dans le créateur de formulaire | Définition |
|--- |--- |--- |
| ![Logique d’affichage pour le champ cible](assets/display-logic-bottom-left.png) | En bas à gauche | Le champ est le champ cible de la logique d’affichage. Si une sélection spécifique est effectuée sur le formulaire, ce champ s’affiche. |
| ![Icône Définir la logique d’affichage](assets/display-logic-bottom-right.png) | En bas à droite | Le champ définit la logique d’affichage. Une sélection ou une valeur spécifique dans ce champ affiche le champ cible. |
| ![Logique de saut pour le champ cible](assets/skip-logic-bottom-left.png) | En bas à gauche | Le champ est le champ cible de la logique de saut. Si une sélection spécifique est effectuée sur le formulaire, celui-ci effectue un saut jusqu’à ce champ et les champs intermédiaires sont masqués. |
| ![Icône Définir la logique de saut](assets/skip-logic-bottom-right.png) | En bas à droite | Le champ définit la logique de saut. Toute sélection ou valeur spécifique dans ce champ saute les autres champs et accède directement au champ cible. |

![Icônes Logique](assets/logic-icons-3.png)

Sélectionnez un champ auquel la logique est appliquée pour afficher les règles logiques existantes dans les paramètres du champ.

![Règles logiques](assets/form-designer-view-only-logic.png)

## Observations relatives à l’utilisation de la logique d’affichage et de la logique de saut

* Pour ajouter une logique d’affichage à un champ personnalisé, un widget ou un saut de section, au moins un champ à choix multiples (boutons radio, liste déroulante ou cases à cocher) doit être positionné avant cette logique dans le formulaire.
Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Vous ne pouvez pas ajouter de logique de saut à un widget ou à un saut de section. Vous pouvez l’ajouter qu’à un champ à choix multiples (boutons radio, liste déroulante ou cases à cocher).
* Vous pouvez ajouter une logique d’affichage et une logique de saut à un champ personnalisé si tous les éléments suivants sont vrais concernant le champ personnalisé :

   * Il s’agit d’un champ à choix multiples (boutons radio, liste déroulante ou cases à cocher).
   * Il est précédé d’un champ à choix multiples.
   * Il est suivi d’un autre champ personnalisé.

* Lorsque vous copiez des formulaires avec une logique d’affichage ou une logique de saut, celle-ci est copiée dans le nouveau formulaire personnalisé.
* Lorsque vous modifiez des objets en masse, tous les champs personnalisés s’affichent dans la zone Modifier les objets, y compris les champs qui sont ignorés ou masqués.
* Gardez ce qui suit à l’esprit lorsque vous créez une règle de logique d’affichage pour un formulaire personnalisé :

   * Les champs personnalisés non inclus dans une instruction de logique d’affichage s’affichent par défaut sur un formulaire personnalisé.
   * Vous pouvez créer des instructions de logique d’affichage à champs multiples.
   * Si la logique d’affichage est appliquée à tous les champs sous un saut de section et qu’ils sont tous masqués en raison de la logique, la section entière est masquée sur le formulaire personnalisé.

## Ajout d’une logique d’affichage à un formulaire personnalisé

La logique d’affichage définit les champs personnalisés qui apparaissent sur le formulaire lorsque l’utilisateur sélectionne une valeur spécifique dans un champ à choix multiples. La logique est ajoutée au champ cible, qui ne s’affiche que lorsque la valeur est sélectionnée.

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés**.
1. Créez un formulaire personnalisé ou ouvrez un formulaire existant. Voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) pour plus d’informations.
1. Ajoutez des champs au formulaire selon vos besoins. Au moins un champ à choix multiples (bouton radio, liste déroulante ou case à cocher) doit être positionné avant le champ cible qui s’affiche.
1. Sélectionnez le champ cible et cliquez sur **Ajouter une logique** en bas à gauche de l’écran.
1. Sélectionnez l’onglet **Logique d’affichage**.
1. Cliquez sur **Ajouter une règle d’affichage** sur le créateur de logique.

   ![Afficher le créateur de logique](assets/custom-form-logic-builder-display-blank.png)

1. Suivez les étapes ci-dessous dans le créateur pour créer l’instruction de logique.

   1. La première option consiste à choisir le champ de définition. Il s’agit du champ avec la valeur de sélection qui affiche la cible. Il doit s’agir d’un champ à choix multiples.
   1. La deuxième option consiste à choisir la valeur de sélection. Seules les valeurs déjà définies pour ce champ sont disponibles.
   1. La troisième option est **Sélectionné** ou **Non sélectionné**. Si vous choisissez **Sélectionné**, lorsque la valeur est sélectionnée, le champ cible s’affiche. Si vous choisissez **Non sélectionné**, lorsque toute autre valeur est sélectionnée dans le champ de définition, le champ cible s’affiche.
   1. Pour ajouter une règle **And** à l’instruction de logique, cliquez sur **Ajouter une règle** directement sous la règle que vous venez de créer. Suivez les mêmes invites pour créer la règle. Toutes les règles And doivent être respectées pour que le champ cible s’affiche.

      ![Afficher le créateur de logique](assets/custom-form-logic-builder-display1.png)

   1. Pour ajouter une règle **Or** à l’instruction de logique, cliquez sur **Ajouter une règle** au bas du bas du créateur de logique. Cliquez ensuite sur **Ajouter une règle** à l’intérieur de la zone Or et suivez les mêmes invites pour créer la règle. Lorsqu’une règle Or est remplie, le champ cible s’affiche.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé de créer l’instruction de logique.

   Les icônes de logique d’affichage sont ajoutées au champ cible et au champ de définition dans le créateur de formulaire.

## Ajouter une logique de saut à un formulaire personnalisé

La logique de saut définit les champs de formulaire personnalisés qui sont ignorés lorsque la personne sélectionne une valeur spécifique dans un champ à choix multiples. Les champs ignorés sont masqués sur le formulaire. La logique est appliquée au champ de définition dans lequel la sélection est effectuée, et non aux champs qui sont ignorés.

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés**.
1. Créez un formulaire personnalisé ou ouvrez un formulaire existant. Voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) pour plus d’informations.
1. Ajoutez des champs au formulaire selon vos besoins. Le champ de définition de la logique de saut doit être un champ à choix multiples (bouton radio, liste déroulante ou case à cocher).
1. Sélectionnez le champ de définition et cliquez sur **Ajouter une logique** en bas à gauche de l’écran.
1. Sélectionnez l’onglet **Logique de saut**.
1. Cliquez sur **Ajouter une règle de saut** dans le créateur de logique.

   ![Créateur de logique de saut](assets/custom-form-logic-builder-skip-blank.png)

1. Suivez les étapes ci-dessous dans le créateur pour créer l’instruction de logique.

   1. Le champ de définition s’affiche sur le créateur. Il s’agit du champ pour lequel vous avez sélectionné la logique de saut.
   1. La première option consiste à choisir la valeur de sélection. Seules les valeurs déjà définies pour le champ sont disponibles.
   1. La deuxième option est **Sélectionné** ou **Non sélectionné**. Si vous choisissez **Sélectionné**, lorsque la valeur est sélectionnée, le champ cible s’affiche et les champs intermédiaires sont ignorés. Si vous choisissez **Non sélectionné**, lorsqu’une autre valeur est sélectionnée dans le champ de définition, le champ cible est affiché et les champs intermédiaires sont ignorés.
   1. La troisième option est le champ cible ou le champ auquel vous passez. Sélectionnez un nom de champ ou **Fin de formulaire**. Vous devrez peut-être d’abord cliquer sur le mot « vide » avant de sélectionner une option.

      ![Créateur de logique de saut](assets/custom-form-logic-builder-skip1.png)

   1. Pour ajouter une règle **Or** à l’instruction de logique, cliquez sur **Ajouter une règle** au bas du créateur de logique. Sélectionnez ensuite les options en suivant les mêmes invites pour créer la règle. Lorsqu’une règle **Or** est remplie, le champ cible s’affiche.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé de créer l’instruction de logique.

   Les icônes de logique de saut sont ajoutées au champ cible et au champ de définition dans le créateur de formulaire.


