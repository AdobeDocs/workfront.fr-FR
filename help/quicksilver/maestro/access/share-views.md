---
title: Partager des vues
description: Vous pouvez partager une vue avec d’autres pour garantir la collaboration lors de l’utilisation d’Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 6%

---

<!--update the metadata and description when we turn this article live-->

# Partager des vues

{{planning-important-intro}}

Vous pouvez partager une vue avec d’autres pour garantir la collaboration lors de l’utilisation d’enregistrements dans Adobe Workfront Planning.

L’octroi d’autorisations à un espace de travail ne donne pas à d’autres utilisateurs les autorisations d’accès aux vues sur les pages de type enregistrement. Vous devez accorder des autorisations pour des vues individuelles dans une page de type enregistrement afin de les partager avec d’autres utilisateurs.

Lorsque vous partagez une vue, vous autorisez d’autres personnes à accéder à tous les éléments de la vue. Par exemple, lorsque vous leur accordez les autorisations Gérer pour une vue, ils peuvent modifier l’aspect du regroupement, du filtre, du tri ou de la barre.


Vous pouvez partager une vue avec les entités suivantes :

* Utilisateurs de Workfront
* Groupes Workfront
<!--* Publicly, with users outside Workfront
-->

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé d’Adobe Workfront Planning. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>N’importe quelle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> Il n’existe aucun contrôle d’accès pour Adobe Workfront Planning </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td> <p>Gestion des autorisations pour un affichage</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/maestro/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Partage des autorisations sur une vue <!--internally-->

Vous pouvez partager les vues que vous avez créées ou les vues auxquelles vous êtes autorisé à accéder <!--with users or groups in Workfront-->.

>[!NOTE]
>
>Les administrateurs système ne peuvent pas afficher ni partager les vues qu’ils n’ont pas créées eux-mêmes. Ils peuvent uniquement accéder aux vues partagées avec eux ou les partager.
>
>Les administrateurs système ne peuvent disposer que des autorisations de gestion pour une vue.

{{step1-to-maestro}}

1. Ouvrez l’espace de travail dont vous souhaitez partager la vue, puis cliquez sur une carte de type enregistrement.

   Cela ouvre la page de type enregistrement.

1. Dans l’onglet Affichage , passez la souris sur la vue que vous souhaitez partager et cliquez sur le **Plus** menu ![](assets/more-menu.png) à droite du nom de la vue, puis cliquez sur **Partager**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

1. (Facultatif) Sélectionnez l’une des options suivantes pour partager la vue :

   * **Seules les personnes invitées peuvent accéder à**: vous devez spécifier les utilisateurs ou les groupes avec lesquels vous souhaitez partager la vue. Il s’agit de l’option par défaut.
   * **Tout le monde dans l’espace de travail peut afficher**: tous les utilisateurs disposant d’autorisations d’affichage ou supérieures sur les espaces de travail peuvent accéder à la vue.

1. Dans le **Accorder l’accès à la vue à** , commencez à saisir le nom d’un utilisateur ou d’un groupe, puis cliquez dessus lorsqu’il s’affiche dans la liste.  <!--***********replace screen shot below when public sharing is released***********-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Sélectionnez l’un des niveaux d’autorisation suivants dans le menu déroulant :
   * Afficher
   * Gérer

     Pour plus d’informations sur les niveaux d’autorisation et les actions que les utilisateurs peuvent effectuer pour chaque niveau, voir [Présentation du partage des autorisations dans Adobe Workfront Planning](../access/sharing-permissions-overview.md).

     Les administrateurs système reçoivent toujours les autorisations Gérer pour les vues partagées avec eux.

1. Cliquez sur **Copier le lien** pour copier un lien vers la vue dans le presse-papiers.
1. Partagez le lien copié avec d’autres personnes. Les utilisateurs qui reçoivent le lien doivent être des utilisateurs actifs et se connecter à Workfront pour pouvoir accéder à la page de type d’enregistrement et l’afficher dans la vue sélectionnée.
1. Cliquer sur **Enregistrer**.

<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## Suppression des autorisations d’un affichage

{{step1-to-maestro}}

1. Ouvrez l’espace de travail dont vous souhaitez arrêter le partage, puis cliquez sur une carte de type enregistrement. Cela ouvre la page de type enregistrement.
1. Pointez sur le nom de l’onglet de la vue à partir de laquelle vous souhaitez supprimer le partage, puis cliquez sur le **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Partager**.
1. Recherchez l’utilisateur ou le groupe à supprimer, puis cliquez sur **Supprimer** dans le menu déroulant des autorisations situé à droite du nom de l’utilisateur ou du groupe.
1. Cliquez sur **Enregistrer**.
L’utilisateur ou les utilisateurs appartenant au groupe supprimé n’ont plus accès à la vue. Les utilisateurs qui ont été supprimés de l’accès ne reçoivent aucune notification leur indiquant qu’ils ont perdu cet accès.

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->