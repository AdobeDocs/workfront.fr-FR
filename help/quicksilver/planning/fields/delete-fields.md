---
title: Supprimer des champs
description: Adobe Workfront Planning vous permet de supprimer les champs personnalisés qui ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 81%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Supprimer des champs

{{planning-important-intro}}

Dans Adobe Workfront Planning, vous pouvez créer des champs personnalisés pour stocker des informations sur les enregistrements.

Pour plus d’informations sur la création de champs personnalisés dans Workfront Planning, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

Vous pouvez supprimer les champs Workfront Planning qui ne sont plus pertinents.

## Remarques concernant la suppression de champs Workfront Planning :

* Vous ne pouvez supprimer un champ que dans la vue Tableau du type d’enregistrement.
* Vous ne pouvez pas supprimer le champ principal d’un enregistrement.
* Toutes les informations stockées dans le champ sont supprimées et ne peuvent pas être récupérées.
* Lorsque vous supprimez un champ d’enregistrement lié, tous les champs de recherche liés sont également supprimés du type d’enregistrement à partir duquel le lien a été établi. Les champs d’enregistrement liés des types d’enregistrement que vous connectez ne sont pas supprimés.

  Pour plus d’informations, consultez la section [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

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
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Votre administrateur ou administratrice Workfront ou de groupes doit ajouter la zone Planning dans votre modèle de disposition. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Vue d’ensemble des accès</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gérer les autorisations d’un espace de travail</a> </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
 </tbody>
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Supprimer des champs

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les champs d’enregistrement.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur la carte d’un type d’enregistrement.

1. (Conditionnel) Si cette option n’est pas déjà sélectionnée, cliquez sur l’onglet d’une **vue Tableau** sur la page de type enregistrement.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue du tableau.

1. Recherchez le champ à supprimer dans les en-têtes de colonne, survolez l’en-tête de colonne avec la souris, puis cliquez sur la flèche pointant vers le bas située après le nom du champ.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Cliquez sur **Supprimer**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Cliquez sur **Supprimer** pour confirmer l’opération.

   Le champ est supprimé de manière irréversible et ne peut plus être associé à aucun enregistrement.
