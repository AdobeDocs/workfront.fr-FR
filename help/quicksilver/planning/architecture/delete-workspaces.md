---
title: Supprimer des espaces de travail
description: Vous pouvez supprimer des espaces de travail lorsqu’ils ne sont plus pertinents.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 74%

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

1. (Conditionnel) Si vous êtes administrateur Workfront, cliquez sur **Mes espaces de travail** pour accéder aux espaces de travail que vous avez créés, ou sur **Autres espaces de travail** pour accéder aux espaces de travail partagés avec vous. <!--change it to Workspaces I'm on-->

1. Cliquez sur la carte de l’espace de travail que vous souhaitez supprimer.

   La page Workspace s’affiche.

<!--***********Replace the first step with this:*******

1. (Optional) Click **Show more** to display additional workspaces. The **Show more** link displays only when you have workspaces that display on more than two rows.
1. (Optional) ClicK **Show less** to limit the number of workspaces that display on the screen. 
1. To delete a workspace, do one of the following:

   * Hover over the workspace card, then click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the card, then click **De,ete**. 
   * Click a workspace card to open the workspace. 
   
   ***********Add (Conditional) If you clicked a workspace card,******to the step below****-->

1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) en regard du nom de l’espace de travail, puis sur **Supprimer**.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. Saisissez &quot;**delete**&quot; dans l’espace fourni, puis cliquez sur **Supprimer définitivement**. Ceci n’est pas sensible à la casse.

   L’espace de travail est supprimé de manière irréversible. Les types d’enregistrement, enregistrements, champs et vues qui leur sont associés sont également supprimés. <!--ensure this is right at or before GA-->
