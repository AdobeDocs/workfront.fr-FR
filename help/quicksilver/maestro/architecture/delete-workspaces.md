---
title: Suppression des espaces de travail
description: Vous pouvez supprimer des espaces de travail lorsqu’ils ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Suppression des espaces de travail

{{maestro-important-intro}}

Dans la planification d’Adobe Workfront, les espaces de travail sont des emplacements centralisés pour que les équipes puissent planifier le travail. Pour plus d’informations, voir [Créer des espaces de travail](../architecture/delete-workspaces.md).

Vous pouvez supprimer les espaces de travail qui ne sont plus pertinents.

Nous vous recommandons de recréer certains ou tous les types d’enregistrements, enregistrements, champs et vues associés à l’espace de travail que vous souhaitez supprimer dans un autre espace de travail avant de le supprimer.

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
<p>Votre entreprise doit être inscrite au programme bêta de planification de Adobe Workbench. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Quelconque</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Nouveau : Standard</p>
   <p>Actuel : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour la planification Adobe Workfront.</p>  
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

*Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Remarques concernant la suppression des espaces de travail

* Lorsque vous supprimez des espaces de travail, tous les types d’enregistrements, enregistrements, leurs champs et vues sont également supprimés.
* Les espaces de travail supprimés et les informations qu’ils contiennent ne peuvent pas être récupérés.

## Suppression d’un espace de travail

{{step1-to-maestro}}

Le dernier espace de travail auquel vous avez accédé s’affiche alors.

1. (Facultatif) Développez la flèche vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail à supprimer.
1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) en regard du nom de l’espace de travail, cliquez sur **Supprimer**.
1. Cliquez sur **Supprimer** pour confirmer.

   L’espace de travail est supprimé et ne peut pas être récupéré. Les types d’enregistrement, enregistrements, champs et vues qui leur sont associés sont également supprimés. <!--ensure this is right after closed beta-->
