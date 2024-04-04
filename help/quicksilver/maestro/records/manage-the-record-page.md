---
title: Gestion de la page d’enregistrement
description: Vous pouvez modifier la mise en page de la boîte d’enregistrement et de la page dans Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7d3778d52f9a3afa12a7bdf348f7400693f8f7ab
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Gestion de la page d’enregistrement

{{maestro-important-intro}}

Vous pouvez modifier la mise en page de la boîte d’enregistrement et de la page dans Adobe Workfront Planning. Vous pouvez afficher la zone d’enregistrement dans une vue d’enregistrement.

La zone d’enregistrement est une vue plus petite de la page d’enregistrement qui s’affiche dans la vue d’un type d’enregistrement.

Lorsque vous modifiez la mise en page d’une zone d’enregistrement et d’une page, la zone et la page changent pour tous les enregistrements du même type.

Vous devez créer des types d’enregistrement et des enregistrements avant de pouvoir commencer à modifier des pages d’enregistrement.

Pour plus d’informations, voir les articles suivants :

* [Création de types d’enregistrement](../architecture/create-record-types.md)

* [Créer des enregistrements](/help/quicksilver/maestro/records/create-records.md)

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
<p>Votre entreprise doit être inscrite au programme bêta de planification Adobe Workfront. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
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
   <p>Nouveau : clair ou supérieur</p>
   Ou
   <p>Actuel : travail ou plus élevé</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Paramétrages du niveau d'accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion ou autorisations supérieures à un espace de travail</a> </p>  
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

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Remarques concernant la modification de pages d’enregistrement

* La réorganisation des champs de la zone d’enregistrement ou de la page réorganise les champs pour tous les enregistrements de ce type et pour tous les utilisateurs accédant à ces enregistrements.
* L’ajout d’une image de couverture à un enregistrement ne fait pas partie de la disposition globale de la zone d’enregistrement ou de la page. Vous pouvez ajouter des images de couverture uniques à chaque enregistrement.

## Réorganiser les champs de la zone d’enregistrement ou de la page

{{step1-to-maestro}}

L’espace de travail auquel vous accédez en dernier s’ouvre.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas située à droite du nom de l’espace de travail pour sélectionner l’espace de travail dont vous souhaitez mettre à jour les enregistrements.
1. Cliquez sur une carte de type enregistrement.

   La page de type enregistrement s’ouvre.

1. Dans une vue de tout type, cliquez sur le nom d’un enregistrement.

   Ou

   Dans la vue Tableau, cliquez sur le bouton **Ouvrir les détails** icon ![](assets/open-details-icon-in-table-name-field.png) à gauche d’un nom d’enregistrement.

   La boîte de l’enregistrement s’ouvre dans la vue.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Vous pouvez afficher la **Ouvrir les détails** à gauche du champ Nom d’un enregistrement dans une vue de tableau uniquement lorsque le champ Nom est un champ principal.

1. (Facultatif) Cliquez sur le **Ouvrir dans un nouvel onglet** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> dans le coin supérieur droit de la zone d’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page d’enregistrement s’ouvre.

   ![](assets/details-page.png)

1. Dans la zone d’enregistrement ou la page, cliquez sur l’icône de capture. ![](assets/grab-icon.png) à gauche du nom d’un champ, puis effectuez un glisser-déposer à l’emplacement de votre choix.

   La nouvelle position du champ est mise à jour dans la zone et la page de tous les enregistrements du même type pour tous les utilisateurs qui visualisent les enregistrements.

   Toutes les modifications apportées à la mise en page de la boîte d’enregistrement ou de la page sont enregistrées automatiquement.


## Ajout d’une image de couverture à la zone d’enregistrement ou à la page

Vous pouvez personnaliser un enregistrement en ajoutant une image de couverture en haut de la zone d’enregistrement ou de la page.

{{step1-to-maestro}}

L’espace de travail auquel vous accédez en dernier s’ouvre.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas située à droite du nom de l’espace de travail pour sélectionner l’espace de travail dont vous souhaitez mettre à jour les enregistrements.

1. Cliquez sur une carte de type enregistrement.

   La page de type enregistrement s’ouvre.

1. Dans une vue de tout type, cliquez sur le nom d’un enregistrement.

   Ou

   Dans la vue Tableau, cliquez sur le bouton **Ouvrir les détails** icon ![](assets/open-details-icon-in-table-name-field.png) à gauche d’un nom d’enregistrement.

   La boîte de l’enregistrement s’ouvre dans la vue.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Vous pouvez afficher la **Ouvrir les détails** à gauche du champ Nom d’un enregistrement dans une vue de tableau uniquement lorsque le champ Nom est un champ principal.

1. (Facultatif) Cliquez sur le **Ouvrir dans un nouvel onglet** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> dans le coin supérieur droit de la zone d’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page d’enregistrement s’ouvre.

   ![](assets/details-page.png)

1. Dans la zone d’enregistrement ou la page, cliquez sur **Ajouter une couverture**. <!--check the casing here; I logged a bug for this-->
La variable **Record cover** s’ouvre.

1. Cliquez sur **Sélectionner pour charger** et recherchez une image sur votre ordinateur pour la sélectionner, l’ajouter, puis cliquez sur **Utiliser une image**.

   L’image est téléchargée en haut de la zone d’enregistrement ou de la page et les modifications sont enregistrées automatiquement.

   ![](assets/record-page-with-cover-image.png)

1. (Facultatif) Passez la souris sur l’image, puis cliquez sur le **Plus** menu ![](assets/more-menu.png) dans le coin inférieur droit de l’image de couverture, effectuez l’une des opérations suivantes :

   * Cliquez sur **Télécharger** si vous souhaitez remplacer l’image de couverture et répéter l’étape 6 pour télécharger et enregistrer une nouvelle image.
   * Cliquez sur **Repositionnement**, et utilisez la variable **Repositionnement** outil ![](assets/reposition-tool-icon.png) pour centrer l’image de couverture, puis cliquez sur **Enregistrer** une fois terminé.
   * Cliquez sur **Supprimer** pour supprimer l’image de couverture.

   Toutes les modifications prennent effet immédiatement.

