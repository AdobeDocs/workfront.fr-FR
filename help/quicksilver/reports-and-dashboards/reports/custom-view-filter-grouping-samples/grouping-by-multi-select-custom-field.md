---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: Regrouper un rapport en fonction d’un champ personnalisé à sélection multiple
description: Vous ne pouvez regrouper par valeur dans un champ personnalisé à sélection multiple dans un rapport Adobe Workfront qu’en mode texte.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 530dff59-0d4c-490e-b464-1d3bb1d0f36f
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 24%

---

# Regrouper un rapport en fonction d’un champ personnalisé à sélection multiple

Vous ne pouvez regrouper par valeur dans un champ personnalisé à sélection multiple dans un rapport Adobe Workfront qu’en mode texte.

Voici quelques exemples de champs personnalisés à sélection multiple :

* Cases à cocher
* Menus déroulants à sélection multiple

Pour plus d’informations sur l’utilisation du mode texte, consultez l’article [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Remarques concernant le regroupement par un champ personnalisé à sélection multiple

* Vous ne pouvez pas créer de graphique pour un rapport qui utilise un regroupement en mode texte. Vous devez créer un champ calculé supplémentaire qui fait référence au champ personnalisé à sélection multiple pour également associer le rapport à la valeur du champ personnalisé à sélection multiple.

  Pour plus d’informations, voir [Créer un rapport selon un champ personnalisé à sélection multiple](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/chart-report-by-multi-select-custom-field.md).
* Les éléments pour lesquels l’un des choix est sélectionné ne sont comptabilisés qu’une seule fois.

  Par exemple, si vous disposez d’un champ personnalisé Case à cocher avec les options Choix 1 et Choix 2 et que vous joignez le formulaire aux tâches, les tâches pour lesquelles Choix 1 et Choix 2 sont sélectionnées sont regroupées séparément des tâches pour lesquelles seul Choix 1 ou Choix 2 est sélectionné.


## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un groupement </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Editer l'accès aux Filtres, Vues, Groupements pour modifier un groupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire, consultez <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Regrouper un rapport par des champs personnalisés à sélection multiple

Pour pouvoir effectuer un groupement selon un champ personnalisé à sélection multiple, les prérequis suivants doivent être remplis :

* Créez le champ personnalisé à sélection multiple dans un formulaire personnalisé.\
  Pour plus d’informations sur la création de formulaires personnalisés et l’ajout de champs personnalisés, reportez-vous à l’article [Concevoir un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Associez le formulaire personnalisé aux objets.
* Renseignez le champ personnalisé à sélection multiple avec une valeur sur chaque objet. 

Pour regrouper un champ personnalisé à sélection multiple dans un rapport :

1. Créez un rapport ou modifiez un rapport existant dans lequel vous souhaitez ajouter un groupement pour un champ personnalisé à sélection multiple.\
   Pour plus d’informations sur la création de rapports, reportez-vous à l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Sélectionnez l&#39;onglet **Groupings** .
1. Cliquez sur **Passer en mode Texte**.

1. Sélectionnez le texte dans la zone **Regrouper votre rapport** et remplacez-le par le code suivant :

   <pre>
   group.0.displayname=Nom du champ personnalisé à sélection multiple
   group.0.valueexpression={DE:Multi-select Custom Field Name}
   group.0.valueformat=HTML
   group.0.textmode=true
   </pre>

1. Remplacez &quot;Nom de champ personnalisé à sélection multiple&quot; par le nom réel de votre champ personnalisé à sélection multiple, tel qu’il apparaît dans Workfront.
1. Cliquez sur **Enregistrer et Fermer**.

   Les objets du rapport sont regroupés selon les valeurs du champ personnalisé à sélection multiple.

   ![](assets/grouping-by-multi-select-field-text-mode-ui-example.png)

   Le nom des regroupements du rapport correspond au nom du champ personnalisé à sélection multiple, suivi des valeurs sélectionnées dans le champ.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Chart a report by multi-select Custom Fields</h2>
<p>(NOTE: this moved to its own article, linked in the Note above!)</p>
<p>You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;</p>
<ul>
<li><a href="#build-a-calculated-custom-field-that-references-a-multi-select-custom-field" class="MCXref xref">Build a calculated custom field that references a multi-select custom field</a> </li>
<li><a href="#build-a-chart-that-references-a-calculated-custom-field" class="MCXref xref">Build a chart that references a calculated custom field</a> </li>
</ul>
<p><strong>Build a calculated custom field that references a multi-select custom field</strong></p>
<p>To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:</p>
<ul>
<li>Build the multi-select custom field in a custom form.<br>.</li>
<li>Attach the custom form to objects.</li>
<li>Populate the multi-select custom field with a value on each object.</li>
</ul>
<p>To build the calculated custom field that references the multi-select custom field:</p>
<ol>
<li value="1">Create a custom form, or edit an existing one.<br>.</li>
<li value="2">Click<strong>Add a Field</strong>, then <strong>Calculated</strong> to add the multi-select custom field to the form.</li>
<li value="3">In the <strong>Label</strong> box, name the new calculated field to indicate that it references the multi-select custom field.<br>For example: "Calculated Multi-select Field."</li>
<li value="4"> <p>In the <strong>Calculation</strong> box, enter the following code:</p><pre>{DE:Multi-select Custom Field}</pre> <p> <img src="assets/calculated-multi-select-custom-field-350x201.png" style="width: 350;height: 201;"> <br> </p> </li>
<li value="5">Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.</li>
<li value="6"> <p>(Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the <strong>Update previous calculations</strong>&nbsp;option.</p> <p>This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.</p> </li>
<li value="7">Click <strong>Done</strong>.</li>
<li value="8">Click <strong>Save +Close</strong>.</li>
</ol>
<p><strong>Build a chart that references a calculated custom field</strong></p>
<ol>
<li value="1"> Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. </li>
<li value="2"> (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report, then click <strong>Edit</strong>. </li>
<li value="3"> <p> (Optional and conditional) Enable the <strong>Recalculate Custom Expressions</strong> field, then click <strong>Save Changes</strong>.</p> <p> <img src="assets/recalculate-custom-expressions-350x259.png" style="width: 350;height: 259;"> <br> </p> </li>
<li value="4"> Click <strong>Report Actions</strong>, then <strong>Edit</strong>. </li>
<li value="5">Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. </li>
<li value="6">Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. </li>
<li value="7"> <p>Select the <strong>Chart</strong> tab, and add a chart to your report.</p> <p>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li>
<li value="8">Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. </li>
<li value="9"> <p>Click <strong>Save + Close</strong>.</p> <p>The report displays the results grouped by the Calculated Multi-select Field in a chart. </p> </li>
</ol>
</div>
-->
