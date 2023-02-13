---
product-area: reporting
navigation-topic: text-mode-reporting
title: Présentation de la syntaxe du mode texte
description: Vous pouvez utiliser l’interface du mode texte pour créer des vues, des filtres, des regroupements et des invites plus complexes dans des listes et des rapports. En mode texte, vous pouvez accéder aux champs et à leurs attributs qui ne sont pas disponibles dans l’interface de mode standard.
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1498'
ht-degree: 0%

---

# Présentation de la syntaxe du mode texte

Vous pouvez utiliser l’interface du mode texte pour créer des vues, des filtres, des regroupements et des invites plus complexes dans des listes et des rapports. En mode texte, vous pouvez accéder aux champs et à leurs attributs qui ne sont pas disponibles dans l’interface de mode standard.

Pour plus d’informations et de considérations sur le mode de texte avant de commencer, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Pour obtenir la liste complète de tous nos champs à déclarer et de leurs attributs, voir la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

## Considérations sur la syntaxe du mode texte

* Vous devez comprendre la syntaxe Adobe Workfront avant de pouvoir commencer à créer des éléments de reporting en mode texte. La syntaxe Workfront pour le mode texte est propre à cette application et possède des caractéristiques uniques que vous devez connaître.
* Avant de commencer à utiliser le mode texte dans vos rapports, nous vous recommandons vivement de suivre nos cours sur les rapports avancés, afin de mieux comprendre notre langage de mode texte. Pour obtenir des documents de formation sur les rapports, voir [Chemins d’apprentissage des rapports et tableaux de bord Workfront](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).
* Vous pouvez personnaliser les vues, les filtres et les regroupements à l’aide de l’interface de mode standard. Cependant, vous ne pouvez créer des invites personnalisées qu’en mode texte.

## Directives courantes pour la création d’éléments de rapport en mode texte

Voici des instructions courantes lorsque vous créez un élément de rapport ou de liste en mode texte :

* Utilisez toujours la casse chameau lorsque vous référencez des objets ou des attributs dans la base de données Workfront.
* Gardez à l’esprit la hiérarchie des objets dans Workfront. Les différences suivantes existent entre les vues, les filtres et les regroupements :

   * Vous pouvez afficher dans une vue un objet qui se trouve à trois objets du rapport ou de l’objet de liste.
   * Vous ne pouvez pas référencer des objets situés à plus de 2 objets de l’objet principal dans une invite de regroupement, de filtrage ou personnalisée.

   **Exemple :** Vous pouvez afficher le nom ou le GUID du propriétaire du Portfolio dans une vue de tâche :

   ```
   valuefield=project:portfolio:ownerID
   ```

   Vous ne pouvez pas regrouper, filtrer ou inviter le propriétaire du Portfolio dans une vue de tâche :

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   Dans ces exemples, l’ID de propriétaire de Portfolio se trouve à trois objets de l’objet de la liste.

   Pour plus d’informations sur la hiérarchie des objets dans Workfront, voir :

   * [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [Explorateur d’API](../../../wf-api/general/api-explorer.md)


* Lorsque cela est possible, utilisez des caractères génériques pour rendre vos rapports et listes plus dynamiques et évitez de les dupliquer pour différents utilisateurs et chronologies similaires.

## Présentation de la casse Camel

Lorsque vous référencez des champs Workfront ou leurs attributs en mode texte, Workfront vous demande de saisir leurs noms en majuscules. Dans ce cas, les champs à nom unique sont orthographiés en minuscules. Les champs composés sont orthographiés selon le modèle suivant :

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>Tous les éléments de création de rapports suivent ce modèle de casse.

Les caractéristiques de la casse des chameaux sont les suivantes :

* Le premier mot commence toujours par une lettre minuscule.
* Les mots suivants commencent toujours par une lettre majuscule.
* Il n&#39;y a pas d&#39;espace entre les mots.

**Exemple :** Pour référencer la date d’achèvement réelle d’un projet, le nom du champ que vous utiliseriez lors de la création d’éléments de rapport en mode texte est :

```
actualCompletionDate
```

.

## Syntaxe du mode texte pour divers éléments de reporting

Les similitudes suivantes existent entre la syntaxe des ensembles d’éléments de reporting ci-dessous, lors de leur création en mode texte :

* Les lignes de code et de syntaxe sont similaires pour les vues et les regroupements.

   Pour plus d’informations sur les lignes clés de codes pour les vues et les regroupements lors de leur création en mode texte, voir :

   * [Modification d’une vue en mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [Mode d’édition de texte dans un groupement](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* Les lignes de code et de syntaxe sont similaires pour les filtres et les invites personnalisées.

   Pour plus d’informations, voir :

   * [Modification d’un filtre à l’aide du mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [Ajout d’une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### Syntaxe des vues et des regroupements

Vous remarquerez peut-être que les lignes de code lors de la création de vues et de regroupements sont similaires.

Pour plus d’informations sur la création de vues et de regroupements, consultez les articles suivants :

* [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

La ligne de code la plus importante pour une vue ou un regroupement est la ligne qui identifie l’objet référencé dans la colonne de la vue ou le regroupement. Selon que ce champ est une référence directe à un champ de la base de données Workfront ou un calcul entre plusieurs champs, la ligne de code peut commencer par

```
valuefield
```

ou

```
valueexpression
```

.

* [Présentation de la syntaxe des champs de valeur pour les vues et les regroupements](#valuefield-syntax-overview-for-views-and-groupings)
* [Présentation de la syntaxe des expressions de valeur pour les vues et les regroupements](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* Bien que les lignes de code dans les exemples ci-dessous soient similaires entre les vues et les regroupements, n’oubliez pas que chaque ligne de code pour un regroupement commence par le numéro de regroupement.
>
>  Pour regrouper par nom de projet dans une liste de projets ou un rapport, utilisez la ligne suivante pour le groupement de premier niveau :
>
>  
```>
>  group.0.valuefield=name
>  ```>
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  
Use the following format to identify the first column of a view: 
>
>  
```>
>  column.0.valuefield=name
>  ```>
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>



```
Valuefield
```

présentation de la syntaxe pour les vues et les regroupements {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

est une ligne de code clé dans les vues et les regroupements qui identifie l’objet que vous référencez directement.

La syntaxe des champs de référencement direct est identique pour les regroupements et les vues.

Les règles suivantes s’appliquent lorsque vous référencez des objets Workfront à l’aide d’un

```
valuefield
```

line :

* Utilisez la casse chameau pour référencer directement les champs.

   **Exemple :** Pour référencer la date d’achèvement de la tâche dans une vue de tâche, utilisez la ligne suivante :

   ```
   valuefield=actualCompletionDate
   ```

* Utilisez des majuscules et des deux-points pour séparer les champs les uns liés aux autres pour le même objet.

   **Exemple :** Pour référencer la date d’achèvement prévue du projet dans une vue de tâche, utilisez la ligne suivante :

   ```
   valuefield=project:plannedCompletionDate
   ```

   Pour plus d’informations sur la façon dont les objets se référencent dans la base de données Workfront, voir la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

* Lorsque vous référencez un champ personnalisé, utilisez le nom du champ tel qu’il apparaît dans l’interface.

   **Exemple :** Pour référencer un champ personnalisé de projet intitulé Détails supplémentaires dans un affichage de tâche, utilisez la ligne suivante :

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

présentation de la syntaxe pour les vues et les regroupements {#valueexpression-syntax-overview-for-views-and-groupings}

Vous pouvez remplacer la variable

```
valuefield=
```

ligne de code avec

```
valueexpression=
```

lors de la création de vues et de groupements en mode texte lorsque vous souhaitez référencer un calcul entre deux champs ou plus.

>[!TIP]
>
>Bien que vous puissiez créer des champs calculés que vous pouvez afficher dans les rapports, les vues et les regroupements calculés sont plus dynamiques. Les vues calculées et les regroupements s’actualisent avec de nouvelles informations chaque fois que vous exécutez le rapport ou affichez une liste.
>
>Pour plus d’informations sur la création de colonnes calculées dans une vue, voir [Champs personnalisés calculés par rapport aux colonnes calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

La création d&#39;un groupement calculé est similaire à la création d&#39;une colonne calculée dans une vue.

Les règles suivantes s’appliquent lorsque vous référencez des objets Workfront à l’aide d’un

```
valueexpression
```

line :

* Utilisez la casse chameau pour référencer directement les champs et placez chaque champ entre accolades.

   **Exemple :** Pour afficher le champ Nom de la tâche dans une colonne de tâche à l’aide de

   ```
   valueexpression
   ```

   , utilisez la ligne suivante :

   ```
   valueexpression={name}
   ```

* Utilisez la casse chameau et les points pour séparer les champs les uns liés aux autres.

   **Exemple :** Pour afficher le nom d&#39;un projet concaténé avec le nom de la tâche dans un rapport de tâche, utilisez les lignes suivantes :

   * Dans une vue :

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * Dans un groupement :

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   Pour plus d’informations sur la façon dont les objets se référencent dans la base de données Workfront, voir la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

* Lors du référencement d’un champ personnalisé, utilisez les règles suivantes :

   * Utilisez le nom du champ tel qu’il apparaît dans l’interface.
   * Précisez le nom du champ avec &quot;DE:&quot;.
   * Placez le champ entre accolades.
   * Séparez les champs associés à l’objet par des points.

   **Exemple :** Pour afficher le champ personnalisé du projet Détails supplémentaires dans une vue de tâche dans une ligne d’expression de valeur, utilisez la ligne suivante :

   ```
   valueexpression={project}.{DE:Additional Details}
   ```

* Vous pouvez utiliser un caractère générique dans une variable

   ```
   valueexpression
   ```

   mais pas dans un

   ```
   valuefield
   ```

   ligne.

   Pour plus d’informations sur les caractères génériques, voir [Variables de filtre génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

```
Valueformat
```

aperçu

La deuxième ligne de code la plus importante dans une vue ou un regroupement est la suivante :

```
valueformat=
```

ligne. Cela indique à Workfront dans quel format renvoyer la valeur que vous spécifiez dans la variable

```
valuefield
```

ou des lignes d’expression de valeur. Bien que vous puissiez utiliser différents formats pour le

```
valueformat
```

lignes, nous vous recommandons de toujours utiliser la valeur suivante lors de l’utilisation de

```
valueexpression
```

:

```
valueformat=HTML
```

### Syntaxe des filtres et des invites personnalisées

La syntaxe de création de filtres est similaire à celle de création d’invites personnalisées.

>[!TIP]
>
>Vous pouvez créer une invite personnalisée en créant d’abord un filtre pour l’instruction que vous souhaitez inclure dans l’invite. Connectez toutes les lignes de code d’un filtre de &quot;&amp;&quot; sans espaces entre les lignes et qui devient votre invite personnalisée.

Pour plus d’informations sur la création de filtres et d’invites personnalisées, voir :

* [Présentation des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Ajout d’une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

Pour plus d’informations sur la création de filtres en mode texte, voir [Modification d’un filtre à l’aide du mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

Vous pouvez utiliser les éléments suivants pour créer des filtres et des invites personnalisés en mode texte :

* Ligne de code référençant l’objet de l’instruction de filtre. Utilisez la casse chameau pour l’objet de filtre.
* Ligne de code faisant référence à l’objet de filtre et au modificateur correspondant à la valeur de l’objet de filtre. Utilisez la casse chameau pour l’objet de filtre de cette ligne.

   >[!TIP]
   >
   >Lorsque vous référencez des plages, deux lignes de modificateur sont nécessaires.

* Un connecteur d’instructions qui connecte plusieurs instructions de filtre :

   * ET

      Il s’agit du connecteur par défaut entre les instructions de filtre.

   * OU

      >[!TIP]
      >
      >Les connecteurs d’instructions sont sensibles à la casse et toujours en majuscules. &quot;AND&quot; peut être omis en mode texte.

* Caractères génériques pour rendre les filtres plus dynamiques et les personnaliser pour l’heure actuelle ou pour l’utilisateur connecté. Pour plus d’informations sur les caractères génériques, voir [Variables de filtre génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
