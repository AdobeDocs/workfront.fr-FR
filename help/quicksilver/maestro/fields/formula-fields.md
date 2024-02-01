---
title: Champs de formule - Aperçu
description: Dans Adobe Maestro, vous pouvez créer des champs de formule qui utilisent des fonctions et des champs existants pour calculer une nouvelle valeur personnalisée.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---


# Champs de formule - Aperçu

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!---
title: Formula fields overview
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{maestro-important-intro}}

Vous pouvez créer des champs personnalisés dans Adobe Maestro en faisant référence à des champs existants et en les reliant par une formule. Pour ce faire, créez un champ personnalisé de type Formule .

Les champs de formule génèrent une nouvelle valeur en utilisant les valeurs existantes d&#39;autres champs d&#39;un type d&#39;enregistrement et une fonction qui indique comment les valeurs existantes doivent être calculées.

Pour plus d’informations, voir [Créer des champs](../fields/create-fields.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé Adobe Maestro. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Quelconque</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Quelconque</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## Observations relatives aux champs de formule

* Les champs de formule font référence à des champs qui appartiennent au même type d&#39;enregistrement. Vous ne pouvez pas référencer des champs d’autres types d’enregistrement lors de la création d’un champ de formule. <!--is this still accurate??-->
* Une fois enregistré, vous ne pouvez pas modifier le type de champ d&#39;un champ Formule.
* Vous pouvez mettre à jour le calcul d&#39;un champ de formule après son enregistrement, et les résultats du calcul sont automatiquement mis à jour pour tous les enregistrements du même type.
* Vous devez ajouter les champs que vous référencez dans les formules telles qu’elles s’affichent dans l’interface Maestro.
* L’utilisation des champs de recherche des types d’enregistrement liés dans une formule sera disponible ultérieurement.

## Formules prises en charge

Les champs de formule Maestro prennent en charge toutes les expressions des champs calculés Workfront. Pour plus d’informations, voir [Présentation des expressions de données calculées](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

En outre, nous prenons en charge les expressions suivantes pour les champs de formule Maestro :

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
   <td> <p>Renvoie une chaîne concaténée par délimiteur.</p> <p>L’expression est formatée comme suit :

<code>ARRAYJOIN(délimiteur,tableau)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Renvoie un tableau avec des valeurs uniques.</p> <p>L’expression est formatée comme suit :

<code>ARRAYUNIQUE(array)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Renvoie l’identifiant d’un enregistrement. Chaque enregistrement possède un identifiant unique.</p> <p>L’expression est formatée comme suit :

<code>{ID}</code>
</p>
   </td></tr>

<tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Définit le fuseau horaire d’une date et d’une heure sur un fuseau horaire spécifique.</p> <p>L’expression est formatée comme suit :

<code>SETTIMEZONE(date,&#39;Amérique/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFAN</strong> </td> 
   <td> <p>Renvoie le numéro de la semaine dans une année. Vous pouvez éventuellement indiquer le jour de la semaine qui commence (utilisez 1 pour le dimanche ou 2 pour le lundi). Si cette option est activée, les semaines commencent le dimanche, par défaut.</p> <p>L’expression est formatée comme suit :

<code>WEEKOFYEAR(date,2)</code>
ou
<code>WEEKOFYEAR(date)</code>
</p>
   </td></tr>

</table>





