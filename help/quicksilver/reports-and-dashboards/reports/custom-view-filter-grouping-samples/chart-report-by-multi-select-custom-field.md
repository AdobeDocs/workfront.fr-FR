---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Tracer un graphique de rapport en fonction d’un champ personnalisé multi-sélection
description: Vous ne pouvez tracer un rapport en fonction d’un champ personnalisé multi-sélection qu’après avoir créé un champ calculé supplémentaire qui capture les choix sélectionnés dans le champ personnalisé multi-sélection.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 97%

---

# Tracer un graphique de rapport en fonction d’un champ personnalisé multi-sélection

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Plutôt que de créer un graphique à partir d’un champ personnalisé multi-sélection, nous vous recommandons de créer des champs distincts pour chaque option d’un champ personnalisé multi-sélection.

Quelques exemples de champs personnalisés multi-sélection incluent :

* Cases à cocher
* Menus déroulants multi-sélection

Pour plus d’informations sur l’utilisation du mode texte, voir l’article [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Toutefois, s’il n’est pas possible d’avoir des champs distincts pour chaque option d’un champ multi-sélection, vous pouvez tracer un rapport en fonction d’un champ personnalisé multi-sélection en utilisant des champs personnalisés calculés pour regrouper d’abord les choix du champ multi-sélection. Ensuite, vous pouvez tracer le rapport en fonction des champs calculés.

>[!NOTE]
>
>Les éléments pour lesquels l’un des choix est sélectionné ne sont comptés qu’une seule fois.
>
>Par exemple, si vous disposez d’un champ personnalisé de type Case à cocher avec les options Choix 1 et Choix 2, et que vous attachez le formulaire à des tâches, les tâches pour lesquelles les Choix 1 et 2 sont sélectionnés s’affichent dans un élément de graphique distinct de celui des tâches pour lesquelles seul le Choix 1 ou 2 est sélectionné.
>
>Les tâches pour lesquelles le Choix 1 a été sélectionné ne s’affichent pas dans le même élément graphique que les tâches pour lesquelles les Choix 1 et 2 ont été sélectionnés.

## Conditions d’accès

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Avant de commencer, vous devez créer un champ personnalisé calculé qui affiche les valeurs sélectionnées dans le champ personnalisé multi-sélection.Pour plus d’informations, voir la section [Créer un champ personnalisé calculé qui fait référence à un champ personnalisé](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) multi-sélection de cet article.

## Tracer un graphique de rapport en fonction de champs personnalisés multi-sélection

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

Vous ne pouvez pas créer un graphique dans un rapport en faisant référence à un champ personnalisé multi-sélection. Au lieu de cela, vous pouvez créer un champ calculé qui enregistre les valeurs du champ personnalisé multi-sélection sur un objet donné et les regroupe en fonction du champ calculé. 

* [Créer un champ personnalisé calculé qui fait référence à un champ personnalisé multi-sélection](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Construire un graphique qui fait référence à un champ personnalisé calculé](#build-a-chart-that-references-a-calculated-custom-field)

### Créer un champ personnalisé calculé qui fait référence à un champ personnalisé multi-sélection {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Pour créer un champ calculé qui fait référence à un champ personnalisé multi-sélection, vous devez disposer des conditions préalables suivantes :

* Un champ personnalisé multi-sélection dans un formulaire personnalisé.\
  Pour plus d’informations sur la création de formulaires personnalisés et l’ajout de champs personnalisés, reportez-vous à l’article [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Un formulaire personnalisé avec le champ personnalisé multi-sélection attaché aux objets.
* Valeurs du champ personnalisé multi-sélection pour chaque objet.

Pour créer le champ personnalisé calculé qui fait référence au champ personnalisé multi-sélection :

1. Créez un formulaire personnalisé ou modifiez un formulaire existant.

   Pour plus d’informations sur la création de formulaires personnalisés, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Sélectionnez l’objet ou les objets que vous souhaitez utiliser avec le formulaire personnalisé.
1. Cliquez sur **Ajouter un champ**, puis sur **Calculé** pour ajouter le champ personnalisé multi-sélection au formulaire.

1. Dans la boîte **Libellé**, nommez le nouveau champ calculé pour indiquer qu’il fait référence au champ personnalisé multi-sélection.

   Par exemple : « Champ multi-sélection calculé »

1. Dans la case **Calcul**, saisissez le code suivant :

   `{DE:Multi-select Custom Field}`

   Cette opération permet d’ajouter les choix sélectionnés dans le champ personnalisé multi-sélection au champ personnalisé calculé. Par exemple, si le formulaire est lié à des tâches et que le choix 1 est sélectionné dans le champ personnalisé multi-sélection, le champ personnalisé calculé affiche la valeur « Choix 1 ». Si les choix 1 et 2 sont sélectionnés pour une tâche différente, le champ personnalisé calculé affiche la valeur « Choix 1, Choix 2 ».

1. Remplacez « Champ personnalisé multi-sélection » par le nom réel de votre champ personnalisé multi-sélection, tel qu’il apparaît dans Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Facultatif) Si le champ personnalisé multi-sélection se trouve déjà dans ce formulaire et si ce formulaire est déjà attaché à des objets, activez l’option **Mettre à jour les calculs (en arrière-plan)**.

   Cela permet de s’assurer que le nouveau champ calculé est automatiquement rempli avec la valeur du champ personnalisé multi-sélection lorsqu’il est ajouté aux formulaires déjà attachés aux objets.

1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer + Fermer**.

   Le champ personnalisé calculé est ajouté au formulaire personnalisé et, si le formulaire est actuellement rattaché à des objets, le champ est rempli avec les informations du champ personnalisé multi-sélection.

### Construire un graphique qui fait référence à un champ personnalisé calculé {#build-a-chart-that-references-a-calculated-custom-field}

1. (Facultatif) Pour vous assurer que tous les champs calculés par lesquels vous souhaitez établir des graphiques sont remplis de valeurs, dans l’onglet Détails du rapport, sélectionnez tous les objets qui contiennent le formulaire personnalisé avec le champ personnalisé multi-sélection et le champ personnalisé calculé, puis cliquez sur **Modifier**.
1. (Facultatif et le cas échéant) Sélectionnez le champ **Recalculer les expressions personnalisées**, puis cliquez sur **Enregistrer les modifications**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >Cette option a été supprimée de la modification de projets en bloc.  Vous pouvez toujours recalculer les expressions pour les projets en bloc en cliquant sur l’icône **Plus** ![](assets/more-icon-45x33.png) en haut d’une liste de projets, puis sur **Recalculer les expressions**.

1. Accédez au rapport dans lequel vous souhaitez ajouter le graphique pour le champ calculé qui fait référence au champ personnalisé multi-sélection.
1. Cliquez sur **Actions de rapport**, puis sur **Modifier**.

1. Sélectionnez l’onglet <strong>Regroupements</strong>, puis cliquez sur <strong>Ajouter un regroupement</strong>.
1. Ajoutez le </strong>champ calculé multi-sélection<strong> que vous avez créé comme regroupement.
1. Sélectionnez l’onglet <strong>Graphique</strong> et ajoutez un graphique à votre rapport.

   Par exemple, choisissez un graphique en **colonnes**.
   <br>Pour plus d’informations sur l’ajout d’un graphique à un rapport, voir la section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Ajouter un graphique à un rapport</a> dans l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.
1. Dans le champ **Axe du bas (X)**, sélectionnez le <strong>champ calculé multi-sélection</strong> à afficher dans le graphique.
1. Cliquez sur <strong>Enregistrer + Fermer</strong>.

   Le rapport affiche les résultats groupés par champ calculé multi-sélection dans un graphique.

   ![](assets/chart-multi-select-field-column-chart-example.png)