---
title: Supprimer les champs
description: Adobe Workfront Planning vous permet de supprimer les champs personnalisés qui ne sont plus pertinents.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 31%

---



# Supprimer des champs

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Dans Adobe Workfront Planning, vous pouvez créer des champs personnalisés pour stocker des informations sur les enregistrements.

Pour plus d’informations sur la création de champs personnalisés dans Workfront Planning, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

Vous pouvez supprimer les champs Workfront Planning qui ne sont plus pertinents.

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

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
<li><p>Tout Workfront et tout package Planning</p></li>
Ou
<li><p>Tout workflow et tout package Planning</p></li></ul>

<p><span class="preview">Pour supprimer des champs des types d’enregistrements globaux :</span></p>
<ul><li><p><span class="preview">Tout package Workfront et un package Planning Plus</span></p></li>
Ou
<li><p><span class="preview">Tous les packages Prime et Ultimate de workflow et de planification</span></p></li></ul>

<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations d’un espace de travail</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

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
   <td><p> Standard </p>
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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Remarques concernant la suppression de champs Workfront Planning :

* Vous ne pouvez supprimer un champ que dans la vue Tableau du type d’enregistrement.
* Vous ne pouvez pas supprimer le champ principal d’un enregistrement.
* Toutes les informations stockées dans le champ sont supprimées et ne peuvent pas être récupérées.
* Lorsque vous supprimez un champ d’enregistrement connecté, tous les champs de recherche connectés sont également supprimés du type d’enregistrement auquel vous vous connectez. Les champs d’enregistrement connectés des types d’enregistrement auxquels vous vous connectez sont également supprimés de l’enregistrement auquel vous vous connectez.

  Par exemple, lorsque vous connectez des campagnes à un autre type d’enregistrement appelé Produit et que vous supprimez le champ Produit connecté et le champ de recherche Statut du produit de la campagne, les éléments suivants sont supprimés :

   * Le champ Produit connecté de la campagne
   * Le champ de recherche Statut du produit de la campagne
   * Le champ connecté à Campaign à partir du produit

  Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* <span class="preview">Vous ne pouvez pas supprimer des champs des enregistrements globaux qui ont été ajoutés à un espace de travail secondaire à partir des espaces de travail secondaires.</span>

## Supprimer des champs

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les champs d’enregistrement.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur la carte d’un type d’enregistrement.

1. (Conditionnel) S&#39;il n&#39;est pas déjà sélectionné, cliquez sur l&#39;onglet d&#39;une **vue Tableau** sur la page du type d&#39;enregistrement.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue Tableau.

1. Recherchez le champ à supprimer dans les en-têtes de colonne, pointez sur l’en-tête de colonne, puis cliquez sur la flèche pointant vers le bas située après le nom du champ.

   ![Menu fléché après le nom du champ dans l’en-tête du tableau mis en surbrillance](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Cliquez sur **Supprimer**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Cliquez sur **Supprimer** pour confirmer.

   Les champs supprimés ne peuvent pas être récupérés.

   Selon le type de champ que vous avez supprimé, voici ce qui se passe :

   * Si vous supprimez un champ qui appartient à l&#39;enregistrement que vous avez sélectionné, le champ est supprimé et ne peut plus être associé à aucun enregistrement. Si ce champ est ajouté comme champ de recherche à d&#39;autres enregistrements, ces champs sont également supprimés.
   * Si vous supprimez un champ de connexion, il est supprimé de l’enregistrement que vous avez sélectionné. En outre, le champ de connexion correspondant de son enregistrement d’origine est également supprimé.
   * Si vous supprimez un champ de recherche qui a été ajouté à partir d’un enregistrement connecté, le champ est supprimé du type d’enregistrement que vous avez sélectionné, mais il reste sur son type d’enregistrement d’origine.
   * <span class="preview">Si vous supprimez un champ d’un type d’enregistrement global dans son espace de travail principal, il est supprimé de tous les espaces de travail où ce type d’enregistrement a été ajouté. Vous ne pouvez pas supprimer des champs des types d’enregistrements globaux de leurs espaces de travail secondaires.</span>
