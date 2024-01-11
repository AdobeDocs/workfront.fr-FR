---
title: Modifier les champs
description: Dans Adobe Maestro, vous pouvez modifier les paramètres des champs déjà créés.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Formula fields
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# Modifier les champs

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour utiliser les fonctionnalités de Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez modifier les paramètres des champs déjà créés.

Pour plus d’informations sur la création de champs Adobe Maestro, voir [Créer des champs](../fields/create-fields.md).

Cet article décrit comment modifier les paramètres des champs Maestro. Pour plus d’informations sur la modification des valeurs de champ pour les enregistrements Maestro, voir [Modifier des enregistrements](/help/quicksilver/maestro/records/edit-records.md).

## Observations relatives à la modification des informations sur les champs

* Vous pouvez modifier les champs que vous avez créés ou créés par d’autres utilisateurs, si vous disposez des autorisations de gestion de l’espace de travail auquel ces champs appartiennent.
* Vous pouvez modifier un champ dans le tableau de type enregistrement.
* Vous ne pouvez pas modifier un champ sur la page Détails d’un enregistrement ou dans la vue de chronologie.
* Une fois le champ enregistré, vous ne pouvez pas le modifier.
* Vous ne pouvez pas désélectionner le paramètre Autoriser les nombres négatifs précédemment sélectionné, pour un champ Nombre, Pourcentage ou Devise si des valeurs négatives sont déjà stockées dans les enregistrements auxquels il est rattaché.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Maestro</p>  
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
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Modifier les champs

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-workfront.png) dans le coin supérieur droit de Workfront ou de la fonction **Menu principal** icon ![](assets/main-menu-shell.png)  dans le coin supérieur gauche, le cas échéant, puis cliquez sur **Maestro** ![](assets/maestro-icon.png).

   L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail pour lequel vous souhaitez supprimer des types d’enregistrement.

   L’espace de travail s’ouvre et les types d’enregistrement et taxonomies qui y sont associés s’affichent.
1. Cliquez sur la carte correspondant au type d’enregistrement ou à la taxonomie dont vous souhaitez modifier les champs.

   Cela ouvre la page du type d’enregistrement.
1. (Conditionnel) Sélectionnez une **Vue Tableau** de la **Affichage** menu déroulant dans le coin supérieur droit de la page de type enregistrement.
1. Pointez sur l’en-tête de colonne d’un champ à modifier, puis cliquez sur la flèche pointant vers le bas située après le nom du champ, puis cliquez sur **Champ Modifier**

   Ou

   Double-cliquez sur l’en-tête de colonne du champ.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Mettre à jour les informations sur le champ et cliquer sur **Enregistrer**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >Une fois le champ enregistré, vous ne pouvez pas le mettre à jour.


1. (Conditionnel) Pour les champs d’enregistrement liés, cliquez sur **Modifier les champs de recherche** et ajouter ou supprimer l’un des champs du type d’enregistrement lié.

   Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).
