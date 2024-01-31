---
title: Partage de vues
description: Vous pouvez partager une vue avec d’autres pour garantir la collaboration lorsque vous travaillez dans Adobe Workfront Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---


<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Partage de vues

{{maestro-important-intro}}

Vous pouvez partager une vue avec d’autres pour garantir la collaboration lorsque vous travaillez dans Adobe Workfront Maestro.

L’octroi d’autorisations à un espace de travail ne donne pas à d’autres utilisateurs les autorisations d’accès aux vues sur les pages de type enregistrement. Vous devez accorder des autorisations pour des vues individuelles dans une page de type enregistrement afin de les partager avec d’autres utilisateurs.

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
   <td> Il n’existe aucun contrôle d’accès pour Adobe Maestro</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td> <p>Gestion des autorisations pour un affichage</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Maestro dans le menu principal. </p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/maestro/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Partage des autorisations sur une vue

Vous pouvez partager les vues que vous avez créées ou celles pour lesquelles vous disposez des autorisations de gestion.

>[!NOTE]
>
>Les administrateurs système ne peuvent pas afficher ni partager les vues qu’ils n’ont pas créées eux-mêmes. Ils peuvent uniquement afficher ou partager les vues partagées avec eux.


Pour partager une vue avec d’autres personnes :

{{step1-to-maestro}}

1. Ouvrez l’espace de travail dont vous souhaitez partager la vue, puis cliquez sur une carte Type d’enregistrement .

   Cela ouvre la page de type enregistrement.

1. Dans le menu déroulant Affichage , passez la souris sur la vue que vous souhaitez partager, puis cliquez sur l’icône **Plus** menu ![](assets/more-menu.png) à droite du nom de la vue, puis cliquez sur **Partager**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Dans le **Accorder l’accès à la vue à** , commencez à saisir le nom d’un utilisateur ou d’un groupe, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Sélectionnez l’un des niveaux d’autorisation suivants dans le menu déroulant :
   * Afficher
   * Gérer

     Pour plus d’informations sur les niveaux d’autorisation et les actions que les utilisateurs peuvent effectuer pour chaque niveau, voir [Présentation des autorisations de partage dans Adobe Maestro](../access/sharing-permissions-overview.md).
1. Cliquez sur **Copier le lien** pour copier un lien vers la vue dans le presse-papiers.
1. Partagez le lien copié avec d’autres personnes. Les utilisateurs qui reçoivent le lien doivent être des utilisateurs actifs et se connecter à Workfront pour pouvoir accéder à la page de type d’enregistrement et l’afficher dans la vue sélectionnée.
1. Cliquer sur **Enregistrer**.

## Suppression des autorisations d’un affichage

{{step1-to-maestro}}

1. Ouvrez l’espace de travail dont vous souhaitez partager la vue, puis cliquez sur une carte Type d’enregistrement .

   Cela ouvre la page de type enregistrement.

1. Dans le menu déroulant Affichage , passez la souris sur la vue que vous souhaitez partager, puis cliquez sur l’icône **Plus** menu ![](assets/more-menu.png) à droite du nom de la vue, puis cliquez sur **Partager**.

1. Recherchez l’utilisateur ou le groupe à supprimer, puis cliquez sur **Supprimer** dans le menu déroulant des autorisations situé à droite du nom de l’utilisateur ou du groupe.

1. Cliquer sur **Enregistrer**.

   L’utilisateur ou les utilisateurs appartenant au groupe supprimé n’ont plus accès à la vue.