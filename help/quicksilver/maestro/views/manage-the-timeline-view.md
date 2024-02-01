---
title: Gestion du mode Chronologie
description: Vous pouvez afficher les enregistrements dans une vue chronologique lors de l’accès à la page de type enregistrement dans Adobe Manager.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 0%

---

# Gestion du mode Chronologie

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Vous pouvez afficher les enregistrements dans une vue chronologique lors de l’accès à la page de type enregistrement dans Adobe Manager.

Pour plus d’informations sur les vues Maestro, voir [Gestion des vues d’enregistrement dans Adobe Maestro](../views/manage-record-views.md).

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
   <td role="rowheader">Configuration du niveau d’accès</td>
   <td> <p>Il n’existe pas de contrôle de niveau d’accès pour Maestro </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations pour l’affichage</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modèle de mise en page</td>
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## Gestion de la vue chronologique {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Lors de la création d’une vue chronologique, tous les enregistrements du type d’enregistrement sélectionné s’affichent dans une chronologie chronologique.

Tenez compte des points suivants :

* Vous ne pouvez créer une vue Chronologie que si au moins deux champs de date sont associés à un type d’enregistrement. Lorsqu’un ou plusieurs champs de date sont associés à un type d’enregistrement, l’option Mode Chronologie est grisée.
* Selon les dates associées aux enregistrements, il se peut que certains enregistrements ne s’affichent pas dans la vue de la chronologie dans les scénarios suivants :

   * Lorsque les dates de début et de fin n’ont aucune valeur
   * Lorsque les dates de début ou de fin n’ont aucune valeur
   * Lorsque la date de début est postérieure à la date de fin

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

Pour gérer une vue de chronologie :

1. Accédez à la page de type enregistrement pour laquelle vous souhaitez afficher la chronologie.
1. Créez une vue chronologique, comme décrit dans l’article . [Gestion des vues d’enregistrement](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Par défaut, les enregistrements associés au type d’enregistrement sélectionné s’affichent sous forme de barres dans une chronologie et sont triés dans l’ordre chronologique de leur Date de début.

   >[!TIP]
   >
   >    Le tri des enregistrements dans la chronologie n’est pas visible dans la vue compacte.


1. Pour parcourir la chronologie, effectuez l’une des opérations suivantes :

   * Cliquez sur les icônes gauche et droite ou utilisez le défilement horizontal pour passer d’un plan à l’autre dans la chronologie.
   * Cliquez sur **Aujourd&#39;hui** pour centrer la chronologie sur la date d’aujourd’hui.
   * Sélectionnez l’une des options suivantes dans le menu déroulant de la période pour mettre à jour les incréments de temps :

      * Année
      * Trimestre
      * Mois
1. Cliquez sur **Basculer vers Standard** affichage des enregistrements dans des lignes distinctes <!--check to see if they updated the name of the setting here-->

   Ou

   Cliquez sur **Basculer vers la vue compacte** pour afficher les enregistrements dont les dates ne se croisent pas sur la même ligne. <!--check to see if they updated the name of the setting here-->

   Les enregistrements s’affichent par défaut dans la vue compacte.

1. Procédez comme suit pour rechercher rapidement les enregistrements correspondant à un mot-clé :

   1. Cliquez sur le bouton **Rechercher** icon ![](assets/search-icon.png) et commencez à saisir un mot-clé associé à n’importe quel champ d’un enregistrement qui s’affiche à l’écran. Le nombre de correspondances correctes s’affiche en regard de l’élément de recherche et l’enregistrement avec la correspondance correcte est mis en surbrillance.

      ![](assets/search-box-and-results-timeline-view.png)

      Vous pouvez utiliser n’importe quel mot ou caractère spécial visible à l’écran.

      Vous ne pouvez pas utiliser de mots-clés associés à des champs qui ne s’affichent pas dans la vue de la chronologie.

   1. Appuyez sur Entrée sur votre clavier pour accéder au champ suivant trouvé.
   1. (Facultatif) S’il existe plusieurs correspondances, cliquez sur les flèches haut et bas situées à droite du mot-clé de recherche pour trouver toutes les correspondances dans le tableau.
   1. Cliquez sur le bouton **x** dans la zone de recherche pour effacer le mot-clé de recherche.

1. Mettez à jour les éléments de vue suivants comme décrit dans les sous-sections ci-dessous :
   * [Filtres](#add-filters)
   * [Regroupement ](#add-grouping)
   * [Paramètres](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### Ajout de filtres

Vous pouvez réduire la quantité d’informations affichées à l’écran à l’aide de filtres.

Tenez compte des points suivants lorsque vous utilisez des filtres dans la vue de chronologie :

<!-- this list is almost identical to the one for the table view - update both-->

* Les filtres que vous créez pour la vue de chronologie fonctionnent indépendamment des filtres de la vue de tableau lorsqu’ils sont appliqués au même type d’enregistrement.

* Les filtres sont propres à la vue que vous sélectionnez. Des filtres différents peuvent être appliqués à deux vues de chronologie du même type d’enregistrement. Deux utilisateurs qui consultent la même vue de chronologie voient le même filtre actuellement appliqué.

* Vous ne pouvez pas nommer les filtres que vous créez pour une vue chronologique.

* Le fait de supprimer des filtres les supprime de toute personne accédant au même type d’enregistrement que vous et qui affiche la même vue que vous.

* L’ajout de filtres en mode Chronologie est identique à l’ajout de filtres dans la vue Tableau.

  Pour plus d’informations, voir la section &quot;Ajouter des filtres&quot; de l’article [Gestion de la vue de tableau](../views/manage-the-table-view.md).

### Ajouter un regroupement

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Vous pouvez regrouper des enregistrements selon des informations similaires lors de l’application d’un groupement à une vue.

L’ajout de regroupements dans la vue de chronologie est similaire à l’ajout de regroupements dans la vue de tableau.

Tenez compte des points suivants lorsque vous utilisez des regroupements dans la vue de chronologie :

* Vous pouvez appliquer des regroupements dans les vues de tableau et de chronologie. Les regroupements de la vue de tableau sont indépendants de ceux de la vue de chronologie du même type d’enregistrement.
* Vous pouvez appliquer 3 niveaux de regroupement dans une vue Maestro. Les enregistrements sont regroupés dans l&#39;ordre des groupements que vous sélectionnez.
* Vous pouvez appliquer jusqu’à 4 niveaux de regroupement lors de l’utilisation de l’API.
* Les regroupements sont propres à la vue sélectionnée. Deux vues de chronologie d’un même type d’enregistrement peuvent être associées à des regroupements différents. Deux utilisateurs qui visualisent la même vue de chronologie voient le même regroupement actuellement appliqué.
* Vous ne pouvez pas nommer les regroupements que vous créez pour une vue chronologique.
* Le fait de supprimer des regroupements les supprime de toute personne accédant au même type d’enregistrement que vous et qui affiche la même vue que vous.

Pour ajouter un groupement dans la vue de frise chronologique :

1. Créez une vue de chronologie pour un type d’enregistrement, comme décrit dans l’article . [Gestion des vues d’enregistrement](../views/manage-record-views.md).
1. Cliquez sur **Regroupement** dans le coin supérieur droit de la vue chronologique.

   ![](assets/grouping-ui-timeline-view.png)

1. Cliquez sur l’un des champs proposés ou cliquez sur **Choisir un champ différent**, recherchez un autre champ, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   >[!TIP]
   >
   >Vous ne pouvez pas sélectionner de champs liés.

   Le groupement est appliqué automatiquement à la chronologie et les enregistrements s&#39;affichent dans la zone de groupement.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Facultatif) Répétez les étapes ci-dessus pour ajouter jusqu’à 3 regroupements.

   Le nombre de champs sélectionnés pour le groupement s&#39;affiche en regard de l&#39;icône Groupement .

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Facultatif) Dans le **Regrouper les enregistrements par** , cliquez sur le bouton **x** icône à droite d&#39;un champ sélectionné pour le groupement afin de supprimer le groupement

   Ou

   Cliquez sur **Effacer tout** pour supprimer tous les champs.

1. Cliquez en dehors du **Regrouper les enregistrements par** pour le fermer.
1. (Facultatif) Cliquez sur **Paramètres**, puis **Couleur** aux regroupements de code-couleur. Pour plus d’informations, voir [Modification des paramètres de vue de la chronologie](#edit-the-timeline-view-settings) dans cet article.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Modification des paramètres de vue de la chronologie {#edit-the-timeline-view-settings}

Mettez à jour les paramètres de vue de la chronologie pour indiquer ce qui s’affiche et comment les informations s’affichent dans la section de la chronologie de la vue.

1. Créez une vue de chronologie pour un type d’enregistrement, comme décrit dans l’article . [Gestion des vues d’enregistrement](../views/manage-record-views.md).
1. Cliquez sur **Paramètres**.
1. Cliquez sur **Date et heure** dans le panneau de gauche, puis sélectionnez une **Date de début** et un **Date de fin** pour l’afficher dans la chronologie. Vous pouvez choisir les dates de début et de fin par défaut ou choisir n’importe quel champ de date disponible. Les barres représentant les enregistrements commencent à la date que vous indiquez pour la date de Début et se terminent à la date correspondant à la date de Fin.

   >[!NOTE]
   >
   >Les enregistrements qui ne comportent aucune valeur pour les dates de début ou de fin ou dont la date de début est postérieure à la date de fin ne s’affichent pas dans la vue de chronologie.

1. Cliquez sur **Style de barre** dans le panneau de gauche, pour indiquer les champs que vous souhaitez afficher dans les barres d’enregistrement.

   Le champ Nom est sélectionné par défaut. <!--adjust this when the primary field is released??-->

1. (Facultatif et conditionnel) Si vous avez ajouté des miniatures aux enregistrements, sélectionnez l’option Miniature pour afficher l’image associée aux enregistrements dans leur barre d’enregistrement.

   >[!NOTE]
   >
   >    Vous devez d’abord ajouter des miniatures dans la vue de tableau avant de pouvoir les afficher dans la vue de chronologie. Pour plus d’informations, voir [Ajout de miniatures aux enregistrements](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

1. Cliquez sur **Ajouter un champ** pour ajouter jusqu’à 4 champs aux barres d’enregistrement.
1. Cliquez dans le **Champs de recherche** puis cliquez sur le champ à ajouter.

   >[!TIP]
   >
   >   * Vous devez créer les champs avant de pouvoir les ajouter aux barres d’enregistrement.
   > 
   >   * Vous devez avoir sélectionné au moins un champ. **Nom** est sélectionné par défaut.

   Un aperçu de l’aspect des barres dans la chronologie s’affiche à droite.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Cliquez sur **Couleur** dans le panneau de gauche, pour personnaliser les couleurs des enregistrements et des regroupements dans la chronologie.

   ![](assets/color-tab-timeline-view.png)

1. (Conditionnel et facultatif) Si vous avez ajouté un groupement à la vue de la chronologie, sélectionnez l’une des options suivantes pour définir la couleur du groupement dans la fenêtre **Définir la couleur du groupement** section :

   * **Par défaut (gris)**: la couleur des groupements est définie sur gris. Il s’agit du paramètre par défaut.
   * **Valeurs de champ**: la couleur des groupements correspond à la couleur du champ par lequel vous effectuez un groupement.
Vous pouvez faire correspondre la couleur des regroupements uniquement aux champs avec des options codées par couleur.

   Par exemple, les champs à sélection multiple ou à sélection unique peuvent comporter des options codées par couleur.

   Si vous effectuez un groupement par champs sans options codées par couleur, la couleur du groupement reste grise.

   >[!TIP]
   >
   >Si vous n’avez pas ajouté de groupes à la vue de la chronologie, cette section ne s’affiche pas.

1. Dans le **Définir la couleur de l’enregistrement** , sélectionnez l’une des options suivantes pour définir une couleur pour les enregistrements :

   * **Type d’enregistrement**: la couleur des enregistrements correspond à celle du type d’enregistrement que vous avez sélectionné. Il s’agit de l’option par défaut.
   * **Valeurs de champ**: la couleur des enregistrements correspond à la couleur d’un champ que vous spécifiez. Passez à l’étape 10. <!--ensure this stays accurate-->
   * **Regroupement**: la couleur des enregistrements correspond à la couleur que vous avez indiquée pour les regroupements. Cette option est grisée lorsque aucun regroupement n’est appliqué à la vue de la chronologie.
   * **Aucun**: les enregistrements s’affichent dans une barre blanche.

1. (Conditionnel) Si vous avez sélectionné **Valeurs de champ** pour les couleurs d’enregistrement, sélectionnez un champ dans la **Correspondance de la couleur de l’enregistrement avec** menu déroulant.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Seuls les champs avec des options codées par couleur s’affichent dans le menu déroulant.

   Par exemple, les champs à sélection multiple ou à sélection unique peuvent comporter des options codées par couleur.

   Si vous ne disposez pas d’un champ avec des options codées par couleur pour le type d’enregistrement sélectionné, cette option est grisée.

1. Cliquer sur **Enregistrer**.

   Les enregistrements s’affichent en mode Chronologie avec les spécifications que vous avez sélectionnées.
