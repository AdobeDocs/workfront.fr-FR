---
title: Suppression des espaces de travail
description: Vous pouvez supprimer des espaces de travail lorsqu’ils ne sont plus pertinents.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Suppression des espaces de travail

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta fermé ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Dans Adobe Maestro, les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail. Pour plus d’informations, voir [Créer des espaces de travail](../architecture-and-fields/create-workspaces.md).

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

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-workfront.png) dans le coin supérieur droit de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> puis cliquez sur **Maestro** ![](assets/maestro-icon.png).

   Le dernier espace de travail auquel vous avez accédé s’affiche alors.

1. (Facultatif) Développez la flèche vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail à supprimer.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) en regard du nom de l’espace de travail, cliquez sur **Supprimer**.
1. Cliquez sur **Supprimer** pour confirmer.

   L’espace de travail est supprimé et ne peut pas être récupéré. Tous les types d’enregistrements, taxonomies, enregistrements et champs qui leur sont associés sont également supprimés. <!--ensure this is right after closed beta-->