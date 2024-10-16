---
title: Supprimer des champs
description: Adobe Workfront Planning vous permet de supprimer les champs personnalisés qui ne sont plus pertinents.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 56%

---



# Supprimer des champs

{{planning-important-intro}}

Dans Adobe Workfront Planning, vous pouvez créer des champs personnalisés pour stocker des informations sur les enregistrements.

Pour plus d’informations sur la création de champs personnalisés dans Workfront Planning, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

Vous pouvez supprimer les champs Workfront Planning qui ne sont plus pertinents.

## Remarques concernant la suppression de champs Workfront Planning :

* Vous ne pouvez supprimer un champ que dans la vue Tableau du type d’enregistrement.
* Vous ne pouvez pas supprimer le champ principal d’un enregistrement.
* Toutes les informations stockées dans le champ sont supprimées et ne peuvent pas être récupérées.
* Lorsque vous supprimez un champ d’enregistrement connecté, tous les champs de recherche connectés sont également supprimés du type d’enregistrement duquel vous vous connectez. Les champs d’enregistrement connectés des types d’enregistrement auxquels vous vous connectez sont également supprimés de l’enregistrement auquel vous vous connectez.

  Par exemple, lorsque vous connectez des campagnes à un autre type d’enregistrement appelé produit et que vous supprimez le champ Produit connecté et le champ de recherche État du produit de la campagne, les éléments suivants sont supprimés :

   * Le champ Produit connecté de l&#39;opération
   * Champ de recherche de l’état du produit de la campagne
   * Le champ Campaign connecté du produit.

  Pour plus d’informations, voir [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

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
<p>L’un des projets Workfront suivants est prévu :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Formule de planification Adobe Workfront*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p> 
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
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Supprimer des champs

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les champs d’enregistrement.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur la carte d’un type d’enregistrement.

1. (Conditionnel) Si cette option n’est pas déjà sélectionnée, cliquez sur l’onglet d’une **vue Tableau** sur la page de type enregistrement.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue Tableau.

1. Recherchez le champ à supprimer dans les en-têtes de colonne, pointez sur l’en-tête de colonne, puis cliquez sur la flèche pointant vers le bas située après le nom du champ.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Cliquez sur **Supprimer**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Cliquez sur **Supprimer** pour confirmer.

   Le champ est supprimé, ne peut pas être récupéré et ne peut plus être associé à aucun enregistrement.
