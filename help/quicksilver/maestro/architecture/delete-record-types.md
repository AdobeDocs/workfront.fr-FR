---
title: Suppression des types d’enregistrement
description: Vous pouvez supprimer des types d’enregistrements opérationnels ou des types d’enregistrements de taxonomie lorsqu’ils ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
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

Vous pouvez supprimer des types d’enregistrements opérationnels ou des types d’enregistrements de taxonomie lorsqu’ils ne sont plus pertinents.

Pour plus d’informations sur les types d’enregistrement et les taxonomies, voir [Présentation des types d’enregistrement et des taxonomies](../architecture/overview-of-record-types-and-taxonomies.md).

Il est recommandé de recréer les champs et les enregistrements associés au type d&#39;enregistrement ou à la taxonomie que vous souhaitez supprimer sur un autre type d&#39;enregistrement avant de les supprimer.

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
   <p> Adobe Workfront</p> <p>Pour connecter les types d’enregistrements Maestro à Experience Manager Assets, vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance de Workfront de votre entreprise doit être intégrée à Adobe Business Platform ou à Adobe Admin Console.</p> </td>
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
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.
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

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Remarques concernant la suppression de types d’enregistrement

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Vous pouvez supprimer uniquement les types d’enregistrement ou les taxonomies des espaces de travail pour lesquels vous disposez des autorisations de gestion.
* La suppression des types d’enregistrement supprime toutes les informations qui leur sont associées, y compris les champs et les enregistrements de ce type. Le type d’enregistrement est supprimé de tous les utilisateurs accédant à l’espace de travail.
* Vous ne pouvez pas récupérer les types d&#39;enregistrements supprimés ni leurs informations.

## Suppression des types d’enregistrement

La suppression des types d’enregistrement de taxonomie est identique à celle des types d’enregistrement opérationnels.

{{step1-to-maestro}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail pour lequel vous souhaitez supprimer des types d’enregistrement.

   L’espace de travail s’ouvre et les types d’enregistrement et taxonomies qui y sont associés s’affichent.
1. Cliquez sur la carte correspondant au type d’enregistrement ou à la taxonomie à supprimer.

   Cela ouvre la page du type d’enregistrement.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Supprimer**.
1. Cliquez sur **Supprimer** pour confirmer.

   Le type d’enregistrement ou la taxonomie sélectionné, ainsi que leurs champs et enregistrements associés, sont supprimés.
