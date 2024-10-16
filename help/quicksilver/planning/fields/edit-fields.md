---
title: Modifier les paramètres de champ
description: Dans Adobe Workfront Planning, vous pouvez modifier les paramètres des champs déjà créés. Cet article décrit comment modifier les paramètres des champs de planification Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 46%

---


# Modifier les paramètres de champ

{{planning-important-intro}}

Vous pouvez modifier les paramètres des champs déjà créés dans Adobe Workfront Planning.

Pour plus d’informations sur la création de champs Adobe Workfront Planning, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

Cet article décrit comment modifier les paramètres des champs Workfront Planning. Pour plus d’informations sur la modification des valeurs de champ pour les enregistrements, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

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
OLD

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
   <td> <p>There are no access controls for Workfront Planning</p>  
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

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Remarques concernant la modification des paramètres de champ

Vous devez tenir compte des points suivants avant d’apporter des modifications à la configuration d’un champ :

* Vous pouvez modifier les champs que vous avez créés ou ceux créés par d’autres personnes, si vous disposez des autorisations de gestion sur l’espace de travail auquel ces champs appartiennent.
* Vous pouvez modifier un champ dans le tableau de type enregistrement.
* Vous ne pouvez pas modifier un champ sur la page d’enregistrement ni dans une autre vue, en dehors de la vue de tableau.
* Une fois le champ enregistré, vous ne pouvez plus le modifier.
* Vous ne pouvez pas désélectionner le paramètre Autoriser les nombres négatifs précédemment sélectionné pour un champ Nombre, Pourcentage ou Devise si des valeurs négatives sont déjà stockées dans les enregistrements auxquels il est joint.
* Vous pouvez modifier la configuration des éléments de champ suivants, après avoir enregistré le champ :

   * Nom ou Description d’un champ
   * Options d’un champ à sélection unique ou à sélection multiple.
   * L&#39;expression d&#39;un champ Formule.

  >[!WARNING]
  >
  >Lorsque des expressions de formule changent ou que des options sont ajoutées ou supprimées d’un champ de type sélectionné, des pertes de données sont survenues pour les enregistrements qui contiennent déjà des informations stockées dans les champs dont la configuration est modifiée.
  >
  >Il n’y a aucun avertissement ou indication que cette perte de données pourrait se produire lorsque vous modifiez la configuration des champs.
  >
  >Les autres utilisateurs ne sont pas informés que la configuration du champ a changé.

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Modifier les paramètres de champ

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez modifier les champs d’enregistrement.

   L’espace de travail s’ouvre et tous les types d’enregistrement de l’espace de travail s’affichent sur les cartes.

1. Cliquez sur la carte d’un type d’enregistrement.

   Cela ouvre la page du type d’enregistrement.

1. (Conditionnel) Cliquez sur l’onglet d’une **vue Tableau**.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue Tableau.
1. Pointez sur l’en-tête de colonne d’un champ à modifier, puis cliquez sur la flèche pointant vers le bas située après le nom du champ, puis sur **Modifier le champ**

   Ou

   Double-cliquez sur l’en-tête de colonne du champ.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Mettez à jour les informations sur le champ et cliquez sur **Enregistrer**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Une fois le champ enregistré, vous ne pouvez plus le mettre à jour.
   >
   >* Lorsque vous modifiez des configurations de champ (options de champ ou expressions de formule), les enregistrements qui contiennent déjà des informations dans les champs modifiés mettent à jour leurs valeurs en temps réel. Il n’y a aucun avertissement et aucun journal d’audit pour les modifications de valeur déclenchées par les modifications de configuration des champs. Tous les utilisateurs qui visualisent les champs verront immédiatement les nouvelles valeurs avec les modifications.

   Les informations des champs sont mises à jour pour toutes les personnes ayant accès à l’espace de travail.

1. (Le cas échéant) Pour les champs d’enregistrement liés, cliquez sur **Modifier les champs de recherche** et ajoutez ou supprimez l’un des champs du type d’enregistrement lié.

   Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

