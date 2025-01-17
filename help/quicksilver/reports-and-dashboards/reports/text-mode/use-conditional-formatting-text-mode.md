---
product-area: reporting
navigation-topic: text-mode-reporting
title: Utiliser la mise en forme conditionnelle en mode texte
description: Utiliser la mise en forme conditionnelle en mode texte
author: Nolan
feature: Reports and Dashboards
exl-id: 48fc8450-35c6-4d59-89d3-0feffe662b25
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '1682'
ht-degree: 99%

---

# Utiliser la mise en forme conditionnelle en mode texte

<!--Audited: 01/2025-->

Le créateur d’interface standard offre une grande flexibilité lors de la création d’éléments de rapport pour répondre aux besoins de votre organisation.

Vous pouvez appliquer une mise en forme conditionnelle dans une vue en utilisant l’interface standard.\
Pour plus d’informations sur l’application de la mise en forme conditionnelle à une vue, voir [Utiliser la mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Accès en modification aux rapports, tableaux de bord et calendriers pour modifier les vues d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion à un rapport pour modifier les vues d’un rapport</p> <p>Gérer les autorisations d’une vue pour la modifier</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mise en forme conditionnelle en mode texte

Le mode texte vous permet de créer des vues, des filtres, des regroupements et des invites plus complexes en vous permettant d’utiliser des champs qui ne sont pas disponibles dans l’interface standard.

Pour obtenir une liste complète de tous nos champs pouvant faire l’objet d’un rapport, voir la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

Pour plus d’informations sur l’utilisation de la syntaxe du mode texte, voir [Vue d’ensemble de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

Vous pouvez également utiliser le mode texte pour mettre en forme les vues dans les rapports et les listes. Grâce à la mise en forme conditionnelle, vous pouvez modifier les vues de vos rapports en changeant le type de police et l’arrière-plan des résultats dans le rapport, ainsi que les icônes et les indicateurs. Nous vous recommandons de toujours créer vos vues en utilisant d’abord l’interface standard et de ne passer à l’interface en mode texte qu’en cas de nécessité absolue.

>[!NOTE]
>
> L’utilisation du style CSS pour personnaliser la mise en forme conditionnelle n’est pas prise en charge. Au lieu de cela, vous devez utiliser les options de mise en forme prédéfinies disponibles dans Adobe Workfront.

## Ajouter une mise en forme conditionnelle aux vues

Pour plus d’informations sur l’application de la mise en forme conditionnelle à une vue dans l’interface du créateur standard, voir [Utiliser la mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

Pour ajouter une mise en forme conditionnelle à une vue dans l’interface en mode texte :

1. Accédez à une liste d’objets.
1. Développez le menu déroulant d’une vue à laquelle vous souhaitez ajouter une mise en forme conditionnelle.
1. Cliquez sur **Personnaliser la vue**.
1. Cliquez sur la colonne de la vue à laquelle vous souhaitez appliquer une mise en forme conditionnelle.
1. Cliquez sur **Basculer en mode texte**.
1. Dans la zone **Afficher dans cette colonne :**, cliquez sur **Cliquez pour modifier le texte**.
1. Ajoutez les exemples de code fournis dans [Mettre en forme les vues à l’aide du mode texte](#format-views-using-text-mode) au bas du texte dans la colonne que vous avez sélectionnée.
1. Cliquez sur **Enregistrer**, puis sur **Enregistrer l’affichage**.

## Mettre en forme les vues à l’aide du mode texte {#format-views-using-text-mode}

Vous pouvez ajouter les composants suivants à une colonne d’une vue pour la mettre en forme de manière conditionnelle en mode texte :

* [Paramètres des colonnes](#column-settings)
* [Règles de colonnes](#column-rules)
* [Mettre en forme de manière conditionnelle une expression de valeur](#conditionally-format-a-valueexpression)

### Paramètres des colonnes {#column-settings}

Vous devez vous familiariser avec l’interface du mode texte avant de pouvoir ajouter une mise en forme conditionnelle à vos vues.

Vous pouvez personnaliser les éléments suivants d’une colonne lorsque vous utilisez la mise en forme conditionnelle dans une vue :

* [En-têtes de colonnes](#column-headers)
* [Format des dates](#format-dates)
* [Format des nombres](#format-numbers)

#### En-têtes de colonnes {#column-headers}

Pour modifier l’en-tête de colonne affiché, ajoutez le code suivant à votre colonne : `displayname= [Name of column]`. Par exemple, pour nommer une colonne Personne propriétaire du projet, le code texte serait le suivant :

`displayname=Project Owner`

#### Formater les dates {#format-dates}

Les dates peuvent être configurées pour être affichées dans différents formats.

Pour plus d’informations, voir [Formater les dates dans les rapports en mode texte](../../../reports-and-dashboards/reports/text-mode/format-dates-in-text-mode-reports.md).

#### Format des nombres {#format-numbers}

Vous pouvez formater les valeurs numériques pour afficher les informations qui répondent le mieux à vos besoins en matière de rapports.

Pour plus d’informations, voir [Formater les nombres, les devises et les pourcentages dans les rapports en mode texte](../../../reports-and-dashboards/reports/text-mode/format-numbers-in-text-mode-reports.md).

### Règles de la colonne {#column-rules}

Les règles de colonne permettent d’ajouter des images, des couleurs, des mises en forme et des remplacements de texte dans une vue. Les règles de colonne peuvent être établies indépendamment ou peuvent contenir plusieurs conditions pour une colonne.

* [Mise en forme conditionnelle](#conditional-formatting)
* [Plusieurs formats conditionnels](#multiple-conditional-formats)
* [Appliquer le texte](#apply-text)
* [Appliquer les formats de ligne](#apply-row-formats)
* [Appliquer les images](#apply-images)

#### Mise en forme conditionnelle {#conditional-formatting}

Une instruction spécifique au mode de texte doit être appliquée lors de l’incorporation de couleur ou du formatage du texte.

>[!NOTE]
>
>La mise en forme conditionnelle peut ne pas être prise en charge dans les colonnes fusionnées.\
>Pour plus d’informations sur la fusion de colonnes en mode texte, voir [Vue : informations sur la fusion de plusieurs colonnes en une colonne partagée](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

Insérez le code suivant dans n’importe quelle colonne à laquelle vous souhaitez ajouter une mise en forme conditionnelle :

```
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

>[!NOTE]
>
>La ligne `styledef.case.0.comparison.icon` est toujours fausse, sauf si vous travaillez avec des icônes.
>
>La ligne `styledef.case.0.comparison.truetext` reste toujours vide, sauf si vous travaillez avec du texte de remplacement.
>
>La ligne `styledef.case.0.comparison.righttext` est vide lorsque le qualificateur est notblank.

Par exemple, si vous voulez afficher le nom de l’entreprise en vert dans un rapport de projet, vous pouvez utiliser le code suivant :

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name ;
styledef.case.0.comparison.righttext= 
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
```

>[!NOTE]
>
>* Si cette instruction peut s’appliquer à la colonne Nom de l’entreprise, elle peut également s’appliquer à n’importe quelle autre colonne du rapport. Le texte vert ne s’affiche que si le projet est associé à une entreprise. N’oubliez pas que `[field name]`, `[value]` et `[qualifier]` déterminent si l’introduction de conditions s’affiche ou non sur la colonne.
>* Pour les qualificateurs, nous avons recommandé d’utiliser `cicontains` plutôt que `equal`. Par défaut, `equal` recherche les numéros d’identification. En utilisant le qualificateur `cicontains`, vous pouvez accéder aux éléments par leur nom.

![](assets/screen-shot-2013-08-15-at-2.53.51-pm-350x199.png){width="500"}


![](assets/screen-shot-2013-08-15-at-2.54.08-pm-350x185.png){width="400"}

Qu’une couleur du texte, un alignement, un style de police ou une couleur d’arrière-plan soient appliqués à un mode texte, la même instruction (illustrée ci-dessus) est utilisée.

Les lignes suivantes doivent être modifiées pour refléter le formatage correspondant nécessaire pour la colonne :

```
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
```

Utilisez les tableaux suivants pour identifier les lignes à modifier et les valeurs à spécifier pour définir le style de format de votre colonne :

| **Couleur du texte** | **Line: textcolor=** |
|---|---|
| Noir | `000000` |
| Bleu foncé | `0c6aca` |
| Bleu sarcelle | `1b878c` |
| Vert | `03a219` |
| Violet | `6408c4` |
| Gris | `767676` |
| Rouge | `d30519` |
| Jaune | `e19503` |

{style="table-layout:auto"}

| **Alignement** | **Line: align=** |
|---|---|
| Alignement à gauche | `left` |
| Alignement à droite | `right` |
| Alignement au centre | `center` |

{style="table-layout:auto"}

| Police | Line: ***fontstyle=*** |
|---|---|
| Gras | `bold` |
| Italiques | `italic` |

{style="table-layout:auto"}

| **Couleur d’arrière-plan** | **Line: bgcolor=** |
|---|---|
| Bleu sarcelle | `dcf6f7` |
| Vert | `def6e2` |
| Gris | `e8e8e8` |
| Bleu | `e8f1ff` |
| Violet | `e9def4` |
| Rouge | `eac6c9` |
| Jaune | `feecc8` |
| Blanc | `ffffff` |

{style="table-layout:auto"}

#### Plusieurs formats conditionnels {#multiple-conditional-formats}

Vous pouvez appliquer plusieurs styles de mise en forme à une instruction. L’instruction de base reste inchangée et toutes les instructions de formatage supplémentaires sont ajoutées à l’instruction.

Par exemple, en utilisant l’instruction précédente pour inclure le nom de l’entreprise dans le texte vert en gras. L’instruction est rédigée à l’aide du code suivant :

```
styledef.case.0.comparison.leftmethod=company:name
styledef.case.0.comparison.lefttext=company:name
styledef.case.0.comparison.righttext=
styledef.case.0.comparison.operator=notblank
styledef.case.0.comparison.operatortype=string
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext= 
styledef.case.0.comparison.trueproperty.0.name=textcolor
styledef.case.0.comparison.trueproperty.0.value=03a219
styledef.case.0.comparison.trueproperty.1.name=fontstyle
styledef.case.0.comparison.trueproperty.1.value=bold
```

>[!NOTE]
>
>Lorsque vous incluez plus d’une instruction de mise en forme conditionnelle, il est nécessaire d’identifier numériquement chaque expression dans l’instruction. Remarquez que l’expression 0 et l’expression 1 ont été identifiées.

#### Appliquer du texte {#apply-text}

Si vous souhaitez remplacer les valeurs par défaut qui apparaissent dans une colonne par une valeur de votre choix, vous pouvez le faire en appliquant du texte à la colonne.

Par exemple, dans un rapport sur les projets, définissez la valeur de la colonne « Date de début prévue » pour qu’au lieu d’afficher la date de début prévue pour le projet, elle affiche le texte « Pas aujourd’hui ». Utilisez le code suivant pour la colonne « Date de début prévue » :

```
case.0.comparison.leftmethod=plannedStartDate
case.0.comparison.lefttext=plannedStartDate
case.0.comparison.righttext=2013-04-10T10:45:00:000
case.0.comparison.operator=ne
case.0.comparison.operatortype=date
case.0.comparison.icon=false
case.0.comparison.truetext=not today
styledef.case.0.comparison.leftmethod=plannedStartDate
styledef.case.0.comparison.lefttext=plannedStartDate
styledef.case.0.comparison.righttext=2013-04-10T10:45:00:000 
styledef.case.0.comparison.operator=ne
styledef.case.0.comparison.operatortype=date&
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.truetext=not today
```

>[!NOTE]
>
>Les lignes commençant par `case.0.` utilisent des comparaisons de cas pour identifier l’utilisation du texte. Les lignes commençant par `styledef.case.0.` sont les premières instructions de mise en forme conditionnelle où l’utilisation du texte est identifiée par le biais de l’expression `truetext`. Veillez à donner une valeur à `truetext`, plutôt que de la laisser vide.

![](assets/screen-shot-2013-08-15-at-3.22.02-pm-350x196.png){width="500"}

![](assets/screen-shot-2013-08-15-at-3.22.16-pm-350x151.png){width="400"}

#### Appliquer des formats aux lignes {#apply-row-formats}

Si vous souhaitez appliquer une condition à l’ensemble de la ligne, utilisez le code suivant avec le code de votre colonne :

```
styledef.case.0.comparison.icon=false
styledef.case.0.comparison.isrowcase=true
styledef.case.0.comparison.leftmethod= [field name]
styledef.case.0.comparison.lefttext= [field name]
styledef.case.0.comparison.operator= [qualifier]
styledef.case.0.comparison.operatortype= [data type]
styledef.case.0.comparison.righttext= [field value]
styledef.case.0.comparison.trueproperty.0.name= [format option]
styledef.case.0.comparison.trueproperty.0.value= [format style]
styledef.case.0.comparison.truetext=
row.0.styledef.applyallcases=true
row.0.styledef.case.0.comparison.icon=false
row.0.styledef.case.0.comparison.isrowcase=true
row.0.styledef.case.0.comparison.leftmethod= [field name]
row.0.styledef.case.0.comparison.lefttext= [field name]
row.0.styledef.case.0.comparison.operator= [qualifier]
row.0.styledef.case.0.comparison.operatortype= [data type]
row.0.styledef.case.0.comparison.righttext= [field value]
row.0.styledef.case.0.comparison.trueproperty.0.name= [format option]
row.0.styledef.case.0.comparison.trueproperty.0.value= [format style]
row.0.styledef.case.0.comparison.truetext=
```

#### Appliquer les images {#apply-images}

Comme pour la mise en forme du texte, des images peuvent être utilisées pour afficher des informations dans les rapports. Workfront dispose d’un certain nombre d’images intégrées pour transmettre des informations visuelles dans le cadre d’un rapport. Pour utiliser des images dans le cadre de la mise en forme conditionnelle, l’instruction suivante est nécessaire :

```
image.case.0.comparison.leftmethod= [field name]
image.case.0.comparison.lefttext= [field name]
image.case.0.comparison.righttext= [field value]
image.case.0.comparison.operator= [qualifier]
image.case.0.comparison.operatortype= [data type]
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=
```

Par exemple, dans un rapport sur les projets, vous souhaitez créer une colonne dans laquelle vous affichez un visage renfrogné pour chaque date d’achèvement prévue qui ne correspond pas à la date d’aujourd’hui. Utilisez le code en mode texte suivant pour ajouter l’icône à votre colonne :

```
image.case.0.comparison.leftmethod=plannedCompletionDate
image.case.0.comparison.lefttext=plannedCompletionDate
image.case.0.comparison.righttext=2013-04-10T13:00:00:000 
image.case.0.comparison.operator=ne 
image.case.0.comparison.operatortype=date
image.case.0.comparison.icon=true
image.case.0.comparison.truetext=/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif
```

>[!NOTE]
>
>Remarquez que l’instruction utilise l’expression `icon=true`. Cette instruction est également différente des autres instructions de mise en forme conditionnelle, car elle n’utilise pas le format `style.def`, mais plutôt un format d’image unique.

![](assets/screen-shot-2013-08-15-at-3.35.08-pm-350x199.png){width="500"}

![](assets/screen-shot-2013-08-15-at-3.35.22-pm-1-350x167.png){width="400"}

Pour utiliser les images disponibles, appliquez le code et les valeurs suivants :

| **Icône** | **Line: image.case.0.comparison.truetext=** |
|---|---|
| Visage renfrogné ![](assets/face-sad.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_frown.gif` |
| Visage heureux ![](assets/face-happy.png) | =`/interface/images/v4_redux/icons/casebuilder/emoticon_smile.gif` |
| Drapeau bleu ![](assets/flag-blue-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_blue.gif` |
| Drapeau vert ![](assets/flag-green-large.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_green.gif` |
| Drapeau rouge ![](assets/flag-red-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_red.gif` |
| Drapeau jaune ![](assets/flag-yellow-style2.png) | =`/interface/images/v4_redux/icons/casebuilder/flag_yellow.gif` |
| Cercle noir ![](assets/dot-black.png) | =`/interface/images/v4_redux/icons/casebuilder/light_black.gif` |
| Cercle bleu ![](assets/dot-blue.png) | =`/interface/images/v4_redux/icons/casebuilder/light_blue.gif` |
| Cercle gris ![](assets/dot-gray.png) | =`/interface/images/v4_redux/icons/casebuilder/light_grey.gif` |
| Cercle vert ![](assets/dot-green.png) | =`/interface/images/v4_redux/icons/casebuilder/light_green.gif` |
| Cercle orange ![](assets/dot-orange.png) | =`/interface/images/v4_redux/icons/casebuilder/light_orange.gif` |
| Cercle rose ![](assets/dot-pink.png) | =`/interface/images/v4_redux/icons/casebuilder/light_pink.gif` |
| Cercle violet ![](assets/dot-purple.png) | =`/interface/images/v4_redux/icons/casebuilder/light_purple.gif` |
| Cercle rouge ![](assets/dot-red.png) | =`/interface/images/v4_redux/icons/casebuilder/light_red.gif` |
| Cercle blanc ![](assets/dot-white.png) | =`/interface/images/v4_redux/icons/casebuilder/light_white.gif` |
| Cercle jaune ![](assets/dot-yellow.png) | =`/interface/images/v4_redux/icons/casebuilder/light_yellow.gif` |

{style="table-layout:auto"}

### Formater une `valueexpression` sous conditions {#conditionally-format-a-valueexpression}

Pour afficher une valeur calculée dans une colonne, vous pouvez remplacer la ligne de code `valuefield` dans la colonne par une `valueexpression`. Une valeur calculée permet d’afficher une nouvelle valeur pour un objet sur la base du calcul entre deux champs existants sur ce même objet.

Pour plus d’informations sur le formatage de `valueexpression line`, voir [Vue d’ensemble de la syntaxe du mode Texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

Vous ne pouvez pas formater de manière conditionnelle une colonne qui contient une ligne de code `valueexpression`. Au lieu de cela, vous pouvez ajouter un champ personnalisé calculé à un formulaire personnalisé et l’associer aux objets que vous affichez dans le rapport. Vous pouvez ensuite formater de manière conditionnelle les colonnes affichant ce champ.

Pour plus d’informations sur les champs calculés personnalisés, voir [Ajouter des champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Ajouter une valeur d’agrégateur dans une colonne en mode Texte

Nous vous recommandons de créer d’abord la colonne dans l’interface du constructeur, d’y ajouter la valeur de l’agrégateur, puis de modifier la colonne en mode Texte.

Tenez compte des éléments suivants lorsque vous ajoutez des agrégateurs à une colonne en mode texte :

* Les valeurs de la colonne doivent avoir un format qui peut être résumé. Par exemple, elles doivent avoir l’un des formats suivants :

   * Nombre
   * Date
   * Devise

* Vous pouvez ajouter un agrégateur à une colonne qui affiche un calcul. La valeur agrégée s’affiche dans le regroupement de la vue ou du rapport. Pour plus d’informations, voir [Regroupement : afficher le résultat de l’agrégation de plusieurs valeurs calculées dans un regroupement](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
* Les lignes de code pour la définition de la colonne doivent être identiques aux lignes de code introduisant l’agrégateur et précédées par « agrégateur ». Par exemple, si vous avez une colonne dans laquelle vous affichez le nombre d’heures prévues d’un projet, le mode Texte des lignes principales de la colonne est le suivant :

```
  valuefield=workRequired
  valueformat=compound
```

Lorsque vous souhaitez agréger les valeurs de toutes les lignes dans le regroupement de la vue, vous pouvez ajouter le code suivant pour ajouter les valeurs de l’agrégateur :

`aggregator.valuefield=workRequired` (la ligne `aggregator.valuefield` doit être la même que la `valuefield` qui décrit la colonne)

`aggregator.valueformat=compound` (la ligne `aggregator.valueformat` doit avoir la même valeur que la `valueformat` qui décrit la colonne)

`aggregator.function=SUM` (il s’agit d’une ligne obligatoire qui indique comment vous souhaitez agréger la colonne. Dans ce cas, vous souhaitez ajouter toutes le nombre d’heures prévues individuelles en un seul nombre dans la ligne de regroupement).

`aggregator.displayformat=minutesAsHoursString` (parce que les heures sont stockées dans Workfront en minutes, nous voulons indiquer le `displayformat` pour les heures lorsqu’elles sont stockées en minutes).
