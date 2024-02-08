---
title: Ajout d’une logique d’affichage et d’exclusion à l’aide du concepteur de formulaires
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez choisir quelles sections d’un formulaire personnalisé doivent être affichées ou ignorées en fonction des choix que fait l’utilisateur lorsqu’il le remplit.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 2d46a047db8117983978f1411095bc8c022abbe2
workflow-type: tm+mt
source-wordcount: '1298'
ht-degree: 0%

---

# Ajout d’une logique d’affichage et d’exclusion à l’aide du concepteur de formulaires

{{highlighted-preview-article-level}}

Vous pouvez choisir quelles sections d’un formulaire personnalisé doivent être affichées ou ignorées en fonction des choix que fait l’utilisateur lorsqu’il le remplit.

>[!NOTE]
>
>La logique s’applique uniquement à un formulaire et ne peut pas être basée sur des sélections d’un autre formulaire.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Formule Adobe Workfront </td> 
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
   <td>Accès administratif aux formulaires personnalisés </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Icônes logiques d’affichage et d’exclusion

Les formulaires personnalisés affichent des icônes pour indiquer la logique appliquée à certains champs. Les icônes d’un champ dans le concepteur de formulaires indiquent que la logique est appliquée au champ.

| Icône | Emplacement sur le champ dans le concepteur de formulaires | Définition |
|--- |--- |--- |
| ![Logique d’affichage pour le champ cible](assets/display-logic-bottom-left.png) | En bas à gauche | Le champ est le champ cible de la logique d’affichage. Si une sélection spécifique est effectuée sur le formulaire, ce champ s’affiche. |
| ![Icône Définir la logique d’affichage](assets/display-logic-bottom-right.png) | En bas à droite | Le champ définit la logique d’affichage. Une sélection ou une valeur spécifique sur ce champ affiche le champ cible. |
| ![Ignorer la logique pour le champ cible](assets/skip-logic-bottom-left.png) | En bas à gauche | Le champ est le champ cible de la logique de saut. Si une sélection spécifique est effectuée sur le formulaire, celui-ci passe à ce champ et les champs intermédiaires sont masqués. |
| ![Icône Définir la logique de saut](assets/skip-logic-bottom-right.png) | En bas à droite | Le champ définit la logique de saut. Une sélection ou une valeur spécifique de ce champ ignore les autres champs et accède directement au champ cible. |

![Icônes logiques](assets/logic-icons-3.png)

Sélectionnez un champ auquel la logique est appliquée pour afficher les règles logiques existantes dans les paramètres du champ.

![Règles logiques](assets/form-designer-view-only-logic.png)

## Observations relatives à l’utilisation de la logique d’affichage et de la logique de saut

* Pour ajouter une logique d’affichage à un champ personnalisé, un widget ou un saut de section, au moins un champ à choix multiples (boutons radio, liste déroulante ou cases à cocher) doit être positionné avant cette logique dans le formulaire.
Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Concevoir un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Vous ne pouvez pas ajouter de logique de saut à un widget ou à un saut de section. Vous pouvez l’ajouter uniquement à plusieurs champs de choix (boutons radio, liste déroulante ou cases à cocher).
* Vous pouvez ajouter une logique d’affichage et ignorer la logique à un champ personnalisé si tous les éléments suivants sont vrais concernant le champ personnalisé :

   * Il s’agit d’un champ à choix multiples (boutons radio, liste déroulante ou cases à cocher).
   * Il est précédé d’un champ à choix multiples.
   * Il est suivi d’un autre champ personnalisé

* Lorsque vous copiez des formulaires avec une logique d’affichage ou ignorez la logique, celle-ci est copiée dans le nouveau formulaire personnalisé.
* Lorsque vous modifiez des objets en bloc, tous les champs personnalisés s’affichent dans la zone Modifier les objets , y compris les champs qui sont ignorés ou masqués.
* Gardez ce qui suit à l’esprit lorsque vous créez une règle de logique d’affichage pour un formulaire personnalisé :

   * Les champs personnalisés non inclus dans une instruction de logique d’affichage s’affichent par défaut sur un formulaire personnalisé.
   * Vous pouvez créer des instructions logiques d’affichage à champs multiples.
   * Si la logique d’affichage est appliquée à tous les champs sous un saut de section et qu’ils sont tous masqués en raison de la logique, la section entière est masquée sur le formulaire personnalisé.

## Ajout d’une logique d’affichage à un formulaire personnalisé

La logique d’affichage définit les champs personnalisés qui apparaissent sur le formulaire lorsque l’utilisateur sélectionne une valeur spécifique dans un champ à choix multiples. La logique est ajoutée au champ cible, qui ne s&#39;affiche que lorsque la valeur est sélectionnée.

{{step-1-to-setup}}

1. Cliquez sur **Forms personnalisée**.
1. Créez un formulaire personnalisé ou ouvrez un formulaire existant. Voir [Concevoir un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) pour plus d’informations.
1. Ajoutez des champs au formulaire selon vos besoins. Au moins un champ à choix multiples (bouton radio, liste déroulante ou case à cocher) doit être positionné avant le champ cible qui s’affichera.
1. Sélectionnez le champ cible et cliquez sur **Ajouter une logique** en bas à gauche de l’écran.
1. Sélectionnez la variable **Logique d’affichage** .
1. Cliquez sur **Ajouter une règle d’affichage** sur le créateur de logique.

   ![Afficher le créateur de logique](assets/custom-form-logic-builder-display-blank.png)

1. Suivez les étapes ci-dessous dans le créateur pour créer l’instruction de logique.

   1. La première option consiste à choisir le champ de définition. Il s’agit du champ avec la valeur de sélection qui affiche la cible. Il doit s’agir d’un champ à choix multiples.
   1. La deuxième option consiste à choisir la valeur de sélection. Seules les valeurs déjà définies pour ce champ sont disponibles.
   1. La troisième option est **Sélectionné** ou **Non sélectionné**. Choix **Sélectionné** signifie que lorsque la valeur est sélectionnée, le champ cible est affiché. Choix **Non sélectionné** signifie que lorsque toute autre valeur est sélectionnée dans le champ de définition, le champ cible est affiché.
   1. Pour ajouter une **Et** à l’instruction logique, cliquez sur **Ajouter une règle** directement sous la règle que vous venez de créer. Suivez les mêmes invites pour créer la règle. Toutes les règles Et doivent être respectées pour que le champ cible s’affiche.

      ![Afficher le créateur de logique](assets/custom-form-logic-builder-display1.png)

   1. Pour ajouter une **Ou** à l’instruction logique, cliquez sur **Ajouter une règle** près du bas du créateur de logique. Cliquez ensuite sur **Ajouter une règle** à l’intérieur de la zone Ou et suivez les mêmes invites pour créer la règle. Lorsqu’une règle Ou est remplie, le champ cible s’affiche.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé de créer l’instruction logique.

   Les icônes de logique d’affichage sont ajoutées au champ cible et au champ de définition dans le concepteur de formulaires.

>[!NOTE]
>
>La logique d’affichage est temporairement indisponible lorsque vous prévisualisez votre formulaire dans le concepteur de formulaires.

## Ajout d’une logique de saut à un formulaire personnalisé

La logique Ignorer définit les champs de formulaire personnalisés qui sont ignorés lorsque l’utilisateur sélectionne une valeur spécifique dans un champ à choix multiples. Les champs ignorés sont masqués sur le formulaire. La logique est appliquée au champ de définition dans lequel la sélection est effectuée, et non aux champs qui sont ignorés.

{{step-1-to-setup}}

1. Cliquez sur **Forms personnalisée**.
1. Créez un formulaire personnalisé ou ouvrez un formulaire existant. Voir [Concevoir un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) pour plus d’informations.
1. Ajoutez des champs au formulaire selon vos besoins. Le champ de définition de la logique de saut doit être un champ à choix multiples (bouton radio, liste déroulante ou case à cocher).
1. Sélectionnez le champ de définition et cliquez sur **Ajouter une logique** en bas à gauche de l’écran.
1. Sélectionnez la variable **Ignorer la logique** .
1. Cliquez sur **Ajouter une règle Ignorer** sur le créateur de logique.

   ![Ignorer le créateur de logique](assets/custom-form-logic-builder-skip-blank.png)

1. Suivez les étapes ci-dessous dans le créateur pour créer l’instruction de logique.

   1. Le champ de définition s’affiche sur le créateur. Il s’agit du champ auquel vous avez sélectionné la logique de saut.
   1. La première option consiste à choisir la valeur de sélection. Seules les valeurs déjà définies pour le champ sont disponibles.
   1. La deuxième option est la suivante : **Sélectionné** ou **Non sélectionné**. Choix **Sélectionné** signifie que lorsque la valeur est sélectionnée, le champ cible est affiché et les champs intermédiaires sont ignorés. Choix **Non sélectionné** signifie que lorsqu&#39;une autre valeur est sélectionnée dans le champ de définition, le champ cible est affiché et les champs intermédiaires sont ignorés.
   1. La troisième option est le champ cible ou l’emplacement où vous pouvez passer. Sélectionnez un nom de champ ou **Fin de formulaire**. Vous devrez peut-être d’abord cliquer sur le mot &quot;vide&quot; avant de sélectionner une option.

      ![Ignorer le créateur de logique](assets/custom-form-logic-builder-skip1.png)

   1. Pour ajouter une **Ou** à l’instruction logique, cliquez sur **Ajouter une règle** près du bas du créateur de logique. Sélectionnez ensuite les options suivant les mêmes messages pour créer la règle. Lorsque **Ou** est remplie, le champ cible s’affiche.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé de créer l’instruction logique.

   Les icônes de logique de saut sont ajoutées au champ cible et au champ de définition dans le concepteur de formulaires.

>[!NOTE]
>
>La logique Ignorer est temporairement indisponible lorsque vous prévisualisez votre formulaire dans le concepteur de formulaires.
