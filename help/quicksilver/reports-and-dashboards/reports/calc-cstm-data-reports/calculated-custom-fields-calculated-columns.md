---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Champs personnalisés calculés par rapport aux colonnes calculées
description: Pour aggréger plusieurs champs dans Adobe Workfront et afficher cette valeur agrégée dans un nouveau champ, vous pouvez créer un champ personnalisé calculé dans un formulaire personnalisé ou une colonne calculée dans une vue.
author: Jenny
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: ce986a912c2ee231b9dc2e1c7a3e9587b20aa0ba
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 90%

---

# Champs personnalisés calculés par rapport aux colonnes calculées

Pour aggréger plusieurs champs dans Adobe Workfront et afficher cette valeur agrégée dans un nouveau champ, vous pouvez créer les éléments suivants :

* Champ personnalisé calculé dans un formulaire personnalisé\
  Pour plus d’informations sur l’ajout d’un champ calculé personnalisé à un formulaire personnalisé, voir [Ajouter des champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Colonne calculée dans une vue\
  Pour plus d’informations sur l’utilisation des calculs dans une vue, voir la section [Utiliser le mode Texte dans les vues](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) dans l’article [Vue d’ensemble des utilisations courantes du mode Texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Bien que vous utilisiez le mode texte pour créer à la fois des champs calculés et des colonnes calculées, la syntaxe pour les créer diffère. Reportez-vous aux articles répertoriés ci-dessus pour savoir comment créer des champs calculés et des colonnes calculées. Pour plus d’informations sur les différentes syntaxes utilisées dans les expressions de données calculées, telles que les champs et colonnes personnalisés calculés, consultez la section [Syntaxe des champs personnalisés calculés par rapport aux colonnes personnalisées calculées](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) dans cet article.

Vous pouvez utiliser les mêmes calculs dans les deux champs calculés ainsi que dans une colonne calculée. Cependant, en fonction de l’objectif de ces calculs, vous pouvez envisager de créer l’un par rapport à l’autre.

## Syntaxe des champs personnalisés calculés par rapport aux colonnes personnalisées calculées

Bien que les fonctions que vous utilisez soient les mêmes, la syntaxe de création d’une expression dans un champ personnalisé calculé peut être différente de celle utilisée pour créer une colonne personnalisée calculée.

Par exemple :

* Dans un champ personnalisé, sur un formulaire personnalisé pour les tâches, vous utiliserez les éléments suivants pour générer le nom du projet parent de la tâche à laquelle le formulaire personnalisé est joint :

  `{project}.{name}`

* Dans une colonne personnalisée d’un rapport, vous pouvez utiliser les éléments suivants pour ajouter une colonne personnalisée Nom du projet à un rapport de tâche :

  `valuefield=project:name`

  Ou

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >La même syntaxe s’applique à tous les éléments de rapport en mode texte dans lesquels des expressions calculées sont utilisées : vues, filtres, regroupements et invites.

Les différences entre les deux syntaxes sont les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Champ personnalisé calculé</strong></td>
   <td><strong>Élément de rapport personnalisé calculé</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Utilisez le nom des champs tel qu’ils apparaissent dans l’interface de Workfront.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>exemple de nom de champ utilisé dans un champ personnalisé calculé : <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Utilisez le nom des objets ou des champs tel qu’ils apparaissent dans la base de données Workfront. Les noms des objets et des champs sont orthographiés en minuscules ou en majuscules s’il s’agit de noms composés. </p> <p>Pour un inventaire de tous les objets et champs Workfront tels qu’ils apparaissent dans la base de données, voir <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorateur d’API</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>exemple de nom de champ utilisé dans un élément de rapport personnalisé calculé : <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Placez les noms de champ entre parenthèses ou accolades.</td> 
   <td> <p>Ne placez pas les noms de champ entre crochets ou parenthèses lors de leur utilisation dans une ligne <code>valuefield </code>.</p> <p>Placez les noms de champ entre accolades lorsque vous les utilisez dans une ligne <code>valueexpression</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Séparer les champs par des points</td> 
   <td> <p>Séparez les champs par deux points lors de leur utilisation dans une ligne <code>valuefield</code>.</p> <p>Séparez les champs par des points lors de leur utilisation dans une ligne <code>valueexpression</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur la syntaxe que vous devez utiliser dans une colonne personnalisée calculée, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Quand utiliser des champs personnalisés calculés ?

* Lorsque vous souhaitez regrouper les résultats agrégés dans un rapport ou afficher ces informations dans un graphique.
* Lorsque vous souhaitez agréger les données au-delà de l’agrégation calculée dans le champ.
* Lorsque vous ne vous souciez pas de la rapidité des données, car celles-ci ne sont pas mises à jour et peuvent changer au fil du temps.

## Actions qui déclenchent la mise à jour d’un champ personnalisé calculé

* Sur la page principale d&#39;un objet, cliquez sur l&#39;icône Plus ![icône Plus](assets/more-icon.png), puis sur **Recalculer les expressions**

* La modification en masse de plusieurs objets lorsque l’option **Recalculer les expressions personnalisées** est activée.
* Modification en masse de plusieurs objets lorsque vous cliquez sur **Recalculer les expressions** dans le menu Plus d’une liste d’objets.
* La modification d’un formulaire personnalisé lorsque l’option **Mettre à jour les calculs précédents** est activée pour le champ personnalisé calculé.

Pour plus d’informations, voir [Modifier les informations dans les champs de formulaire personnalisés](/help/quicksilver/workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Quand utiliser les colonnes calculées dans une vue ?

* Lorsque vous souhaitez que les données en temps réel soient disponibles dans un rapport.

  Les vues calculées sont toujours actualisées, car le calcul est effectué lors de l’exécution du rapport ou de l’application de la vue.

* Lorsque vous n’avez pas l’intention d’effectuer des regroupements en fonction de résultats agrégés, ni d’utiliser ces informations dans un graphique.
* Lorsque vous ne prévoyez pas d’agréger les données au-delà de l’agrégation calculée dans la colonne (les données ne peuvent être agrégées qu’une seule fois).
* Lorsque vous souhaitez que le calcul inclue une référence à la date actuelle à l’aide des caractères génériques $$TODAY ou $$NOW.

  >[!TIP]
  >
  >N’utilisez pas cette référence dans les champs personnalisés calculés, car ils ne sont recalculés que lorsque l’objet joint est modifié. Ces types de calculs deviennent obsolètes.

## Exemples de champs et de colonnes personnalisés calculés

Pour obtenir des exemples de champs personnalisés calculés, consultez [Données personnalisées calculées dans les rapports](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Pour obtenir des exemples de colonnes personnalisées calculées dans les vues, consultez les articles suivants :

* [Vue d’ensemble des utilisations courantes du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Exemples de vues, de filtres et de regroupements personnalisés : index des articles](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
