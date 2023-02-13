---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Référencer un formulaire personnalisé dans un rapport
description: Vous pouvez référencer les formulaires personnalisés d’un objet dans les options Vues, Filtres et Groupements d’un rapport pour cet objet.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---

# Référencer un formulaire personnalisé dans un rapport

Vous pouvez référencer les formulaires personnalisés d’un objet dans les options Vues, Filtres et Groupements d’un rapport pour cet objet.

Vous pouvez référencer le contenu des formulaires personnalisés à inclure dans un rapport ou vous pouvez référencer des informations sur les formulaires personnalisés à inclure dans un rapport.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Le formulaire personnalisé doit exister avant de pouvoir le référencer dans un rapport.

Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Référence au contenu des formulaires personnalisés

Vous pouvez référencer des champs dans des formulaires personnalisés. Après l’application d’un formulaire personnalisé à un objet, tous les champs associés à ce formulaire personnalisé peuvent être référencés dans un rapport, comme le serait tout autre champ de l’objet.

>[!NOTE]
>
>Pour les champs comportant plusieurs options, toutes les options sont disponibles dans les Filtres et invites du rapport, y compris celles qui sont masquées.\
>Pour plus d’informations sur le masquage de choix à partir d’un champ personnalisé avec plusieurs options, consultez l’article . [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Lors de la création du rapport, il vous suffit d’utiliser le type d’objet du formulaire comme source du champ et d’utiliser le nom du champ personnalisé comme nom du champ.

Par exemple, un formulaire personnalisé peut être appliqué à tous les projets qui incluent un champ personnalisé. **Consultant**. Pour créer un rapport qui répertorie tous les projets pour lesquels Olivia Kim est consultant, utilisez la variable **Projet** type d’objet comme source de champ, et utilisez **Consultant** comme nom du champ. Définissez le qualificateur de filtre sur **Égal**, puis tapez Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

Pour plus d’informations sur la création d’un rapport, reportez-vous à l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Informations de référence sur les formulaires personnalisés

Vous pouvez référencer des informations sur des formulaires personnalisés, tels que le nom de tout formulaire personnalisé associé à un objet.

&#x200B; Selon l’élément (Affichage, Filtre ou Groupement), vous pouvez référencer :

* Le Principal formulaire personnalisé appliqué à un objet :

   Il s’agit du formulaire qui s’affiche en premier sur la page Détails de l’objet.

* Tous les formulaires personnalisés (si plusieurs formulaires personnalisés sont appliqués à un objet)

Vous pouvez référencer des formulaires personnalisés sur des vues, des filtres et des regroupements :

* [Référence aux formulaires personnalisés dans une vue de rapport (colonne)](#reference-custom-forms-in-a-report-view-column)
* [Référence aux formulaires personnalisés dans un filtre de rapport](#reference-custom-forms-in-a-report-filter)
* [Référencer des formulaires personnalisés dans un groupement de rapports](#reference-custom-forms-in-a-report-grouping)

### Référence aux formulaires personnalisés dans une vue de rapport (colonne) {#reference-custom-forms-in-a-report-view-column}

Pour afficher tous les formulaires personnalisés associés à un objet :

1. Commencer à créer un rapport comme décrit dans l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sur le **Colonnes** , développez le type d’objet auquel le formulaire personnalisé à référencer est appliqué, puis cliquez sur **Nom de la catégorie**.\
   Par exemple, pour afficher tous les formulaires personnalisés associés à une tâche, développez la **Tâche** source du champ, puis cliquez sur **Nom de la catégorie** nom du champ.\
   ![](assets/qs-category-name-column-350x267.png)

Pour afficher uniquement le Principal formulaire personnalisé associé à l’objet :

1. Commencer à créer un rapport comme décrit dans l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sur le **Colonnes** , développez l’onglet **Catégorie** source du champ, puis cliquez sur **Nom** nom du champ.\
   ![](assets/qs-category-name-column-2-350x248.png)

### Référence aux formulaires personnalisés dans un filtre de rapport {#reference-custom-forms-in-a-report-filter}

Pour filtrer tous les formulaires personnalisés associés au type d’objet :

1. Commencer à créer un rapport comme décrit dans l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sur le **Filtres** onglet, développer **Catégories**, puis cliquez sur **Nom**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. Sélectionnez le qualificateur de condition à utiliser :

   * Vide
   * Non vide
   * Contient
   * Ne contient pas (non sensible à la casse)
   * Égal à (non sensible à la casse)
   * Non égal à (non sensible à la casse)

   Pour plus d’informations sur chaque qualificateur, consultez l’article [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Si le champ pour lequel vous filtrez les données comporte plusieurs options et que vous utilisez la variable **Différent de** ou **Ne contient pas** qualificateurs, cela filtre les résultats qui contiennent uniquement le choix que vous spécifiez. Si le champ contient des options supplémentaires, y compris celle spécifiée, ces résultats ne sont pas filtrés à partir du rapport. Cela inclut le filtrage de plusieurs Forms personnalisées si elles sont jointes au même objet.

1. Commencez à saisir le nom du formulaire personnalisé sur lequel vous souhaitez filtrer les données, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif) Cliquez sur **Ajouter une autre règle de filtre**, puis répétez les étapes 2 à 4 pour créer des règles de filtrage supplémentaires.
1. Cliquez sur **Enregistrer + Fermer**.

Pour filtrer uniquement sur le Principal formulaire personnalisé associé au type d’objet :

1. Commencer à créer un rapport comme décrit dans l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sur le **Filtres** , développez l’onglet **Catégorie** source du champ, puis cliquez sur **Nom** nom du champ.\
   ![](assets/qs-category-name-filter-350x437.png)

1. Sélectionnez le qualificateur de condition à utiliser :

   * Vide
   * Non vide
   * Contient
   * Ne contient pas (non sensible à la casse)
   * Égal à (non sensible à la casse)
   * Non égal à (non sensible à la casse)

   Pour plus d’informations sur chaque qualificateur, consultez l’article [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Commencez à saisir le nom du formulaire personnalisé sur lequel vous souhaitez filtrer les données, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif) Cliquez sur **Ajouter une autre règle de filtre**, puis répétez les étapes 2 à 4 pour créer des règles de filtrage supplémentaires.
1. Cliquez sur **Enregistrer + Fermer**.

### Référencer des formulaires personnalisés dans un groupement de rapports {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>Vous ne pouvez regrouper les éléments que par le Principal formulaire personnalisé associé à l’objet ; vous ne pouvez pas regrouper les éléments selon tous les formulaires associés à l’objet.

1. Commencer à créer un rapport comme décrit dans l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sur le **Groupements** onglet, développer **Catégorie**, puis cliquez sur **Nom**.\
   ![](assets/qs-category-name-grouping-350x373.png)
