---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Graphique un rapport selon un champ personnalisé à sélection multiple
description: Il n’est pas possible de tracer un rapport selon un champ personnalisé à sélection multiple. Vous devez créer un champ calculé supplémentaire qui fait référence au champ personnalisé à sélection multiple pour également associer le rapport à la valeur du champ personnalisé à sélection multiple.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Graphique un rapport selon un champ personnalisé à sélection multiple

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Il n’est pas possible de tracer un rapport selon un champ personnalisé à sélection multiple. Vous devez créer un champ calculé supplémentaire qui fait référence au champ personnalisé à sélection multiple pour également associer le rapport à la valeur du champ personnalisé à sélection multiple.

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

Avant de commencer, vous devez créer un champ personnalisé calculé qui affiche les valeurs sélectionnées à partir du champ personnalisé à sélection multiple. Pour plus d’informations, voir [Créer un champ personnalisé calculé qui référence un champ personnalisé à sélection multiple](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) dans cet article.

## Créer un rapport selon des champs personnalisés à sélection multiple

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

Vous ne pouvez pas créer de graphique dans un rapport en référençant un champ personnalisé à sélection multiple. Vous pouvez plutôt créer un champ calculé qui enregistre les valeurs du champ personnalisé à sélection multiple sur un objet et un groupe donné par le champ calculé. 

* [Créer un champ personnalisé calculé qui référence un champ personnalisé à sélection multiple](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Créer un graphique qui référence un champ personnalisé calculé](#build-a-chart-that-references-a-calculated-custom-field)

### Créer un champ personnalisé calculé qui référence un champ personnalisé à sélection multiple {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Pour pouvoir créer un champ calculé qui référence un champ personnalisé à sélection multiple, les conditions préalables suivantes doivent être remplies :

* Créez le champ personnalisé à sélection multiple dans un formulaire personnalisé.\
   Pour plus d’informations sur la création de formulaires personnalisés et l’ajout de champs personnalisés, reportez-vous à l’article [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Associez le formulaire personnalisé aux objets.
* Renseignez le champ personnalisé à sélection multiple avec une valeur sur chaque objet.

Pour créer le champ personnalisé calculé qui référence le champ personnalisé à sélection multiple :

1. Créez un formulaire personnalisé ou modifiez un formulaire existant.\
   Pour plus d’informations sur la création de formulaires personnalisés, reportez-vous à l’article [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Sélectionnez le ou les objets que vous prévoyez d’utiliser avec le formulaire personnalisé.
1. Cliquez sur **Ajouter un champ**, puis **Calculé** pour ajouter le champ personnalisé à sélection multiple au formulaire.

1. Dans le **Libellé** , nommez le nouveau champ calculé pour indiquer qu’il fait référence au champ personnalisé à sélection multiple.\
   Par exemple : &quot;Champ à sélection multiple calculé&quot;.

1. Dans le **Calcul** saisissez le code suivant :

   ```
   {DE:Multi-select Custom Field}
   ```

1. Remplacez &quot;Champ personnalisé à sélection multiple&quot; par le nom réel de votre champ personnalisé à sélection multiple, tel qu’il apparaît dans Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Facultatif) Si le champ personnalisé à sélection multiple figure déjà sur ce formulaire et si ce formulaire est déjà joint à des objets, activez l’option **Mise à jour des calculs précédents** .\
   Cela permet de s’assurer que le nouveau champ est automatiquement renseigné avec la valeur du champ personnalisé à sélection multiple, car il est ajouté aux formulaires attachés aux objets déjà présents.

1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer +Fermer**.

### Créer un graphique qui référence un champ personnalisé calculé {#build-a-chart-that-references-a-calculated-custom-field}

1. (Facultatif) Pour vous assurer que tous les champs calculés à partir desquels vous souhaitez effectuer un graphique sont renseignés par des valeurs, sélectionnez tous les objets de votre rapport qui contiennent le formulaire personnalisé avec le champ personnalisé à sélection multiple et le champ personnalisé calculé, puis cliquez sur **Modifier**.
1. (Facultatif et conditionnel) Activez la variable **Recalculer des expressions personnalisées** , puis cliquez sur **Enregistrer les modifications**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >Cette option a été supprimée de la modification des projets en bloc.  Vous pouvez toujours recalculer les expressions pour les projets en masse en cliquant sur le bouton **Plus** icon ![](assets/more-icon-45x33.png) en haut de la liste d’un projet, puis **Recalculer les expressions**.


1. Accédez au rapport dans lequel vous souhaitez ajouter le graphique pour le champ calculé qui référence le champ personnalisé à sélection multiple.
1. Cliquez sur **Actions de rapport**, puis **Modifier**.

1. Sélectionnez la <strong>Groupements</strong> , puis cliquez sur <strong>Ajouter un groupement</strong>.
1. Ajoutez la variable<strong>Champ à sélection multiple calculé</strong> vous avez créé en tant que regroupement.
1. Sélectionnez la <strong>Graphique</strong> puis ajoutez un graphique à votre rapport.<br>Pour plus d’informations sur l’ajout d’un graphique à un rapport, reportez-vous à la section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Ajout d’un graphique à un rapport</a> dans l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Création d’un rapport personnalisé</a>.
1. Sélectionnez la <strong>Champ à sélection multiple calculé</strong> comme l’un des champs à afficher dans le graphique.
1. Cliquez sur <strong>Enregistrer + Fermer</strong>.<br>Le rapport affiche les résultats regroupés par champ à sélection multiple calculé dans un graphique.
