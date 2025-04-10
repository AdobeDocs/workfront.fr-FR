---
title: Ajout de règles logiques aux Forms et champs personnalisés
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: L’utilisateur ou l’utilisatrice peut choisir quelles sections d’un formulaire personnalisé doivent être affichées ou ignorées en fonction des choix effectués lors du remplissage.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: f94ad0f289064f243aadb08226bd5e53357f650d
workflow-type: tm+mt
source-wordcount: '1680'
ht-degree: 66%

---

# Ajout de règles logiques aux formulaires et champs personnalisés

Les règles logiques vous permettent de personnaliser davantage les champs de votre formulaire.

Par exemple, vous pouvez afficher ou ignorer des champs ou des sections dans un formulaire personnalisé en fonction des choix effectués par un utilisateur ou une utilisatrice lors du remplissage.

>[!NOTE]
>
>La logique ne s’applique qu’à un seul formulaire et ne peut pas être basée sur les sélections d’un autre formulaire.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Formule Adobe Workfront </td> 
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
   <td>Accès administratif aux formulaires personnalisés </td> 
  </tr>  
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Icônes de logique d’affichage et de saut

Les formulaires personnalisés affichent des icônes pour indiquer quand la logique d’affichage ou d’omission est appliquée à certains champs. Les icônes sur un champ dans le créateur de formulaire indiquent que la logique est appliquée au champ.

| Icône | Emplacement du champ dans le créateur de formulaire | Définition |
|--- |--- |--- |
| ![Logique d’affichage pour le champ cible](assets/display-logic-bottom-left.png) | En bas à gauche | Le champ est le champ cible pour la logique d’affichage. Si une sélection spécifique est effectuée dans le formulaire, ce champ est affiché. |
| ![Définition de l’icône de la logique d’affichage](assets/display-logic-bottom-right.png) | En bas à droite | Le champ définit la logique d’affichage. Une sélection ou une valeur spécifique dans ce champ affiche le champ cible. |
| ![Logique de saut pour le champ cible](assets/skip-logic-bottom-left.png) | En bas à gauche | Le champ est le champ cible pour la logique de saut. Si une sélection spécifique est effectuée dans le formulaire, le formulaire ignore ce champ et les champs intermédiaires sont masqués. |
| ![Définition de l’icône de logique de saut](assets/skip-logic-bottom-right.png) | En bas à droite | Ce champ définit la logique de saut. Une sélection ou une valeur spécifique dans ce champ permet d’ignorer les autres champs et d’accéder directement au champ cible. |

![Icônes de logique](assets/logic-icons-3.png)

Sélectionnez un champ auquel la logique est appliquée pour afficher les règles de logique existantes dans les paramètres du champ.

![Règles de logique](assets/form-designer-view-only-logic.png)

## Observations relatives à l’utilisation des logiques d’affichage et de saut

* Pour ajouter une logique d’affichage sur un champ personnalisé, un widget ou un saut de section, il faut placer au moins un champ à choix multiples (cases d’option, liste déroulante ou cases à cocher) avant celui-ci dans le formulaire.
Pour plus d’informations sur les champs personnalisés et les widgets dans les formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Vous ne pouvez pas ajouter de logique de saut à un widget ou à un saut de section. Vous ne pouvez l’ajouter qu’à un champ à choix multiples (cases d’option, liste déroulante ou cases à cocher).
* Vous ne pouvez pas appliquer la logique d’affichage ou d’omission pour afficher ou masquer les choix d’un champ à options multiples. Par exemple, vous ne pouvez pas restreindre les choix qui s’affichent pour un champ Liste déroulante, un groupe de cases à cocher ou un champ de bouton radio, en fonction de la logique d’affichage ou d’omission d’un autre champ.
* Vous pouvez ajouter une logique d’affichage et une logique de saut à un champ personnalisé si toutes les conditions suivantes sont remplies :

   * Il s’agit d’un champ à choix multiples (cases d’option, liste déroulante ou cases à cocher).
   * Il est précédé d’un champ à choix multiples.
   * Il est suivi d’un autre champ personnalisé.

* Lorsque vous copiez des formulaires avec une logique d’affichage ou une logique de saut, celle-ci est copiée dans le nouveau formulaire personnalisé.
* Lorsque vous modifiez des objets en masse, tous les champs personnalisés s’affichent dans la zone de modification des objets, y compris les champs qui sont ignorés ou masqués.
* Gardez ce qui suit à l’esprit lorsque vous créez une règle de logique d’affichage pour un formulaire personnalisé :

   * les champs personnalisés non inclus dans une instruction de logique d’affichage s’affichent par défaut sur un formulaire personnalisé.
   * Vous pouvez créer des instructions de logique d’affichage à champs multiples.
   * Si la logique d’affichage est appliquée à tous les champs sous un saut de section et qu’ils sont tous masqués à la suite de cette logique, la section entière sera masquée dans le formulaire personnalisé.

## Ajouter une logique d’affichage à un formulaire personnalisé

La logique d’affichage définit les champs personnalisés qui apparaissent dans le formulaire lorsque l’utilisateur ou l’utilisatrice sélectionne une valeur spécifique dans un champ à choix multiple. La logique est ajoutée au champ cible, qui ne s’affiche que lorsque la valeur est sélectionnée.

<!--
>[!NOTE]
>
><span class="preview">This procedure describes the basic mode for display logic. Advanced display logic is also available. For more information, see [Add advanced display logic to a custom form](#add-advanced-display-logic-to-a-custom-form), in this article.</span>
-->

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés**.
1. Créez un formulaire personnalisé ou ouvrez un formulaire existant. Pour plus d’informations, consultez [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Ajoutez des champs au formulaire si nécessaire. Au moins un champ à choix multiple (case d’option, liste déroulante ou case à cocher) doit être placé avant le champ cible qui s’affichera.
1. Sélectionnez le champ cible et cliquez sur **Ajouter une logique**.
1. Sélectionnez l’onglet **Affichage** dans le créateur de logiques.
1. Cliquez sur **Ajouter une règle d’affichage**.

   ![Créateur de logique d’affichage](assets/simple-display-logic1-val-only-in-menu.png)

1. Suivez les étapes ci-dessous pour créer l’instruction logique dans le créateur.

   1. La première option consiste à choisir le champ de définition. Il s’agit du champ avec la valeur de sélection qui affiche la cible. Il doit s’agir d’un champ à choix multiple.
   1. La deuxième option consiste à choisir la valeur de sélection. Seules les valeurs déjà définies pour ce champ sont disponibles.
   1. La troisième option est **Sélectionné** ou **Non sélectionné**. Choisir **Sélectionné** signifie que lorsque la valeur est sélectionnée, le champ cible s’affiche. Choisir **Non sélectionné** signifie que lorsqu’une autre valeur est sélectionnée dans le champ de définition, le champ cible s’affiche.
   1. Pour ajouter une règle **And** à l’instruction de la logique, cliquez sur **Ajouter une règle** directement sous la règle que vous venez de créer. Suivez les mêmes instructions pour créer la règle. Toutes les règles And doivent être respectées pour que le champ cible s’affiche.

      ![Créateur de logique d’affichage](assets/simple-display-logic2.png)

   1. Pour ajouter une règle **Or** à l’instruction de la logique, cliquez sur **Ajouter une règle** en bas du créateur de logique. Ensuite, cliquez sur **Ajouter une règle** dans la zone Or et suivez les mêmes instructions pour créer la règle. Lorsqu’une règle Or est respectée, le champ cible s’affiche.

1. Cliquez sur **Appliquer** lorsque vous avez fini de créer l’instruction logique.

   Les icônes de logique d’affichage sont ajoutées au champ cible et au champ de définition dans le créateur de formulaire.

<!--
<div class="preview">

## Add advanced display logic to a custom form

The advanced display logic for custom form fields allows you to build complex logic using formulas. You can apply this logic to the following field types: drop-down, radio button, checkbox, typeahead, single line text, paragraph text, date field, text with formatting, and calculated fields.

### Examples

You can use advanced display logic to control the visibility of custom form sections based on user roles and the visibility of a field based on another field's status.

No logic is applied to the default section on the form, so it is always visible to all users.

Using the following condition, the Resources Required section is only displayed when a user with the job role of Resource Manager views the form.

```IF($$USER.{roleID}="123abc", true)```

Note that ```123abc``` represents the role ID of the Resource Manager.

![Form section displayed for role](assets/advanced-display-on-form1.png)

The same condition with a different role ID is applied to the Project Financial KPIs section to define that  only the Financial Advisor role can view the section.

Using the following condition, the Sold KPI field only becomes visible when the project is complete. This logic is applied directly to the field instead of to a form section. There is no need to specify which role can view the field, because that is already defined in the section that the field is in.

```IF({status}="CPL", true)```

![Field is visible on complete project](assets/advanced-display-on-form2.png)

### Define advanced display logic

{{step-1-to-setup}}

1. Click **Custom Forms**.
1. Create a new custom form or open an existing form. See [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) for details.
1. Add fields to the form as needed.
1. Select the field to apply logic to, and click **Add Logic**.
1. Select the **Display** tab on the logic builder.
1. Turn on **Advanced mode**.
   
   This option might be turned on automatically, for fields that do not support the simple mode of display logic.

   ![Advanced mode for display logic](assets/advanced-display-logic-blank-editor.png)

1. Build the display condition in the editor.

   For more information about calculations and expressions, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) and [Overview of calculated data expressions](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Click **Apply**.
   
   The logic is applied to the field and the display logic icon is added in the form designer.

</div>
-->

## Ajouter une logique de saut à un formulaire personnalisé

La logique de saut définit des champs de formulaire personnalisés qui sont ignorés lorsque l’utilisateur ou l’utilisatrice sélectionne une valeur spécifique dans un champ à choix multiple. Les champs ignorés sont masqués dans le formulaire. La logique est appliquée au champ de définition dans lequel s’effectue la sélection, et non aux champs qui sont ignorés.

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés**.
1. Créez un formulaire personnalisé ou ouvrez un formulaire existant. Pour plus d’informations, consultez [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Ajoutez des champs au formulaire si nécessaire. Le champ définissant la logique de saut doit être un champ à choix multiple (case d’option, liste déroulante ou case à cocher).
1. Sélectionnez le champ de définition et cliquez sur **Ajouter une logique** en bas à gauche de l’écran.
1. Sélectionnez l’onglet **Ignorer** dans le créateur de logiques.
1. Cliquez sur **Ajouter une règle d’omission**.

   ![Créateur de logique de saut](assets/skip-logic1-val-only-in-menu.png)

1. Suivez les étapes ci-dessous pour créer l’instruction logique dans le créateur.

   1. Le champ de définition est indiqué sur le créateur. Il s’agit du champ que vous avez sélectionné pour appliquer la logique de saut.
   1. La première option consiste à choisir la valeur de sélection. Seules les valeurs déjà définies pour le champ sont disponibles.
   1. La deuxième option est **Sélectionné** ou **Non sélectionné**. Choisir **Sélectionné** signifie que lorsque la valeur est sélectionnée, le champ cible est affiché et les champs situés entre les deux sont ignorés. Choisir **Non sélectionné** signifie que lorsqu’une autre valeur est sélectionnée dans le champ de définition, le champ cible est affiché et les champs situés entre les deux sont ignorés.
   1. La troisième option est le champ cible, c’est-à-dire l’endroit où il faut accéder en ignorant les autres champs. Sélectionnez un nom de champ ou cliquez sur **Fin du formulaire**. Vous devrez peut-être cliquer sur le mot « vide » avant de sélectionner une option.

      ![Créateur de logique de saut](assets/skip-logic2.png)

   1. Pour ajouter une règle **Or** à l’instruction de logique, cliquez sur **Ajouter une règle** en bas du créateur de logique. Sélectionnez ensuite les options en suivant les mêmes invites pour élaborer la règle. Lorsqu’une règle **Or** est respectée, le champ cible s’affiche.

1. Cliquez sur **Appliquer** lorsque vous avez fini de créer l’instruction logique.

   Les icônes de logique de saut sont ajoutées au champ cible et au champ de définition dans le créateur de formulaire.

## Ajouter une logique de validation à un formulaire personnalisé

La logique de validation est créée à l’aide de formules et vous pouvez la rendre aussi simple ou complexe que nécessaire. La validation peut être basée sur les valeurs d’autres champs ou l’état d’objets, et vous pouvez fournir un message d’erreur pour lorsque la validation échoue.

Si le champ avec la logique appliquée remplit les conditions de validation définies lorsqu’un utilisateur remplit le formulaire personnalisé, le champ est mis en surbrillance et le message d’erreur s’affiche.

Vous pouvez appliquer la logique de validation aux types de champ suivants : texte monoligne, paragraphe, liste déroulante à sélection unique, liste déroulante à sélection multiple, recherche externe, saisie semi-automatique, date, groupe de cases à cocher et boutons radio.

### Exemples

En utilisant la condition suivante, le champ Budget affiche un message sous le champ lorsque l’utilisateur saisit une valeur qui déclenche le message. Par exemple, si la valeur saisie est négative, le premier message s’affiche. Si l’utilisateur ou l’utilisatrice tente de modifier le statut du projet sur Actuel avant de saisir une valeur de budget, le deuxième message s’affiche.

```
IF({DE:Budget Field} < 0,
     "Budget cannot be negative",
     IF({DE:Budget Field} == 0 && {status} == "CUR", "Budget must be specified before moving to Current status")
)
```

Un autre exemple simple est qu’un champ de numéro de téléphone doit contenir un certain nombre de chiffres pour être valide.

Un autre exemple de validation basée sur d’autres champs est un champ pour la taille de la salle de réunion (petite, moyenne ou grande) et un champ distinct pour le nombre de participants à la réunion. Le nombre de personnes pour chaque taille de chambre est écrit dans la formule de validation. Si le nombre de participants que l&#39;utilisateur entre est trop élevé pour la salle de réunion choisie, le message d&#39;erreur s&#39;affiche.

### Définition de la logique de validation

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés**.
1. Créez un formulaire personnalisé ou ouvrez un formulaire existant. Pour plus d’informations, consultez [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Ajoutez des champs au formulaire selon vos besoins.
1. Sélectionnez le champ auquel appliquer la logique, puis cliquez sur **Ajouter une logique**.
1. Sélectionnez l’onglet **Validation** dans le créateur de logiques.

   ![Créateur de logique de validation](assets/validation-logic-blank-editor-val-only-in-menu.png)

1. Créez la condition de validation dans l’éditeur, y compris le message d’erreur à afficher lorsque la validation n’est pas remplie.

   Pour plus d’informations sur les calculs et les expressions, voir [Ajouter des champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) et [Présentation des expressions de données calculées](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Cliquez sur **Appliquer**.

   La logique est appliquée au champ dans le concepteur de formulaire.

<!--
<div class="preview">

## Add formatting logic to a custom form

Formatting logic highlights a field value when it meets the defined conditions. The applied formatting will work on multiple fields at once.

You can apply formatting logic to the following field types: single line text, paragraph, single-select dropdown, multi-select dropdown, external lookup, typeahead, calculated, date, checkbox group, and radio buttons.

Formatting applied to custom forms is separate from formatting applied to lists and reports. For information on report formatting, see [Use conditional formatting in views](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Example

Using the following condition, the Budget field appears red when the user enters a value of 1000 or more. The field appears yellow when the user enters a value of 500 or more.

To add a hover-over definition of the formatting, use the Instructions field in the custom form. For example, a message on the Budget field could say "Please enter a budget within a reasonable range. Values over 500 are a warning notice, and above 1000 is considered too high."

```
IF(
     {DE:Budget Field} >=1000,
     FORMAT($$NEGATIVE),
     IF({DE:Budget Field} >= 500, FORMAT($$NOTICE))
)
```

### Define formatting logic

{{step-1-to-setup}}

1. Click **Custom Forms**.
1. Create a new custom form or open an existing form. See [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) for details.
1. Add fields to the form as needed.
1. Select the field to apply logic to, and click **Add Logic**.
1. Select the **Formatting** tab on the logic builder.

   ![Formatting logic builder](assets/formatting-logic-blank-editor.png)

1. Build the formatting condition in the editor.

   You can add up to five formatting rules per field.

   The field highlighting color options are:

   * `$$POSITIVE (green)`
   * `$$INFORMATIVE (blue)`
   * `$$NEGATIVE (red)`
   * `$$NOTICE (orange)`
   
   The text formatting options are:
   
   * `$$BOLD`
   * `$$ITALIC`
   * `$$UNDERLINE`

   Only one color option may be used per function, along with up to three additional text formatting options. If no color option is specified, the system's default color is applied.

   For more information about calculations and expressions, see [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) and [Overview of calculated data expressions](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Click **Apply**.
   
   The logic is applied to the field in the form designer.

</div>
-->
