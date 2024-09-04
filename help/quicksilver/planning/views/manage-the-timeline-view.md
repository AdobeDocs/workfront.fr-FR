---
title: Gérer la vue chronologique
description: Accédez aux enregistrements et modifiez-les dans une vue de chronologie sur la page de type d’enregistrement de la planification Adobe Workfront. Personnalisez la chronologie à l’aide de filtres, de regroupements et de paramètres. Utilisez la fonction Ventilation pour afficher les enregistrements connectés.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '2620'
ht-degree: 60%

---

# Gérer la vue chronologique

{{planning-important-intro}}

Vous pouvez afficher les enregistrements dans une vue chronologique lors de l’accès à la page du type d’enregistrement dans Adobe Workfront Planning.

Pour plus d’informations sur les vues d’enregistrement, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

Pour pouvoir accéder à Workfront Planning, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des projets Workfront suivants est prévu :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Formule de planification Adobe Workfront*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations pour une vue</p>  
   <p>Afficher les autorisations d’une vue pour modifier temporairement les paramètres d’affichage</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


## Gérer une vue chronologique {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Lors de la création d’une vue chronologique, tous les enregistrements du type sélectionné s’affichent dans un ordre chronologique.

Tenez compte des points suivants :

* Vous ne pouvez créer une vue chronologique que si vous avez au moins deux champs de date associés à un type d’enregistrement. Lorsque vous avez un ou plusieurs champs de date associés à un type d’enregistrement, l’option de vue chronologique est grisée.

  Vous pouvez effectuer une sélection dans les champs de date suivants lors de la création d’une vue de chronologie :

   * Dates d’enregistrement
   * Enregistrer les champs générés par le système : Date de création, Date de dernière modification
   * Dates de recherche à partir des types d’enregistrements ou d’objets connectés.
* En fonction des dates associées aux enregistrements, certains enregistrements peuvent ne pas s’afficher dans la vue chronologique dans les scénarios suivants :

   * Lorsque les dates de début et de fin n’ont pas de valeur.
   * Lorsque les dates de début ou de fin n’ont pas de valeur.
   * Lorsque la date de début est postérieure à la date de fin.

Pour gérer une vue chronologique :

1. Accédez à la page du type d’enregistrement pour lequel vous souhaitez consulter la chronologie.
1. Créez une vue chronologique, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Les enregistrements associés au type d’enregistrement que vous avez sélectionné s’affichent sous forme de barres dans une chronologie et sont triés par ordre chronologique de leur date de début, par défaut.

   >[!TIP]
   >
   >    Le tri des enregistrements dans la chronologie n’est pas visible dans la vue compacte.

1. (Facultatif et conditionnel) Lorsque le nom de l’enregistrement est tronqué, passez la souris sur une barre d’enregistrement pour afficher le nom complet de l’enregistrement et des informations supplémentaires.

1. Effectuez l’une des opérations suivantes pour naviguer dans la chronologie :

   * Cliquez sur les icônes gauche et droite ou utilisez le défilement horizontal pour passer d’un plan à l’autre dans la chronologie. L’actualisation de la page préserve la période sélectionnée.
   * Cliquez sur **Aujourd’hui** pour centrer la chronologie sur la date d’aujourd’hui.
   * Sélectionnez l’une des options suivantes dans le menu déroulant de la période pour mettre à jour les incréments de temps :

      * Année
      * Trimestre
      * Mois
1. Cliquez sur **Passer en vue standard** pour afficher les enregistrements sur des lignes séparées.<!--check to see if they updated the name of the setting here-->

   Ou

   Cliquez sur **Passer en vue compacte** pour afficher les enregistrements dont les dates ne se croisent pas sur la même ligne.<!--check to see if they updated the name of the setting here-->

   Les enregistrements s’affichent par défaut dans la vue compacte.

1. Procédez comme suit pour trouver rapidement les enregistrements correspondant à un mot-clé :

   1. Cliquez sur l’icône **Rechercher** ![](assets/search-icon.png) et commencez à saisir un mot-clé associé à n’importe quel champ d’un enregistrement qui s’affiche à l’écran. Le nombre de correspondances correctes s’affiche à côté de l’élément de la recherche et l’enregistrement correspondant est surligné.

      ![](assets/search-box-and-results-timeline-view.png)

      Vous pouvez utiliser n’importe quel mot ou caractère spécial visible à l’écran.

      Vous ne pouvez pas utiliser de mots-clés associés à des champs qui ne s’affichent pas dans la vue chronologique.

   1. Appuyez sur la touche Entrée de votre clavier pour passer au champ suivant.
   1. (Facultatif) S’il y a plus d’une correspondance, cliquez sur les flèches haut et bas situées à droite du mot-clé de recherche pour accéder à l’ensemble des correspondances dans le tableau.
   1. Cliquez sur l’icône **x** dans le champ de recherche pour effacer le mot-clé de la recherche.

1. Mettez à jour les éléments de vues suivants, comme décrit dans les sous-sections ci-dessous :
   * [Filtres](#add-filters)
   * [Regroupement ](#add-grouping)
   * [Paramètres](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not yet in timeline; also check the anchor and make sure it's correct-->

1. (Facultatif) Cliquez sur **Ventilation** pour afficher les enregistrements connectés dans la chronologie.

   Pour plus d’informations, reportez-vous à la section [Utilisation de la fonction de ventilation pour afficher les enregistrements connectés dans la vue de chronologie](#break-down-connected-records-in-the-timeline-view)

### Ajouter des filtres

Vous pouvez réduire la quantité d’informations affichées à l’écran en utilisant des filtres.

Tenez compte des points suivants lorsque vous utilisez des filtres dans la vue chronologique :

<!-- this list is almost identical to the one for the table view - update both-->

* Les filtres que vous créez pour une vue chronologique fonctionnent indépendamment des filtres de toute autre vue appliquée au même type d’enregistrement.

* Les filtres sont propres à la vue que vous sélectionnez. Des filtres différents peuvent être appliqués à deux vues chronologiques du même type d’enregistrement.

* Deux personnes qui consultent la même vue chronologique voient le même filtre actuellement appliqué.

* Vous ne pouvez pas nommer les filtres que vous créez pour une vue chronologique.

* En supprimant les filtres, vous les supprimez pour toutes les personnes qui accèdent au même type d’enregistrement que vous et qui consultent la même vue que vous.

* L’ajout de filtres dans la vue chronologique est identique à l’ajout de filtres dans la vue tableau.

  Pour plus d’informations, consultez la section « Ajout de filtres » dans l’article [Gestion de la vue tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

* Vous pouvez filtrer par champ d’enregistrement ou champ de recherche connecté.
* Vous pouvez filtrer par champs de recherche qui affichent plusieurs valeurs.


### Ajouter un regroupement

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Vous pouvez regrouper des enregistrements par des informations similaires lorsque vous appliquez un regroupement à une vue.

L’ajout de regroupements dans la vue chronologique est identique à l’ajout de regroupements dans la vue tableau.

Tenez compte des points suivants lorsque vous utilisez des regroupements dans la vue chronologique :

* Vous pouvez utiliser des regroupements à la fois dans la vue tableau et dans la vue chronologique. Les regroupements de la vue de tableau sont indépendants de ceux de la vue chronologique du même type d’enregistrement.
* Vous pouvez appliquer 3 niveaux de regroupement dans une vue. Les enregistrements sont regroupés dans l’ordre des regroupements que vous sélectionnez.
&lt;!--* Vous pouvez appliquer jusqu’à 4 niveaux de regroupement lorsque vous utilisez l’API. --vérifier celui-ci pour l’instant-->
* Les regroupements sont propres à la vue que vous sélectionnez. Vous pouvez appliquer des regroupements différents à deux vues de tableau du même type d’enregistrement. Deux utilisateurs ou utilisatrices qui consultent la même vue de tableau voient le regroupement qui est actuellement appliqué.
* Vous ne pouvez pas nommer les regroupements que vous créez pour une vue de tableau.
* En supprimant les regroupements, vous les supprimez pour toutes les personnes qui accèdent au même type d’enregistrement que vous et qui consultent la même vue que vous.
* Vous pouvez modifier les enregistrements répertoriés dans un regroupement.
* Vous pouvez regrouper par champs d’enregistrement ou de recherche connectés.
* Lorsque vous effectuez un regroupement par champs de recherche avec plusieurs valeurs (qui n’ont pas été résumées par un agrégateur), les enregistrements sont regroupés selon chaque combinaison unique de valeurs de champ.
* Vous pouvez référencer un champ situé à 4 niveaux au maximum du type d’enregistrement actif. Par exemple, si vous créez un regroupement pour un type d’enregistrement Activité et que l’activité est connectée au type d’enregistrement Produit connecté au type d’enregistrement Campagne connecté à un projet Workfront, vous pouvez référencer l’état du projet dans le regroupement que vous créez pour le type d’enregistrement Activité .
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Pour ajouter un regroupement dans la vue chronologique :

1. Créez une vue chronologique pour un type d’enregistrement, comme décrit dans l’article [Gestion des vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. Cliquez sur **Regroupement** dans le coin supérieur droit de la vue chronologique.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Cliquez sur l’un des champs proposés ou cliquez sur **Choisir un champ différent**, recherchez un autre champ, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   Le regroupement est appliqué automatiquement à la chronologie et les enregistrements s’affichent dans la zone de regroupement.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Facultatif) Répétez les étapes ci-dessus pour ajouter jusqu’à 3 regroupements.

   Le nombre de champs sélectionnés pour le regroupement s’affiche à côté de l’icône de regroupement.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Facultatif) Dans la zone **Regrouper les enregistrements par**, cliquez sur l’icône **x** à droite d’un champ sélectionné pour le regroupement pour le supprimer.

   Ou

   Cliquez sur **Tout effacer** pour supprimer tous les champs.

1. Cliquez en dehors de la zone **Regrouper les enregistrements par** pour la fermer.
1. (Facultatif) Cliquez sur **Paramètres**, puis sur **Couleur** pour attribuer des couleurs aux regroupements. Pour plus d’informations, consultez la section [Modifier les paramètres de la vue chronologique](#edit-the-timeline-view-settings) dans cet article.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Modifier les paramètres de la vue chronologique {#edit-the-timeline-view-settings}

Mettez à jour les paramètres de la vue chronologique pour indiquer le type d’informations qui s’affichent dans la section chronologique de la vue et la façon dont elles s’affichent.

1. Créez une vue chronologique pour un type d’enregistrement, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. Cliquez sur **Paramètres**.
1. Cliquez sur **Date et heure** dans le panneau de gauche, puis sélectionnez une **Date de début** et une **Date de fin** à afficher sur la chronologie. Vous pouvez choisir les dates de début et de fin par défaut ou n’importe quel champ de date disponible. Les barres représentant les enregistrements commencent à la date que vous indiquez pour la date de début et se terminent à la date correspondant à la date de fin.

   >[!NOTE]
   >
   >Les enregistrements qui n’ont pas de valeurs pour les dates de début ou de fin ou dont la date de début est postérieure à la date de fin ne s’affichent pas dans la vue chronologique.

1. Cliquez sur **Style de barre** dans le panneau de gauche, pour indiquer les champs que vous souhaitez afficher dans les barres d’enregistrement.

   Le champ principal (ou titre) de l’enregistrement, tel que défini dans la vue de table de l’enregistrement, est sélectionné par défaut. <!--adjust this when the primary field is released??-->

1. (Facultatif et le cas échéant) Si vous avez ajouté des miniatures aux enregistrements, sélectionnez l’option Miniature pour afficher l’image associée aux enregistrements dans leur barre d’enregistrement.

   >[!NOTE]
   >
   >    Vous devez d’abord ajouter les miniatures dans la vue de tableau, avant de pouvoir les afficher dans la vue chronologique. Pour plus d’informations, voir [Ajout d’une miniature à un enregistrement](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Cliquez sur **Ajouter un champ** pour ajouter jusqu’à 4 champs aux barres d’enregistrement.
1. Cliquez dans la zone **Champs de recherche** et cliquez sur le champ que vous souhaitez ajouter.

   >[!TIP]
   >
   >   * Vous devez créer les champs avant de les ajouter aux barres d’enregistrement.
   > 
   >   * Vous devez disposer d’au moins un champ sélectionné. Le **nom** est sélectionné par défaut.

   Un aperçu de l’aspect des barres sur la chronologie s’affiche à droite.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Cliquez sur **Couleur** dans le panneau de gauche pour personnaliser les couleurs des enregistrements et des regroupements dans la chronologie.

   ![](assets/color-tab-timeline-view.png)

1. (Le cas échéant et facultatif) Si vous avez ajouté un regroupement à la vue chronologique, sélectionnez l’une des options suivantes pour définir une couleur pour le regroupement dans la section **Définir la couleur du regroupement** :

   * **Par défaut (gris)** : la couleur des regroupements est le gris. Il s’agit de la valeur par défaut.
   * **Valeurs de champ** : la couleur des groupements correspond à la couleur du champ par lequel vous effectuez un groupement.

     >[!NOTE]
     >
     >    * Vous ne pouvez faire correspondre la couleur qu’aux champs contenant des options codées par couleur. Par exemple, vous pouvez faire correspondre la couleur aux champs État ou aux champs auxquels des options sont associées.
     >    
     >    * Vous ne pouvez pas faire correspondre la couleur aux champs de recherche des types d’enregistrement ou d’objet liés.


   Par exemple, les champs à sélection multiple ou unique peuvent avoir des options codées par couleur.

   Si vous effectuez un regroupement par champs sans les options de codage par couleur, la couleur du regroupement reste grise.

   >[!TIP]
   >
   >Si vous n’avez pas ajouté de regroupements à la vue chronologique, cette section ne s’affiche pas.

1. Dans la section **Définir la couleur de l’enregistrement**, sélectionnez l’une des options suivantes pour définir la couleur des enregistrements :

   * **Type d’enregistrement** : la couleur des enregistrements correspond à la couleur du type d’enregistrement que vous avez sélectionné. Il s’agit de l’option par défaut.
   * **Valeurs des champs** : la couleur des enregistrements correspond à la couleur d’un champ que vous spécifiez. Passez à l’étape 10. <!--ensure this stays accurate-->
   * **Regroupement** : la couleur des enregistrements correspond à la couleur que vous avez indiquée pour les regroupements. Cette option est grisée lorsqu’aucun regroupement n’est appliqué à la vue chronologique.
   * **Aucune** : les enregistrements s’affichent dans une barre blanche.

1. (Le cas échéant) Si vous avez sélectionné **Valeurs de champ** pour les couleurs des enregistrements, sélectionnez un champ dans le menu déroulant **Faire correspondre la couleur de l’enregistrement à**.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Seuls les champs dont les options sont codées en couleur s’affichent dans le menu déroulant.

   Par exemple, les champs à sélection multiple ou unique peuvent avoir des options codées par couleur.

   Si vous n’avez pas de champ avec des options codées par couleur pour le type d’enregistrement sélectionné, cette option est grisée.

1. Cliquer sur **Enregistrer**.

   Les enregistrements s’affichent dans la vue chronologique avec les spécifications que vous avez sélectionnées.

### Utilisez la fonction Ventilation pour afficher les enregistrements connectés dans la vue de chronologie.

Vous pouvez afficher les enregistrements connectés dans la vue de chronologie d’un enregistrement à l’aide de la fonction Ventilation . La ventilation des enregistrements selon leur connexion vous permet d’afficher les chronologies des autres enregistrements connectés et de comprendre comment ils peuvent affecter les performances et les échéances de vos enregistrements.

#### Remarques concernant l’utilisation de la fonction de ventilation

* Vous pouvez afficher les enregistrements ou les objets connectés sous les enregistrements du type d’enregistrement sélectionné dans la vue de la chronologie.
* Vous pouvez afficher les éléments suivants dans la vue de chronologie à l’aide de la fonction Ventilation :
   * Enregistrements Workfront Planning connectés au type d&#39;enregistrement sélectionné.
   * Types d’objet Workfront ou ressources Experience Manager connectées au type d’enregistrement sélectionné.
   * Workfront Planning enregistre ou objets d&#39;une autre application connectés à des enregistrements connectés au type d&#39;enregistrement sélectionné.

     Par exemple, vous pouvez connecter des campagnes à des portefeuilles. En outre, vous pouvez connecter un autre type d’enregistrement, &quot;produits&quot;, aux projets, ainsi qu’aux campagnes. Lorsque vous créez la vue de chronologie de campagne, vous pouvez ventiler les campagnes par portfolios, produits et projets.

* Vous ne pouvez pas afficher les types d’objets qui ne sont connectés qu’aux objets Workfront dans Workfront, mais qui ne sont pas connectés à un type d’enregistrement Workfront Planning. Vous pouvez uniquement afficher les types d’objets ou d’enregistrements connectés dans Workfront Planning.

  Par exemple, les tâches sont connectées aux projets dans Workfront. La fonction Ventilation vous permet d’afficher les projets connectés aux campagnes dans Planification , mais pas les tâches liées aux projets dans Workfront.

  Si vous souhaitez afficher à la fois les portefeuilles et les projets dans la vue chronologique d’un type d’enregistrement de planification Workfront, les portefeuilles et les projets doivent être connectés à l’enregistrement de planification ou à un enregistrement connecté à l’enregistrement de planification dont vous gérez la vue chronologique.
* Vous ne pouvez afficher que les types d’enregistrement associés à au moins deux champs de date.
* Les champs de date pour les types d’enregistrement que vous souhaitez afficher dans la vue de chronologie doivent être visibles dans la vue de tableau du type d’enregistrement sélectionné, sous forme de champs de recherche.
* Les dates de début et de fin des types d’enregistrement que vous souhaitez afficher dans la vue de chronologie doivent être classées par ordre chronologique. Par exemple, si un enregistrement a une date de début le 31 janvier et une date de fin le 1er janvier, il ne s’affiche pas dans la vue de la chronologie. Pour plus d’informations, reportez-vous à la section [Gestion d’une vue de chronologie](#manage-a-timeline-view) de cet article.
* Il existe une limite de 5 types d’enregistrement que vous pouvez inclure dans la ventilation d’un enregistrement.

#### Ventiler les enregistrements connectés dans la vue de chronologie

1. Créez une vue chronologique pour un type d’enregistrement, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. (Conditionnel) Si vous affichez la vue de la chronologie en mode standard, cliquez sur **Ventilation**.
1. Développez la zone **Sélectionner un type d’enregistrement lié** et sélectionnez un type d’enregistrement connecté. <!--add a new screen shot - submitted a bug to remove the "the"-->

   ![](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    Si vous ne disposez d’aucun enregistrement connecté ou si les enregistrements connectés ne possèdent pas au moins deux champs de date, la zone **Sélectionner un type d’enregistrement lié** n’est pas disponible.

1. Choisissez une **Date de début** et un **Champ de date de fin**.

   >[!TIP]
   >
   >    Les dates de Début et de Fin doivent être séquentielles. Si la date de fin est antérieure à la date de début, aucun enregistrement ne s’affiche dans la chronologie.

   Une flèche pointant vers la droite s’affiche sur la barre de l’enregistrement sélectionné dans la chronologie, si ces derniers sont connectés à d’autres enregistrements.
1. Cliquez sur la flèche pointant vers la droite pour développer un type d’enregistrement et afficher les connexions.

   ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

1. (Facultatif) Répétez les étapes ci-dessus pour ajouter d’autres enregistrements connectés.



