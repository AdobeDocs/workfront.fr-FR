---
title: Duplication d'enregistrements
description: Vous pouvez dupliquer un enregistrement existant en mode Tableau. Une copie identique de l’enregistrement existant est ajoutée à la page de type enregistrement.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 32%

---


# Duplication d&#39;enregistrements

<!--update the metadata after GA-->

{{planning-important-intro}}

Dans Adobe Workfront Planning, un enregistrement est une instance d’un type d’enregistrement.

Vous pouvez dupliquer un enregistrement existant en mode Tableau. Une copie identique de l’enregistrement existant est ajoutée à la page de type enregistrement.

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
   <p>Actuelle : formule</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Adobe Workfront Planning </p>  
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

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Dupliquer un enregistrement <!--in a record type table (I don't think you can create them elsewhere right now)-->

Vous pouvez créer des enregistrements dans la vue table d’une page de type enregistrement en dupliquant une page existante. Un enregistrement identique à celui existant est créé et ajouté sous l’enregistrement d’origine.


{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement. Pour plus d’informations sur la création d’un type d’enregistrement, voir [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page de type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type d’enregistrement s’ouvre dans la vue de tableau.
Tous les enregistrements du type sélectionné s&#39;affichent dans la vue.

1. (Conditionnel) Sélectionnez une vue de tableau.

1. Utilisez l’une des méthodes suivantes :

   * Passez la souris sur le nom d’un enregistrement, puis cliquez sur le menu **Plus** en ligne avec le nom de l’enregistrement, puis cliquez sur l’icône **Dupliquer** ![](assets/duplicate-icon-gray.png) .

     ![](assets/more-menu-from-record-in-table-view.png)

   * Sélectionnez un enregistrement, puis cliquez sur l’icône **Dupliquer** ![](assets/duplicate-icon-white-and-blue.png) de la barre d’outils située au bas de la page.

     ![](assets/duplicate-icon-in-toolbar-in-table-view.png)

   Un enregistrement identique portant le même nom est créé sous l’enregistrement d’origine. Tous les champs du nouvel enregistrement sont renseignés avec les mêmes informations que dans l’enregistrement d’origine.

1. (Facultatif) Commencez à mettre à jour les informations sur le nouvel enregistrement dans les champs disponibles dans la vue de tableau, ou cliquez sur l’enregistrement et mettez à jour les informations dans l’aperçu de l’enregistrement ou la page.

   >[!NOTE]
   >
   >  * Il n’existe aucun champ obligatoire pour les enregistrements. Nous vous recommandons toutefois d’ajouter des informations pour le champ principal d’un enregistrement, car il est utile d’identifier les enregistrements lors de la liaison d’enregistrements. Pour plus d’informations sur les champs principaux, voir [Gestion de la vue de table](/help/quicksilver/planning/views/manage-the-table-view.md) et [Présentation des champs de Principal](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Les champs qui font référence à d’autres types d’enregistrement ou à des champs calculés sont en lecture seule.

   Pour plus d&#39;informations sur la modification des enregistrements, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

1. (Facultatif) Utilisez les raccourcis clavier suivants pour annuler ou rétablir l’ajout de nouveaux enregistrements ou de leurs informations lors de leur ajout dans la vue de tableau :

   * Ctrl+Z (⌘+Z pour Mac) pour annuler une modification
   * Ctrl + Maj + Z (⌘ + Maj + Z pour Mac) pour rétablir une modification.