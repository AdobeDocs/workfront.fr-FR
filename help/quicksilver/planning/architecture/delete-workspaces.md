---
title: Supprimer des espaces de travail
description: Vous pouvez supprimer des espaces de travail lorsqu’ils ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 58%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Supprimer des espaces de travail

{{planning-important-intro}}

Dans Adobe Workfront Planning, les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail.
 Pour plus d’informations, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

Vous pouvez supprimer les espaces de travail qui ne sont plus pertinents.

Avant de supprimer un espace de travail, nous vous recommandons de créer à nouveau certains ou tous les types d’enregistrements, enregistrements, champs et vues associés à l’espace de travail dans un autre espace de travail.

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
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gérer les autorisations d’un espace de travail</a> </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Votre administrateur ou administratrice Workfront ou de groupes doit ajouter la zone Planning dans votre modèle de disposition. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Vue d’ensemble des accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Remarques relatives à la suppression des espaces de travail

* Lorsque vous supprimez des espaces de travail, tous les types d’enregistrements, enregistrements, champs associés et vues sont également supprimés.
* Les espaces de travail supprimés et les informations qu’ils contiennent ne peuvent pas être récupérés.

## Supprimer un espace de travail

{{step1-to-planning}}

1. (Conditionnel) Si vous êtes administrateur Workfront, cliquez sur **Espaces de travail sur** pour accéder aux espaces de travail que vous avez créés, ou sur **Autres espaces de travail** pour accéder aux espaces de travail partagés avec vous.

1. (Facultatif) Cliquez sur **Tout afficher** pour afficher des espaces de travail supplémentaires. Le lien **Tout afficher** s’affiche uniquement lorsque vous avez plus de deux lignes de cartes d’espace de travail.
1. (Facultatif) Cliquez sur **Afficher moins** pour limiter le nombre d’espaces de travail qui s’affichent à l’écran.
1. Pour supprimer un espace de travail, effectuez l’une des opérations suivantes :

   * Passez la souris sur la carte de l’espace de travail, puis cliquez sur le menu **Plus** ![](assets/more-menu.png) dans le coin supérieur droit de la carte.
Ou
   * Cliquez sur une carte d’espace de travail pour ouvrir l’espace de travail, puis cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du nom de l’espace de travail.
1. Cliquez sur **Supprimer**.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. Saisissez &quot;**delete**&quot; dans l’espace fourni, puis cliquez sur **Supprimer définitivement**. Ceci n’est pas sensible à la casse.

   L’espace de travail est supprimé de manière irréversible. Les types d’enregistrement, enregistrements, champs et vues qui leur sont associés sont également supprimés. <!--ensure this is right at or before GA-->
