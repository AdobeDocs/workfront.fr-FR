---
title: Gérer la vue chronologique
description: Accédez aux enregistrements et modifiez-les dans une vue chronologique sur la page Type d’enregistrement Adobe Workfront Planning. Cet article décrit comment créer une vue de chronologie et modifier ou supprimer une vue existante. Personnalisez la chronologie à l’aide de filtres, de regroupements et de paramètres. Utilisez la fonction Répartition pour afficher les enregistrements connectés.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 3dfac5ada17248f5c67380b56b9a0969b10b73e6
workflow-type: tm+mt
source-wordcount: '2878'
ht-degree: 53%

---

# Gérer la vue chronologique

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez afficher les enregistrements dans une vue chronologique lors de l’accès à la page du type d’enregistrement dans Adobe Workfront Planning.

Pour plus d’informations sur les vues d’enregistrement, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
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
   <p>Autorisations d’affichage d’une vue pour modifier temporairement les paramètres d’affichage ou la dupliquer</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut Planning.</p>
<p><span class="preview">Dans l’environnement de Prévisualisation, les utilisateurs et utilisatrices standard et les administrateurs et administratrices système ont Planning activé par défaut.</span></p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gérer une vue chronologique {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Lors de la création d’une vue chronologique, tous les enregistrements du type sélectionné s’affichent dans un ordre chronologique.

Tenez compte des points suivants :

* Vous ne pouvez créer une vue chronologique que si vous avez au moins deux champs de date associés à un type d’enregistrement. Lorsque vous avez un ou plusieurs champs de date associés à un type d’enregistrement, l’option de vue chronologique est grisée.

  Vous pouvez effectuer un choix parmi les champs de date suivants lors de la création d’une vue chronologique :

   * Dates d’enregistrement
   * Enregistrer les champs générés par le système : date de création, date de dernière modification
   * Dates de recherche à partir d&#39;enregistrements ou de types d&#39;objets connectés.
* En fonction des dates associées aux enregistrements, certains enregistrements peuvent ne pas s’afficher dans la vue chronologique dans les scénarios suivants :

   * Lorsque les dates de début et de fin n’ont pas de valeur.
   * Lorsque les dates de début ou de fin n’ont pas de valeur.
   * Lorsque la date de début est postérieure à la date de fin.

Pour gérer une vue chronologique :

1. Accédez à la page du type d’enregistrement pour lequel vous souhaitez consulter la chronologie.
1. Créez une vue chronologique, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   ![Exemple de vue Chronologie](assets/timeline-view-example.png)

   Les enregistrements associés au type d’enregistrement que vous avez sélectionné s’affichent sous forme de barres dans une chronologie et sont triés par ordre chronologique de leur date de début, par défaut.

   >[!TIP]
   >
   >    Le tri des enregistrements dans la chronologie n’est pas visible dans la vue compacte.

1. (Facultatif et conditionnel) Lorsque le nom d’enregistrement est tronqué, passez la souris sur une barre d’enregistrement pour afficher le nom complet de l’enregistrement et des informations supplémentaires.

1. Effectuez l’une des opérations suivantes pour naviguer dans la chronologie :

   * Cliquez sur les icônes de gauche et de droite ou utilisez le défilement horizontal pour vous déplacer vers l’arrière et vers l’avant dans la chronologie. L’actualisation de la page conserve la période sélectionnée.
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

   1. Cliquez sur l’icône **Rechercher** ![Icône Rechercher](assets/search-icon.png) et commencez à saisir un mot-clé associé à n’importe quel champ d’un enregistrement qui s’affiche à l’écran. Le nombre de correspondances correctes s’affiche à côté de l’élément de la recherche et l’enregistrement correspondant est surligné.

      ![Zone de recherche et vue chronologique des résultats](assets/search-box-and-results-timeline-view.png)

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

1. (Facultatif) Cliquez sur **Répartition** pour afficher les enregistrements connectés sur le journal.

   Pour plus d’informations, consultez la section [Utilisation de la fonction Répartition pour afficher les enregistrements connectés dans la vue chronologique](#break-down-connected-records-in-the-timeline-view)

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

* Vous pouvez filtrer par champs d’enregistrement connectés ou champs de recherche.
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
* Vous pouvez effectuer un regroupement par champs d’enregistrement connectés ou champs de recherche.
* Lorsque vous regroupez des champs de recherche avec plusieurs valeurs (qui n’ont pas été résumées par un agrégateur), les enregistrements sont regroupés selon chaque combinaison unique de valeurs de champ.
* Vous pouvez référencer un champ qui se trouve à jusqu’à 4 niveaux du type d’enregistrement actuel. Par exemple, si vous créez un regroupement pour un type d’enregistrement Activité et que l’Activité est connectée au type d’enregistrement Produit connecté au type d’enregistrement Campagne connecté à un projet Workfront, vous pouvez référencer le statut du projet dans le regroupement que vous créez pour le type d’enregistrement Activité.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Pour ajouter un regroupement dans la vue chronologique :

1. Créez une vue chronologique pour un type d’enregistrement, comme décrit dans l’article [Gestion des vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. Cliquez sur **Regroupement** dans le coin supérieur droit de la vue chronologique.

   ![Regroupement de la vue chronologique de l’interface utilisateur avec des champs liés](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Cliquez sur l’un des champs proposés ou cliquez sur **Choisir un champ différent**, recherchez un autre champ, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   Le regroupement est appliqué automatiquement à la chronologie et les enregistrements s’affichent dans la zone de regroupement.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Facultatif) Répétez les étapes ci-dessus pour ajouter jusqu’à 3 regroupements.

   Le nombre de champs sélectionnés pour le regroupement s’affiche à côté de l’icône de regroupement.

   <!-- update screen shot with view redesign-->

   ![Le regroupement s’applique dans la vue Chronologie](assets/grouping-applied-in-timeline-view.png)

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

1. Cliquez sur **Style de barre** dans le panneau de gauche pour indiquer les informations à afficher sur les barres d’enregistrement.

   Le champ principal (ou titre) de l&#39;enregistrement, tel que défini dans la vue Tableau de l&#39;enregistrement, est sélectionné par défaut. <!--adjust this when the primary field is released??-->

1. (Facultatif et le cas échéant) Si vous avez ajouté des miniatures aux enregistrements, sélectionnez l’option Miniature pour afficher l’image associée aux enregistrements dans leur barre d’enregistrement.

   >[!NOTE]
   >
   >    Vous devez d’abord ajouter les miniatures dans la vue de tableau, avant de pouvoir les afficher dans la vue chronologique. Pour plus d’informations, voir [Ajouter une miniature à un enregistrement](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Cliquez sur **Ajouter un champ**, puis dans la zone **Rechercher des champs**, et cliquez sur le champ à ajouter.

   >[!TIP]
   >
   >   * Vous devez créer les champs avant de les ajouter aux barres d’enregistrement.
   > 
   >   * Vous devez disposer d’au moins un champ sélectionné. Le **nom** est sélectionné par défaut.
   >
   >   * Vous pouvez ajouter jusqu’à 5 champs.

   Un aperçu de l’aspect des barres sur la chronologie s’affiche à droite.

   ![Enregistrement des paramètres de chronologie du panneau des détails avec aperçu](assets/record-details-panel-timeline-settings-with-preview.png)

1. <span class="preview">(Facultatif et conditionnel) Si vous affichez la frise chronologique en mode Standard, activez le paramètre **Tronquer les détails de la barre**. Lorsqu’elle est activée, les informations des barres d’enregistrement sont tronquées et ne s’affichent entièrement que lorsque vous passez la souris sur les barres. Ce paramètre est désactivé par défaut et les informations sont entièrement affichées sur les barres. </span>

   ![Paramètre Tronquer activé dans la zone des paramètres de la chronologie mise en surbrillance](assets/truncate-setting-enabled-on-timeline-settings-highlighted.png)

   >[!TIP]
   >
   >* <span class="preview">Le paramètre Tronquer les détails de la barre n’est pas disponible lors de l’affichage de la vue chronologique en mode Compact, et il n’est pas disponible dans la vue Calendrier</span>.
   >
   >* <span class="preview">Si vous répartissez la vue chronologique pour afficher les objets connectés, le paramètre Tronquer les détails de la barre s’applique uniquement au type d’enregistrement principal. Elle ne s’applique pas aux barres d’enregistrement connectées.</span>


1. Cliquez sur **Couleur** dans le panneau de gauche pour personnaliser les couleurs des enregistrements et des regroupements dans la chronologie.

   ![Vue chronologique de l’onglet Couleur](assets/color-tab-timeline-view.png)

1. (Le cas échéant et facultatif) Si vous avez ajouté un regroupement à la vue chronologique, sélectionnez l’une des options suivantes pour définir une couleur pour le regroupement dans la section **Définir la couleur du regroupement** :

   * **Par défaut (gris)** : la couleur des regroupements est le gris. Il s’agit de la valeur par défaut.
   * **Valeurs de champ** : la couleur des regroupements correspond à celle du champ que vous regroupez.

     >[!NOTE]
     >
     >    * Vous ne pouvez faire correspondre la couleur qu’aux champs avec des options codées par couleur. Par exemple, vous pouvez associer la couleur aux champs État ou aux champs avec des options associées aux couleurs.
     >    
     >    * Vous ne pouvez pas faire correspondre la couleur aux champs de recherche à partir d&#39;enregistrements liés ou de types d&#39;objets.


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

   ![Menu déroulant du sélecteur de champ en mode Chronologie](assets/field-selector-drop-down-menu-timeline-view.png)

   Seuls les champs dont les options sont codées en couleur s’affichent dans le menu déroulant.

   Par exemple, les champs à sélection multiple ou unique peuvent avoir des options codées par couleur.

   Si vous n’avez pas de champ avec des options codées par couleur pour le type d’enregistrement sélectionné, cette option est grisée.

1. Cliquer sur **Enregistrer**.

   Les enregistrements s’affichent dans la vue chronologique avec les spécifications que vous avez sélectionnées.

### Répartir les enregistrements connectés dans la vue chronologique

Vous pouvez afficher les enregistrements connectés dans la vue chronologique d&#39;un enregistrement à l&#39;aide de la fonction Répartition. La répartition des enregistrements en fonction de leurs connexions vous permet d&#39;afficher la chronologie d&#39;autres enregistrements connectés et de comprendre comment ils peuvent affecter les performances et les échéances de vos enregistrements.

#### Remarques concernant l’utilisation de la fonction Répartition

* Vous pouvez afficher les enregistrements ou les objets connectés sous les enregistrements du type d&#39;enregistrement sélectionné dans la vue chronologique.
* Vous pouvez afficher les éléments suivants dans la vue Chronologie à l’aide de la fonction Répartition :
   * Enregistrements Workfront Planning connectés au type d&#39;enregistrement sélectionné.
   * Types d’objet Workfront ou ressources Experience Manager connectées au type d’enregistrement sélectionné.
   * Enregistrements ou objets Workfront Planning d&#39;une autre application connectés à des enregistrements connectés au type d&#39;enregistrement sélectionné.

     Par exemple, vous pouvez lier des campagnes à des portfolios. En outre, vous pouvez connecter un autre type d’enregistrement, products, à des projets, ainsi qu’à des campagnes. Lorsque vous créez la vue chronologique de la campagne, vous pouvez répartir les campagnes par portfolios, produits et projets.

* Vous ne pouvez pas afficher les types d&#39;objets qui sont connectés uniquement aux objets Workfront dans Workfront, mais qui ne sont pas connectés à un type d&#39;enregistrement Workfront Planning. Vous ne pouvez afficher que les types d&#39;objet ou d&#39;enregistrement connectés dans Workfront Planning.

  Par exemple, les tâches sont liées à des projets dans Workfront. Grâce à la fonction Répartition, vous pouvez afficher les projets connectés aux campagnes dans Planning, mais pas les tâches connectées aux projets dans Workfront.

  Si vous souhaitez afficher à la fois les portefeuilles et les projets dans la vue chronologique d&#39;un type d&#39;enregistrement Planning Workfront, les portefeuilles et les projets doivent être connectés à l&#39;enregistrement Planning ou à un enregistrement connecté à l&#39;enregistrement Planning dont vous gérez la vue chronologique.
* Vous pouvez uniquement afficher les types d’enregistrements associés à au moins deux champs de date.
* Les champs de date des types d’enregistrement que vous souhaitez afficher dans la vue chronologique doivent être visibles dans la vue Tableau du type d’enregistrement sélectionné, sous la forme de champs de recherche.
* Les dates de début et de fin des types d’enregistrements à afficher dans la vue chronologique doivent être dans l’ordre chronologique. Par exemple, si un enregistrement a une date de Début fixée au 31 janvier et une date de Fin fixée au 1er janvier, il ne s&#39;affiche pas dans la vue chronologique. Pour plus d’informations, consultez la section [Gérer une vue chronologique](#manage-a-timeline-view) de cet article.
* Vous pouvez inclure une limite de 5 types d’enregistrements dans la répartition d’un enregistrement.

#### Répartir les enregistrements connectés

1. Créez une vue chronologique pour un type d’enregistrement, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. (Conditionnel) Si vous affichez la vue chronologique en mode Standard, cliquez sur **Répartition**.
1. Développez la zone **Sélectionner un type d’enregistrement lié** et sélectionnez un type d’enregistrement connecté. <!--add a new screen shot - submitted a bug to remove the "the"-->

   ![Sélecteur de répartition et bouton en mode Chronologie](assets/breakdown-picker-and-button-on-timeline.png)

   >[!TIP]
   >
   >    Si vous n&#39;avez aucun enregistrement connecté ou si les enregistrements connectés n&#39;ont pas au moins deux champs de date, la zone **Sélectionner un type d&#39;enregistrement lié** n&#39;est pas disponible.

1. Choisissez un **Date de début** et un **Champ de date de fin**.

   >[!TIP]
   >
   >    Les dates de début et de fin doivent être séquentielles. Si la date de fin est antérieure à la date de début, aucun enregistrement ne s’affiche dans le journal.

   Une flèche pointant vers la droite s&#39;affiche sur la barre de l&#39;enregistrement sélectionné dans la chronologie, s&#39;ils sont connectés à d&#39;autres enregistrements.
1. Cliquez sur la flèche pointant vers la droite pour développer un type d’enregistrement et afficher ses connexions.

   ![Campagnes réparties par programmes dans la vue Chronologie](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)

1. (Facultatif) Répétez les étapes ci-dessus pour ajouter d’autres enregistrements connectés.



