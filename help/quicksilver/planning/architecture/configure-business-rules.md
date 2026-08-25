---
title: Configurer les règles métier de type d’enregistrement
description: Vous pouvez configurer des règles métier de type enregistrement qui définissent la manière dont les enregistrements de ce type sont gérés dans Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 159b845c7b755117197d18f8474c01d4b19d53b8
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 14%

---


# Configurer des règles métier de type enregistrement

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Vous pouvez configurer des règles métier de type enregistrement qui définissent la manière dont les enregistrements de ce type sont gérés dans Adobe Workfront Planning.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès afin d’effectuer les étapes de cet article :  

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
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Tout Workfront ou workflow avec un package Planning</p></li>
Ou
<li><p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Norme de workflow</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Norme de planification</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations sur un espace de travail et sur un type d’enregistrement</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant la configuration des règles métier

* Vous pouvez configurer des règles indiquant à quel moment les enregistrements peuvent être modifiés ou supprimés.
* Vous ne pouvez pas configurer de règles pour le moment où les enregistrements sont créés. Toute personne disposant d’autorisations de niveau Gérer pour le type d’enregistrement peut créer des enregistrements.
* Vous pouvez créer une condition pour votre règle métier qui fait référence à tous les types de champ, à l’exception des suivants :
  * Champs de formule
  * Champs de recherche
  * Champs de référence

## Configuration des règles métier

1. Accédez à un type d’enregistrement.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur Règles métier.



