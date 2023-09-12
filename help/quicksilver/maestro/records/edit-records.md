---
title: Modifier des enregistrements
description: Vous pouvez modifier les informations d’enregistrement dans Adobe Maestro. Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Modifier des enregistrements

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta fermé ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez modifier les informations d’enregistrement dans Adobe Maestro. Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
Pour plus d’informations, voir [Création de types d’enregistrement](../architecture-and-fields/create-record-types.md).

&lt;!— mentionnez ici que les champs de la vue Détails sont identiques à ceux de la vue Tableau — cet article est lié à la vue Gestion des enregistrements pour faire référence à ces informations—>

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

## Remarques concernant la modification d’enregistrements

* Vous pouvez modifier les enregistrements que vous ou un autre utilisateur avez créés. <!--will change with access levels-->
* Si les enregistrements modifiés sont liés à d&#39;autres enregistrements, les nouvelles informations des enregistrements que vous modifiez se répercutent sur les enregistrements liés.
* Vous ne pouvez pas modifier les enregistrements en masse. <!--this will probably change-->

## Modifier des enregistrements

Vous pouvez modifier un enregistrement à partir des zones suivantes :

* [Sur la page Détails d’un enregistrement](#edit-a-record-from-the-records-details-page)
* [En mode Tableau d’un type d’enregistrement](#edit-a-record-from-the-record-type-table-view)

### Modifier un enregistrement à partir de la page Détails de l’enregistrement

1. Cliquez sur le bouton **Menu Principal** ![](assets/main-menu-workfront.png) dans le coin supérieur droit, ou le **Menu Principal** ![](assets/main-menu-shell.png) dans le coin supérieur gauche, s’il est disponible, cliquez sur Maestro.

   L’espace de travail auquel vous accédez en dernier s’ouvre.
1. Utilisez l’une des méthodes suivantes :

   * Dans une vue Tableau, cliquez sur le nom d’un enregistrement.
   * Dans la vue Tableau, passez la souris sur le nom d’un enregistrement, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Affichage**

     ![](assets/contextual-menu-for-record-row.png)
   * Dans la vue Chronologie, cliquez sur une barre d’enregistrement.

   L&#39;enregistrement **Détails** s’ouvre.

1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez sur **Modifier**

   Ou

   Cliquez dans n’importe quel champ modifiable de la page Détails pour modifier les informations.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

   >[!NOTE]
   >
   >    Les champs liés ou les champs qui contiennent des calculs ou qui sont générés par le système ne sont pas modifiables.


1. Cliquez sur **Enregistrer les modifications**. <!--logged a bug for this - this needs to be "Save"-->

### Modification d’un enregistrement à partir de la vue de table de type enregistrement

1. Cliquez sur le bouton **Menu Principal** ![](assets/main-menu-workfront.png) dans le coin supérieur droit, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> puis cliquez sur **Maestro** ![](assets/maestro-icon.png).

   L’espace de travail auquel vous avez accédé la dernière fois s’ouvre.
1. Cliquez sur une carte de type enregistrement.

   La page de type enregistrement s’ouvre.
1. (Conditionnel) Dans la variable **Affichage** Sélectionnez une vue Tableau dans le menu déroulant situé dans le coin supérieur droit du tableau. Il doit s’agir de la vue par défaut, sauf si vous avez visualisé le type d’enregistrement dans la vue chronologique lors de votre dernier accès.

   Les enregistrements associés au type d&#39;enregistrement sélectionné s&#39;affichent dans la vue Tableau.
1. Cliquez dans la ligne d’un enregistrement pour commencer à modifier les informations sur l’enregistrement en ligne, puis appuyez sur **Entrée** sur votre clavier pour enregistrer vos modifications. Les modifications sont enregistrées automatiquement.

   >[!TIP]
   >
   >Les champs liés ne sont pas modifiables. Les informations de ces champs sont renseignées automatiquement à partir des enregistrements liés. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture-and-fields/connect-record-types.md).



