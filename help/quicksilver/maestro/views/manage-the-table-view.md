---
title: Gestion de la vue de tableau
description: Vous pouvez afficher les enregistrements et leurs champs dans une vue de tableau lors de l’accès à la page de type enregistrement dans Adobe Maestro.
hidefromtoc: true
hide: true
source-git-commit: 4a3cf7211eef2b161a29b74e8e9b2b12c21eaf4d
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 5%

---


# Gestion de la vue de tableau

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Maestro. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta fermé ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez afficher les enregistrements et leurs champs dans une vue de tableau lors de l’accès à la page de type enregistrement dans Adobe Maestro.

Pour plus d’informations sur les vues Maestro et leur gestion, voir [Gestion des vues d’enregistrement](../views/manage-record-views.md).

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

## Gestion de l’affichage d’un tableau {#manage-a-table-view}

<!--insert screen shot of table view-->

Lors de la création d&#39;une vue de tableau, tous les enregistrements du type sélectionné s&#39;affichent dans un tableau. Chaque ligne est un enregistrement unique et chaque colonne est un champ d’enregistrement. Tous les champs et tous les enregistrements s&#39;affichent par défaut.

Pour gérer une vue de tableau :

1. Créez une vue de tableau, comme décrit dans l’article [Gestion des vues d’enregistrement](../views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. Mettez à jour les éléments de vue suivants comme décrit dans les sous-sections ci-dessous :
   * [Colonnes (ou champs)](#add-columns-or-fields)
   * [Lignes (ou enregistrements)](#add-rows-or-records)
   * [Filtres](#add-filters)
   * [Regroupement](#add-groupings)
   * [Trier](#sort-information)


### Ajouter des colonnes (ou des champs) {#add-columns}

Les en-têtes de colonne d’une vue Tableau Maestro affichent les champs associés aux enregistrements de la vue. Les mêmes champs affichés dans la vue de tableau s’affichent également dans la section Détails d’un enregistrement Maestro. Pour plus d’informations, voir [Modifier des enregistrements](../records/edit-records.md).

<!-- this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default. -->

L’ajout de colonnes à une vue est identique à l’ajout de champs à un type d’enregistrement.

Vous pouvez ajouter jusqu’à 500 champs (ou colonnes) dans une vue de tableau.

1. Accédez à une page de type enregistrement et sélectionnez une **Tableau** vue depuis le menu déroulant des vues.
1. Commencez à ajouter des champs (ou des colonnes), comme décrit dans l’article [Créer des champs](../architecture-and-fields/create-fields.md).

   Les colonnes que vous ajoutez sont visibles par tous les utilisateurs qui accèdent au type d&#39;enregistrement et sont ajoutés en tant que nouveaux champs dans la page Détails des enregistrements du type d&#39;enregistrement sélectionné.

1. Pour réorganiser les colonnes du tableau, effectuez l’une des opérations suivantes :

   * Saisissez l’en-tête de colonne et faites-le glisser à l’emplacement souhaité. La colonne que vous avez déplacée brièvement s’affiche avec un arrière-plan bleu jusqu’à ce que vous apportez d’autres ajustements au tableau.

   * Cliquez sur **Champs** dans la barre d’outils du tableau, puis effectuez un glisser-déposer des champs dans l’ordre souhaité, puis cliquez en dehors de la fonction **Visibilité des champs et boîte de commande** pour le fermer.

     ![](assets/fields-setting-table-view-toolbar-expanded.png)

   >[!TIP]
   >
   >* Le champ Nom est toujours le premier champ de la vue Tableau.
   >
   >* Vous ne pouvez pas déplacer le champ Nom vers une autre position.
   >
   >* Vous ne pouvez pas masquer le champ Nom .
   >
   >* Le champ Nom est figé et ne fait pas partie du défilement horizontal.

1. Pour augmenter la largeur des colonnes, cliquez et faites glisser les lignes de séparation des colonnes et déposez-les à l’emplacement de votre choix.

   >[!TIP]
   >
   >Les modifications apportées à la largeur et à l’ordre des colonnes sont permanentes et visibles par tous les utilisateurs qui accèdent au type d’enregistrement.

1. Pour masquer une colonne, survolez son en-tête, cliquez sur la flèche pointant vers le bas, puis cliquez sur **Masquer le champ**

   Ou

   Cliquez sur **Champs** dans la barre d’outils du tableau et désactivez le bouton d’activation/désactivation associé aux champs à masquer.

   >[!TIP]
   >
   >Le nombre de champs masqués s’affiche à gauche de l’icône Champs de la barre d’outils.


1. Dans la **Champs** , activez le bouton d’activation/désactivation associé aux champs que vous souhaitez afficher dans les colonnes du tableau. Tous les champs s’affichent par défaut.

### Ajouter des lignes (ou des enregistrements) {#add-rows}

Les lignes d’un tableau Maestro affichent des enregistrements individuels du type d’enregistrement sélectionné.

Vous pouvez avoir jusqu’à 10 000 enregistrements (ou lignes) pour un type d’enregistrement dans Maestro.

L’ajout de lignes à une vue de tableau Maestro est identique à la création d’enregistrements dans un tableau.

Pour plus d’informations, voir [Créer des enregistrements](../records/create-records.md).

<!-- this is not possible right now:

1. To reorder the rows, click the row header, drag and drop it in the desired location. 

    The changes you make to the row order are permanent and visible to all users who access the record type
-->

### Ajout de filtres {#add-filters}

<!-- this section links from the timeline view; consider splitting them if they become different-->

Les filtres permettent de réduire la quantité d’informations affichées à l’écran.

Tenez compte des points suivants lorsque vous utilisez des filtres dans la vue Tableau :
<!-- this list is almost identical to the one for the table view - update both-->

* Les filtres que vous créez pour la vue de tableau fonctionnent indépendamment des filtres de la vue de chronologie lorsqu’ils sont appliqués au même type d’enregistrement.

* Les filtres sont propres à la vue que vous sélectionnez. Des filtres différents peuvent être appliqués à deux vues de tableau d’un même type d’enregistrement. Deux utilisateurs qui visualisent la même vue de tableau voient le même filtre actuellement appliqué.

* Vous ne pouvez pas nommer les filtres que vous créez et appliquez à une vue de tableau.

* Le fait de supprimer des filtres les supprime de toute personne accédant au même type d’enregistrement que vous et utilise la même vue que vous.

* L’ajout de filtres à la vue du tableau est identique à l’ajout de filtres à la vue de la chronologie.

Pour ajouter un filtre à une vue de tableau :

1. Créez une vue de tableau pour une page de type enregistrement, comme décrit dans l’article . [Gestion des vues d’enregistrement](../views/manage-record-views.md).
1. Sélectionnez une vue de tableau, puis cliquez sur **Filtres** dans le coin supérieur droit du tableau.
1. Cliquez sur **Ajouter une condition** et ajoutez les informations suivantes :

   * Sélectionnez un champ en fonction duquel vous souhaitez filtrer les données <!-- the tip below might change-->

   * Sélectionnez une option (ou un modificateur de filtre) pour définir le type de condition que le champ doit remplir.

     Le tableau ci-dessous présente les modificateurs disponibles pour chaque type de champ.

     >[!TIP]
     >
     > Vous ne pouvez pas sélectionner de champs liés. Pour plus d’informations, voir [Créer des champs](../architecture-and-fields/create-fields.md).

     <table>
        <thead>
        <tr>
            <th><b>Type de champ</b></th>
            <th><b>Modificateurs</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Paragraphe à une seule ligne </td>
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
            <td>Sélection multiple</td>
            <td><p>A l’un des</p>
            <p>Dispose de tous les</p>
            <p>Est exactement</p>
            <p>N’a aucun(e) des</p>
            <p>Est vide</p>
            <p>N’est pas vide</p></td>
        </tr>
        <tr>
            <td>Numérique, pourcentage, devise</td>
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

   * Sélectionnez une valeur pour le champ sélectionné.

   ![](assets/filter-ui-table-view.png)

   Le nombre de conditions de filtrage que vous pouvez ajouter est illimité.

1. (Facultatif) Cliquez sur **Ajouter une condition** pour ajouter une autre option de filtrage et répéter les étapes ci-dessus. Le nombre de filtres appliqués s’affiche à gauche de l’icône Filtres .
1. Cliquez sur les opérateurs suivants pour indiquer comment les conditions de filtrage sont jointes et doivent être appliquées :

   * **Et**: toutes les conditions spécifiées doivent être remplies.
   * **Ou**: l’une des conditions spécifiées doit être remplie. Il s’agit de l’option par défaut.

   La liste des enregistrements est filtrée automatiquement.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Facultatif) Cliquez sur **Filtres**, puis cliquez sur le bouton **x** pour supprimer un filtre. <!--right now you cannot "clear all" for filters, but this might come later-->

<!-- this is not available yet

### Add groupings {#add-groupings}

*******************this section might link in the future from the timeline view; right now it's only documented there; also, check the steps below because this was not released to the table when they were written*****************

You can group records by similar information when applying  a grouping to a view.

You can apply groupings both in the table and timeline views. The groupings of the table view are independent from those in the timeline view of the same record type. 

Consider the following:

* You can apply 3 levels of grouping in a Maestro view. The records are grouped in the order of groupings that you select. (***************check on this; this might be true for timeline, but not for table??? One dev said in a demo that there are unlimited groupings in a table - check *********************)
* You can apply up to 4 levels of grouping when using the API. 

To add a grouping:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. (Conditional) To apply a grouping in the table view, do the following:
    
    1. ***************start adding steps for building a grouping - see if there it a global setting or just per column; also, see if the steps are different for a table vs a timeline view?!**********************
1. (Conditional) To apply a grouping in the timeline view, do the following:

    1. Go to a timeline view, then click **Group**. ************************did they rename this to "Grouping"?!****************************
        ******************insert screen shot***********
    1. Click one of the 5 suggested fields, or click **Choose a different field** to display all fields, then click one when it displays in the list. 
    
        >[!TIP]
        >
        > You cannot select linked fields. For information, see [Create fields](../architecture-and-fields/create-fields.md).  
    The grouping is applied automatically to the timeline and records display inside the grouping box.    <********************ensure this is correct functionality here*************
    
    1. (Optional) Click **Add grouping** to add up to 3 groupings. 

        The number of groupings applied displays to the left of the Grouping icon in the upper-right corner of the toolbar. **********ensure this says "grouping" and not "group"*****************
    
    1. (Optional) Click **Clear all** to remove all groupings.  

-->

### Ajouter un tri {#sort-information}

En appliquant un tri, vous pouvez organiser les informations dans un ordre donné.

Vous pouvez trier les informations suivantes :

* Tous les enregistrements dans une vue de tableau. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Tenez compte des points suivants lors du tri des enregistrements dans la vue de tableau :

<!-- if this is available for the timeline view, update both when you update one-->

* Le tri est unique à la vue que vous sélectionnez. Des critères de tri différents peuvent être appliqués à deux affichages de tableau d’un même type d’enregistrement. Deux utilisateurs qui consultent le même tableau voient le même tri appliqué actuellement.

* Vous ne pouvez pas nommer les tri que vous créez et appliquez à une vue de tableau.

* Le tri que vous créez est conservé lorsque vous quittez la page.

* Vous pouvez trier en fonction du nombre de champs affichés dans la vue de tableau d’un type d’enregistrement.

* Le fait de supprimer des critères de tri les supprime de toute personne accédant au même type d’enregistrement que vous et utilise la même vue que vous.

Pour trier <!--ungrouped (add this when sorting for groupings will be available--> enregistrements, procédez comme suit :

1. Créez une vue de tableau, comme décrit dans l’article [Gestion des vues d’enregistrement](../views/manage-record-views.md).
1. Cliquez sur le bouton **Tri** icon ![](assets/sort-icon.png) dans le coin supérieur droit du tableau.

   Ou

   Passez la souris sur le nom d’une colonne dans la vue du tableau, cliquez sur la flèche pointant vers le bas située à droite du nom de l’en-tête de colonne, puis cliquez sur **Tri par ce champ**. Le champ est ajouté en tant que sélection de tri dans l’icône Tri située dans le coin supérieur droit de la vue du tableau.
1. Dans le **Tri des enregistrements par** , cliquez sur l’un des champs proposés ou cliquez sur **Choisir un champ différent** et recherchez un autre champ, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   Le tri est appliqué automatiquement à la vue du tableau et les enregistrements s&#39;affichent triés selon les critères que vous avez sélectionnés.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Facultatif) Répétez les étapes ci-dessus pour trier par champs supplémentaires.

   Le nombre de champs par lesquels vous effectuez un tri s’affiche à gauche de l’icône Tri dans le coin supérieur droit de la barre d’outils. Vous ne pouvez sélectionner que les champs qui s&#39;affichent dans les colonnes du tableau.

   >[!TIP]
   >
   > Vous ne pouvez pas sélectionner de champs liés. Pour plus d’informations, voir [Créer des champs](../architecture-and-fields/create-fields.md).

1. (Facultatif) Dans la variable **Tri des enregistrements par** , cliquez sur le bouton **x** à droite d’un champ de tri pour supprimer le tri

   Ou

   Cliquez sur **Effacer tout** pour supprimer tous les champs du tri.

1. Cliquez en dehors du **Tri des enregistrements par** pour le fermer.

   Les informations affichées dans le tableau sont triées selon les critères que vous avez sélectionnés.

   Les champs sélectionnés pour le tri affichent une icône de tri suivie d’un nombre indiquant l’ordre dans lequel le tri est appliqué.

   ![](assets/sorting-in-table-view.png)


<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->