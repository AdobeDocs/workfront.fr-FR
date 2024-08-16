---
title: Gestion de la mise en page de la page d’enregistrement
description: Vous pouvez modifier la mise en page de l’aperçu des enregistrements et de la page dans Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: d56a4721353f8b7db856eab5a3ae3b53396bd079
workflow-type: tm+mt
source-wordcount: '1054'
ht-degree: 13%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Gestion de la mise en page de la page d’enregistrement

{{planning-important-intro}}

Vous pouvez modifier la mise en page de l’aperçu des enregistrements et de la page dans Adobe Workfront Planning.

L’aperçu de l’enregistrement est une vue plus petite de la page d’enregistrement qui s’affiche dans la vue d’un type d’enregistrement.

Lorsque vous modifiez la mise en page d’un aperçu d’enregistrement et d’une page, les modifications affectent les zones d’aperçu et les pages de détails de tous les enregistrements du même type.

Cet article explique comment modifier la mise en page et l’aspect d’une boîte d’aperçu d’enregistrement ou d’une page d’enregistrement. Pour plus d&#39;informations sur la modification des enregistrements, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

Vous devez créer des types d’enregistrement et des enregistrements avant de pouvoir commencer à modifier des pages d’enregistrement.

Pour plus d’informations, voir les articles suivants :

* [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md)

* [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md)

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
   Ou
   <p>Actuelle : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Adobe Workfront Planning</p>  
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

Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant la modification de pages d’enregistrement

* Par défaut, les détails et les pages de prévisualisation d&#39;un enregistrement affichent tous les champs associés à l&#39;enregistrement.

* Vous ne pouvez pas ajouter de nouveaux champs pour un enregistrement dans la page de prévisualisation ou de détails. Vous devez ajouter de nouveaux champs dans la vue de tableau pour les afficher dans les pages de prévisualisation et de détails.

* Vous pouvez ajouter des sections à une page d’aperçu ou de détails d’enregistrement afin d’organiser les informations selon des critères communs et faciliter leur recherche.

* Les modifications suivantes affectent tous les enregistrements du même type et sont visibles par tous les utilisateurs accédant à ces enregistrements :

   * Réorganisation des champs
   * Ajout ou suppression de sections

* Les modifications d’affichage que vous apportez dans l’aperçu de l’enregistrement sont immédiatement visibles dans la page des détails de l’enregistrement. Les modifications apportées à la page d’enregistrement sont également visibles dans la zone d’aperçu des enregistrements.

* L’ajout d’une image de couverture ou d’une miniature à un enregistrement ne fait pas partie de la disposition globale de l’aperçu ou de la page d’enregistrement. Vous pouvez ajouter des images de couverture ou des miniatures uniques à chaque enregistrement. Pour plus d’informations, voir [Ajout d’une image de couverture à un enregistrement](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) et [Ajout d’une miniature à un enregistrement](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Ajout de sections à un aperçu d’enregistrement ou à une page

Tenez compte des points suivants lors de l’ajout de sections à une page d’enregistrement :

* Le nombre de sections d’une page ne peut pas être limité.
* Vous ne pouvez pas avoir de section vide. Vous devez avoir au moins un champ dans une section.
* Vous pouvez faire glisser des champs d’une section vers une autre. Pour plus d&#39;informations, reportez-vous à la section [Réorganiser les champs dans la page d&#39;aperçu des enregistrements ou de détails](#rearrange-fields-in-the-record-preview-or-details-page) de cet article.
* Lorsque vous supprimez tous les champs d’une section, celle-ci est automatiquement supprimée et ne peut pas être récupérée.

Pour ajouter une section à un aperçu d’enregistrement ou à une page :

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’ouvre.

1. Dans une vue de tout type, cliquez sur le nom d’un enregistrement.

   Ou

   Dans la vue table, cliquez sur l&#39;icône **Ouvrir les détails** ![](assets/open-details-icon-in-table-name-field.png) dans la première colonne.

   L’aperçu de l’enregistrement s’ouvre dans la vue.

   ![](assets/details-box.png)

1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page d’enregistrement s’ouvre. <!--The Details tab opens by default. -->

   ![](assets/details-page.png)

1. Dans la page ou l’aperçu de l’enregistrement <!--**Details** tab of the-->, passez la souris sur l’espace blanc situé à gauche des champs, puis cliquez sur l’icône **Ajouter une section** ![](assets/add-section-icon.png) pour ajouter une section.
1. Cliquez dans le nom de la section et remplacez **Section sans titre** par un nom, puis cliquez sur Entrée. Les champs affichés sous la section font automatiquement partie de la nouvelle section.
1. Commencez à faire glisser des champs vers la nouvelle section, comme décrit dans la section [Réorganiser les champs dans la page de prévisualisation des enregistrements ou de détails](#rearrange-fields-in-the-record-preview-or-details-page) de cet article.

1. (Facultatif) Pointez sur le nom d’une section et cliquez sur le menu **Plus** ![](assets/more-menu.png) .

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Facultatif) Pour modifier la section, effectuez l’une des opérations suivantes :

   * Cliquez sur **Renommer** pour renommer la section.

     >[!TIP]
     >
     > Vous pouvez renommer une section intégrée en cliquant sur son nom.

   * Cliquez sur **Déplacer vers le haut** pour déplacer la section vers le haut d’une position.

     Ou

     Cliquez sur **Déplacer vers le bas** pour déplacer la section vers le bas d’une position.
Tous les champs de la section sont déplacés avec la section .

   * Cliquez sur **Supprimer** pour supprimer la section. La section est supprimée et elle ne peut pas être récupérée. Tous les utilisateurs accédant aux enregistrements de ce type ne verront plus la section supprimée.

1. Cliquez sur la flèche pointant vers le bas située à gauche du nom d’une section pour la réduire ou sur la flèche pointant vers la droite pour la développer.
Par défaut, toutes les sections sont développées.

1. (Facultatif) Cliquez sur l’icône **grab** ![](assets/grab-icon.png) située à gauche du nom d’une section, puis faites-la glisser et déposez-la à l’emplacement de votre choix.

   La nouvelle position de la section est mise à jour dans l&#39;aperçu et la page de tous les enregistrements du même type pour tous les utilisateurs qui visualisent les enregistrements.

   Toutes les modifications apportées aux sections et à l’ordre des champs sont enregistrées automatiquement.

<!--1. (Optional) Click the **Connections** tab. All records or objects that are connected to the selected record display under the names of the record type, or the application they belong to. 

      ![](assets/connections-tab-on-record-in-workfront-planning.png)

      For information about connecting records from the Connections tab, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->

## Réorganiser les champs dans l’aperçu ou la page de l’enregistrement

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’ouvre.

1. Dans une vue de tout type, cliquez sur le nom d’un enregistrement.

   Ou

   Dans la vue table, cliquez sur l&#39;icône **Ouvrir les détails** ![](assets/open-details-icon-in-table-name-field.png) dans la première colonne.

   L’aperçu de l’enregistrement s’ouvre dans la vue.

   ![](assets/details-box.png)

1. (Facultatif) Cliquez sur l’icône **Ouvrir dans un nouvel onglet** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> dans le coin supérieur droit de l’aperçu de l’enregistrement pour ouvrir la page de l’enregistrement dans un nouvel onglet.

   La page de l’enregistrement s’ouvre.

   ![](assets/details-page.png)

1. Dans l’aperçu de l’enregistrement ou la page, cliquez sur l’icône **grab** ![](assets/grab-icon.png) située à gauche du nom d’un champ, puis faites-le glisser et déposez-le à l’emplacement de votre choix. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   La nouvelle position du champ est mise à jour dans la prévisualisation et la page de tous les enregistrements du même type pour tous les utilisateurs qui visualisent les enregistrements.

   Toutes les modifications apportées à la mise en page de l’aperçu de l’enregistrement ou de la page sont automatiquement enregistrées.

