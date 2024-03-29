---
title: Suppression des types d’enregistrement
description: Vous pouvez supprimer des types d’enregistrement lorsqu’ils ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Suppression des types d’enregistrement

{{maestro-important-intro}}

Vous pouvez supprimer des types d’enregistrement lorsqu’ils ne sont plus pertinents.

Cependant, la suppression des types d’enregistrement supprime également toutes les informations associées aux types d’enregistrement. Pour plus d’informations, voir [Remarques concernant la suppression de types d’enregistrement](#considerations-when-deleting-record-types) dans cet article.

Pour plus d’informations sur les types d’enregistrement, voir [Présentation des types d’enregistrement](../architecture/overview-of-record-types-and-taxonomies.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<p>Votre entreprise doit être inscrite au programme bêta de planification d’Adobe Workfront. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
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
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour la planification Adobe Workfront.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Planning dans votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Remarques concernant la suppression de types d’enregistrement

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Vous ne pouvez supprimer que les types d’enregistrement des espaces de travail auxquels vous disposez des autorisations de gestion.
* La suppression des types d’enregistrement supprime les informations suivantes qui leur sont associées :

   * Tous les enregistrements de ce type.
   * Tous les champs associés au type d’enregistrement.
   * Toutes les vues (y compris les filtres, les regroupements et les critères de tri) du type d’enregistrement.
* Le type d’enregistrement est supprimé de tous les utilisateurs accédant à l’espace de travail.
* Vous ne pouvez pas récupérer les types d&#39;enregistrements supprimés ni leurs informations.
* Il est recommandé de recréer les champs et les enregistrements associés au type d&#39;enregistrement que vous souhaitez supprimer sur un autre type d&#39;enregistrement avant de les supprimer.

## Suppression des types d’enregistrement

{{step1-to-maestro}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail pour lequel vous souhaitez supprimer des types d’enregistrement.

   L’espace de travail s’ouvre et les types d’enregistrement et taxonomies qui y sont associés s’affichent.
1. Cliquez sur la carte correspondant au type d’enregistrement à supprimer.

   Cela ouvre la page du type d’enregistrement.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Supprimer**.
1. Cliquez sur **Supprimer** pour confirmer.

   Le type d’enregistrement sélectionné, ainsi que leurs champs, enregistrements associés et vues, sont supprimés.
