---
title: Modifier des champs
description: Dans Adobe Workfront Planning, vous pouvez modifier les paramètres des champs déjà créés. Cet article décrit comment modifier les paramètres des champs de planification Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 6%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Modifier des champs

{{planning-important-intro}}

Vous pouvez modifier les paramètres des champs déjà créés dans Adobe Workfront Planning.

Pour plus d’informations sur la création de champs de planification Adobe Workfront, voir [Créer des champs](../fields/create-fields.md).

Cet article décrit comment modifier les paramètres des champs de planification Workfront. Pour plus d’informations sur la modification des valeurs de champ pour les enregistrements, voir [Modifier des enregistrements](/help/quicksilver/maestro/records/edit-records.md).

## Remarques concernant la modification des paramètres de champ

Vous devez tenir compte des points suivants avant d’apporter des modifications à la configuration d’un champ :

* Vous pouvez modifier les champs que vous avez créés ou créés par d’autres utilisateurs, si vous disposez des autorisations de gestion de l’espace de travail auquel ces champs appartiennent.
* Vous pouvez modifier un champ dans le tableau de type enregistrement.
* Vous ne pouvez pas modifier un champ sur la page d’enregistrement ni dans une autre vue, en dehors de la vue de tableau.
* Une fois le champ enregistré, vous ne pouvez pas le modifier.
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
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta de planification Adobe Workfront. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
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
   <td> <p>Il n’existe aucun contrôle d’accès pour Workfront Planning</p>  
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
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Planning dans votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Modifier les paramètres de champ

{{step1-to-maestro}}

    L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail pour lequel vous souhaitez supprimer des types d’enregistrement.

   L’espace de travail s’ouvre et les types d’enregistrement qui lui sont associés s’affichent.
1. Cliquez sur la carte correspondant au type d’enregistrement dont vous souhaitez modifier les champs.

   Cela ouvre la page du type d’enregistrement.
1. (Conditionnel) Cliquez sur l’onglet d’un **Vue Tableau**.
1. Pointez sur l’en-tête de colonne d’un champ à modifier, puis cliquez sur la flèche pointant vers le bas située après le nom du champ, puis cliquez sur **Champ Modifier**

   Ou

   Double-cliquez sur l’en-tête de colonne du champ.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Mettre à jour les informations sur le champ et cliquer sur **Enregistrer**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Une fois le champ enregistré, vous ne pouvez pas le mettre à jour.

   Les informations des champs sont mises à jour pour toutes les personnes ayant accès à l’espace de travail.

   <!--After the release of the RTBE for field configurations, replace the tip with this:

    >[!TIP]
    >
    >* You cannot update the field type after the field is saved.
    >
    >* When you modify field configurations (field options or formula expressions), records that already contain information in the modified fields will update their values in real-time. There is no warning and no audit log for the value changes triggered by field configuration changes. All users who view the fields will immediately see the new values with the modifications. 
    -->


1. (Conditionnel) Pour les champs d’enregistrement liés, cliquez sur **Modifier les champs de recherche** et ajouter ou supprimer l’un des champs du type d’enregistrement lié.

   Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).
