---
title: Ajouter une page Enregistrements connectés à un enregistrement
description: Vous pouvez afficher les informations des enregistrements ou objets connectés en ajoutant un onglet pour une page Enregistrements connectés à un enregistrement. Les enregistrements connectés dans une vue Tableau sont alors ajoutés à l’onglet.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5e0be9d9-efa5-4b16-bd56-f9c85bc57ced
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1843'
ht-degree: 3%

---

# Ajouter une page Enregistrements connectés à un enregistrement

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Vous pouvez afficher des informations provenant d&#39;enregistrements ou d&#39;objets connectés en ajoutant un onglet pour la page Enregistrements connectés à un enregistrement dans Adobe Workfront Planning. Les enregistrements connectés dans une vue Tableau sont alors ajoutés à l’onglet.

Tenez compte des points suivants lors de l’ajout d’une page Enregistrements connectés à un enregistrement :

* Vous pouvez ajouter une page Enregistrements connectés à un enregistrement après avoir connecté des enregistrements ou des types d&#39;objet au type d&#39;enregistrement à partir de sa vue Tableau.

* Vous pouvez ajouter une page Enregistrements connectés à partir de la zone d&#39;aperçu d&#39;un enregistrement ou de la page de l&#39;enregistrement.

* Vous ne pouvez avoir qu’une seule page d’enregistrements connectée pour un type d’enregistrement spécifique.

  Par exemple, si vous créez une page d’enregistrements connectés pour une campagne et que vous souhaitez afficher ses Rôles connectés, vous ne pouvez avoir qu’une seule page d’enregistrements connectés pour les Rôles.

* Les pages Enregistrements connectés affichent uniquement les objets connectés ou les enregistrements d’un type d’objet ou d’enregistrement. La page n’affiche pas tous les enregistrements de ce type.

* Selon l’objet ou le type d’enregistrement que vous affichez sur la page enregistrements connectés, vous pouvez les afficher dans les vues suivantes :

   * Vous pouvez afficher les enregistrements Planning connectés dans les types de vues suivants :
      * Tableau
      * Journal
      * Calendrier
   * Vous pouvez afficher les projets Workfront connectés dans une vue Liste.

* Vous pouvez ajouter des pages Enregistrements connectés pour les types d’objet ou d’enregistrement connectés suivants :

   * Types d’enregistrements Workfront Planning
   * Projets Workfront

     Vous pouvez afficher les projets Workfront connectés même si vous ne disposez pas des autorisations pour y accéder dans Workfront.

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront et tout package Planning</p>
<p>Tout workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
<tr>
<td> 
   <p> Produits supplémentaires</p> </td> 
   <td> 
   <p> En plus d’Adobe Workfront, vous devez disposer des éléments suivants si vous souhaitez ajouter une page d’enregistrement connectée pour les objets des applications suivantes :</p>
   <ul><li><p>Une licence Adobe Experience Manager Assets et une intégration entre AEM Assets et Workfront pour connecter les ressources AEM aux types d’enregistrements Planning.</p>
   <p>Pour plus d’informations, voir <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront pour Experience Manager Assets et Assets Essentials : index d’article</a>. </p></li>
   <li><p> Une licence Adobe GenStudio for Performance Marketing permettant de connecter des types d’enregistrements aux marques GenStudio</p>
   <p>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/get-started">Prise en main d’Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <p>Autorisations de niveau Contribution ou supérieur à un espace de travail et à un type d’enregistrement </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> 
  </td>
  </tr>   
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Ajouter une page Enregistrements connectés à un enregistrement

Vous devez d’abord connecter les types d’enregistrements à d’autres types d’enregistrements ou à des projets Workfront avant d’ajouter une page d’enregistrements connectés à un enregistrement.

1. Cliquez sur le nom de l’enregistrement pour l’ouvrir dans n’importe quelle vue d’une page de type d’enregistrement.
1. Cliquez sur **Ajouter une page** dans l’une des zones suivantes :

   * Fenêtre d&#39;aperçu de l&#39;enregistrement
   * la page de détails de l’enregistrement, après avoir cliqué sur l’icône **Ouvrir dans un nouvel onglet** ![Ouvrir les détails dans une nouvelle icône d’onglet](assets/open-details-in-a-new-tab-icon.png) dans le coin supérieur droit de la page d’aperçu.

   La boîte de dialogue **Créer une page** s’ouvre.

   ![Boîte de dialogue modale Ajouter la page Enregistrements connectés](assets/add-connection-view-page-modal.png)

1. Ajoutez le **Nom de la page**, cliquez sur **Page des enregistrements connectés** pour le **Type de page**, puis cliquez sur **Créer**.
1. (Facultatif) Cliquez sur le nom d&#39;un enregistrement ou d&#39;un type d&#39;objet connecté dans la liste, ou recherchez-le, puis cliquez dessus lorsqu&#39;il s&#39;affiche dans la liste pour créer la page de cet enregistrement ou de ce type d&#39;objet.

   >[!TIP]
   >
   >Vous pouvez créer une page d’enregistrements connectés par type d’enregistrement. Si un type d’enregistrement connecté comporte déjà une page, elle ne s’affiche plus en tant qu’option.
   >

1. (Facultatif et conditionnel) Si plusieurs champs connectés de l’enregistrement ou du type d’objet pour lequel vous créez la page s’affichent, cliquez sur le champ dont vous souhaitez afficher les enregistrements ou les objets dans la page des enregistrements connectés dans la liste **Sélectionner le champ de référence**.

   ![Sélectionner la liste des champs de référence](assets/select-reference-field-list-on-connected-records-page.png)

   L’une des pages suivantes est ajoutée à la page des enregistrements connectés :

   * Vue Tableau d’un type d’enregistrement
   * Vue Liste d’un type d’objet de projet

   Les enregistrements ou projets connectés à l&#39;enregistrement actif s&#39;affichent dans la vue Tableau ou Liste.

   >[!TIP]
   >
   >Vous devez ajouter les enregistrements connectés dans la table ou la zone Détails d&#39;un enregistrement avant de pouvoir les afficher dans une page d&#39;enregistrements connectés. Dans le cas contraire, le tableau ou la liste est vide.

   Les cinq premiers champs des enregistrements connectés s’affichent par défaut. Aucun champ de recherche n’est affiché par défaut.

   ![Vue du tableau connecté à l’audience sous les détails de la campagne](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Conditionnel) Selon le type d’enregistrements affiché dans la page d’enregistrement connectée, effectuez l’une des opérations suivantes :

   * Gérer les enregistrements Planning
Pour plus d&#39;informations, consultez la section [Gérer la page des enregistrements connectés pour les enregistrements Planning](#manage-the-connected-records-page-for-planning-records) dans cet article.
   * Gestion de projets Workfront
Pour plus d’informations, consultez la section [Gérer la page des enregistrements connectés pour les projets Workfront](#manage-the-connected-records-page-for-workfront-projects) dans cet article.

1. (Facultatif) Double-cliquez sur le nom de l’onglet **Page des enregistrements connectés**

   Ou

   Passez la souris sur le nom de l’onglet, puis cliquez sur **Plus** ![Menu Plus](assets/more-menu.png), puis sur **Renommer** pour renommer en nouvel onglet de la page des enregistrements connectés.

1. (Facultatif) Pointez sur le nom de l’onglet de la page enregistrements connectés, cliquez sur **Plus** ![Menu Plus](assets/more-menu.png), puis cliquez sur **Supprimer** pour supprimer de l’onglet.

### Gérer la page des enregistrements connectés pour les enregistrements Planning

<!--

#### Manage the connected records page for Planning records in the Production environment

When you create a connected records page for  connected Planning records in the Production environment, do the following: (****or AEM Assets - AEM is not available yet?? see note below********)

1. Go to a record type page and click the name of a record. This opens the record's preview page.
1. Click the tab for a connected records page that display Planning records.
   The records connected to the record you selected display in the table view. 
1. Click **Connect** at the bottom of the table view to connect existing records, select them from the connection box, then click outside the box to close it. The records are automatically added to the table and connected to the record you selected. The records must exist before you can add them.

   For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).

1. Edit any information from the connected records inline in the table view. 
1. Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png)

   Or 
   
   Select one of the records, then click one of the following options in the blue bar at the bottom of the list: 

   * **View** to open the record page in a new tab
   * **Copy link** to copy a link to the record page
   * **Edit thumbnail** to open the **Record thumbnail** box and edit the record's thumbnail image
   * **Duplicate** to duplicate the connected record. The duplicated record is also connected to the current record.
   * **Insert record above or below** to add new records to the connected record type. New records added here are also connected to the current record. This option is not available in the blue bar when selecting a record in the table.
   * **Delete** to delete the record. Deleting a connected record deletes it from its record type and from everywhere where the record is connected. The deleted records move to the **Recently deleted** bin of their record type.

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

      >[!TIP]
      >
      >You can select more than one record or object to delete them.
      >

1. Inline edit any of the records in the table on the connected records page.
1. Use any of the following view elements in the toolbar of a connected record page to manage the table view:

   * **Filters**
   * **Sort**
   * **Grouping**
   * **Fields**, to display, hide, or rearrange fields
   * **Row height**
   * **Search**

   For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

   >[!NOTE]
   >
   >You cannot create, edit, or delete fields in the table view of a connected record's tab.
   >

#### Manage the connected records page for Planning records in the Preview environment

When you create a connected records page for connected Planning records in the Preview environment, do the following: (***********or AEM Assets -- AEM is not available yet?? see note below**********)

-->

1. Accédez à une page de type d’enregistrement et cliquez sur le nom d’un enregistrement. Cette action ouvre la page d&#39;aperçu de l&#39;enregistrement.
1. Cliquez sur l&#39;onglet d&#39;une page d&#39;enregistrements connectée affichant les enregistrements Planning.
Les enregistrements liés à l&#39;enregistrement que vous avez sélectionné s&#39;affichent dans la vue Tableau.
1. Cliquez sur **Connecter des enregistrements** dans le coin supérieur droit de la page d&#39;enregistrement connectée. Pour connecter des enregistrements existants, sélectionnez-les dans la zone de connexion, puis cliquez en dehors de la zone pour la fermer. Les enregistrements sont automatiquement ajoutés à la table et connectés à l’enregistrement que vous avez sélectionné. Les enregistrements doivent exister avant de pouvoir les ajouter.

   Pour plus d’informations, consultez [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).

1. Cliquez sur **Nouvelle ligne** au bas du tableau pour ajouter de nouveaux enregistrements. Les nouveaux enregistrements sont automatiquement connectés aux enregistrements que vous avez sélectionnés.
1. Modifiez toutes les informations des enregistrements connectés en ligne dans la vue Tableau.
1. Pointez sur le nom d’un enregistrement connecté, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png)

   Ou

   Sélectionnez l&#39;un des enregistrements, puis cliquez sur l&#39;une des options suivantes dans la barre bleue située en bas de la liste :

   * **Afficher** pour ouvrir la page d’enregistrement dans un nouvel onglet
   * **Copier le lien** pour copier un lien vers la page d’enregistrement
   * **Modifier la miniature** pour ouvrir la zone **Miniature d’enregistrement** et modifier l’image de la miniature de l’enregistrement
   * **Dupliquer** pour dupliquer l&#39;enregistrement connecté. L&#39;enregistrement dupliqué est également connecté à l&#39;enregistrement actif.
   * **Insérez un enregistrement au-dessus ou en dessous** pour ajouter de nouveaux enregistrements au type d’enregistrement connecté. Les nouveaux enregistrements ajoutés ici sont également connectés à l’enregistrement actif. Cette option n’est pas disponible dans la barre bleue lors de la sélection d’un enregistrement dans le tableau.
   * **Supprimer** pour supprimer l’enregistrement. La suppression d&#39;un enregistrement connecté le supprime de son type d&#39;enregistrement et de tous les endroits où l&#39;enregistrement est connecté. Les enregistrements supprimés se déplacent vers la classe **Récemment supprimés** de leur type d’enregistrement.

     Pour plus d&#39;informations sur la modification des enregistrements en mode Tableau, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >Vous pouvez sélectionner plusieurs enregistrements ou objets pour les supprimer.

1. Modifiez sur la ligne l’un des enregistrements de la table de la page enregistrements connectés.
1. Utilisez l’un des éléments d’affichage suivants dans la barre d’outils d’une page d’enregistrement connectée pour gérer la vue du tableau :

   * **Filtres**
   * **Trier**
   * **Regroupement**
   * **Champs**, pour afficher, masquer ou réorganiser les champs
   * **Hauteur de ligne**
   * **Rechercher**

   Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Vous ne pouvez pas créer, modifier ou supprimer des champs dans la vue Tableau de l&#39;onglet d&#39;un enregistrement connecté.
   >

1. Cliquez sur le menu déroulant des vues dans le coin supérieur droit de la page des enregistrements connectés, puis cliquez sur **Nouvelle vue** pour ajouter une nouvelle vue à la page, puis procédez comme suit :

   1. Ajoutez un **Nom de la vue**.
   1. Dans la zone **Type de vue**, sélectionnez l&#39;un des types de vues suivants :

      * Tableau
Pour plus d’informations, voir [Gérer la vue Tableau](/help/quicksilver/planning/views/manage-the-table-view.md)
      * Chronologie
Pour plus d’informations, voir [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).
      * Calendrier
Pour plus d’informations, voir [&#x200B; Gérer la vue Calendrier &#x200B;](/help/quicksilver/planning/views/manage-the-calendar-view.md).

        Pour plus d’informations, consultez la section [Gérer plusieurs vues à partir de la page des enregistrements connectés](#manage-multiple-views-from-the-connected-records-page) dans cet article.

   1. Cliquez sur **Créer**.
Une nouvelle vue est ajoutée au menu déroulant des vues.

   1. (Facultatif) Pointez sur le nom d’une vue que vous avez créée, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur l’une des options suivantes :

      * **Renommer**, pour ajouter un nouveau nom à la vue.
      * **Partager**

        Pour plus d’informations, consultez la section [Partager des vues](/help/quicksilver/planning/access/share-views.md).
      * **Exporter**

      * **Supprimer**
Pour plus d’informations, voir [Supprimer des vues d’enregistrement](/help/quicksilver/planning/views/delete-record-views.md).

        ![Menu Afficher plus sur la page Projets - Enregistrements connectés](assets/view-more-menu-projects-connected-records-page.png)

        >[!NOTE]
        >
        >Vous ne pouvez pas supprimer une vue système créée par Workfront.

### Gérer la page des enregistrements connectés pour les projets Workfront

Lorsque vous créez une page d’enregistrements connectés pour les projets Workfront connectés, procédez comme suit pour gérer la page :

1. Accédez à une page de type d’enregistrement et cliquez sur le nom d’un enregistrement. Cette action ouvre la page d&#39;aperçu de l&#39;enregistrement.
1. Cliquez sur l’onglet d’une page d’enregistrements connectée qui affiche les projets Workfront.
Les projets connectés à l’enregistrement que vous avez sélectionné s’affichent dans la vue Liste.
1. Cliquez sur **Connecter des enregistrements** dans le coin supérieur droit de la page d’enregistrement connectée pour connecter des projets existants.

   Pour plus d’informations, consultez la section [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).
1. Double-cliquez dans une cellule de la vue Liste pour modifier les champs d’un projet. Certains champs sont en lecture seule.
1. Effectuez l’une des opérations suivantes pour modifier la vue Liste :

   * Cliquez sur **Nouvelle ligne** pour créer un projet sans modèle. Le nouveau projet est automatiquement connecté à l’enregistrement actif.

     Pour plus d’informations, voir [Création d’objets Workfront à partir de Workfront Planning lorsque vous les connectez à des enregistrements](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).
   * Cliquez sur **Créer des enregistrements** dans le coin supérieur droit de la vue pour ajouter des projets existants. Les projets sont immédiatement connectés à l’enregistrement sélectionné.

   * Pointez sur un nom de projet dans la liste, cliquez sur le menu **Plus** [Plus](assets/more-menu.png), puis sur **Affichage** pour ouvrir le projet dans un autre onglet

     Ou

     Sélectionnez un ou plusieurs projets, puis, dans la barre d’actions située au bas de la liste, cliquez sur **Supprimer** ou **Déconnecter** pour supprimer l’élément de la liste.


   * Cliquez sur le menu déroulant des affichages, puis sur **Nouvel affichage** pour ajouter un nouvel affichage à la page, puis procédez comme suit, ou cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite d’un nouveau nom, puis **Renommer**, **Partager** ou **Supprimer** l’affichage.

     Vous ne pouvez pas renommer, partager ou supprimer des vues système ou des vues pour lesquelles vous ne disposez pas d&#39;autorisations de gestion.

     ![Menu Afficher plus sur la page Projets - Enregistrements connectés](assets/view-more-menu-projects-connected-records-page.png)

   * Cliquez sur l’un des éléments suivants pour mettre à jour les éléments de la vue :

      * **Filtrer** pour limiter la quantité d’informations dans la liste
      * **Colonnes** pour masquer les colonnes ou modifier leur ordre
      * L’icône **+** dans le coin supérieur droit de la vue Tableau pour ajouter des champs existants à la liste. Des champs doivent exister avant de pouvoir les ajouter.

   Pour plus d’informations sur la gestion des objets dans une vue Liste, voir [&#x200B; Gérer la vue Liste &#x200B;](/help/quicksilver/planning/views/manage-the-list-view.md).

<!-- this is repetitive from an earlier section above: 

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. (Conditional) When displaying Planning records in the connected records page, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: 

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Delete**

   <!--not possible right now: * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).
      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. -->


<!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      TIP      
      You can select more than one record or object to disconnect them.
      -->
