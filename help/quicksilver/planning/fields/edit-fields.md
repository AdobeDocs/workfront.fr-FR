---
title: Modifier les paramètres de champ
description: Dans Adobe Workfront Planning, vous pouvez modifier les paramètres des champs déjà créés. Cet article décrit comment modifier les paramètres des champs de planification Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: dc8e6f730ec88fc66c3486987e064b5f0760fb80
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 50%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit fields
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Modifier les paramètres de champ

{{planning-important-intro}}

Vous pouvez modifier les paramètres des champs déjà créés dans Adobe Workfront Planning.

Pour plus d’informations sur la création de champs Adobe Workfront Planning, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

Cet article décrit comment modifier les paramètres des champs Workfront Planning. Pour plus d’informations sur la modification des valeurs de champ pour les enregistrements, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

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
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Nouvelle : standard</p>
   <p>Actuelle : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Workfront Planning</p>  
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

Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Remarques concernant la modification des paramètres de champ

Vous devez tenir compte des points suivants avant d’apporter des modifications à la configuration d’un champ :

* Vous pouvez modifier les champs que vous avez créés ou créés par d’autres utilisateurs et utilisatrices, si vous disposez des autorisations de gestion sur l’espace de travail auquel ces champs appartiennent.
* Vous pouvez modifier un champ dans le tableau de type enregistrement.
* Vous ne pouvez pas modifier un champ sur la page d’enregistrement ni dans une autre vue, en dehors de la vue de tableau.
* Une fois le champ enregistré, vous ne pouvez pas modifier son type.
* Vous ne pouvez pas désélectionner le paramètre Autoriser les nombres négatifs précédemment sélectionné, pour un champ Nombre, Pourcentage ou Devise si des valeurs négatives sont déjà stockées dans les enregistrements auxquels il est rattaché.
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

   La page du type d’enregistrement s’affiche.

1. (Conditionnel) Cliquez sur l’onglet d’une **vue Tableau**.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue du tableau.
1. Pointez sur l’en-tête de colonne d’un champ à modifier, cliquez sur la flèche pointant vers le bas située après le nom du champ, puis cliquez sur **Modifier un champ**.

   Ou

   Double-cliquez sur l’en-tête de colonne du champ.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Mettez à jour les informations sur le champ et cliquez sur **Enregistrer**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Une fois le champ enregistré, vous ne pouvez pas mettre à jour son type.
   >
   >* Lorsque vous modifiez des configurations de champ (options de champ ou expressions de formule), les enregistrements qui contiennent déjà des informations dans les champs modifiés mettent à jour leurs valeurs en temps réel. Il n’y a aucun avertissement et aucun journal d’audit pour les modifications de valeur déclenchées par les modifications de configuration des champs. Tous les utilisateurs qui visualisent les champs verront immédiatement les nouvelles valeurs avec les modifications.

   Les informations des champs sont mises à jour pour toutes les personnes ayant accès à l’espace de travail.

1. (Le cas échéant) Pour les champs d’enregistrement liés, cliquez sur **Modifier les champs de recherche** et ajoutez ou supprimez l’un des champs du type d’enregistrement lié.

   Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

