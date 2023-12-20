---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Champs personnalisés calculés par rapport aux colonnes calculées
description: Pour regrouper plusieurs champs dans Adobe Workfront et afficher cette valeur agrégée dans un nouveau champ, vous pouvez créer un champ personnalisé calculé dans un formulaire personnalisé ou une colonne calculée dans une vue.
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# Champs personnalisés calculés par rapport aux colonnes calculées

Pour regrouper plusieurs champs dans Adobe Workfront et afficher cette valeur agrégée dans un nouveau champ, vous pouvez créer les éléments suivants :

* Un champ personnalisé calculé dans un formulaire personnalisé\
  Pour plus d’informations sur l’ajout d’un champ personnalisé calculé à un formulaire personnalisé, consultez la section [Ajouter un champ calculé à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#add-a-calculated-field-to-a-custom-form) dans l’article [Ajout de données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Une colonne calculée dans une vue\
  Pour plus d’informations sur l’utilisation des calculs dans une vue, voir la section [Utilisation du mode Texte dans les vues](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) dans l’article [Présentation des utilisations courantes du mode Texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Bien que vous utilisiez le mode texte pour créer à la fois des champs calculés et des colonnes calculées, la syntaxe pour les créer diffère. Reportez-vous aux articles répertoriés ci-dessus pour savoir comment créer des champs calculés et des colonnes calculées. Pour plus d’informations sur les différentes syntaxes utilisées dans les expressions de données calculées, telles que les champs et colonnes personnalisés calculés, consultez la section [Syntaxe des champs personnalisés calculés par rapport aux colonnes personnalisées calculées](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) dans cet article.

Vous pouvez utiliser les mêmes calculs dans les deux champs calculés ainsi que dans une colonne calculée. Cependant, en fonction de l’objectif de ces calculs, vous pouvez envisager de créer l’un par rapport à l’autre.

## Syntaxe des champs personnalisés calculés par rapport aux colonnes personnalisées calculées

Bien que les fonctions que vous utilisez soient les mêmes, la syntaxe de création d’une expression dans un champ personnalisé calculé peut être différente de celle utilisée pour créer une colonne personnalisée calculée.

Par exemple :

* Dans un champ personnalisé, sur un formulaire personnalisé pour les tâches, vous utiliserez les éléments suivants pour générer le nom du projet parent de la tâche à laquelle le formulaire personnalisé est joint :

  `{project}.{name}`

* Dans une colonne personnalisée d’un rapport, vous pouvez utiliser les éléments suivants pour ajouter une colonne personnalisée Nom du projet à un rapport de tâche :

  `valuefield=project:name`

  Ou

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >La même syntaxe s’applique à tous les éléments de rapport en mode texte dans lesquels des expressions calculées sont utilisées : vues, filtres, regroupements et invites.

Les différences entre les deux syntaxes sont les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Champ personnalisé calculé</strong></td>
   <td><strong>Elément de rapport personnalisé calculé</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Utilisez le nom des champs tel qu’ils apparaissent dans l’interface de Workfront.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Exemple de nom de champ utilisé dans un champ personnalisé calculé : <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Utilisez le nom des objets ou des champs tel qu’ils apparaissent dans la base de données Workfront. Les noms des objets et des champs sont orthographiés en minuscules ou en majuscules s’il s’agit de noms composés. </p> <p>Pour un inventaire de tous les objets et champs Workfront tels qu’ils apparaissent dans la base de données, voir <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorateur d’API</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>Exemple de nom de champ utilisé dans un élément de rapport personnalisé calculé : <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Placez les noms de champ entre parenthèses ou accolades.</td> 
   <td> <p>Ne placez pas les noms de champ entre crochets ou parenthèses lors de leur utilisation dans une <code>valuefield </code>ligne.</p> <p>Placez les noms de champ entre accolades lorsque vous les utilisez dans une balise <code>valueexpression</code> ligne.</p> </td> 
  </tr> 
  <tr> 
   <td>Séparez les champs par des points</td> 
   <td> <p>Séparez les champs par deux-points lors de leur utilisation dans un <code>valuefield</code>ligne.</p> <p>Séparez les champs par des points lors de leur utilisation dans une <code>valueexpression</code>ligne.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur la syntaxe que vous devez utiliser dans une colonne personnalisée calculée, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Quand utiliser des champs personnalisés calculés

* Lorsque vous souhaitez regrouper les résultats agrégés dans un rapport ou afficher ces informations dans un graphique
* Lorsque vous souhaitez agréger les données au-delà de l’agrégation calculée dans le champ.
* Lorsque vous n’êtes pas préoccupé par la rapidité des données, car celles-ci ne sont pas mises à jour et peuvent changer au fil du temps.

## Actions qui déclenchent la mise à jour d’un champ personnalisé calculé

* Sur la page principale d’un objet, cliquez sur l’icône Plus ![](assets/more-icon.png), puis cliquez sur **Recalculer les expressions**

* Modification en masse de plusieurs objets lors de **Recalculer des expressions personnalisées** est activé
* Modification d’un formulaire personnalisé **Mise à jour des calculs précédents** est activé pour le champ personnalisé calculé

## Quand utiliser les colonnes calculées dans une vue

* Lorsque vous souhaitez que les données en temps réel soient disponibles sur un rapport.

  Les vues calculées sont toujours actualisées, car le calcul est effectué lors de l’exécution du rapport ou de l’application de la vue.

* Lorsque vous n’avez pas l’intention de regrouper en fonction de résultats agrégés, ni d’utiliser ces informations dans un graphique.
* Lorsque vous ne prévoyez pas d’agréger les données au-delà de l’agrégation calculée dans la colonne (les données ne peuvent être agrégées qu’une seule fois).
* Lorsque vous souhaitez que le calcul inclue une référence à la date actuelle à l’aide des caractères génériques $$TODAY ou $$NOW .

  >[!TIP]
  >
  >N’utilisez pas cette référence dans les champs personnalisés calculés, car ils ne recalculent que lorsque l’objet joint est modifié. Ces types de calculs deviennent obsolètes.

## Exemples de champs et de colonnes personnalisés calculés

Pour obtenir des exemples de champs personnalisés calculés, voir [Données personnalisées calculées dans les rapports](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Pour des exemples de colonnes personnalisées calculées dans les vues, consultez les articles suivants :

* [Présentation des utilisations courantes du mode Texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Exemples de filtrage, de filtrage et de regroupement personnalisés : index de l&#39;article](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
