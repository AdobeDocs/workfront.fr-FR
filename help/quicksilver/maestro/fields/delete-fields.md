---
title: Supprimer des champs
description: Dans Adobe Maestro, vous pouvez supprimer des champs personnalisés qui ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Maestro, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Supprimer des champs

{{maestro-important-intro}}

Dans Adobe Maestro, vous pouvez créer des champs personnalisés pour stocker des informations sur les enregistrements.

Pour plus d’informations sur la création de champs personnalisés dans Maestro, voir [Créer des champs](../fields/create-fields.md).

Vous pouvez supprimer les champs Maestro qui ne sont plus pertinents.

## Observations relatives à la suppression des champs Maestro :

* Vous ne pouvez supprimer un champ que dans la vue de tableau de type enregistrement.
* Vous ne pouvez pas supprimer le champ principal d’un enregistrement.
* Toutes les informations stockées dans le champ sont supprimées et ne peuvent pas être récupérées.
* Lorsque vous supprimez un champ d’enregistrement lié, tous les champs de recherche liés sont également supprimés du type d’enregistrement à partir duquel vous créez un lien. Les champs d’enregistrement liés des types d’enregistrement auxquels vous créez un lien ne sont pas supprimés.

  Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <td role="rowheader"><p>Paramétrages du niveau d'accès</p></td>
   <td> <p>Il n’existe pas de contrôle de niveau d’accès pour Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Supprimer des champs

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-maestro}}

Cela ouvre le dernier espace de travail accessible dans Maestro.
1. Cliquez sur la carte d’un type d’enregistrement dont vous souhaitez supprimer les champs.
1. (Conditionnel) Sélectionnez une **Vue Tableau** de la **Affichage** menu déroulant dans le coin supérieur droit de la page de type enregistrement.
1. Recherchez le champ à supprimer dans les en-têtes de colonne, survolez l’en-tête de colonne avec la souris, puis cliquez sur la flèche pointant vers le bas située après le nom du champ.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Cliquez sur **Supprimer**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Cliquez sur **Supprimer** pour confirmer.

   Le champ est supprimé, ne peut pas être récupéré et ne peut plus être associé à aucun enregistrement.
