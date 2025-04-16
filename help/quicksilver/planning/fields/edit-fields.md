---
title: Modifier les paramètres de champ
description: Dans Adobe Workfront Planning, vous pouvez modifier les paramètres des champs déjà créés. Cet article décrit comment modifier les paramètres des champs Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 594504c6a7acc9341471371ca279379042a45457
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 36%

---


# Modifier les paramètres de champ

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez modifier les paramètres des champs existants dans Adobe Workfront Planning.

Pour plus d’informations sur la création de champs Adobe Workfront Planning, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

Cet article décrit comment modifier les paramètres des champs Workfront Planning. Pour plus d’informations sur la modification des valeurs de champ pour les enregistrements, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
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
   <td>   <p>Gestion des autorisations relatives à un espace de travail <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considérations relatives à la modification des paramètres de champ

Vous devez tenir compte des points suivants avant d’apporter des modifications à la configuration d’un champ :

* Vous ne pouvez modifier les paramètres de champ qu’à partir du tableau de type d’enregistrement.
* Vous ne pouvez pas modifier un champ sur la page d’enregistrement ou dans un autre affichage, en dehors de la vue Tableau.
* Une fois le champ enregistré, vous ne pouvez plus le modifier.
* Vous ne pouvez pas désélectionner le paramètre Autoriser les nombres négatifs précédemment sélectionné pour un champ Nombre, Pourcentage ou Devise si des valeurs négatives sont déjà stockées dans les enregistrements auxquels il est joint.
* Vous pouvez modifier la configuration des éléments de champ suivants après avoir enregistré le champ :

   * Nom ou description d’un champ
   * Options d’un champ à sélection unique ou à sélection multiple.
   * Expression d’un champ de formule.

  >[!WARNING]
  >
  >Lorsque des expressions de formule sont modifiées ou que des options sont ajoutées ou supprimées dans un champ de type select, il y aura une perte de données pour les enregistrements qui contiennent déjà des informations stockées dans les champs dont la configuration est modifiée.
  >
  >Aucun avertissement ni indication que cette perte de données peut se produire lorsque vous modifiez la configuration des champs.
  >
  >Les autres utilisateurs ne sont pas informés que la configuration du champ a changé.

* Vous pouvez modifier des champs de recherche existants à partir d’enregistrements connectés.

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Modifier les paramètres de champ

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les champs d’enregistrement.

   L’espace de travail s’ouvre et tous les types d’enregistrements qu’il contient s’affichent sur des cartes.

1. Cliquez sur la carte d’un type d’enregistrement.

   Cela ouvre la page du type d’enregistrement.

1. (Conditionnel) Cliquez sur l’onglet d’une **Vue Tableau**.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue Tableau.
1. Pointez sur l’en-tête de colonne d’un champ à modifier, puis cliquez sur la flèche pointant vers le bas située après le nom du champ, puis sur **Modifier le champ**

   Ou

   Double-cliquez sur l’en-tête de colonne du champ.

   ![Menu fléché après le nom du champ dans l’en-tête du tableau mis en surbrillance](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Mettez à jour les informations sur le champ et cliquez sur **Enregistrer**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Une fois le champ enregistré, vous ne pouvez plus le mettre à jour.
   >
   >* Lorsque vous modifiez les configurations de champ (options de champ ou expressions de formule), les enregistrements qui contiennent déjà des informations dans les champs modifiés mettent à jour leurs valeurs en temps réel. Il n’existe aucun avertissement ni journal d’audit pour les modifications de valeur déclenchées par les modifications de configuration des champs. Tous les utilisateurs qui consultent les champs verront immédiatement les nouvelles valeurs avec les modifications.

   Les informations de champ sont mises à jour pour toutes les personnes ayant accès à l’affichage de l’espace de travail.

1. (Conditionnel) Pour les champs d’enregistrement connectés, cliquez sur **Modifier les champs de recherche** et ajoutez ou supprimez l’un des champs de recherche du type d’enregistrement connecté.

   Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).