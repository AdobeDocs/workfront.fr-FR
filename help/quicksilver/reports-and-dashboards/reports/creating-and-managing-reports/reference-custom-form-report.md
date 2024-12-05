---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Référencer un formulaire personnalisé dans un rapport
description: Vous pouvez faire référence aux formulaires personnalisés d’un objet dans les vues, les filtres et les regroupements d’un rapport pour cet objet.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 394eb1aed6508399b6459430acec7c0729036edc
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 95%

---

# Référencer un formulaire personnalisé dans un rapport

<!-- Audited: 11/2024 -->

Vous pouvez faire référence aux formulaires personnalisés d’un objet dans les vues, les filtres et les regroupements d’un rapport pour cet objet.

Vous pouvez référencer le contenu des formulaires personnalisés à inclure dans un rapport, ou vous pouvez référencer des informations sur les formulaires personnalisés eux-mêmes à inclure dans un rapport.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
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
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et regroupements</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Le formulaire personnalisé doit exister avant que vous puissiez le référencer dans un rapport.

Pour plus d’informations sur la création de formulaires personnalisés, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Référencer le contenu des formulaires personnalisés

Vous pouvez faire référence à des champs dans des formulaires personnalisés. Une fois qu’un formulaire personnalisé est appliqué à un objet, tous les champs associés à ce formulaire personnalisé peuvent être référencés dans un rapport comme n’importe quel autre champ de l’objet.

>[!NOTE]
>
>Pour les champs à options multiples, toutes les options sont disponibles dans les filtres et les invites du rapport, y compris celles qui sont masquées.\
>Pour plus d’informations sur le masquage de choix à partir d’un champ personnalisé avec plusieurs options, consultez l’article [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Lors de la création du rapport, il suffit d’utiliser le type d’objet du formulaire comme source de champ et le nom du champ personnalisé comme nom de champ.

Par exemple, vous pouvez avoir un formulaire personnalisé appliqué à tous les projets qui comprend le champ personnalisé **Consultant ou consultante**. Pour créer un rapport qui répertorie tous les projets pour lesquels Olivia Kim est consultante, utilisez le type d’objet **Projet** comme source de champ et **Consultant ou consultante** comme nom de champ. Définissez le qualificateur du filtre sur **Égal à**, puis saisissez Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Référencer des informations sur les formulaires personnalisés

Vous pouvez référencer des informations sur les formulaires personnalisés, telles que le nom des formulaires personnalisés associés à un objet.

En fonction de l’élément (vue, filtre ou regroupement), vous pouvez faire référence à un des éléments suivants :

* Formulaire personnalisé principal appliqué à un objet :

  C’est le formulaire qui apparaît en premier sur la page Détails de l’objet.

* Tous les formulaires personnalisés (si plusieurs formulaires personnalisés sont appliqués à un objet).

Vous pouvez faire référence à des formulaires personnalisés dans les vues, les filtres et les regroupements :

* [Référencer des formulaires personnalisés dans un rapport via l’onglet Vue (colonne)](#reference-custom-forms-in-a-report-view-column)
* [Référencer des formulaires personnalisés dans un rapport via l’onglet Filtre](#reference-custom-forms-in-a-report-filter)
* [Référencer des formulaires personnalisés dans un rapport via l’onglet Regroupement](#reference-custom-forms-in-a-report-grouping)

### Référencer des formulaires personnalisés dans un rapport via l’onglet Vue (colonne) {#reference-custom-forms-in-a-report-view-column}

Pour afficher tous les formulaires personnalisés associés à un objet, procédez comme suit :

1. Commencez à créer un rapport comme décrit dans l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Dans l’onglet **Colonnes**, développez le type d’objet auquel s’applique le formulaire personnalisé que vous souhaitez référencer, puis cliquez sur **Nom de la catégorie**.\
   Par exemple, pour afficher tous les formulaires personnalisés associés à une tâche, développez la source de champ **Tâche**, puis cliquez sur le nom de champ **Nom de la catégorie**.\
   ![](assets/qs-category-name-column-350x267.png)

Pour afficher uniquement le formulaire personnalisé principal associé à l’objet, procédez comme suit :

1. Commencez à créer un rapport comme décrit dans l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Dans l’onglet **Colonnes**, développez la source de champ **Catégorie**, puis cliquez sur le nom de champ **Nom**.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Référencer des formulaires personnalisés dans un rapport via l’onglet Filtre {#reference-custom-forms-in-a-report-filter}

Pour filtrer tous les formulaires personnalisés associés au type d’objet, procédez comme suit :

1. Commencez à créer un rapport comme décrit dans l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Dans l’onglet **Filtres**, développez **Catégories**, puis cliquez sur **Nom**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. Sélectionnez le qualificateur de condition que vous souhaitez utiliser :

   * Vide
   * Non vide
   * Contient
   * Ne contient pas
   * Égal à (non sensible à la casse)
   * Non égal à (non sensible à la casse)

   Pour plus d’informations sur chaque qualificateur, consultez l’article [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Si le champ que vous filtrez comporte plusieurs options et que vous utilisez les qualificateurs **Non égal à** ou **Ne contient pas**, les résultats qui ne contiennent que l’option que vous avez spécifiée sont filtrés. Si le champ contient des options supplémentaires, y compris celle spécifiée, ces résultats ne sont pas filtrés dans le rapport. Cela inclut le filtrage de plusieurs formulaires personnalisés s’ils sont attachés au même objet.

1. Commencez à saisir le nom du formulaire personnalisé sur lequel vous voulez effectuer un filtrage, puis cliquez sur son nom lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif) Cliquez sur **Ajouter une autre règle de filtrage**, puis répétez les étapes 2 à 4 pour créer d’autres règles de filtrage.
1. Cliquez sur **Enregistrer et fermer**.

Pour n’effectuer le filtrage que sur le formulaire personnalisé principal associé au type d’objet, procédez comme suit :

1. Commencez à créer un rapport, tel que décrit dans l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Dans l’onglet **Filtres**, développez la source du champ **Catégorie**, puis cliquez sur le champ **Nom**.\
   ![](assets/qs-category-name-filter-350x437.png)

1. Sélectionnez le qualificateur de condition que vous souhaitez utiliser :

   * Vide
   * Non vide
   * Contient
   * Ne contient pas
   * Égal à (non sensible à la casse)
   * Non égal à (non sensible à la casse)

   Pour plus d’informations sur chaque qualificateur, voir l’article [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Commencez à saisir le nom du formulaire personnalisé sur lequel vous voulez effectuer un filtrage, puis cliquez sur son nom lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif) Cliquez sur **Ajouter une autre règle de filtrage**, puis répétez les étapes 2 à 4 pour créer d’autres règles de filtrage.
1. Cliquez sur **Enregistrer et fermer**.

### Référencer des formulaires personnalisés dans un rapport via l’onglet Regroupement {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>Vous ne pouvez regrouper les éléments qu’en fonction du formulaire personnalisé principal associé à l’objet. Vous ne pouvez pas regrouper les éléments en tenant compte de tous les formulaires associés à l’objet.

1. Commencez à créer un rapport, tel que décrit dans l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Dans l’onglet **Regroupements**, développez le choix **Catégorie**, puis cliquez sur **Nom**.\
   ![](assets/qs-category-name-grouping-350x373.png)
