---
title: Supprimer des enregistrements
description: Vous pouvez supprimer les enregistrements que vous ou un autre utilisateur ou une autre utilisatrice avez créés. Vous ne pouvez pas récupérer des enregistrements supprimés.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 89%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Supprimer des enregistrements

{{planning-important-intro}}

Vous pouvez supprimer les enregistrements qui ne sont plus pertinents dans Adobe Workfront Planning.

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
   <td role="rowheader"><p>Licence Adobe Workfront*</p>
   </td>
   <td>
   <p>Nouvelle : standard</p>
   <p>Actuelle : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Autorisations Contribuer ou supérieures pour à un espace de travail</a> </p>  
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


<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considérations relatives à la suppression d’enregistrements

* Vous pouvez supprimer les enregistrements que vous ou un autre utilisateur ou une autre utilisatrice avez créés.
* Vous ne pouvez pas récupérer des enregistrements supprimés. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Si les enregistrements supprimés sont liés à d&#39;autres enregistrements, les enregistrements liés ne sont pas supprimés, mais les informations de l’enregistrement supprimé sont également supprimées.
* Vous ne pouvez pas supprimer des enregistrements en masse. <!--this will probably change-->
* Vous ne pouvez pas supprimer des enregistrements à partir de la vue de chronologie.

## Supprimer des enregistrements

Vous pouvez supprimer un enregistrement à partir des zones suivantes :

* [À partir de la page de l’enregistrement](#delete-a-record-from-the-records-page)
* [À partir de la vue de tableau d’un type d’enregistrement](#delete-a-record-from-the-record-type-table-view)

### Supprimer un enregistrement à partir de la page de l’enregistrement

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dont vous souhaitez supprimer les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’ouvre.
1. Utilisez l’une des méthodes suivantes :

   * Dans une vue de tableau, cliquez sur le nom d’un enregistrement.
   * Dans la vue de tableau, pointez sur le nom d’un enregistrement, cliquez sur le menu **Plus** ![](assets/more-menu.png), puis sur **Afficher**.

     ![](assets/contextual-menu-for-record-row.png)
   * Dans une vue de chronologie, cliquez sur une barre d’un enregistrement.

   La page de l’enregistrement s’ouvre.

1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) à droite du nom de l’enregistrement, cliquez sur **Supprimer**, puis à nouveau sur **Supprimer** pour confirmer.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
L’enregistrement est supprimé et ne peut pas être récupéré.

### Supprimer un enregistrement à partir de la vue de tableau de type d’enregistrement

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dont vous souhaitez supprimer les enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’ouvre.
1. (Conditionnel) Dans le menu déroulant **Afficher** situé dans le coin supérieur gauche du tableau, sélectionnez une vue de tableau. Il s’agit de la vue par défaut, sauf si vous avez visualisé le type d’enregistrement dans la vue Chronologique lors de votre dernier accès.

   Les enregistrements associés au type d’enregistrement sélectionné s’affichent dans la vue Tableau.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez avec le bouton droit de la souris sur une ligne d’enregistrement, puis cliquez sur **Supprimer**.
   * Cliquez sur le menu **Plus** ![](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez sur **Supprimer**.

     ![](assets/contextual-menu-for-record-row.png)

   * Cliquez sur l’icône **Ouvrir les détails** ![](assets/open-details-icon-in-table-name-field.png) pour ouvrir la boîte contenant les informations détaillées de l’enregistrement, cliquez sur **Plus** ![](assets/more-menu.png) à droite du nom de l’enregistrement, puis sur **Supprimer**.

   L’enregistrement est supprimé et ne peut pas être récupéré.

1. (Facultatif) Utilisez les raccourcis clavier suivants pour annuler ou rétablir la suppression d’un enregistrement :

   * Ctrl+Z (⌘+Z pour Mac) pour annuler une modification
   * Ctrl+Maj+Z (⌘+Maj+Z pour Mac) pour rétablir une modification
