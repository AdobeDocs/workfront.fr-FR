---
product-area: reporting
navigation-topic: reporting-elements
title: Créer des regroupements dans Adobe Workfront
description: Vous pouvez créer un regroupement personnalisé à partir de zéro ou personnaliser un regroupement existant.
author: Nolan
feature: Reports and Dashboards
exl-id: 64cc52b7-d97b-4b41-9101-530e7db2d26e
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 92%

---

# Créer des regroupements dans Adobe Workfront

<!-- Audited: 11/2024 -->

<!--(NOTE: This is a third part of an article split in 3 about creating and customizing groupings (2 how-tos and one reference)-->

Les résultats d’un rapport ou d’une liste peuvent être organisés avec un regroupement. Les regroupements classent les informations en fonction d’un élément d’information particulier.

Vous pouvez créer un regroupement personnalisé à partir de zéro ou personnaliser un regroupement existant. Suivez les étapes ci-dessous pour créer un regroupement à partir de zéro.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Contributeur ou version ultérieure</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Requête ou supérieure</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Accès Modifier aux Rapports, Tableaux de bord et Calendriers pour créer un regroupement dans un rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td><p>Autorisations de gestion relatives à un rapport pour modifier un regroupement dans un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un regroupement

1. Accédez au rapport ou à la liste dans laquelle vous souhaitez créer votre regroupement personnalisé.
1. Cliquez sur l’icône **Regroupement**.

   ![Sélection d’un nouveau regroupement](assets/newgrouping-nwe-standard-350x304.png)

1. Cliquez sur **+ Nouveau regroupement**.
Le créateur d’interface pour la création du regroupement s’ouvre.

1. Dans la zone **Aperçu du groupement**, cliquez sur **Ajouter un groupement** pour définir comment vous souhaitez que les informations du rapport soient organisées. Vous trouverez ci-dessous un aperçu de ce à quoi ressemble un regroupement dans le rapport.

1. Commencez à saisir le nom du champ qui représente la manière dont vous souhaitez organiser les informations dans le rapport, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif et le cas échéant) Lors de la création d’un regroupement dans une liste mise à jour, sélectionnez **Réduire ce regroupement par défaut** si vous souhaitez que les résultats du regroupement s’affichent de manière réduite plutôt que développée.Ce paramètre est désactivé par défaut et les résultats du regroupement s’affichent toujours dans la liste étendue.

   Pour plus d’informations sur les listes mises à jour et héritées, consultez la section [Différence entre les listes mises à jour et héritées](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) dans l’article [Commencer avec les listes dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Edit existing grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Lorsque vous ajustez manuellement les regroupements lors de l’affichage d’une liste, Workfront mémorise vos préférences manuelles jusqu’à ce que vous vous déconnectiez. Lorsque vous vous reconnectez, la liste s’affiche en fonction de ce paramètre.
   >* Les résultats d’un regroupement s’affichent toujours de façon développée après que l’on y a accédé à partir d’un élément de graphique ou d’une liste héritée. Dans ce genre de cas, ce paramètre est ignoré.

1. Répétez les étapes 4, 5 et 6 pour définir des regroupements supplémentaires.\
   Vous pouvez définir jusqu’à trois regroupements pour organiser les informations. Vous pouvez organiser vos informations encore davantage en utilisant jusqu’à quatre regroupements grâce à un rapport de matrice. Pour plus d’informations sur les rapports de matrice, voir la section [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Cliquez sur **Enregistrer le regroupement**.

## Informations supplémentaires

Voir aussi :

* [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
* [Éléments de création de rapports : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)
* [Modifier les regroupements existants](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h1>Create or edit groupings in Adobe Workfront</h1>
<p class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</p>
<p>You can organize the results of a report or list with a grouping. Groupings categorize data based on a particular piece of information. For more information on groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p>
<p>You can create groupings in lists and reports in the following ways:</p>
<ul>
<li> <p>From scratch</p> </li>
<li> <p>Edit an existing grouping that you originally created or that was shared with you</p> </li>
<li> <p>Copy an existing grouping</p> <p>To copy an existing grouping, you can edit it and save it as a new grouping.</p> </li>
</ul>
<h2>Types of grouping-building interfaces</h2>
<p>You can create groupings using the types of grouping builders described in the table below.</p>
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<col>
</col>
<tbody>
<tr>
<td><strong>Builder type</strong> </td>
<td><strong>Grouping object</strong> </td>
<td><strong>Where available</strong> </td>
</tr>
<tr>
<td><strong>Standard builder</strong> </td>
<td>All objects</td>
<td>Reports and lists</td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<td rowspan="2">
<div class="preview">
<p><strong>Beta builder</strong> </p>
</div> </td>
<td>
<div class="preview">
<p>Projects</p>
<p>Tasks</p>
<p>Issues</p>
</div> </td>
<td>
<div class="preview">
<p>Lists</p>
</div> </td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<td colspan="2"> <note type="note">
<span class="preview">Beta builders for groupings are not available in reports.</span>
</note> </td>
</tr>
</tbody>
</table>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Consider the following when creating groupings using the different builders:
</div>
<ul data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<li>
<div class="preview">
You can switch back and forth between the standard builder and the beta builder, where the beta option is available.
</div> </li>
<li>
<div class="preview">
After you have enabled the beta builder in one area, it is the default experience for all areas where it is available.
</div> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span class="preview">If you enable the beta builder in a project list, it is the default experience for building task and issue groupings in lists as well.</span> </p> </li>
<li> <p><span class="preview">Groupings are available in both builders, regardless of which experience you used to originally build them.</span> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span class="preview">If you created a grouping using the standard builder, you can find and modify it in the beta builder interface as well.</span> </p> </li>
</ul>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Request or higher</p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to&nbsp;filters, views, and groupings</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage access to a grouping to be able to modify or copy it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
<h2>Create a grouping in the standard builder</h2>
<p>Regardless of the method you use to create groupings, creating a grouping from scratch or from an existing grouping is similar.</p>
<ol>
<li value="1"> <p>Go to a list or a report where you want to create a grouping or that contains the grouping that you want to customize.</p> </li>
<li value="2"> <p>Click the <strong>Grouping</strong> icon .</p> <p> <img src="assets/newgrouping-nwe-standard-350x304.png" alt="Select New Grouping" style="width: 350;height: 304;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>New Grouping</strong> at the top of the list of groupings.</p>
<p>Or</p>
<p>Hover over the grouping you want to modify and click the <strong>Edit</strong> icon <img src="assets/edit-icon.png">.</p>
</div> <p>The builder for customizing the grouping opens.</p> </li>
<li value="4"> <p>In the <strong>Grouping Preview</strong> section, click <strong>Add Grouping</strong> to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below.</p> </li>
<li value="5"> <p>Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list.</p> </li>
<li value="6"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional and conditional) When customizing a grouping in an updated list, select <strong>Collapse this grouping by default</strong> if you want the results in the grouping to display collapsed rather than expanded.&nbsp;This setting is disabled by default and the results of the grouping always display in the expanded list.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> For information about updated and legacy lists, see the section <a href="../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated" class="MCXref xref">The difference between the updated and the legacy lists</a>&nbsp;in the article <a href="../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md" class="MCXref xref">Get started with lists in&nbsp;Adobe Workfront</a>.</p>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Edit existing grouping article and Common uses of text mode)</p>
<note type="tip">  
<ul>
<li>When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting.</li>
<li> <p>The results of a grouping always display expanded after accessing them from a chart element or in a legacy list. In these cases, this setting is ignored.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Legacy lists in classic do NOT have this option; legacy lists in NWE DO have this option but it's not functional; this is conditioned only for QS)</p>
</li>
</ul>
</note> </li>
<li value="7"> <p>Repeat Steps  4, 5, and 6  to define additional groupings.</p> <p>You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Create a matrix report</a>.</p> </li>
<li value="8"> <p>(Optional) Click <strong>Switch to Text Mode</strong> to add a grouping using the Text Mode interface.</p> <p>For more information about creating a grouping using the text mode interface, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md" class="MCXref xref">Edit text mode in a grouping</a>.</p> </li>
<li value="9"> <p>Click <strong>Save Grouping</strong> to create a new grouping.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Save as New Grouping</strong> to create a new grouping from the selected one.</p> <p>The new grouping displays in the list of groupings.</p> </li>
<li value="10"> <p>(Optional) Remove groupings you no longer want to display in the list.</p> <p>For information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md" class="MCXref xref">Remove filters, views, and groupings</a>.</p> </li>
</ol>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Create a grouping in the beta builder</h2>
<h3>Enable the beta builder</h3>
<p>The beta builder toggle is disabled by default. You must enable it to use the beta builder.</p>
<ol>
<li value="1">Go to a project, task, or issue list.</li>
<li value="2"> <p>Click the <strong>Grouping</strong> icon <img src="assets/groupingicon.png" alt="Grouping icon">, then enable the beta builder toggle.</p> <p>The beta builder interface opens.</p> <note type="tip">
The header of the grouping builder interface is blue when the beta builder is enabled. This enables the beta builder for all areas of Workfront where it is available.
</note> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace shot below!)</p>
<p> <img src="assets/beta-toggle-groupings-nwe-350x300.png" alt="Beta toggle for groupings" style="width: 350;height: 300;"> </p> </li>
<li value="3"> <p>Continue with <a href="#create-a-grouping-in-the-beta-builder" class="MCXref xref">Create a grouping in the beta builder</a>, below.</p> </li>
</ol>
<p><strong>Create a grouping in the beta builder</strong></p>
<ol>
<li value="1"> <p>Go to a project, task, or issue list where you want to create a grouping, and click the <strong>Grouping</strong> icon <img src="assets/groupingicon.png" alt="Grouping icon">.</p> </li>
<li value="2"> <p>Click <strong>New Grouping</strong> to create a new grouping.</p> <p>Or</p> <p>Hover over an existing grouping in the My groupings area, then click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> to edit an existing grouping.</p> <p>Or</p> <p>Hover over an existing grouping in the My groupings area, select the <strong>More</strong> icon <img src="assets/more-icon.png" alt="More icon">, and select <strong>Duplicate</strong> to copy a grouping.</p> </li>
<li value="3"> <p>Start typing the name of a field in the Group by area, then select it when it displays in the list.</p> <p>You can also select <strong>Search all fields</strong> to view a list of all fields to group by. The fields in the advanced search are grouped by object category.</p> <note type="tip">
As you build the grouping, the results appear immediately in the list.
</note> </li>
<li value="4"> <p>(Optional) Click <strong>Add grouping</strong> to add a second or third grouping.</p> <p> <img src="assets/gouping-groupby-options-350x202.png" alt="Group by options" style="width: 350;height: 202;"> </p> </li>
<li value="5"> <p>(Optional) To reorder the groupings, select a grouping and drag it to the new position.</p> <p>Or</p> <p>Select a grouping and use the keyboard arrow keys to change the order.</p> </li>
<li value="6"> <p>(Optional) Make other selections for the groupings as needed:</p>
<ul>
<li> <p>When grouping by date you must choose a date option such as week, month, or quarter.</p> </li>
<li> <p>Select <img src="assets/grouping-expandicon.png" alt="Expand grouping icon"> to set a grouping to be expanded by default.</p> </li>
<li> <p>Select <img src="assets/delete.png" alt="Delete icon"> to delete a grouping.</p> </li>
</ul> <p> <img src="assets/grouping-editgrouping-350x409.png" alt="Edit grouping" style="width: 350;height: 409;"> </p> </li>
<li value="7"> <p>(Optional) Select <strong>Text Mode</strong> to continue building the grouping using the Text Mode interface.</p> <p>For more information about creating a grouping using the text mode interface, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md" class="MCXref xref">Edit text mode in a grouping</a>.</p> </li>
<li value="8"> <p>(Optional) To use the grouping as an ad hoc grouping without saving it:</p>
<ul>
<li> <p>When working in a new grouping, close the beta builder.</p> </li>
<li> <p>When editing an existing grouping, select <strong>Apply</strong>.</p> </li>
</ul> </li>
<li value="9"> <p>Select <strong>Save as new</strong> for a new grouping, or <strong>Save</strong> for an existing grouping.</p> </li>
<li value="10"> <p>Type a name for the grouping.</p> </li>
<li value="11"> <p>(Optional) Select an icon for the grouping to represent the field type.</p> </li>
<li value="12"> <p>(Optional) Type a description of the grouping.</p> </li>
<li value="13"> <p>Select <strong>Save</strong>.</p> <p>The grouping is saved in the My groupings list.</p> </li>
</ol>
</div>
</div>
-->
