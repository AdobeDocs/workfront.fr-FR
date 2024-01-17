---
title: Suppression d’enregistrements
description: Vous pouvez supprimer les enregistrements que vous ou un autre utilisateur avez créés. Vous ne pouvez pas récupérer les enregistrements supprimés.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Suppression d’enregistrements

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour utiliser les fonctionnalités de Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez supprimer les enregistrements qui ne sont plus pertinents dans Adobe Manager.

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
   <td role="rowheader"><p>Licence Adobe Workfront</p>
   </td>
   <td>
   <p>Quelconque</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Paramétrages du niveau d'accès</p></td>
   <td> <p>Il n’existe pas de contrôle de niveau d’accès pour Maestro </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Attribution ou autorisations supérieures à un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considérations relatives à la suppression d’enregistrements

* Vous pouvez supprimer les enregistrements que vous ou un autre utilisateur avez créés.
* Vous ne pouvez pas récupérer les enregistrements supprimés. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* Si les enregistrements supprimés sont liés à d&#39;autres enregistrements, les enregistrements liés ne sont pas supprimés, mais les informations de l&#39;enregistrement supprimé sont également supprimées.
* Vous ne pouvez pas supprimer des enregistrements en bloc. <!--this will probably change-->
* Vous ne pouvez pas supprimer d’enregistrements de la vue de chronologie.
* Vous ne pouvez pas supprimer un type d’enregistrement lié à une autre application. Par exemple, si vous liez un enregistrement Maestro à un objet Workfront, vous ne pouvez pas supprimer l’objet Workfront de la page d’enregistrement de l’objet Workfront.

## Suppression d’enregistrements

Vous pouvez supprimer un enregistrement des zones suivantes :

* [Sur la page Détails d’un enregistrement](#delete-a-record-from-the-records-details-page)
* [En mode Tableau d’un type d’enregistrement](#delete-a-record-from-the-record-type-table-view)

### Supprimer un enregistrement de la page Détails de l’enregistrement

{{step1-to-maestro}}

L’espace de travail auquel vous accédez en dernier s’ouvre.

1. Cliquez sur un type d’enregistrement.

   La page de type enregistrement s’ouvre.
1. Utilisez l’une des méthodes suivantes :

   * Dans une vue Tableau, cliquez sur le nom d’un enregistrement.
   * Dans la vue Tableau, passez la souris sur le nom d’un enregistrement, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Affichage**

     ![](assets/contextual-menu-for-record-row.png)
   * Dans la vue Chronologie, cliquez sur une barre d’enregistrement.

   L&#39;enregistrement **Détails** s’ouvre.

1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez sur **Supprimer**, puis **Supprimer** pour confirmer.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
L’enregistrement est supprimé et ne peut pas être récupéré.

### Supprimer un enregistrement de la vue de table de type enregistrement

{{step1-to-maestro}}

L’espace de travail auquel vous avez accédé la dernière fois s’ouvre.

1. Cliquez sur un type d’enregistrement.

   La page de type enregistrement s’ouvre.
1. (Conditionnel) Dans la variable **Affichage** Sélectionnez une vue Tableau dans le menu déroulant situé dans le coin supérieur droit du tableau. Il doit s’agir de la vue par défaut, sauf si vous avez visualisé le type d’enregistrement dans la vue chronologique lors de votre dernier accès.

   Les enregistrements associés au type d&#39;enregistrement sélectionné s&#39;affichent dans la vue Tableau.
1. Cliquez avec le bouton droit de la souris sur une ligne d’enregistrement, puis cliquez sur **Supprimer**.

   ![](assets/contextual-menu-for-record-row.png)

   L’enregistrement est supprimé et ne peut pas être récupéré.

1. (Facultatif) Utilisez les raccourcis clavier suivants pour annuler ou rétablir la suppression d’un enregistrement :

   * Ctrl + Z (⌘ + Z pour Mac) pour annuler une modification.
   * Ctrl + Maj + Z (⌘ + Maj + Z pour Mac) pour rétablir la modification
