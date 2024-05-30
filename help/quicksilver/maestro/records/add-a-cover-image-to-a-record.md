---
title: Ajout d’une image de couverture à un enregistrement
description: Vous pouvez personnaliser des enregistrements en ajoutant une image de couverture à la page d’enregistrement dans Adobe Workfront Planning, lors de la modification d’un enregistrement.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 5%

---


<!--update the metadata with real information-->

# Ajout d’une image de couverture à un enregistrement

{{planning-important-intro}}

Vous pouvez personnaliser des enregistrements en ajoutant une image de couverture à la page d’enregistrement dans Adobe Workfront Planning, lors de la modification d’un enregistrement.

Pour plus d’informations sur la modification d’enregistrements, voir [Modifier des enregistrements](/help/quicksilver/maestro/records/edit-records.md).

Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.

Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

## Conditions d’accès

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>N’importe quelle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Attribution ou autorisations supérieures à un espace de travail </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td>  <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/maestro/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Considérations relatives aux images de couverture de page d’enregistrement

Vous pouvez personnaliser la page d’un enregistrement en y ajoutant une image de couverture.

Tenez compte des points suivants :

* Une image de couverture est propre à un enregistrement et ne s’applique pas à tous les enregistrements du même type.
* Vous pouvez uniquement ajouter des fichiers image comme images de couverture.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Vous pouvez ajouter une image de couverture à des enregistrements individuels à partir de l’aperçu de l’enregistrement dans n’importe quelle vue ou à partir de la page d’enregistrement.
* Vous ne pouvez pas ajouter d’images de couverture en ligne à partir de n’importe quel affichage d’enregistrement.

## Ajout d’une image de couverture à un enregistrement

Vous pouvez personnaliser un enregistrement en ajoutant une image de couverture en haut de l’aperçu de l’enregistrement ou de la page.

{{step1-to-maestro}}

L’espace de travail auquel vous accédez en dernier s’ouvre.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas située à droite du nom de l’espace de travail pour sélectionner l’espace de travail dont vous souhaitez mettre à jour les enregistrements.

1. Cliquez sur une carte de type enregistrement.

   La page de type enregistrement s’ouvre.

1. Dans une vue de tout type, cliquez sur le nom d’un enregistrement.

   Ou

   Dans la vue Tableau, cliquez sur le bouton **Ouvrir les détails** icon ![](assets/open-details-icon-in-table-name-field.png) à gauche d’un nom d’enregistrement.

   L’aperçu de l’enregistrement s’ouvre dans la vue.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Vous pouvez afficher la **Ouvrir les détails** à gauche du champ Nom d’un enregistrement dans une vue de tableau uniquement lorsque le champ Nom est un champ principal.

1. (Facultatif) Cliquez sur le **Ouvrir dans un nouvel onglet** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page d’enregistrement s’ouvre.

   ![](assets/details-page.png)

1. Dans l’aperçu de l’enregistrement ou la page, cliquez sur **Ajouter une couverture**. <!--check the casing here; I logged a bug for this-->
La variable **Record cover** s’ouvre.

1. Cliquez sur **Sélectionner pour charger** et recherchez une image sur votre ordinateur pour la sélectionner, l’ajouter, puis cliquez sur **Utiliser une image**.

   L’image est téléchargée en haut de l’aperçu de l’enregistrement ou de la page et les modifications sont enregistrées automatiquement.

   ![](assets/record-page-with-cover-image.png)

1. (Facultatif) Passez la souris sur l’image, puis cliquez sur le **Plus** menu ![](assets/more-menu.png) dans le coin inférieur droit de l’image de couverture, effectuez l’une des opérations suivantes :

   * Cliquez sur **Télécharger** si vous souhaitez remplacer l’image de couverture et répéter l’étape 6 pour télécharger et enregistrer une nouvelle image.
   * Cliquez sur **Repositionnement**, et utilisez la variable **Repositionnement** outil ![](assets/reposition-tool-icon.png) pour centrer l’image de couverture, puis cliquez sur **Enregistrer** une fois terminé.
   * Cliquez sur **Supprimer** pour supprimer l’image de couverture.

   Workfront enregistre automatiquement vos modifications.
