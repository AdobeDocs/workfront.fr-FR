---
title: Gérer la vue chronologique
description: Accédez aux enregistrements et modifiez-les dans une vue de chronologie sur la page de type d’enregistrement de la planification Adobe Workfront. Personnalisez la chronologie à l’aide de filtres, de regroupements et de paramètres. Utilisez la fonction Ventilation pour afficher les enregistrements connectés.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '1941'
ht-degree: 81%

---

# Gérer la vue chronologique

<!--
title: Manage the timeline view 
description: You can display records in a timeline view, when accessing the record type page in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Vous pouvez afficher les enregistrements dans une vue chronologique lors de l’accès à la page du type d’enregistrement dans Adobe Workfront Planning.

Pour plus d’informations sur les vues d’enregistrement, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <p>Actuelle : formule </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> Il n’existe aucun contrôle d’accès pour Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Autorisations de gestion d’une vue</p>  
   <p>Afficher les autorisations d’une vue pour modifier temporairement les paramètres d’affichage</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Vue d’ensemble des accès</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--EDIT PERMISSIONS AND ACCESS AND REPLACE THE table above with the following table at Planning GA release: 
## Access requirements

You must have the following to be able to access Workfront Planning: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following new Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning plan*</p></td>
   <td>
<p>Any of the following Workfront Planning plans:</p>
<ul><li>Planning</li>
<li>Planning Plus</li>
</ul>
<p>For more information about what is included in each Workfront Planning plan, see <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront pricing and packaging</a>. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <ul><li><p>Any, to view Workfront Planning information</p></li>
   <li><p>Standard, to create workspaces</p></li></ul>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a> and and <a href="../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md">Assign users to a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

*********ensure that the link ^^^^^^^^above^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************

-->


## Gérer une vue chronologique {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Lors de la création d’une vue chronologique, tous les enregistrements du type d’enregistrement sélectionné s’affichent sous forme de chronologie.

Tenez compte des points suivants :

* Vous ne pouvez créer une vue chronologique que si au moins deux champs de date sont associés à un type d’enregistrement. Lorsqu’un ou plusieurs champs de date sont associés à un type d’enregistrement, l’option Vue chronologique est grisée.

  Vous pouvez effectuer une sélection dans les champs de date suivants lors de la création d’une vue de chronologie :

   * Dates d’enregistrement
   * Enregistrer les champs générés par le système : Date de création, Date de dernière modification
   * Dates de recherche à partir des types d’enregistrements ou d’objets connectés.
* Selon les dates associées aux enregistrements, il se peut que certains enregistrements ne s’affichent pas dans la vue chronologique dans les scénarios suivants :

   * Lorsque les dates de début et de fin n’ont aucune valeur.
   * Lorsque les dates de début ou de fin n’ont aucune valeur.
   * Lorsque la date de début est postérieure à la date de fin.

Pour gérer une vue chronologique, procédez comme suit :

1. Accédez à la page du type d’enregistrement pour lequel vous souhaitez afficher la chronologie.
1. Créez une vue chronologique, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Par défaut, les enregistrements associés au type d’enregistrement sélectionné s’affichent sous forme de barres dans une chronologie et sont triés dans l’ordre chronologique de leur Date de début.

   >[!TIP]
   >
   >    Le tri des enregistrements dans la chronologie n’est pas visible dans la vue compacte.

1. (Facultatif et conditionnel) Lorsque le nom de l’enregistrement est tronqué, passez la souris sur une barre d’enregistrement pour afficher le nom complet de l’enregistrement et des informations supplémentaires.

1. Pour parcourir la chronologie, effectuez l’une des opérations suivantes :

   * Cliquez sur les icônes gauche et droite ou utilisez le défilement horizontal pour passer d’un plan à l’autre dans la chronologie. L’actualisation de la page préserve la période sélectionnée.
   * Cliquez sur **Aujourd’hui** pour centrer la chronologie sur la date d’aujourd’hui.
   * Sélectionnez l’une des options suivantes dans le menu déroulant de la période pour mettre à jour les incréments de temps :

      * Année
      * Trimestre
      * Mois
1. Cliquez sur la vue **Passer en vue standard** pour afficher les enregistrements dans des lignes distinctes <!--check to see if they updated the name of the setting here-->

   Ou

   Cliquez sur **Passer en vue compacte** pour afficher les enregistrements dont les dates ne se croisent pas sur la même ligne. <!--check to see if they updated the name of the setting here-->

   Les enregistrements s’affichent par défaut dans la vue compacte.

1. Procédez comme suit pour rechercher rapidement les enregistrements correspondant à un mot-clé :

   1. Cliquez sur l’icône **Rechercher** ![](assets/search-icon.png) et commencez à saisir un mot-clé associé à n’importe quel champ d’un enregistrement qui s’affiche à l’écran. Le nombre de correspondances correctes s’affiche en regard de l’élément de recherche et l’enregistrement avec la correspondance correcte est mis en surbrillance.

      ![](assets/search-box-and-results-timeline-view.png)

      Vous pouvez utiliser n’importe quel mot ou caractère spécial visible à l’écran.

      Vous ne pouvez pas utiliser de mots-clés associés à des champs qui ne s’affichent pas dans la vue chronologique.

   1. Appuyez sur Entrée sur votre clavier pour accéder au champ suivant trouvé.
   1. (Facultatif) S’il existe plusieurs correspondances, cliquez sur les flèches haut et bas situées à droite du mot-clé de recherche pour trouver toutes les correspondances dans le tableau.
   1. Cliquez sur l’icône **x** dans la zone de recherche pour effacer le mot-clé de recherche.

1. Mettez à jour les éléments de vue suivants comme décrit dans les sous-sections ci-dessous :
   * [Filtres](#add-filters)
   * [Regroupement ](#add-grouping)
   * [Paramètres](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### Ajouter des filtres

Tirez part ides filtres pour réduire la quantité d’informations affichées à l’écran.

Tenez compte des points suivants lorsque vous utilisez des filtres dans la vue chronologique :

<!-- this list is almost identical to the one for the table view - update both-->

* Les filtres que vous créez pour une vue chronologique fonctionnent indépendamment des filtres de toute autre vue appliquée au même type d’enregistrement.

* Les filtres sont propres à la vue que vous sélectionnez. Des filtres différents peuvent être appliqués à deux vues chronologiques du même type d’enregistrement.

* Deux personnes qui consultent la même vue chronologique voient le même filtre actuellement appliqué.

* Vous ne pouvez pas nommer les filtres que vous créez pour une vue chronologique.

* La suppression d’un filtre le supprime pour toute personne accédant au même type d’enregistrement que vous et qui affiche la même vue que vous.

* L’ajout de filtres en vue chronologique est identique à l’ajout de filtres dans la vue de tableau.

  Pour plus d’informations, consultez la section « Ajouter des filtres » de l’article [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

* Vous pouvez filtrer par champ d’enregistrement ou champ de recherche connecté.
* Vous pouvez filtrer par champs de recherche qui affichent plusieurs valeurs.


### Ajouter un regroupement

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Vous pouvez regrouper des enregistrements selon des informations similaires lors de l’application d’un regroupement à une vue.

L’ajout de regroupements dans la vue chronologique est similaire à l’ajout de regroupements dans la vue de tableau.

Tenez compte des points suivants lorsque vous utilisez des regroupements dans la vue chronologique :

* Vous pouvez appliquer des regroupements dans les vues de tableau et chronologique. Les regroupements de la vue de tableau sont indépendants de ceux de la vue chronologique du même type d’enregistrement.
* Vous pouvez appliquer 3 niveaux de regroupement dans une vue. Les enregistrements sont regroupés dans l’ordre des regroupements que vous sélectionnez.
&lt;!--* Vous pouvez appliquer jusqu’à 4 niveaux de regroupement lors de l’utilisation de l’API. --point à vérifier—>
* Les regroupements sont propres à la vue sélectionnée. Deux vues de tableau d’un même type d’enregistrement peuvent avoir des regroupements différents. Deux personnes qui consultent le même tableau voient le même regroupement appliqué actuellement.
* Vous ne pouvez pas nommer les regroupements que vous créez pour une vue de tableau.
* La suppression de regroupements les supprime pour toute personne accédant au même type d’enregistrement que vous et qui affiche la même vue que vous.
* Vous pouvez modifier les enregistrements répertoriés sous un regroupement.
* Vous pouvez regrouper par champs d’enregistrement ou de recherche connectés.
* Lorsque vous effectuez un regroupement par champs de recherche avec plusieurs valeurs (qui n’ont pas été résumées par un agrégateur), les enregistrements sont regroupés selon chaque combinaison unique de valeurs de champ.
* Vous pouvez référencer un champ situé à 4 niveaux au maximum du type d’enregistrement actif. Par exemple, si vous créez un regroupement pour un type d’enregistrement Activité et que l’activité est connectée au type d’enregistrement Produit connecté au type d’enregistrement Campagne connecté à un projet Workfront, vous pouvez référencer l’état du projet dans le regroupement que vous créez pour le type d’enregistrement Activité .
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Pour ajouter un regroupement dans la vue chronologique :

1. Créez une vue chronologique pour un type d’enregistrement, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. Cliquez sur **Regroupement** dans le coin supérieur droit de la vue chronologique.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Cliquez sur l’un des champs proposés ou cliquez sur **Choisir un champ différent**, recherchez un autre champ, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   Le regroupement est appliqué automatiquement à la chronologie et les enregistrements s’affichent dans la zone de regroupement.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Facultatif) Répétez les étapes ci-dessus pour ajouter jusqu’à 3 regroupements.

   Le nombre de champs sélectionnés pour le regroupement s’affiche en regard de l’icône Regroupement.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Facultatif) Dans la zone **Regrouper les enregistrements par**, cliquez sur l’icône **x** en regard d’un champ sélectionné pour le regroupement afin de supprimer le regroupement.

   Ou

   Cliquez sur **Effacer tout** pour supprimer tous les champs.

1. Cliquez en dehors de la zone **Regrouper les enregistrements par** pour la fermer.
1. (Facultatif) Cliquez sur **Paramètres**, puis sur **Couleur** pour attribuer des couleurs aux regroupements. Pour plus d’informations, consultez la section [Modifier les paramètres de la vue chronologique](#edit-the-timeline-view-settings) de cet article.
   <!--1. (Optional) Click **Breakdown** to display connected records on the timeline. For information, see the section [Use the Breakdown feature to display connected records in the timeline view](#break-down-connected-records-in-the-timeline-view)-->

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Modifier les paramètres de la vue chronologique {#edit-the-timeline-view-settings}

Mettez à jour les paramètres de la vue chronologique pour indiquer la nature et le mode d’affichage des informations dans la vue chronologique.

1. Créez une vue chronologique pour un type d’enregistrement, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. Cliquez sur **Paramètres**.
1. Cliquez sur **Date et heure** dans le panneau de gauche, puis sélectionnez une **Date de début** et une **Date de fin** pour l’afficher dans la chronologie. Vous pouvez choisir les dates de début et de fin par défaut ou choisir n’importe quel champ de date disponible. Les barres représentant les enregistrements commencent à la date que vous indiquez pour la date de début et se terminent à la date correspondant à la date de fin.

   >[!NOTE]
   >
   >Les enregistrements qui ne comportent aucune valeur pour les dates de début ou de fin ou dont la date de début est postérieure à la date de fin ne s’affichent pas dans la vue chronologique.

1. Cliquez sur **Style de barre** dans le panneau de gauche pour indiquer les champs à afficher dans les barres d’enregistrement.

   Le champ principal (ou titre) de l’enregistrement, tel que défini dans la vue de table de l’enregistrement, est sélectionné par défaut. <!--adjust this when the primary field is released??-->

1. (Facultatif et le cas échéant) Si vous avez ajouté des miniatures aux enregistrements, sélectionnez l’option Miniature pour afficher l’image associée aux enregistrements dans leur barre d’enregistrement.

   >[!NOTE]
   >
   >    Vous devez d’abord ajouter des miniatures dans la vue de tableau avant de pouvoir les afficher dans la vue chronologique. Pour plus d’informations, voir [Ajout d’une miniature à un enregistrement](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Cliquez sur **Ajouter un champ** pour ajouter jusqu’à 4 champs aux barres d’enregistrement.
1. Cliquez dans la zone **Champs de recherche**, puis cliquez sur le champ à ajouter.

   >[!TIP]
   >
   >   * Vous devez créer les champs avant de pouvoir les ajouter aux barres d’enregistrement.
   > 
   >   * Vous devez sélectionner au moins un champ. Le champ **Nom** est sélectionné par défaut.

   Une prévisualisation de l’aspect des barres dans la chronologie s’affiche à droite.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Cliquez sur **Couleur** dans le panneau de gauche pour personnaliser les couleurs des enregistrements et des regroupements dans la chronologie.

   ![](assets/color-tab-timeline-view.png)

1. (Conditionnel et le cas échéant) Si vous avez ajouté un regroupement à la vue chronologique, sélectionnez l’une des options suivantes pour définir la couleur du regroupement dans la section **Définir la couleur du regroupement** :

   * **Par défaut (gris)** : la couleur des regroupements est définie sur gris. Il s’agit du paramètre par défaut.
   * **Valeurs de champ** : la couleur des groupements correspond à la couleur du champ par lequel vous effectuez un groupement.

     >[!NOTE]
     >
     >    * Vous ne pouvez faire correspondre la couleur qu’aux champs contenant des options codées par couleur. Par exemple, vous pouvez faire correspondre la couleur aux champs État ou aux champs auxquels des options sont associées.
     >    
     >    * Vous ne pouvez pas faire correspondre la couleur aux champs de recherche des types d’enregistrement ou d’objet liés.


   Par exemple, les champs à sélection unique ou multiple peuvent comporter des choix de code couleur.

   Si vous effectuez un regroupement par champs sans choix de code couleur, la couleur du regroupement reste grise.

   >[!TIP]
   >
   >Si vous n’avez pas ajouté de regroupements à la vue chronologique, cette section ne s’affiche pas.

1. Dans la section **Définir la couleur de l’enregistrement**, sélectionnez l’une des options suivantes pour définir une couleur pour les enregistrements :

   * **Type d’enregistrement** : la couleur des enregistrements correspond à celle du type d’enregistrement que vous avez sélectionné. Il s’agit de l’option par défaut.
   * **Valeurs de champ** : la couleur des enregistrements correspond à la couleur d’un champ que vous spécifiez. Passez à l’étape 10. <!--ensure this stays accurate-->
   * **Regroupement** : la couleur des enregistrements correspond à la couleur que vous avez indiquée pour les regroupements. Cette option est grisée lorsque aucun regroupement n’est appliqué à la vue chronologique.
   * **Aucun** : les enregistrements s’affichent dans une barre blanche.

1. (Le cas échéant) Si vous avez sélectionné **Valeurs de champ** pour les couleurs d’enregistrement, sélectionnez un champ dans le menu déroulant **Faire correspondre la couleur de l’enregistrement à**.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Seuls les champs avec des choix de code couleur s’affichent dans le menu déroulant.

   Par exemple, les champs à sélection unique ou multiple peuvent comporter des choix de code couleur.

   Si vous ne disposez pas d’un champ avec des choix de code couleur pour le type d’enregistrement sélectionné, cette option est grisée.

1. Cliquer sur **Enregistrer**.

   Les enregistrements s’affichent en vue chronologique avec les spécifications que vous avez sélectionnées.

<!--
### Use the Breakdown feature to display connected records in the timeline view

You can display connected records in a record's timeline view by using the Breakdown feature. Breaking down records by their connections allows you to view the timelines of other connected records and understand how they might affect the performance and deadlines of your records. 

#### Considerations when using the Breakdown feature

* You can display connected records or objects under the records of the selected record type in the timeline view. 
* You can display the following in the timeline view, using the Breakdown feature:
    * Workfront Planning records connected to the selected record type. 
    * Workfront (*************or AEM Assets*************)  object types connected to the selected record type.
    * Workfront Planning records or objects from other application that are connected to records connected to the selected record type. 
    
        For example, you might connect campaigns to portfolios. In addition, you might connect  another record type, products, with projects, as well as with campaigns. When you build the campaign timeline view, you can break down the campaigns by portfolios, products, and projects. 

* You cannot display object types that are connected only to Workfront objects in Workfront, but are not connected to a Workfront Planning record type. You can only display object or record types that are connected in Workfront Planning. 

    For example, tasks, are connected to projects in Workfront. Using the Breakdown feature, you can display projects that are connected to campaigns in Planning, but not tasks connected to projects in Workfront. 

    If you want to display both portfolios and projects in the timeline view of a Workfront Planning record type, both the portfolios and the projects must be connected to the Planning record or to a record connected to the Planning record whose timeline view you are managing.
* You can only display record types that are associated with at least two date fields. 
* The date fields for the record types you want to display in the timeline view must be visible in the table view of the selected record type, as lookup fields. 
* The Start and End dates of the record types you want to display in the timeline view must by in chronological order. For example, if a record has a Start date of January 31 and an End date of January 1, it does not display in the timeline view. For more information, see the section [Manage a timeline view](#manage-a-timeline-view) in this article. 
* There is a limit of 5 record types that you can include in a record's breakdown. 


#### Break down connected records in the timeline view

1. Create a timeline view for a record type, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 
1. Click **Breakdown**.
1. Expand the **Select a linked record type** box and select a connected record type. (**************add new screen shot***************)

    ![](assets/breakdown-picker-and-button-on-timeline.png)

    >[!TIP]
    >
    >    If you do not have any connected records, or if the connected records do not have at least two date fields, the **Select a linked record type** box is not available.

1. Choose a **Start date** and an **End date field**.

    >[!TIP]
    >
    >    The Start and End dates must be sequential. If the End date is before the Start date, no records will display in the timeline. 

    A right-pointing arrow displays on the selected record's bar in the timeline, if they they are connected with other records. 

    ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)    


1. (Optional) Repeat the steps above to add more connected records. 

    >[!TIP]
    >
    >    You can add up to 5 connected records in a timeline using the Breakdown feature. 


-->