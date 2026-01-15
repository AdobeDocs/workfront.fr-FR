---
title: Modifier les paramètres de champ
description: Dans Adobe Workfront Planning, vous pouvez modifier les paramètres des champs déjà créés. Cet article décrit comment modifier les paramètres des champs Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 22%

---


# Modifier les paramètres de champ

<!--leave the choice value information in yellow till January 2026-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez modifier les paramètres des champs existants dans Adobe Workfront Planning.

Pour plus d’informations sur la création de champs Adobe Workfront Planning, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

Cet article décrit comment modifier les paramètres des champs Workfront Planning. Pour plus d’informations sur la modification des valeurs de champ pour les enregistrements, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

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
<p>Tout Workfront et tout package Planning</p> <p>Tout workflow et tout package Planning</p>
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
   <td>   <p>Manage permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Considérations relatives à la modification des paramètres de champ

Vous devez tenir compte des points suivants avant d’apporter des modifications à la configuration d’un champ :

* Vous ne pouvez modifier les paramètres de champ qu’à partir du tableau de type d’enregistrement.
* Vous ne pouvez pas modifier les paramètres d’un champ sur la page d’enregistrement ou dans tout autre affichage, en dehors de la vue Tableau.
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
* Outre la modification du champ décrite dans la section [Modifier les paramètres de champ](#edit-field-settings-1) de cet article, vous pouvez modifier les choix d’un champ à sélection unique ou multiple lorsque vous modifiez un enregistrement dans la vue Tableau, au fur et à mesure que vous mettez à jour les valeurs de champ. Pour plus d&#39;informations, reportez-vous à la section [&#x200B; Ajouter de nouveaux choix à un champ de sélection existant lors de la modification d&#39;enregistrements en mode Tableau &#x200B;](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view) de cet article.

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

1. Mettez à jour les informations sur le champ et cliquez sur **Enregistrer**.

   Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Une fois le champ enregistré, vous ne pouvez plus le mettre à jour.
   >
   >* Lorsque vous modifiez les configurations de champ (options de champ ou expressions de formule), les enregistrements qui contiennent déjà des informations dans les champs modifiés mettent à jour leurs valeurs en temps réel. Il n’existe aucun avertissement ni journal d’audit pour les modifications de valeur déclenchées par les modifications de configuration des champs. Tous les utilisateurs qui consultent les champs verront immédiatement les nouvelles valeurs avec les modifications.

   Les informations de champ sont mises à jour pour toutes les personnes ayant accès à l’affichage de l’espace de travail.

1. (Conditionnel) Pour les champs d’enregistrement connectés, cliquez sur **Modifier les champs de recherche** et ajoutez ou supprimez l’un des champs de recherche du type d’enregistrement connecté.

   Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).


## Ajouter de nouveaux choix à un champ de sélection existant lors de la modification d’enregistrements en mode Tableau

<!--some of this information is also available in Edit records article - update both when necessary-->

Vous pouvez ajouter de nouveaux choix à un champ à sélection unique ou multiple existant lors de la modification d’enregistrements en mode Tableau.

>[!IMPORTANT]
>
>La fonctionnalité décrite dans cette section n’est disponible que dans la vue Tableau. Il n’est disponible dans aucune autre zone où des champs à sélection unique ou multiple s’affichent.

**EXEMPLE**

Vous pouvez avoir un champ à sélection unique appelé Statut qui comporte les choix Nouveau et Fermé, et vous souhaitez ajouter un choix pour un statut En cours . Vous pouvez ajouter ce choix en effectuant l’une des opérations suivantes :

* Modification du champ. Pour plus d’informations, consultez la section [Modifier les paramètres de champ](#edit-field-settings-1) de cet article.
* Ajout d’une nouvelle option lors de la modification de l’enregistrement en mode Tableau, comme décrit ci-dessous.

Pour ajouter un nouveau choix à un champ de sélection existant lors de la modification d’un enregistrement :

1. Accédez à une page de type d’enregistrement et ouvrez la vue Tableau .
1. Ajoutez le champ à sélection unique ou multiple auquel vous souhaitez ajouter un choix en mode Tableau sous la forme d’une nouvelle colonne. Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).
1. Commencez à modifier le champ en ligne en double-cliquant sur la cellule du champ.
1. Saisissez le nom du choix à ajouter, puis cliquez sur **Ajouter un choix**.

   ![Ajouter un choix dans un champ à sélection unique en mode Tableau](assets/add-choice-in-table-view-for-single-select-field.png)

   Le nouveau choix est ajouté immédiatement au champ à sélection unique.

   Une nouvelle valeur est également ajoutée à chaque choix. Vous pouvez utiliser les valeurs de choix dans les appels API ou d’autres intégrations. Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

