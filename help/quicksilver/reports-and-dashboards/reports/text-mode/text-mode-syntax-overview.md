---
product-area: reporting
navigation-topic: text-mode-reporting
title: Vue d’ensemble de la syntaxe du mode texte
description: Vous pouvez utiliser l’interface en mode texte pour créer des vues, des filtres, des regroupements et des invites personnalisées plus complexes dans les listes et les rapports. En utilisant le mode texte, vous pouvez accéder à des champs et à leurs attributs qui ne sont pas disponibles dans l’interface du mode standard.
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 98%

---

# Vue d’ensemble de la syntaxe du mode texte

<!--Audited: 1/2025-->

Vous pouvez utiliser l’interface en mode texte pour créer des vues, des filtres, des regroupements et des invites personnalisées plus complexes dans les listes et les rapports. En utilisant le mode texte, vous pouvez accéder à des champs et à leurs attributs qui ne sont pas disponibles dans l’interface du mode standard.

Pour obtenir des informations et des observations sur le mode texte avant de commencer, voir la section [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Pour obtenir une liste complète de tous nos champs pouvant faire l’objet d’un rapport et de leurs attributs, voir la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

Pour plus d’informations sur la création de rapports en mode texte, y compris des cours, des vidéos et des tutoriels, consultez la section Formation du site Adobe Experience League.

## Observations sur la syntaxe du mode texte

* Vous devez comprendre la syntaxe d’Adobe Workfront avant de commencer à créer des éléments de rapport en mode texte. La syntaxe Workfront en mode texte est propre à cette application et possède des caractéristiques uniques avec lesquelles vous devez vous familiariser.
* Avant de commencer à utiliser le mode texte dans vos rapports, nous vous recommandons vivement de suivre nos cours sur les rapports avancés, afin de mieux comprendre notre langage en mode texte.
* Vous pouvez personnaliser les vues, les filtres et les regroupements à l’aide de l’interface du mode standard. Cependant, vous ne pouvez créer des invites personnalisées qu’en mode texte.

## Lignes directrices communes pour l’élaboration d’éléments de rapport en mode texte

Les lignes directrices suivantes s’appliquent à la construction de tout élément de rapport ou de liste en mode texte :

* Utilisez toujours le format « camel case » lorsque vous faites référence à des objets ou à des attributs dans la base de données Workfront.
* Tenez compte de la hiérarchie des objets dans Workfront. Les différences suivantes existent entre les vues, les filtres et les regroupements :

   * Vous pouvez afficher un objet qui se trouve à trois objets du rapport ou de l’objet de liste dans une vue.
   * Vous ne pouvez pas faire référence à des objets situés à plus de deux objets de l’objet principal dans un regroupement, un filtre ou une invite personnalisée.

  **Exemple :** vous pouvez afficher le nom ou le GUID de la personne propriétaire du portfolio dans une vue de tâche :

  `valuefield=project:portfolio:ownerID`

  Vous ne pouvez pas grouper, filtrer ou demander la personne propriétaire du portfolio dans une vue de tâche :

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`

  Dans ces exemples, l’identifiant de la personne propriétaire du portfolio se trouve à trois objets de l’objet de la liste.

  Pour plus d’informations sur la hiérarchie des objets dans Workfront, voir la section suivante :

   * [Comprendre les objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [Explorateur d’API](../../../wf-api/general/api-explorer.md)

* Utilisez des caractères génériques autant que possible pour rendre vos rapports et vos listes plus dynamiques et éviter de les dupliquer pour différentes personnes et des délais similaires.

## Vue d’ensemble du camel case

Lorsque vous faites référence à des champs Workfront ou à leurs attributs en mode texte, Workfront vous demande de taper leur nom en camel case. Dans ce cas, les champs à nom unique sont écrits en minuscules. Les champs composés sont orthographiés selon le modèle suivant :

`camelCaseSyntax`

>[!IMPORTANT]
>
>Tous les éléments du rapport suivent cette casse.

Les caractéristiques du camel case sont les suivantes :

* Le premier mot commence toujours par une minuscule.
* Les mots suivants commencent toujours par une majuscule.
* Il n’y a pas d’espace entre les mots.

**Exemple :** pour référencer la date d’achèvement réelle d’un projet, le nom du champ à utiliser lors de la création d’un élément de rapport en mode texte est le suivant :

`actualCompletionDate`

## Syntaxe en mode texte pour divers éléments de rapport

Les similitudes suivantes existent entre la syntaxe des ensembles d’éléments de rapport ci-dessous, lorsqu’ils sont créés en mode texte :

* Les lignes de code et la syntaxe sont similaires pour les vues et les regroupements.

  Pour plus d’informations sur les lignes de code clés des vues et des regroupements lors de leur création en mode texte, voir la section :

   * [Modifier une vue en mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Modification d’un regroupement à l’aide du mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Les lignes de code et la syntaxe sont similaires pour les filtres et les invites personnalisées.

  Pour plus d’informations, voir :

   * [Modifier un filtre en mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Syntaxe pour les vues et les regroupements

Les lignes de code lors de la création des vues et des regroupements sont similaires.

Pour plus d’informations sur la création de vues et de regroupements, voir les articles suivants :

* [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

La ligne de code la plus importante pour une vue ou un regroupement est celle qui identifie l’objet référencé dans la colonne de la vue ou dans le regroupement. Cette ligne de code peut commencer par `valuefield` ou par `valueexpression` selon que ce champ fait directement référence à un champ de la base de données Workfront ou qu’il s’agit d’un calcul entre plusieurs champs.

Le tableau suivant répertorie les lignes de codes les plus courantes dans une vue ou un regroupement :

| Ligne de code | Description |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | Identifie l’objet référencé dans la colonne de la vue ou dans le regroupement. Il s’agit d’une référence directe à l’objet référencé. |
| `valueexpression` | Identifie l’objet référencé dans la colonne de la vue ou dans le regroupement. Il s’agit d’un calcul entre plusieurs champs. |
| `valueformat` | Identifie le format dans lequel Workfront renvoie la valeur spécifiée dans les lignes valuefield ou valueexpression. |
| `width` | Identifie la largeur d’une colonne en pixels. |
| `stretch` | Identifie les colonnes qui occupent un espace supplémentaire dont la vue n’a pas besoin. |

>[!TIP]
>
>* Bien que les lignes de code dans les exemples ci-dessous soient similaires entre les vues et les regroupements, n’oubliez jamais que chaque ligne de code pour un regroupement commence par le numéro du regroupement.
>
>  Pour effectuer un regroupement par nom de projet dans une liste de projets ou un rapport, utilisez la ligne suivante pour le regroupement de premier niveau :
>
>  `group.0.valuefield=name`
>  
>* Si vous modifiez plusieurs colonnes d’une vue dans la même colonne (comme dans le cas des colonnes partagées), rappelez-vous que chaque ligne de code de chaque colonne commence par le numéro de la colonne.
>
>  Utilisez le format suivant pour identifier la première colonne d’une vue :
>
>  `column.0.valuefield=name`
>  
>  Pour plus d’informations sur le partage de colonnes, voir la section [Vue : fusionner des informations provenant de plusieurs colonnes dans une colonne partagée](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### Vue d’ensemble de la syntaxe de `Valuefield` pour les vues et les regroupements

`Valuefield=` est une ligne de code clé dans les vues et les regroupements qui identifie l’objet auquel vous faites directement référence.

La syntaxe de référencement direct des champs est identique pour les regroupements et les vues.

Les règles suivantes s’appliquent au référencement des objets Workfront à l’aide d’une ligne `valuefield` :

* Utilisez la casse « camel case » pour faire directement référence à des champs.

  **Exemple :** pour référencer la date d’achèvement réelle de la tâche dans une vue de tâche, utilisez la ligne suivante :

  `valuefield=actualCompletionDate`

* Utilisez le camel case et les deux-points pour séparer les champs liés les uns aux autres pour le même objet.

  **Exemple :** pour faire référence à la date d’achèvement prévue du projet dans une vue de tâche, utilisez la ligne suivante :

  `valuefield=project:plannedCompletionDate`

  Pour plus d’informations sur la manière dont les objets font référence les uns aux autres dans la base de données Workfront, voir l’[explorateur d’API](../../../wf-api/general/api-explorer.md).

* Lorsque vous faites référence à un champ personnalisé, utilisez le nom du champ, tel qu’il apparaît dans l’interface.

  **Exemple :** pour référencer un champ personnalisé de projet intitulé Détails supplémentaires dans une vue de tâche, utilisez la ligne suivante :

  `valuefield=project:Additional Details`

#### Vue d’ensemble de la syntaxe de `Valueexpression` pour les vues et les regroupements

Vous pouvez remplacer la ligne de code `valuefield=` par `valueexpression=` lorsque vous construisez des vues et des regroupements en mode texte et que vous souhaitez référencer un calcul entre deux champs ou plus.

>[!TIP]
>
>Même s’il est possible de créer des champs calculés que vous pouvez afficher dans des rapports, les vues et les regroupements calculés sont plus dynamiques. Les vues et les regroupements calculés sont actualisés avec de nouvelles informations à chaque fois que vous exécutez le rapport ou que vous affichez une liste.
>
>Pour plus d’informations sur la création de colonnes calculées dans une vue, voir l’article [Champs personnalisés calculés et colonnes calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

La création d’un regroupement calculé est similaire à la création d’une colonne calculée dans une vue.

Les règles suivantes s’appliquent au référencement des objets Workfront à l’aide d’une ligne `valueexpression` :

* Utilisez le camel case pour référencer directement les champs et mettez chaque champ entre accolades.

  **Exemple :** pour afficher le champ Nom de la tâche dans une colonne de tâche à l’aide de `valueexpression`, utilisez la ligne suivante :

  `valueexpression={name}`


* Utilisez le camel case et des points pour séparer les champs liés les uns aux autres.

  **Exemple :** pour afficher le nom d’un projet concaténé avec le nom de la tâche dans un rapport de tâche, utilisez les lignes suivantes :

   * Dans une vue :

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * Dans un regroupement :

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Pour plus d’informations sur la manière dont les objets se référencent entre eux dans la base de données Workfront, consultez l’[explorateur d’API](../../../wf-api/general/api-explorer.md).

* Lorsque vous référencez un champ personnalisé, utilisez les règles suivantes :

   * Utilisez le nom du champ exactement tel qu’il apparaît dans l’interface.
   * Faites précéder le nom du champ par « DE: ».
   * Placez le champ entre accolades.
   * Séparez les champs relatifs à l’objet par des points.

  **Exemple :** pour afficher le champ personnalisé Détails supplémentaires du projet dans une vue de tâche dans une ligne valueexpression, utilisez la ligne suivante :

  `valueexpression={project}.{DE:Additional Details}`

* Vous pouvez utiliser un caractère générique dans une ligne `valueexpression` mais pas dans une ligne `valuefield`.

  Pour plus d’informations sur les caractères génériques, consultez la section [Vue d’ensemble des variables de filtrage des caractères génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### Vue d’ensemble de `Valueformat` pour les vues et les regroupements

La deuxième ligne de code la plus importante dans une vue ou un regroupement est la ligne `valueformat=`. Cette ligne indique à Workfront le format dans lequel il doit renvoyer la valeur que vous avez spécifiée dans les lignes `valuefield` ou `valueexpression`. Bien que vous puissiez utiliser différents formats pour les lignes `valueformat`, nous vous recommandons de toujours utiliser la valeur suivante pour les lignes `valueexpression` :

`valueformat=HTML`

Pour d’autres valeurs de `valueformat`, consultez également les articles suivants :

* [Mettre en forme des dates dans les rapports en mode texte](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [Mettre en forme des nombres, des devises et des pourcentages dans les rapports en mode texte](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### Vue d’ensemble de `width` pour les vues

`width=` est la ligne de code où vous pouvez spécifier la largeur de chaque colonne en pixels. Workfront fournit une largeur suggérée pour chaque champ. Cependant, selon le type de champ et le format, vous pouvez effectuer des ajustements.

Vous devez utiliser la ligne de code supplémentaire `usewidths=true` pour faire respecter la largeur spécifiée pour la colonne.

**Exemple :** pour afficher une colonne d’une largeur de 80 pixels, utilisez les lignes suivantes :

`width=80`

`usewidths=true`

#### Vue d’ensemble de `stretch` pour les vues

La ligne `stretch` est utilisée pour identifier les colonnes qui occupent un espace supplémentaire dont la vue n’a pas besoin. La largeur de l’interface utilisateur de l’espace de travail pour un utilisateur ou ue utilisatrice type est d’environ 850 pixels. Cela signifie que si vous avez une vue dotée de quatre colonnes (150 pixels chacune), votre vue occupe 600 des 850 pixels. Il y a 250 pixels supplémentaires dans l’interface utilisateur qui seront ajoutés aux colonnes pour lesquelles un pourcentage d’extension a été fourni.

L’étirement d’une colonne est appliqué lorsque vous utilisez la ligne de code supplémentaire `usewidths=true` pour au moins une des colonnes de la vue.

**Exemple :** pour indiquer qu’une colonne peut utiliser 70 % de l’espace vide d’une vue, utilisez les lignes suivantes :

`stretch=70`

`usewidths=true`

### Syntaxe des filtres et des invites personnalisées

La syntaxe de création des filtres est similaire à celle de la création d’invites personnalisées.

>[!TIP]
>
>Vous pouvez créer une invite personnalisée en commençant par créer un filtre pour l’instruction que vous souhaitez inclure dans l’invite. Reliez toutes les lignes de code dans un filtre par « &amp; », sans espace entre les lignes, et vous obtiendrez votre invite personnalisée.

Pour plus d’informations sur la création de filtres et d’invites personnalisées, consultez la section :

* [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Pour plus d’informations sur la création de filtres en mode texte, consultez la section [Modifier un filtre en mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Vous pouvez utiliser les éléments suivants pour créer des filtres et des invites personnalisées en mode texte :

* Ligne de code faisant référence à l’objet de l’instruction de filtrage. Utilisez le camel case pour l’objet filter.
* Une ligne de code faisant référence à l’objet filter et au modificateur de la valeur de ce dernier. Utilisez des majuscules pour l’objet filter dans cette ligne.

  >[!TIP]
  >
  >Lorsqu’il s’agit de faire référence à des périodes, deux lignes de modification sont nécessaires.

* Un connecteur d’instruction qui relie plusieurs instructions de filtre :

   * ET

     Il s’agit du connecteur par défaut entre les instructions de filtre.

   * OU

     >[!TIP]
     >
     >Les connecteurs d’instruction sont sensibles à la casse et toujours écrits en majuscules. Le connecteur « AND » peut être omis en mode texte.

* Des caractères génériques pour rendre les filtres plus dynamiques et les personnaliser en fonction de l’heure actuelle ou de la personne connectée. Pour plus d’informations sur les caractères génériques, consultez la section [Vue d’ensemble des variables de filtrage des caractères génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
