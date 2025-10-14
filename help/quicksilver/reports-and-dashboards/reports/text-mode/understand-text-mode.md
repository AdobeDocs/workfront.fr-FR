---
product-area: reporting
navigation-topic: text-mode-reporting
title: Vue d’ensemble du mode texte
description: Vous pouvez créer un rapport ou une liste dans Adobe Workfront à l’aide de l’interface standard ou du mode texte lors de la création des éléments qui composent le rapport ou la liste.
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 86%

---

# Vue d’ensemble du mode texte

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

Vous pouvez créer un rapport ou une liste dans Adobe Workfront à l’aide de l’interface standard ou du mode texte lors de la création des éléments qui composent le rapport ou la liste.

L’interface standard vous permet de référencer des champs et leurs attributs qui sont facilement disponibles dans l’interface de Workfront.

En mode texte, vous pouvez référencer des champs et des attributs qui peuvent ne pas être disponibles en mode standard, mais qui sont disponibles dans la base de données Workfront.

Pour plus d’informations sur la création de rapports en mode texte, notamment les classes, vidéos et tutoriels, consultez la section « Formation » du site Adobe Experience League.

## Remarques avant d’utiliser le mode texte

>[!TIP]
>
>Vous pouvez également développer les capacités des champs personnalisés calculés en utilisant une version du mode texte pour les champs personnalisés. La syntaxe et les règles de création d’un champ personnalisé calculé sont différentes de celles utilisées dans les rapports et listes. Pour plus d’informations sur l’ajout d’un champ calculé personnalisé, voir [&#x200B; Ajouter des champs calculés à un formulaire &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Avant de commencer à utiliser le mode texte dans vos rapports, nous vous recommandons vivement de suivre nos cours sur les rapports avancés, afin de mieux comprendre notre langage en mode texte.
* Pour préserver l’intégrité de vos rapports lors des mises à jour du logiciel Workfront, l’utilisation du mode standard est préférable. Si le mode texte permet de créer des vues, des filtres et des regroupements plus complexes, il est également plus compliqué à maintenir et ne peut être garanti en cas de mise à jour du logiciel Workfront.
* Pour la conception de vos rapports, il est préférable d’utiliser principalement l’interface standard et de passer au mode texte seulement pour des ajustements mineurs.

  >[!TIP]
  >
  >L’utilisation du mode de création standard vous permet d’obtenir des éléments constitutifs et des modèles de code essentiels que vous pouvez ensuite utiliser lorsque vous modifiez le code en mode texte.

* Pour générer efficacement des rapports et des listes en mode texte, vous devez utiliser une syntaxe et des règles spécifiques. Assurez-vous de connaître la syntaxe Workfront pour le mode texte avant de commencer.

  Pour plus d’informations sur la syntaxe et les règles d’utilisation du mode texte, consultez la section [Vue d’ensemble de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

* Après avoir personnalisé un élément de rapport en mode texte, vous ne pourrez peut-être pas revenir au mode standard (dans une vue) ou le code de l’élément que vous avez créé sera supprimé (dans les filtres et les regroupements). En effet, tous les champs pris en charge en mode texte ne le sont pas en mode standard.

## Interface du mode standard

L’interface du mode standard affiche des champs permettant de mapper les éléments d’application que vous souhaitez afficher dans un rapport ou une liste. L’interface du mode standard est un ensemble de menus déroulants à partir desquels vous pouvez sélectionner les champs que vous souhaitez afficher dans vos rapports ou listes.

Pour plus d’informations sur l’interface du mode standard et pour savoir comment créer un rapport ou une liste, consultez ce qui suit :

* [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* [Éléments de rapport : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Interface du mode texte

Le mode Texte permet de créer des vues, des filtres, des regroupements et des invites plus complexes en vous offrant la possibilité d’utiliser des champs qui ne sont pas disponibles dans l’interface du mode Standard. En mode texte Workfront, il existe un ensemble d’instructions codées qui indiquent les objets que vous souhaitez afficher dans un rapport ou une liste.

Pour obtenir une liste complète de tous nos champs pouvant faire l’objet d’un rapport, consultez la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Tous les champs disponibles via l’API ne sont pas disponibles via l’interface du mode texte. Si vous utilisez le champ correct dans votre code de mode texte et que vous n’affichez pas les résultats attendus, il se peut que le champ ne puisse faire l’objet d’un rapport que via l’API.

## Accéder aux éléments de reporting et modifer le mode texte {#access-reporting-elements-and-edit-text-mode}

Accéder à l’interface du mode texte est identique pour les vues, les regroupements et les filtres lorsque l’on y accède à partir d’un rapport ou d’une liste.

Pour plus d’informations sur l’utilisation du mode texte dans les vues, les filtres et les regroupements, consultez ce qui suit :

* [Modifier une vue en utilisant le mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [Modifier un filtre en utilisant le mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [Modification d’un regroupement à l’aide du mode texte](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Les invites personnalisées ne peuvent être modifiées qu’en mode texte. Vous ne pouvez accéder aux invites qu’à partir d’un rapport.

Pour plus d’informations sur l’accès à l’interface du mode texte des invites personnalisées, consultez la section [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Raisons courantes d’utiliser le mode texte {#common-reasons-to-use-text-mode}

À l’exception de la création d’invites personnalisées exclusives au mode texte, nous conseillons d’utiliser le Report Builder pour élaborer vos vues, filtres et regroupements. Cependant, dans certains cas, vous pouvez utiliser le mode texte pour améliorer vos rapports et listes.

Pour plus d’informations sur les utilisations courantes du mode texte, consultez la section [Vue d’ensemble des utilisations courantes du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
