---
title: Ajout de miniatures aux enregistrements
description: Vous pouvez modifier les informations d’enregistrement dans Adobe Maestro et associer chaque enregistrement à des miniatures individuelles afin de les rendre facilement reconnaissables.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Ajout de miniatures aux enregistrements

{{maestro-important-intro}}

Vous pouvez associer des enregistrements à des miniatures uniques dans Adobe Maestro afin de les rendre facilement reconnaissables.

Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

## Exigences d’accès

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td> <p>Il n’existe aucun contrôle d’accès pour Maestro </p>  
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
   <td>  <p>Tous les utilisateurs, y compris les administrateurs Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Maestro dans le menu principal. </p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/maestro/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Points à prendre en compte concernant les miniatures d’enregistrements

Pour faire la distinction visuelle entre les enregistrements dans une vue de tableau, vous pouvez associer une miniature unique à chaque enregistrement.

Tenez compte des points suivants :

* Vous pouvez uniquement ajouter des fichiers image sous forme de miniatures.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Vous pouvez ajouter une miniature à des enregistrements individuels dans la vue de tableau.
* Les miniatures appartiennent aux informations d’enregistrement et s’affichent dans les vues où s’affichent les enregistrements. Par exemple, les miniatures s’affichent avec les informations d’enregistrement dans les zones suivantes :

   * Le champ principal d’un enregistrement dans la vue de tableau
   * La barre d’enregistrement en mode Chronologie.
* Vous ne pouvez pas ajouter de miniatures d’enregistrement à partir de la page Détails de l’enregistrement ou en mode Chronologie.
* Les miniatures ne s’affichent pas dans la page Détails de l’enregistrement.

## Ajout d’une miniature à un enregistrement

{{step1-to-maestro}}

1. Sélectionnez l’espace de travail pour lequel vous souhaitez ajouter des miniatures, puis cliquez sur la carte de type d’enregistrement.

   Cela ouvre la page de type enregistrement.
1. Sélectionnez une vue de tableau dans la **Affichage** menu déroulant. Tous les enregistrements du type que vous avez sélectionné s&#39;affichent dans un tableau.
1. Passez la souris sur les informations du champ principal, puis cliquez sur le **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Miniature**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Le champ principal est le champ qui s’affiche dans la première colonne d’une vue de tableau. Le champ principal est toujours gelé et ne peut pas être masqué ni déplacé.

   La variable **Miniature d’enregistrement** s’ouvre.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. Dans le **Télécharger** , faites glisser et déposez un fichier à ajouter en tant que miniature ou cliquez sur **Sélectionner pour charger**, puis recherchez un fichier image à ajouter. Le fichier doit être enregistré sur votre ordinateur.
1. (Facultatif) Utilisez l’outil de dimensionnement pour recadrer et redimensionner l’image.
1. Cliquez sur **Utiliser une image** pour ajouter l’image en tant que miniature.
Cela ferme la fenêtre **Miniature d’enregistrement** de la boîte.
1. (Conditionnel) Si vous disposez au moins des autorisations de contribution à la vue de tableau, cliquez sur **Champs** dans le coin supérieur droit de la vue du tableau.
1. Sélectionnez la variable **Miniature** pour afficher la miniature. Cette option est désélectionnée par défaut.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   La miniature s’affiche à gauche de la valeur du champ principal.
1. (Facultatif et conditionnel) Si vous ne disposez pas des autorisations de contributeur ou d’une autorisation ultérieure pour l’affichage, sélectionnez une nouvelle vue dans la **Affichage** ou créer une vue.
1. (Facultatif) Pour supprimer la miniature, passez la souris sur le champ principal et cliquez sur le bouton **Plus** menu ![](assets/more-menu.png)> **Miniature** > le **Supprimer** icon ![](assets/remove-image-icon.png), puis cliquez sur **Enregistrer les modifications**.
