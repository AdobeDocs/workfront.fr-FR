---
title: Suppression des espaces de travail
description: Vous pouvez supprimer des espaces de travail lorsqu’ils ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Suppression des espaces de travail

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour utiliser les fonctionnalités de Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Dans Adobe Maestro, les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail. Pour plus d’informations, voir [Créer des espaces de travail](../architecture/delete-workspaces.md).

Vous pouvez supprimer les espaces de travail qui ne sont plus pertinents.

Nous vous recommandons de recréer certains ou tous les types d’enregistrements et taxonomies associés à l’espace de travail que vous souhaitez supprimer dans un autre espace de travail avant de le supprimer.

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
<p>Votre entreprise doit être inscrite au programme bêta Adobe Maestro. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
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

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Remarques concernant la suppression des espaces de travail

* Vous pouvez supprimer tout espace de travail que vous ou toute personne de votre entreprise avez créé. <!--this will change with access levels and permissions-->
* Lorsque vous supprimez des espaces de travail, tous les types d’enregistrement, taxonomies et leurs champs sont également supprimés. <!--asked Lilit because the confirmation says the records don't delete, but not sure how they can exist outside of a workspace?!-->
* Les espaces de travail supprimés et les informations qu’ils contiennent ne peuvent pas être récupérés.

## Suppression d’un espace de travail

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-workfront.png) dans le coin supérieur droit de Workfront ou de la fonction **Menu principal** icon ![](assets/main-menu-shell.png)  dans le coin supérieur gauche, le cas échéant, puis cliquez sur **Maestro** ![](assets/maestro-icon.png).

   Le dernier espace de travail auquel vous avez accédé s’affiche alors.

1. (Facultatif) Développez la flèche vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail à supprimer.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) en regard du nom de l’espace de travail, cliquez sur **Supprimer**.
1. Cliquez sur **Supprimer** pour confirmer.

   L’espace de travail est supprimé et ne peut pas être récupéré. Tous les types d’enregistrements, taxonomies, enregistrements et champs qui leur sont associés sont également supprimés. <!--ensure this is right after closed beta-->
