---
product-area: reporting
navigation-topic: text-mode-reporting
title: Vue d’ensemble des utilisations courantes du mode texte
description: Vue d’ensemble des utilisations courantes du mode texte
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 92%

---

# Vue d’ensemble des utilisations courantes du mode texte

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

Vous pouvez développer vos capacités de création de rapports à l’aide du mode texte dans les rapports et les éléments de rapport. Vous pouvez également utiliser une version du mode texte pour créer des champs personnalisés calculés plus complexes. Pour plus d’informations sur le mode texte, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Cet article présente quelques exemples courants d’utilisation du mode texte pour développer les capacités de création de rapports ou de champs personnalisés calculés dans Adobe Workfront. Pour obtenir une liste plus exhaustive d’exemples, voir ce qui suit :

* [Exemples de vue, de filtre et de regroupement personnalisés : index des articles](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [Données personnalisées calculées dans les rapports](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

Pour plus d’informations sur la création de rapports en mode texte, notamment les classes, vidéos et tutoriels, consultez la section « Formation » du site Adobe Experience League.

## Instances dans lesquelles vous pouvez utiliser le mode texte dans les listes et les rapports.

Nous vous recommandons d’utiliser le créateur de rapports et de listes pour créer vos vues, filtres et regroupements. Cependant, dans certains cas, vous pouvez utiliser le mode texte pour améliorer vos rapports et listes.

Vous pouvez utiliser le mode texte lorsque vous souhaitez obtenir les résultats suivants dans Workfront :

* Créez des champs personnalisés calculés dans un formulaire personnalisé.\
  Pour plus d’informations sur les champs personnalisés calculés, voir [Utiliser le mode texte dans les champs personnalisés calculés](#use-text-mode-in-calculated-custom-fields) dans cet article.
* Améliorez les filtres, les vues et les regroupements au-delà de ce qui est possible dans le Report Builder. Pour plus d’informations sur l’utilisation du mode texte pour les filtres, les vues et les regroupements, reportez-vous aux sections suivantes de cet article :

   * [Utiliser le mode texte dans les vues](#use-text-mode-in-views)
   * [Utiliser le mode texte dans les filtres](#use-text-mode-in-filters)
   * [Utiliser le mode texte dans les regroupements](#use-text-mode-in-groupings)

* Créez des invites personnalisées. Vous ne pouvez créer des invites personnalisées qu&#39;en mode texte.

  Pour plus d’informations sur la création d’invites personnalisées, voir [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Utiliser le mode texte dans les champs personnalisés calculés {#use-text-mode-in-calculated-custom-fields}

Vous pouvez utiliser le mode texte pour ajouter un champ personnalisé calculé à un formulaire personnalisé.

Pour plus d’informations sur l’ajout d’un champ personnalisé calculé à un formulaire personnalisé, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Pour plus d’informations sur la création d’un champ personnalisé calculé en mode texte, voir [&#x200B; Ajouter des champs calculés à un formulaire &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Par exemple, vous pouvez ajouter un champ personnalisé calculé qui affiche la date et l’heure du moment où un élément a été marqué comme En cours. Vous pouvez utiliser ce calcul pour d’autres statuts.

Pour plus d’informations, voir [Exemple de champ personnalisé calculé : afficher une date et heure de statut dans un formulaire personnalisé](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md).

## Utiliser le mode texte dans les vues {#use-text-mode-in-views}

Vous pouvez utiliser le mode texte dans les vues pour développer les champs et les objets que vous pouvez afficher dans la vue.

Pour obtenir des exemples des raisons les plus courantes d’utilisation du mode texte dans une vue, reportez-vous aux articles suivants :

* [Vue : afficher les objets non inclus dans l’interface standard](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [Vue : afficher le résultat d’un calcul entre deux champs d’une colonne](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)
* [Vue : modifier la largeur d’une colonne de manière définitive](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [Vue : fusionner les informations de plusieurs colonnes dans une seule colonne partagée](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [Vue : supprimer le lien vers un objet d’une colonne](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)
* [Référencer des collections dans un rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [Vue : masquer le contenu d’une colonne](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)
* [Vue : afficher une image au lieu d’une chaîne de caractères dans une colonne](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)
* [Vue : afficher les mises en retrait de tâches dans une liste de tâches](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [Vue : calculer les différences d’heure et de date](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## Utiliser le mode texte dans les filtres {#use-text-mode-in-filters}

Vous pouvez utiliser le mode texte lors de la création de filtres pour développer les champs et les objets en fonction desquels vous pouvez filtrer.

Pour obtenir des exemples des raisons les plus courantes d’utilisation le mode texte dans un filtre, reportez-vous aux articles suivants :

* [Filtre : créer plusieurs règles de filtrage qui référencent le même champ (instructions « AND »).](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [Filtre : afficher uniquement les éléments avec un statut d’approbation](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [Filtre : afficher les éléments par statut de même nom lorsque les statuts sont associés à des groupes différents](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [Filtre : éliminer des éléments d’une liste en comparant deux champs](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)
* La section [Exemples de filtres en mode texte s’étendant sur plusieurs niveaux dans la hiérarchie d’objets](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples) dans l’article [Créer des filtres en mode texte complexes à l’aide des instructions EXISTS](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)
* La section [Créer des filtres en mode texte complexes pour les objets manquants](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters) dans l’article [Créer des filtres en mode texte complexes à l’aide des instructions EXISTS](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)

## Utiliser le mode texte dans les regroupements {#use-text-mode-in-groupings}

Vous pouvez utiliser le mode texte lors de la création de regroupements pour développer les champs et les objets selon lesquels effectuer les regroupements dans les listes et les rapports.

Pour obtenir des exemples des raisons les plus courantes d’utilisation du mode texte dans un regroupement, reportez-vous aux articles suivants :

* [Regroupement : organiser les résultats d’une liste en fonction d’une valeur calculée commune à tous les objets du regroupement](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [Regroupement : ajouter un quatrième regroupement à une liste](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [Regroupement : modifier le nom d’affichage dans un regroupement](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [Regroupement : indiquer si les résultats d’un regroupement doivent être réduits ou développés en mode texte](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)
