---
title: Aperçu des champs de formule
description: Dans Adobe Workfront Planning, vous pouvez créer des champs de formule qui utilisent des fonctions et des champs existants pour calculer une nouvelle valeur personnalisée.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 799115d836d67a81fe69cd04c8e75014d48d2443
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 54%

---

# Vue d’ensemble des champs de formule

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez créer des champs personnalisés dans Adobe Workfront Planning en vous référant à des champs existants et en les connectant dans un champ de type Formule .

Les champs de type formule génèrent une nouvelle valeur en utilisant des valeurs existantes provenant d’autres champs d’un type d’enregistrement et une fonction qui indique comment les valeurs existantes doivent être calculées.

Pour plus d’informations, consultez la section « Formule » de l’article [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès pour Workfront Planning.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

OLD:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfornt planining</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Remarques sur les champs de formule

* Les champs de formule font référence à des champs appartenant au même type d&#39;enregistrement.
* Vous ne pouvez référencer des champs d&#39;autres types d&#39;enregistrements que lorsque vous connectez un autre type d&#39;enregistrement à celui pour lequel vous créez un champ de formule.
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

## Formules prises en charge

Les champs de formule Adobe Workfront Planning prennent en charge la plupart des expressions des champs calculés Workfront.

<!-- make the note available when WF releases the expressions listed in it: 

>[!NOTE]
>
>The following Workfront expressions are not supported for Workfront Planning formula fields: 
>
>* SORTASCARRAY
>* SORTDESCARRAY
>* ADDHOUR
>* SWITCH
>* FORMAT
-->

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
   <td><strong>TABLEAU</strong> </td>
   <td> <p>Convertit une chaîne en tableau. Le délimiteur peut être n’importe quelle chaîne.</p>
   <p>L’expression est formatée comme suit :</p>
   <p><code>ARRAY(string1, "delimiter")</code></p>
   </td>
  </tr>
  <tr>
   <td><strong>ARRAYELEMENT</strong> </td>
   <td> <p>Renvoie l’élément au nombre spécifié dans le tableau . Si l’index est hors limites, il renvoie vide.</p>
   <p>L’expression est formatée comme suit :</p>
   <p><code>ARRAYELEMENT(array, number)</code></p>
   </td>
  </tr>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Renvoie une chaîne concaténée par délimiteur.</p> <p>L’expression est formatée comme suit :

<code>ARRAYJOIN(delimiter,array)</code>
</p>
   </td></tr>
  <tr>
   <td><strong>ARRAYLENGTH</strong> </td>
   <td> <p>Renvoie le nombre d’éléments dans le tableau et est formaté comme suit :</p>
   <p><code>ARRAYLENGTH(array)</code></p>
   </td>
  </tr>

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
