---
title: Gestion de la vue Tableau
description: Vous pouvez afficher les enregistrements et leurs champs dans une vue Tableau lors de l'accès à la page de type d'enregistrement dans Adobe Workfront Planning. Cet article décrit comment créer une vue de tableau et modifier ou supprimer une vue existante.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 7f96cddc18e70dff34beb33ef2785af69a55c36f
workflow-type: tm+mt
source-wordcount: '2872'
ht-degree: 66%

---

# Gérer la vue de tableau

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez afficher les enregistrements et leurs champs dans la vue de tableau lors de l’accès à la page du type d’enregistrement dans Adobe Workfront Planning.

Pour plus d’informations sur les vues d’enregistrement et leur gestion, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

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
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification de front de travail n’est pas disponible pour les plans de front hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur ce qui est inclus dans chaque plan Workfront Planning, contactez votre responsable de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Plateforme Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
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
   <p>Autorisations d’affichage d’une vue pour modifier temporairement les paramètres d’affichage</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD:

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

## Modifier des enregistrements à l’aide de la vue Tableau

Vous ne pouvez modifier les informations d’enregistrement que dans la vue Tableau.

Pour plus d&#39;informations sur la modification des enregistrements en mode Tableau, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

## Gérer une vue tableau {#manage-a-table-view}

<!--insert screen shot of table view-->

Lors de la création d’une vue tableau, tous les enregistrements du type sélectionné s’affichent dans un tableau. Chaque ligne est un enregistrement unique et chaque colonne est un champ d’enregistrement. Tous les champs et tous les enregistrements s’affichent par défaut.

Pour gérer une vue tableau :

1. Créez une vue tableau, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   ![Exemple de vue Tableau](assets/table-view-example.png)

1. (Facultatif) Cliquez sur **Hauteur de ligne**, puis sélectionnez l’une des options suivantes pour modifier la hauteur des lignes du tableau :
   * Court
   * Moyen
   * Grand

1. Mettez à jour les éléments de vue suivants comme décrit dans les sous-sections ci-dessous :
   * [Colonnes (ou champs)](#add-columns-or-fields)
   * [Lignes (ou enregistrements)](#add-rows-or-records)
   * [Filtres](#add-filters)
   * [Regroupement ](#add-groupings)
   * [Trier](#add-a-sort)
   * [Activer l’indicateur de présence en temps réel](#enable-the-real-time-presence-indicator)


### Ajouter des colonnes (ou des champs) {#add-columns}

Les en-têtes de colonne d’une vue de tableau affichent les champs associés aux enregistrements de la vue. Les mêmes champs affichés dans la vue de tableau s’affichent également dans la section Détails d’un enregistrement. Pour plus d’informations, consultez la section [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

L’ajout de colonnes à une vue est identique à l’ajout de champs à un type d’enregistrement.

Vous pouvez ajouter jusqu’à 500 champs (ou colonnes) dans une vue tableau.

1. Accédez à une page de type enregistrement et cliquez sur un onglet de vue Tableau, ou cliquez sur **+ Vue** pour ajouter une nouvelle vue, puis choisissez **Table**.

1. Commencez à ajouter des champs (ou des colonnes), comme décrit dans l’article [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

   Les colonnes que vous ajoutez sont visibles par toutes les personnes qui accèdent au type d’enregistrement et sont ajoutées en tant que nouveaux champs sur la page de l’enregistrement.

1. Pour réorganiser les colonnes du tableau, effectuez l’une des opérations suivantes :

   * Saisissez l’en-tête de colonne et faites-le glisser à l’endroit souhaité. La colonne que vous avez déplacée s’affiche brièvement sur fond bleu jusqu’à ce que vous procédiez à d’autres ajustements dans le tableau.

   * Cliquez sur **Champs** dans la barre d’outils du tableau, puis faites glisser les champs dans l’ordre souhaité et cliquez en dehors de la case **Visibilité et ordre des champs** pour la fermer.

     ![Barre d’outils du mode Tableau des champs développée](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* Le champ Nom est toujours le premier champ de la vue tableau, par défaut. Il est considéré comme un champ principal.
     >
     >* Vous ne pouvez pas déplacer le champ Nom, à moins que vous ne désigniez un autre champ comme champ principal. Pour plus d’informations, passez à l’étape 4. <!--accurate?-->
     >
     >

   * Remplacez le champ de la première colonne par un autre en modifiant le champ principal. Pour plus d’informations, passez à l’étape 4. <!--accurate?-->

1. (Facultatif) Pointez sur un nom de champ dans l’en-tête de colonne d’un champ qui ne s’affiche pas dans la première colonne du tableau, cliquez sur la flèche pointant vers le bas à droite du nom du champ, puis sur **Définir comme champ principal**.

   ![Définir comme champ principal en mode Tableau](assets/set-as-primary-field-option-table-view.png)

1. Cliquez sur **Définir le champ** pour confirmer.

   Le champ devient champ principal, ce qui signifie qu’il s’affiche en tant que première colonne de la vue du tableau. Le champ principal précédent est déplacé dans la deuxième colonne.

   Les champs primaires deviennent le titre de l’enregistrement et s’affichent dans la zone d’en-tête de la page de l’enregistrement, et partout où les enregistrements s’affichent. Par exemple, le titre de l’enregistrement s’affiche dans les champs connectés et dans toutes les vues. Pour plus d’informations sur les champs principaux, voir [Vue d’ensemble](/help/quicksilver/planning/fields/primary-field-overview.md) du champ principal.

1. Cliquez sur les lignes de séparation des colonnes et déposez-les à l’endroit souhaité pour augmenter la largeur des colonnes.

   >[!TIP]
   >
   >Les modifications de la largeur et de l’ordre des colonnes sont permanentes et visibles par tous les utilisateurs et utilisatrices qui accèdent au type d’enregistrement.

1. Pointez sur l’en-tête de la colonne, cliquez sur la flèche pointant vers le bas, puis sur **Masquer le champ**

   Ou

   Cliquez sur **Champs** dans la barre d’outils du tableau et désactivez le bouton (bascule) associé aux champs (ou colonnes) que vous souhaitez masquer. La boîte de dialogue **Visibilité et ordre des champs** s’affiche.

   >[!TIP]
   >
   >Le nombre de champs masqués s’affiche à gauche de l’icône Champs dans la barre d’outils.


1. Cliquez sur l’icône **Champs** et activez le bouton (bascule) associé aux champs que vous souhaitez afficher dans les colonnes du tableau. Tous les champs s’affichent par défaut.

1. Procédez comme suit pour trouver rapidement les enregistrements correspondant à un mot-clé :

   1. Cliquez sur l’icône **Rechercher** ![Icône Rechercher](assets/search-icon.png) et commencez à saisir un mot-clé associé à n’importe quel champ d’un enregistrement qui s’affiche à l’écran. Le nombre de correspondances correctes s’affiche à côté de l’élément de recherche et le champ correspondant est mis en surbrillance.

      ![Zone de recherche avec le contour bleu des résultats en mode Tableau](assets/search-box-with-results-blue-outline-table-view.png)

      Vous pouvez utiliser n’importe quel mot ou caractère spécial visible à l’écran.

      Vous ne pouvez pas utiliser de mots-clés associés à des champs masqués dans la vue de tableau.

   1. Appuyez sur la touche **Entrée** de votre clavier pour passer au champ suivant.

   1. (Facultatif) S’il y a plus d’une correspondance, cliquez sur les flèches haut et bas situées à droite du mot-clé de recherche pour accéder à l’ensemble des correspondances dans le tableau.

   1. Cliquez sur l’icône **x** dans le champ de recherche pour effacer le mot-clé de recherche.


### Ajouter des lignes (ou des enregistrements) {#add-rows}

Les lignes d’une vue de tableau affichent des enregistrements individuels du type d’enregistrement sélectionné.

Vous pouvez avoir jusqu’à 50 000 enregistrements (ou lignes) pour un type d’enregistrement.

1. Accédez à une page de type enregistrement et cliquez sur un onglet de vue Tableau, ou cliquez sur **+ Vue** pour ajouter une nouvelle vue, puis choisissez **Table**.

1. Commencez à ajouter des enregistrements (ou lignes), comme décrit dans l’article [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).

   Les enregistrements que vous ajoutez dans la vue de tableau sont enregistrés immédiatement et sont visibles par tous les utilisateurs et utilisatrices qui disposent d’une autorisation d’affichage ou de niveau supérieure sur l’espace de travail.

1. (Facultatif) Ajoutez une miniature à chaque enregistrement et cliquez sur **Champs** dans le coin supérieur droit du tableau, puis sélectionnez le bouton (bascule) du champ **Miniature** pour l’afficher à gauche du champ principal. Il est désélectionné par défaut.

   Pour plus d’informations, voir [Ajouter une miniature à un enregistrement](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. (Facultatif) Sélectionnez un ou plusieurs enregistrements d’affilée, puis faites glisser et déposez l’icône **![de poignée** Icône](assets/handle-icon.png) de poignée à gauche de l’enregistrement pour réorganiser les lignes.

   >[!NOTE]
   >
   >Vous ne pouvez pas réorganiser les lignes si vous appliquez au moins un tri à la vue de tableau.
   >
   >Les modifications apportées à l’ordre des lignes sont visibles par tous les utilisateurs qui accèdent au type d’enregistrement

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### Ajouter des filtres {#add-filters}

Les filtres permettent de réduire la quantité d’informations affichées à l’écran.

Tenez compte des points suivants lorsque vous utilisez des filtres en mode Tableau :

<!-- this list is almost identical to the one for the table view - update both-->

* Les filtres que vous créez pour la vue en tableau fonctionnent indépendamment des filtres de la vue chronologique lorsqu’ils sont appliqués au même type d’enregistrement.

* Les filtres sont propres à la vue que vous sélectionnez. Des filtres différents peuvent être appliqués à deux vues en tableau du même type d’enregistrement. Deux utilisateurs et utilisatrices qui consultent la même vue en tableau voient le même filtre que celui qui est actuellement appliqué.

* Vous ne pouvez pas nommer les filtres que vous créez et appliquez à une vue en tableau.

* Supprimer des filtres les rend inaccessibles à toute personne accédant au même type d’enregistrement que vous et utilisant la même vue que vous.

* Ajouter des filtres à la vue en tableau est identique à l’ajout de filtres à la vue chronologique.

* Vous pouvez filtrer par champs d’enregistrement connectés ou par champ de recherche.

* Vous pouvez filtrer par champ de recherche qui affiche plusieurs valeurs.

* Vous pouvez référencer un champ distant de 4 niveaux du type d’enregistrement actif. Par exemple, si vous créez un filtre pour un type d’enregistrement d’activité et que l’activité est connectée au type d’enregistrement de produit qui est connecté au type d’enregistrement Campaign qui est connecté à un projet Workfront, vous pouvez référencer le budget du projet dans le filtre que vous créez pour le type d’enregistrement d’activité.

Pour ajouter un filtre à une vue en tableau, procédez comme suit :

1. Créez une vue en tableau pour une page de type enregistrement, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. Sélectionnez une vue en tableau, puis cliquez sur **Filtres** dans le coin supérieur droit du tableau.
1. Cliquez sur **Ajouter une condition** et ajoutez les informations suivantes :

   * **Sélectionnez un champ** que vous souhaitez filtrer par <!-- the tip below might change-->

   * **Sélectionnez une option** (ou un modificateur de filtre) pour définir le type de condition auquel le champ doit répondre

     Le tableau ci-dessous présente les modificateurs disponibles pour chaque type de champ.

     <table>
        <thead>
        <tr>
            <th><b>Type de champ</b></th>
            <th><b>Modificateurs</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Ligne unique, paragraphe, formule </td>
            <td><p>Contient</p>
            <p>Ne contient pas</p>
            <p>Est</p>
            <p>N’est pas</p>
            <p>Est vide</p>
            <p>N’est pas vide</p></td>
        </tr>
        <tr><td>Sélection unique</td>
            <td><p>Est</p>
            <p>N’est pas</p>
            <p>Est l’un des</p>
            <p>N’est aucun de</p>
            <p>Est vide</p>
            <p>N’est pas vide</p></td>
        </tr>
        <tr>
            <td>Multi-sélection, personnes</td>
            <td><p>A l’un des</p>
            <p>Dispose de tous les</p>
            <p>Est exactement</p>
            <p>N’a aucun(e) des</p>
            <p>Est vide</p>
            <p>N’est pas vide</p></td>
        </tr>
        <tr>
            <td>Nombre, pourcentage, devise</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>Est vide</p>
            <p>N’est pas vide</p></td>
        </tr>
        <tr>
            <td>Date</td>
            <td><p>Est</p>
            <p>N’est pas</p>
            <p>Est après</p>
            <p>Est avant</p>
            <p>Est compris entre</p><p>N’est pas compris entre</p>
            <p>Est vide</p><p>N’est pas vide</p></td>
        </tr>

     <tr>
            <td>Case à cocher</td>
            <td><p>Est</p>
        </tr>
        </tbody>
        </table>

   * Choisissez une valeur pour le champ sélectionné.

   ![Vue Tableau de l’interface utilisateur de filtrage](assets/filter-ui-table-view.png)

   Il n’y a pas de limite au nombre de conditions de filtrage que vous pouvez ajouter.

1. (Facultatif) Cliquez sur **Ajouter une condition** pour ajouter une autre option de filtrage et répétez les étapes ci-dessus. Le nombre de filtres appliqués s’affiche à gauche de l’icône Filtres.
1. Cliquez sur les opérateurs suivants pour indiquer comment les conditions de filtrage sont liées et doivent être appliquées :

   * **AND** : toutes les conditions spécifiées doivent être remplies.
   * **OU** : L’une des conditions spécifiées doit être remplie. Il s’agit de l’option par défaut.

   1. (Facultatif) Ajoutez des opérateurs ET **ou** OU **supplémentaires** entre plusieurs groupes de conditions.

      ![Filtres à plusieurs niveaux dans les vues](assets/multi-tiered-filters-in-views.png)

   La liste des enregistrements est filtrée automatiquement. <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Facultatif) Cliquez sur l’icône **x** pour supprimer une condition de filtrage.
1. (Facultatif) Cliquez sur **Filtres** pour fermer la zone des filtres. <!--right now you cannot "clear all" for filters, but this might come later-->

### Ajouter des regroupements {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

Vous pouvez regrouper des enregistrements par des informations similaires lorsque vous appliquez un regroupement à une vue.

L’ajout de regroupements dans la vue de tableau est similaire à l’ajout de regroupements dans la vue chronologique.

Tenez compte des points suivants :

* Vous pouvez utiliser des regroupements à la fois dans la vue tableau et dans la vue chronologique. Les regroupements de la vue de tableau sont indépendants de ceux de la vue chronologique du même type d’enregistrement.
* Vous pouvez appliquer 3 niveaux de regroupement dans une vue. Les enregistrements sont regroupés dans l’ordre des regroupements que vous sélectionnez.
&lt;!--* Vous pouvez appliquer jusqu’à 4 niveaux de regroupement lorsque vous utilisez l’API. --vérifier celui-ci pour l’instant-->
* Les regroupements sont propres à la vue que vous sélectionnez. Vous pouvez appliquer des regroupements différents à deux vues de tableau du même type d’enregistrement. Deux utilisateurs ou utilisatrices qui consultent la même vue de tableau voient le regroupement qui est actuellement appliqué.
* Vous ne pouvez pas nommer les regroupements que vous créez pour une vue de tableau.
* En supprimant les regroupements, vous les supprimez pour toutes les personnes qui accèdent au même type d’enregistrement que vous et qui consultent la même vue que vous.
* Vous pouvez modifier les enregistrements répertoriés dans un regroupement.
* Vous pouvez effectuer un regroupement par champs d’enregistrement connectés ou champs de recherche.
* Lorsque vous regroupez des champs de recherche avec plusieurs valeurs (qui n’ont pas été résumées par un agrégateur), les enregistrements sont regroupés selon chaque combinaison unique de valeurs de champ.
* Vous pouvez référencer un champ distant de 4 niveaux du type d’enregistrement actif. Par exemple, si vous créez un regroupement pour un type d’enregistrement d’activité et que l’activité est connectée au type d’enregistrement de produit qui est connecté au type d’enregistrement Campaign qui est connecté à un projet Workfront, vous pouvez référencer l’état du projet dans le groupe que vous créez pour le type d’enregistrement d’activité.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

Pour ajouter un regroupement :

1. Créez une vue chronologique pour un type d’enregistrement, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. Cliquez sur **Regroupement** dans le coin supérieur droit de la vue de tableau.

   ![Regroupement de la vue Tableau de l’interface utilisateur avec des champs liés](assets/grouping-ui-table-view-with-linked-fields.png)

1. Cliquez sur l’un des champs proposés ou cliquez sur **Choisir un autre champ**, recherchez un autre champ, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   Le regroupement est appliqué automatiquement au tableau et les enregistrements s’affichent sous la ligne de séparation du regroupement.

1. (Facultatif) Cliquez sur **Ajouter une condition** et répétez les étapes ci-dessus pour ajouter jusqu’à 3 regroupements.

   Le nombre de champs sélectionnés pour le regroupement s’affiche à côté de l’icône de regroupement.

   ![Regroupement appliqué en mode Tableau](assets/grouping-applied-in-table-view.png)

1. (Facultatif) Dans la zone **Regrouper les enregistrements par**, cliquez sur l’icône **x** à droite d’un champ sélectionné pour le regroupement pour le supprimer.

   Ou

   Cliquez sur **Tout effacer** pour supprimer tous les champs.

1. Cliquez en dehors de la zone **Regrouper les enregistrements par** pour la fermer.
1. (Facultatif) Cliquez sur **+ Nouvel enregistrement** à la fin de tout regroupement pour ajouter de nouveaux enregistrements, puis actualisez votre page pour ajouter le nouvel enregistrement au regroupement approprié. <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

### Ajouter un tri {#sort-information}

En appliquant un tri, vous pouvez organiser les informations dans un ordre donné.

Vous pouvez trier les informations suivantes :

* Tous les enregistrements dans une vue en tableau.<!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Tenez compte des éléments suivants lorsque vous triez les enregistrements dans la vue en tableau :

<!-- if this is available for the timeline view, update both when you update one-->

* Le tri est propre à la vue que vous sélectionnez. Des critères de tri différents peuvent être appliqués à deux vues en tableau du même type d’enregistrement. Deux utilisateurs ou utilisatrices qui consultent la même vue en tableau voient le même tri que celui qui est actuellement appliqué.

* Les tris que vous créez et appliquez à une vue en tableau ne peuvent pas être nommés.

* Le tri que vous créez est préservé lorsque vous quittez cette vue.

* Vous pouvez trier autant de champs que vous le souhaitez dans la vue en tableau d’un type d’enregistrement.

* Vous ne pouvez pas trier par champs d’enregistrement connectés, mais vous pouvez trier par champs de recherche à partir de types d’enregistrements connectés.

* Lorsque vous triez par champs de recherche avec plusieurs valeurs (qui n’ont pas été résumées par un agrégateur), la première valeur est utilisée pour le tri.

* Supprimer des critères de tri les rend inaccessibles à toute personne accédant au même type d’enregistrement que vous et utilisant la même vue que vous.

* Vous pouvez référencer un champ qui se trouve à jusqu’à 4 niveaux du type d’enregistrement actuel. Par exemple, si vous créez un tri pour un type d’enregistrement Activité et que l’Activité est connectée au type d’enregistrement Produit connecté au type d’enregistrement Campaign connecté à un projet Workfront, vous pouvez référencer le statut du projet dans le tri que vous créez pour le type d’enregistrement Activité.

Pour trier les enregistrements <!--ungrouped (add this when sorting for groupings will be available-->, procédez comme suit :

1. Créez une vue en tableau, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).
1. Cliquez sur l’icône **Trier** ![icône Trier](assets/sort-icon.png) dans le coin supérieur droit du tableau

   Ou

   Pointez sur le nom d’une colonne dans la vue en tableau, cliquez sur la flèche pointant vers le bas à droite du nom de l’en-tête de la colonne, puis cliquez sur **Trier par ce champ**. Le champ est ajouté en tant que sélection de tri dans l’icône de tri dans le coin supérieur droit de la vue en tableau.

1. (Conditionnel) Dans la zone **Trier les enregistrements par**, cliquez sur l&#39;un des champs suggérés, ou cliquez sur **Choisir un autre champ** et recherchez un autre champ, puis cliquez dessus lorsqu&#39;il s&#39;affiche dans la liste.

   Le tri est appliqué automatiquement à la vue en tableau et les enregistrements s’affichent triés selon les critères que vous avez sélectionnés.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Facultatif) Cliquez sur **Ajouter une condition** et répétez les étapes ci-dessus pour trier par champs supplémentaires.

   Le nombre de champs que vous triez s’affiche à gauche de l’icône de tri dans le coin supérieur droit de la barre d’outils. Vous ne pouvez sélectionner que les champs qui s’affichent dans les colonnes de la vue de tableau.

1. (Facultatif) Dans la zone **Trier les enregistrements par**, sélectionnez l’icône **x** en regard d’un champ de tri pour supprimer le tri.

   Ou

   Cliquez sur **Tout effacer** pour supprimer tous les champs du tri.

1. Cliquez en dehors de la zone **Trier les enregistrements par** pour la fermer.

   ![Tri en mode Tableau](assets/sorting-in-table-view.png)

   Les informations affichées dans le tableau sont triées en fonction des critères sélectionnés.

   Les champs qui doivent être triés affichent une icône de tri suivie d’un nombre qui indique l’ordre dans lequel le tri est appliqué.

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->

### Activer l’indicateur de présence en temps réel

Les avatars des autres utilisateurs qui modifient les informations d’enregistrement en même temps que vous affichez dans le coin supérieur droit de toutes les vues d’enregistrement, par défaut.

Lorsque vous affichez la vue de table, vous pouvez également voir quel champ un autre utilisateur modifie au moment où vous affichez l’enregistrement.

Pour plus d’informations, consultez la section « Activer l’indicateur de présence en temps réel » de l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

