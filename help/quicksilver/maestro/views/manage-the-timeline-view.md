---
title: Gestion du mode Chronologie
description: Vous pouvez afficher les enregistrements dans une vue chronologique lors de l’accès à la page de type enregistrement dans Adobe Manager.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

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

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez afficher les enregistrements dans une vue chronologique lors de l’accès à la page de type enregistrement dans Adobe Manager.

Pour plus d’informations sur les vues Maestro, voir [Gestion des vues d’enregistrement dans Adobe Maestro](../views/manage-record-views.md).

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

Lors de la création d’une vue de chronologie, tous les enregistrements du type d’enregistrement sélectionné s’affichent par défaut dans une chronologie sous forme de barres.

Pour gérer une vue de chronologie :

1. Accédez à la page de type enregistrement pour laquelle vous souhaitez afficher la chronologie.
1. Créez une vue chronologique, comme décrit dans l’article . [Gestion des vues d’enregistrement](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Les enregistrements associés au type d’enregistrement que vous avez sélectionné s’affichent dans une chronologie chronologique sous la forme de barres.

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

1. Mettez à jour les éléments de vue suivants comme décrit dans les sous-sections ci-dessous :
   * [Filtres](#add-filters)
   * [Regroupement](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [Paramètres](#edit-the-timeline-view-settings)

### Ajout de filtres

Les filtres permettent de réduire la quantité d’informations affichées à l’écran.

Tenez compte des points suivants lorsque vous utilisez des filtres dans la vue de chronologie :

<!-- this list is almost identical to the one for the table view - update both-->

* Les filtres que vous créez pour la vue de chronologie fonctionnent indépendamment des filtres de la vue de tableau lorsqu’ils sont appliqués au même type d’enregistrement.

* Les filtres sont propres à la vue que vous sélectionnez. Des filtres différents peuvent être appliqués à deux vues de chronologie du même type d’enregistrement. Deux utilisateurs qui consultent la même vue de chronologie voient le même filtre actuellement appliqué.

* Vous ne pouvez pas nommer les filtres que vous créez et appliquez à une vue chronologique.

* Le fait de supprimer des filtres les supprime de toute personne accédant au même type d’enregistrement que vous et utilise la même vue que celle que vous utilisez.

L’ajout de filtres en mode Chronologie est identique à l’ajout de filtres dans la vue Tableau.

Pour plus d’informations, voir la section &quot;Ajouter des filtres&quot; de l’article [Gestion de la vue de tableau](../views/manage-the-table-view.md).

### Ajouter un regroupement

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


Vous pouvez regrouper des enregistrements selon des informations similaires lors de l’application d’un groupement à une vue.

Tenez compte des points suivants lorsque vous utilisez des regroupements dans la vue de chronologie :

* Vous pouvez appliquer des regroupements dans les vues de tableau et de chronologie. Les regroupements de la vue de tableau sont indépendants de ceux de la vue de chronologie du même type d’enregistrement.
* Vous pouvez appliquer 3 niveaux de regroupement dans une vue Maestro. Les enregistrements sont regroupés dans l&#39;ordre des groupements que vous sélectionnez.
* Vous pouvez appliquer jusqu’à 4 niveaux de regroupement lors de l’utilisation de l’API.

Pour ajouter un groupement :

1. Créez une vue chronologique, comme décrit dans l’article . [Gestion des vues d’enregistrement](../views/manage-record-views.md).
1. Cliquez sur **Regroupement**.

   ![](assets/grouping-ui-timeline-view.png)

1. Cliquez sur l’un des champs proposés ou cliquez sur **Choisir un champ différent** et recherchez un autre champ, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   >[!TIP]
   >
   >Vous ne pouvez pas sélectionner de champs liés.

   Le groupement est appliqué automatiquement à la chronologie et les enregistrements s&#39;affichent dans la zone de groupement. Le nombre d’éléments d’un groupement s’affiche sur la ligne de groupement.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Facultatif) Répétez les étapes ci-dessus pour ajouter jusqu’à 3 regroupements.

   Le nombre de groupements appliqués s&#39;affiche à gauche de l&#39;icône Groupement située dans le coin supérieur droit de la barre d&#39;outils.

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Facultatif) Cliquez sur le **x** icône à droite d&#39;un groupement pour supprimer le groupement

   Ou

   Cliquez sur **Effacer tout** pour supprimer tous les regroupements.

1. Cliquez en dehors du **Regrouper les enregistrements par** pour le fermer.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Modification des paramètres de vue de la chronologie {#edit-the-timeline-view-settings}

Mettez à jour les paramètres de vue de la chronologie pour indiquer les informations qui s’affichent dans la section de la chronologie de la vue.

1. Créez une vue chronologique, comme décrit dans l’article . [Gestion des vues d’enregistrement](../views/manage-record-views.md).
1. Cliquez sur **Paramètres**.
1. Cliquez sur **Date et heure** dans le panneau de gauche, puis sélectionnez une **Date de début** et un **Date de fin** pour l’afficher dans la chronologie. Vous pouvez choisir les dates de début et de fin par défaut ou choisir n’importe quel champ de date disponible. Les barres représentant les enregistrements commencent à la date que vous indiquez pour la date de Début et se terminent à la date correspondant à la date de Fin.

   >[!NOTE]
   >
   >    Les enregistrements qui ne comportent aucune valeur pour les dates de début ou de fin ou dont la date de début est postérieure à la date de fin ne s’affichent pas dans la vue de chronologie.


1. Cliquez sur **Détails de l’enregistrement** pour indiquer les champs que vous souhaitez afficher dans les bandes d’enregistrement.

   Le champ Nom est sélectionné par défaut.

1. Cliquez sur **Ajouter un champ** pour ajouter jusqu’à 4 champs aux barres d’enregistrement.
1. Cliquez dans le **Champs de recherche** puis cliquez sur le champ à ajouter.

   >[!TIP]
   >
   >   * Vous devez créer les champs avant de pouvoir les ajouter aux barres d’enregistrement.
   > 
   >   * Vous devez avoir sélectionné au moins un champ. **Nom** est sélectionné par défaut.

   Un aperçu de l’aspect des barres dans la chronologie s’affiche à droite.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Cliquer sur **Enregistrer**.

   Les enregistrements s’affichent en mode Chronologie avec les spécifications que vous avez sélectionnées.

