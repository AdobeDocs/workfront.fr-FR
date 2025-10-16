---
title: Aperçu des champs de formule
description: Dans Adobe Workfront Planning, vous pouvez créer des champs de formule qui utilisent des fonctions et des champs existants pour calculer une nouvelle valeur personnalisée.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 29%

---

# Vue d’ensemble des champs de formule

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Vous pouvez créer des champs personnalisés dans Adobe Workfront Planning en vous référant à des champs existants et en les connectant dans un champ de type Formule .

Les champs de type formule génèrent une nouvelle valeur en utilisant des valeurs existantes provenant d’autres champs d’un type d’enregistrement et une fonction qui indique comment les valeurs existantes doivent être calculées.

Pour plus d’informations, consultez la section « Formule » de l’article [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

<!--do we need these for an overview article?

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront and any Planning package</p>
<p>Any Workflow and any Planning package</p>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

-->

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

## Remarques sur les champs de formule

* Les champs de formule font référence à des champs appartenant au même type d&#39;enregistrement.
* Vous ne pouvez référencer des champs d&#39;autres types d&#39;enregistrements que lorsque vous connectez un autre type d&#39;enregistrement à celui pour lequel vous créez un champ de formule.
* Le référencement des types d’enregistrements connectés ou de leurs champs de recherche dans une formule dépend de vos autorisations sur les types d’enregistrements connectés. Si vous ne disposez pas des autorisations nécessaires pour afficher le type d’enregistrement, vous ne pouvez pas référencer leurs champs dans une formule.
* Vous ne pouvez pas modifier le type de champ d&#39;un champ de formule après l&#39;avoir enregistré.
* Vous pouvez mettre à jour le calcul d’un champ de formule après l’avoir enregistré, et les résultats du calcul sont automatiquement mis à jour pour tous les enregistrements du même type.
* Vous devez ajouter les champs que vous référencez dans les formules tel qu’ils s’affichent dans l’interface de Workfront Planning.
* Vous ne pouvez référencer que les champs qui s&#39;affichent dans la vue Tableau d&#39;un type d&#39;enregistrement ou dans la page Détails de l&#39;enregistrement.
* Vous pouvez définir le format de la valeur d&#39;un calcul de formule en choisissant parmi les options de format suivantes :

   * Texte
   * Nombre
   * Pourcentage
   * Devise
   * Balises
   * Date

  Pour plus d’informations, consultez la section « Formule » de l’article [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).
* Vous pouvez référencer des champs de formule dans de nouvelles formules. Une fois que la valeur est mise à jour dans un champ référencé dans un champ de formule, tous les champs suivants référençant ce champ ou les champs de formule qui contiennent ce champ sont automatiquement mis à jour.

* Lorsque vous mettez à jour un champ de formule ou un champ susceptible de l’impacter, une alerte vous informe de l’impact de votre modification. L’alerte s’affiche dans les cas suivants :

   * Lorsque vous mettez à jour un champ de formule (à l’exclusion des modifications de nom et de description) lorsque ce champ comporte des champs de formule ou de recherche dépendants. L’alerte répertorie ces champs dépendants et vous demande si vous souhaitez continuer.

   * Lorsque vous supprimez un champ utilisé dans une expression de formule ou comme champ de recherche. L’alerte répertorie la formule dépendante et les champs de recherche et vous demande si vous souhaitez continuer la suppression.

## Limites des champs de formule

* Vous pouvez ajouter un maximum de 20 champs de formule pour un type d’enregistrement.

  Les champs de recherche de formule ajoutés à partir des types d’enregistrements connectés ne sont pas comptabilisés par rapport à cette limite.

* L’expression de la formule ne peut pas dépasser 50 000 caractères.

* Les champs de formule peuvent s’afficher comme `#ERROR!` dans les cas suivants :
   * Lorsqu’un champ utilisé dans une formule est supprimé.
   * Lorsqu’un champ utilisé dans un champ de recherche agrégé s’affiche sous la forme `#ERROR!`.

     Par exemple, si vous affichez un champ de recherche qui contient des champs de formule de recherche agrégés et que l&#39;un des champs de formule référencés s&#39;affiche sous la forme `#ERROR!`.
   * Lorsqu’une valeur de formule ne peut pas être affichée au format sélectionné.

     Par exemple, si je sélectionne Nombre pour le Format d&#39;un champ de formule et que les champs utilisés dans la formule sont des champs de texte qui affichent uniquement des valeurs non numériques, le résultat de la formule s&#39;affichera sous la forme `#ERROR!`, car il ne peut pas analyser le texte en un nombre.


## Formules prises en charge

Les champs de formule Adobe Workfront Planning prennent en charge la plupart des expressions des champs calculés Workfront.

>[!NOTE]
>
>Les expressions Workfront ci-dessous ne sont pas prises en charge pour les champs de formule Workfront Planning :
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* SWITCH
>* FORMAT

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Pour obtenir une liste complète des expressions Workfront, voir [Présentation des expressions de données calculées](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

En outre, nous prenons en charge les expressions suivantes pour les champs de formule Workfront Planning. Les expressions suivantes ne sont pas prises en charge pour les expressions Workfront :

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expression...</th> 
   <th>Explication et exemple</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Renvoie une chaîne concaténée par délimiteur.</p> <p>L’expression est formatée comme suit :

<code>ARRAYJOIN(delimiter,array)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Renvoie un tableau avec des valeurs uniques.</p> <p>L’expression est formatée comme suit :

<code>ARRAYUNIQUE(array)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Renvoie l’ID d’un enregistrement. Chaque enregistrement possède un ID unique.</p> <p>L’expression est formatée comme suit :

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong> JSONELEMENT </strong> </td> 
   <td> <p>Renvoie les données du fichier JSON en fonction du chemin JSONP fourni. Si le JSONPath n’existe pas dans le fichier JSON, un résultat vide est renvoyé. </p> <p>L'expression est formatée comme suit :
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Définit le fuseau horaire d’une date et d’une heure sur un fuseau horaire spécifié.</p> <p>L’expression est formatée comme suit :

<code>SETTIMEZONE(date, &#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Renvoie le numéro de la semaine dans une année. Vous pouvez éventuellement indiquer le jour de début de la semaine (utilisez 1 pour dimanche ou 2 pour lundi). Si cette option est omise, les semaines commencent le dimanche, par défaut.</p> <p>L’expression est formatée comme suit :

<code>WEEKOFYEAR(date,2)</code>
ou
<code>WEEKOFYEAR(date)</code>
</p>
   </td></tr>

</table>
