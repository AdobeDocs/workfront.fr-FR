---
title: Vue d’ensemble des champs de formule
description: Dans Adobe Workfront Planning, vous pouvez créer des champs de formule qui utilisent des fonctions et des champs existants pour calculer une nouvelle valeur personnalisée.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 7580c7638c9e4d0f9aa53d208d9773fa1524ab54
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 86%

---

# Vue d’ensemble des champs de formule

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--this article is linked to the UI in the formula box, "Learn more..."-->

<!---
title: Formula fields overview
description: In Adobe Workfront Planning, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

Vous pouvez créer des champs personnalisés dans la Planification Adobe Workfront en vous référant à des champs existants et en les reliant dans un champ de type Formule .

Les champs Formule génèrent une nouvelle valeur en utilisant les valeurs existantes d’autres champs d’un type d’enregistrement et une fonction qui indique comment les valeurs existantes doivent être calculées.

Pour plus d’informations, reportez-vous à la section &quot;Formule&quot; de l’article [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite à l’étape d’accès anticipé pour la planification Workfront </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>N’importe quelle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe pas de contrôle d’accès pour Workfront Planning.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gérer les autorisations d’un espace de travail</a> </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Votre administrateur ou administratrice Workfront ou de groupes doit ajouter la zone Planning dans votre modèle de disposition. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Vue d’ensemble des accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## Considérations relatives aux champs de formule

* Les champs de formule font référence à des champs qui appartiennent au même type d&#39;enregistrement. Vous ne pouvez pas référencer des champs d’autres types d’enregistrements lors de la création d’un champ de formule. <!--is this still accurate??-->
* Une fois enregistré, vous ne pouvez pas modifier le type de champ d&#39;un champ Formule.
* Vous pouvez mettre à jour le calcul d’un champ de formule après l’avoir enregistré, et les résultats du calcul sont automatiquement mis à jour pour tous les enregistrements du même type.
* Vous devez ajouter les champs que vous référencez dans les formules tel qu’ils s’affichent dans l’interface de Workfront Planning.

## Formules prises en charge

Les champs de formule Adobe Workfront Planning prennent en charge toutes les expressions des champs calculés Workfront. Pour plus d’informations, voir [Vue d’ensemble des expressions de données calculées](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Nous prenons également en charge les expressions suivantes pour les champs de formule Workfront Planning :

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
   <td> <p>Renvoie une chaîne concaténée par délimiteur.</p> <p>L’expression est mise en forme comme suit :

<code>ARRAYJOIN(délimiteur,tableau)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Renvoie un tableau avec des valeurs uniques.</p> <p>L’expression est mise en forme comme suit :

<code>ARRAYUNIQUE(tableau)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Renvoie l’ID d’un enregistrement. Chaque enregistrement possède un ID unique.</p> <p>L’expression est mise en forme comme suit :

<code>{ID}</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Définit le fuseau horaire d’une date et d’une heure sur un fuseau horaire spécifique.</p> <p>L’expression est mise en forme comme suit :

<code>SETTIMEZONE(date, « Amérique/Los_Angeles »)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Renvoie le numéro de la semaine dans une année. Vous pouvez éventuellement indiquer le jour de début de la semaine (utilisez 1 pour dimanche ou 2 pour lundi). Si cette option est omise, les semaines commencent le dimanche, par défaut.</p> <p>L’expression est mise en forme comme suit :

<code>WEEKOFYEAR(date,2)</code>
ou
<code>WEEKOFYEAR(date)</code>
</p>
   </td></tr>

</table>
