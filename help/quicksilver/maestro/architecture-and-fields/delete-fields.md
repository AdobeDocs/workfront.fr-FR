---
title: Supprimer des champs
description: Dans Adobe Maestro, vous pouvez supprimer des champs personnalisés qui ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Supprimer des champs

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Dans Adobe Maestro, vous pouvez créer des champs personnalisés pour stocker des informations sur les enregistrements.

Pour plus d’informations sur la création de champs personnalisés dans Maestro, voir [Créer des champs](../architecture-and-fields/create-fields.md).

Vous pouvez supprimer les champs Maestro qui ne sont plus pertinents.

## Observations relatives à la suppression des champs Maestro :

* Vous pouvez supprimer les champs que vous avez créés ou créés par d’autres utilisateurs. <!--this will change with access levels/ permissions-->
* Vous ne pouvez supprimer un champ que dans le tableau de type enregistrement.
* Toutes les informations stockées dans le champ sont supprimées et ne peuvent pas être récupérées.
  <!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe de produit</p> </td>
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
<p>Tous</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Tous</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Niveau d’accès</td>
   <td> <p>Tous</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modèle de mise en page</td>
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/grant-access.md">Accorder l’accès à Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Supprimer des champs

<!--When they release the sharing of fields between other records, revise this section.  -->

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-workfront.png) dans le coin supérieur droit de Workfront, <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> puis cliquez sur **Maestro** ![](assets/maestro-icon.png).

   Cela ouvre le dernier espace de travail accessible dans Maestro.
1. Cliquez sur la carte d’un type d’enregistrement dont vous souhaitez supprimer les champs.
1. (Conditionnel) Sélectionnez une **Vue Tableau** de la **Affichage** menu déroulant dans le coin supérieur droit de la page de type enregistrement.
1. Recherchez le champ à supprimer dans les en-têtes de colonne, survolez l’en-tête de colonne avec la souris, puis cliquez sur la flèche pointant vers le bas située après le nom du champ.
1. Cliquez sur **Supprimer**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Cliquez sur **Supprimer** pour confirmer.

   Le champ est supprimé, ne peut pas être récupéré et ne peut plus être associé à aucun enregistrement.