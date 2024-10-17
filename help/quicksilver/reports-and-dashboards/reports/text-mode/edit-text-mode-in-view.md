---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modifier une vue en mode texte
description: 'NOTE : ajoutez une section dans cet article : /Content/Reports and Dashboard/Reports/Reporting Elements/create-customize-views.html *** Également, faites un brouillon de cette zone dans l’article Vue d’ensemble du mode Texte )'
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 96%

---

# Modifier une vue en mode texte

<!--Audited: 01/2024-->

<!--
<add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

Vous pouvez modifier une vue dans une liste ou un rapport à l’aide du mode Texte pour accéder à des champs qui ne sont pas disponibles dans l’interface standard et créer des vues plus complexes.

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
   <td> <p>Nouveau : Standard </p>
   <p>Actuel : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux rapports, aux tableaux de bord et aux calendriers pour la modification des éléments de rapport dans un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion à un rapport pour modifier les vues d’un rapport</p> <p>Gérer les autorisations d’une vue pour la modifier</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.
Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer à utiliser le mode texte dans un rapport ou une liste, assurez-vous toujours de bien connaître la syntaxe du mode texte Workfront.

Pour plus d’informations, voir :

* [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Vue d’ensemble de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exemples de vues, de filtres et de regroupements personnalisés : index des articles](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modifier le mode Texte dans une vue

La modification d’une vue en mode Texte est identique pour les rapports et les listes.L’accès à la vue depuis un rapport ou depuis une liste diffère.

>[!TIP]
>
>Nous vous recommandons de créer autant de la vue que possible en mode standard, puis de la convertir en mode Texte pour l’éditer.

Pour plus d’informations sur la création de vues, voir [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Utilisez l’une des méthodes suivantes :

   1. Pour accéder à la vue depuis un rapport, accédez au rapport, puis cliquez sur l’onglet **Actions de rapport** > **Modifier** > **Colonnes (affichage)**.
   1. Pour accéder à la vue depuis une liste, accédez à la liste. Depuis le menu déroulant **Affichage**, placez le pointeur de la souris sur la vue à modifier, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png).

      Le créateur de vues s’ouvre.

1. Sélectionnez une colonne dans la vue.

   Ou

   Sélectionnez l’onglet **Colonnes (vue)** du créateur de rapports, puis sélectionnez une colonne.

   >[!TIP]
   >
   >Pour modifier une vue en mode Texte, vous devez modifier une colonne à la fois.

1. Cliquez sur **Passer en mode Texte** dans le coin supérieur droit du créateur, puis cliquez sur **Modifier le mode Texte**.

   >[!NOTE]
   >
   >Lorsque vous modifiez une colonne en mode Texte, Workfront ajoute la ligne de code `textmode=true` à la colonne. Cela indique que la colonne est modifiée en mode Texte.

   Le tableau suivant décrit les lignes clés dans une vue en mode Texte :

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Exemple de ligne</th> 
      <th>Description</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><ol><tr><tr><ol><tr><tr><tr><tr><tr><tr><tr><tr><tr><tr><div class="example" data-mc-autonum="<b>Example: </b>"><code><strong>valuefield</strong>=</cod></p> </td> 
      <td> <p>This is the name of the object or of the field as it appears in the database. For more information about how objects and fields appear in the database, see <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>The following scenarios exist:</p> 
        
        <li value="1"> <p> If the name of the field you display is a phrase instead of a single noun, you must use camel case syntax for the <code>valuefield</code>. For example, for the Planned Start Date of a task the code is: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>If you want to display a custom field, the <code>valuefield</code> value is the actual name of the field, as you see it in the interface. For example, for a custom field named "More information", the code is:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>If you want to display objects that are related to other objects in a view using the <code>valuefield</code> line of code the object names and attributes are separated by colons. </p> <p>For example, a column in a task view that would display the name of the Portfolio Owner has the following value for the valuefield line:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>This indicates that from the object of the report (task), you can access the next related object (project), from there, you can access the following related object from project (portfolio), then the portfolio owner (owner) and then their name (name). </p> </li> 
       </ol> <p>For information about how objects connect to one another, see the section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependency and hierarchy of objects</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>.</p> <p>Note: If you choose a field in text mode that is not valid in the standard interface, you are not able to switch back to the standard interface within the column.</p> </td> 
     </tr> 
      
      <td><code><strong>valueformat=</strong></code> </td> 
      <td> <p>This line represents the format used to display the <code>valuefield</code>. The <code>valueformat</code> identifies whether an object or field displays as text, number, percentage, or date.</p> <p>We recommend using <code>HTML</code> for your <code>valueformat</code>, especially when using <code>valueexpression</code>, to ensure the most accurate display of your information. </p> <p>For information about additional values for this line, see <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Use conditional formatting in Text Mode</a>.</p> </td> 
     </tr> 
      
      <td> <p><code><strong>valueexpression=</strong></code> </p> </td> 
      <td> <p>You can add this line to replace <code>valuefield</code>, if you want to display a calculated field in the column.</p> <p>You must enclose the <code>valuefield</code> of the objects in curly brackets every time you use it in a <code>valueexpression</code>.</p> <p>The following scenarios exist: </p> 
        
        <li value="1"> <p>If you want to display a field in a column in upper case, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> of the object is spelled as it appears in the API Explorer. </p> </li> 
        <li value="2">If you want to add multiple <code>valuefields</code> by stringing them together, you must separate them by a period.</li> 
        <li value="3"> <p>For example, if you want to display the name of the Primary Assignee of a task using <code>valueexpression</code>, you would use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>If you want to use a custom field in a <code>valueexpression</code> line you must precede the name of the field by <code>DE:</code> to indicate that it is a custom field. The name of the field is spelled as it appears in the interface. </p> <p>Important: When you use a custom field that is placed in a custom form section that has restricted permissions for some users, the calculation of the valueexpression is blank when those users view this calculation in a report. For information about adjusting permissions on custom form sections, see <span help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Design a form with the form designer</a></span>.</p> <p>For example, if you have a custom field labeled "Developer Name" and you want to display this field in upper case in a column, you can use the following <code>valueexpression</code> to indicate this:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>When referencing a Typeahead type custom field, use the following expression to reference the name of the object selected in a field labeled "Developer Name":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
      
      <td> <p><code><strong>descriptionkey=</strong></code> / <code><strong>description=</strong></code> </p> </td> 
      <td> <p>This line defines the text of a tool tip as you mouse over the name of the column. In this case it is using a key to translate the name value in the description text. If you want to modify the description, change this line to read: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
      
      <td><code><strong>namekey=</code> / <code><strong>name=</strong></code> </td> 
      <td> <p>This line defines the column label. In this case it is using the abbreviated value based on the key.</p> <p>If you want to modify the column name you can change this value to: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> allows you to enter any text for the column name, while<code>namekey</code> requires you enter a key that is used to translate the name of a column.</p> <p>To change the column name you can also add the <code>displayname </code>line, if one is not present.</p> </td> 
     </tr> 
      
      <td><code><strong>displayname =</strong></code> </td> 
      <td> <p>You can add the following line to change the name of a column, which suspends the <code>namekey/name</code> value:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
      
      <td><code><strong>querysort=</strong> </code></td> 
      <td>This line defines how the results are sorted when the column header is clicked. If it is not present then the column cannot be sorted after the report is run.</td> 
     </tr> 
      
      <td><code><strong>width=</strong></code> </td> 
      <td> <p>This line represents the number of pixels that are used for the column. If the line is omitted or set to 0 (zero) then the column does not appear in the view.</p> <p>When you modify this field manually in text mode, you must also add the <code>usewidths=true</code> value to your column.</p> </td> 
     </tr> 
      
      <td><code><strong>usewidths=true</strong></code> </td> 
      <td> <p>You must use this line in addition to the <code>width=</code> line when customizing the width of a column. </p> </td> 
     </tr> 
      
      <td><code><strong>makeFieldEditable=</strong></code> </td> 
      <td> <p>This line defines whether the value displayed in a column is inline editable or not. If this line equals <strong>true</strong>, the value in the column is inline editable. If this line equals <code>false</code>, the value in the column is not inline editable.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valuefield=</strong> </code></td> 
      <td> <p>Insert this line only when you want the value displayed in a column to link to the object associated with it. The link opens the details page of the object. This value should match the <code>valuefield=</code> line. When you insert this, you must also add the <code>link.valueformat=</code> line. </p> <p> For example, you can insert <code>link.valuefield=priority</code> in an issue view, and the Priority of the issue displays as a link. Clicking this link opens the Issue page.</p> </td> 
     </tr> 
      
      <td><code><strong>link.valueformat=</strong> </code></td> 
      <td> <p>Insert this line only when you have inserted the <code>link.valuefield</code> line to add a link to the value in a column. The link opens the details page of the object. This value should match the <code>valueformat=</code> line and indicates the format used to display the <code>valuefield</code>. </p> <p>Important: When viewing the text mode in a built-in column that also includes a link, you notice a number of lines referring to the link. Some of those lines might no longer be supported or are unnecessary when you create your own custom column in text mode and add the link statements to it. The lines that are mandatory when adding a linked value are<code> link.valuefield</code> and <code>link.valueformat</code>. </p> </td> 
     </tr> 
      
      <td><code><strong>aggregator.function=</strong></code> </td> 
      <td> <p>This refers to how the values of each column are summarized. There are multiple lines that start with <code>aggregator.</code> and they all refer to the aggregator that summarizes the results of the column. </p> <p>As a general rule, the <code>aggregator.</code> lines match those of the column object. </p> 
       
        <span class="autonumber"><span><b>Example: </b></span></span> 
        <p>The Planned&nbsp;Hours column in a task report summarized by Sum may look like the following: </p>

   <div>
         <code>textmode=true</code>
         <code>valuefield=workRequired</code>
         <code>valueformat=compound</code>
         <code>aggregator.function=SUM</code>
         <code>aggregator.valuefield=workRequired</code>
         <code>aggregator.displayformat=minutesAsHoursString</code>
         <code>aggregator.valueformat=compound</code>
         <code>namekey=workRequired</code>
         <code>shortview=false</code> 
        </div> 
       </div>

   <div>
      Les lignes <code>aggregator. </code> peuvent contenir un <code>valuefield </code> ou <code>valueexpression</code>.
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Appliquer** si vous souhaitez enregistrer vos modifications et continuer à modifier la vue.
1. Cliquez sur **Enregistrer + Fermer** pour enregistrer votre rapport.

   Ou

   Cliquez sur **Enregistrer la vue** pour enregistrer la vue dans une liste.
