---
title: Suppression des types d’enregistrement
description: Vous pouvez supprimer des types d’enregistrements opérationnels ou des types d’enregistrements de taxonomie lorsqu’ils ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 1%

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

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez supprimer des types d’enregistrements opérationnels ou des types d’enregistrements de taxonomie lorsqu’ils ne sont plus pertinents.

Pour plus d’informations sur les types d’enregistrement et les taxonomies, voir [Présentation des types d’enregistrement et des taxonomies](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

Il est recommandé de recréer les champs et les enregistrements associés au type d&#39;enregistrement ou à la taxonomie que vous souhaitez supprimer sur un autre type d&#39;enregistrement avant de les supprimer.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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

## Remarques concernant la suppression de types d’enregistrement

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Vous pouvez supprimer tout type d’enregistrement ou toute taxonomie que vous ou toute autre personne de votre entreprise avez créé. <!--this will change with access levels and permissions-->
* La suppression des types d’enregistrement supprime toutes les informations qui leur sont associées, y compris les champs et les enregistrements de ce type.
* Vous ne pouvez pas récupérer les types d&#39;enregistrements supprimés ni leurs informations.

## Suppression des types d’enregistrement

La suppression des types d’enregistrement de taxonomie est identique à celle des types d’enregistrement opérationnels.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-workfront.png) dans le coin supérieur droit de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> puis cliquez sur **Maestro** ![](assets/maestro-icon.png).

   L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail pour lequel vous souhaitez supprimer des types d’enregistrement.

   L’espace de travail s’ouvre et les types d’enregistrement et taxonomies qui y sont associés s’affichent.
1. Cliquez sur la carte correspondant au type d’enregistrement ou à la taxonomie à supprimer.

   Cela ouvre la page du type d’enregistrement.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Supprimer**.
1. Cliquez sur **Supprimer** pour confirmer.

   Le type d’enregistrement ou la taxonomie sélectionné, ainsi que leurs champs et enregistrements associés, sont supprimés.
