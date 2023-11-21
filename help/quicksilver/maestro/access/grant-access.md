---
title: Accorder l’accès à Adobe Maestro
description: Découvrez comment accorder l’accès et partager des informations dans Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Accorder l’accès à Adobe Maestro

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour avoir accès à Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Tous les utilisateurs de votre entreprise peuvent avoir accès à Maestro, si les conditions préalables suivantes sont réunies :

<!--the first requisite will be removed when we go to GA-->

* Votre entreprise est inscrite au programme bêta fermé Adobe Maestro.
* En tant qu’administrateur système, vous devez ajouter la zone Maestro au menu principal à l’aide d’un modèle de mise en page.

  Maestro ne s’affiche par défaut dans le menu principal pour aucun utilisateur, y compris les administrateurs système.

  Pour plus d’informations, voir [Personnalisation du menu principal à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>Aucun niveau d’accès ou autorisation n’est associé aux utilisateurs ou aux informations dans Maestro. Tous les utilisateurs pour lesquels Maestro est activé dans leur environnement peuvent afficher, modifier et supprimer toutes les informations ajoutées à Maestro par un autre utilisateur.

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
   <td role="rowheader"><p>Niveau d’accès</p></td>
   <td> <p>N’importe lequel utilise Maestro</p>
   <p>Administrateur système ou Prévoyez de partager la zone Maestro dans un modèle de mise en page</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
When permissions is released:

* leave as is for Access levels (I think)
* Add a new row for Permissions: System admin or Manage access to the workspace to share a workspace with others
-->

## Partage de la zone Maestro dans le menu principal avec d’autres

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

Une fois que votre entreprise a été inscrite au programme bêta Maestro, vous pouvez ajouter la zone Maestro au menu principal de tous les utilisateurs à l’aide d’un modèle de mise en page.

1. Connexion à **Workfront** en tant qu’administrateur Workfront.

1. Ajoutez la variable **Maestro** icon ![](assets/maestro-icon.png) à la fonction **Menu Principal** en utilisant une **Modèle de mise en page**.

   Pour plus d’informations, voir [Personnalisation du menu principal à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Attribuez le modèle de mise en page aux utilisateurs auxquels vous souhaitez accéder à Maestro.

   Pour plus d’informations, voir [Affecter des utilisateurs à un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Tous les utilisateurs affectés au modèle peuvent désormais accéder à Maestro dans leur menu principal.

   Les utilisateurs peuvent commencer à créer des espaces de travail, des types d’enregistrements, des enregistrements et des champs.

<!--

## Share permissions to a workspace

The following users can share a workspace with other users:

* System administrators can share all workspaces, including the ones that they did not create.
* All other users can share only workspaces for which they have Manage permissions to. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner or Workfront, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner of Workfront, if available, then click **Maestro**.
1. Open the workspace you want to remove permissions to, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu to the right of a user or group name, then click **Remove**. 
1. Click **Save**.

    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 

-->