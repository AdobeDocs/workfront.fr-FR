---
title: Ajouter une page Enregistrements connectés à un enregistrement
description: Vous pouvez afficher les informations des enregistrements ou objets connectés en ajoutant un onglet pour une page Enregistrements connectés à un enregistrement. Les enregistrements connectés dans une vue Tableau sont alors ajoutés à l’onglet.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 54ba4509269784ebe25fb5283b539c440454362a
workflow-type: tm+mt
source-wordcount: '1577'
ht-degree: 4%

---


# Ajouter une page Enregistrements connectés à un enregistrement

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Vous pouvez afficher des informations provenant d&#39;enregistrements ou d&#39;objets connectés en ajoutant un onglet pour la page Enregistrements connectés à un enregistrement dans Adobe Workfront Planning. Les enregistrements connectés dans une vue Tableau sont alors ajoutés à l’onglet.

Tenez compte des points suivants lors de l’ajout d’une page Enregistrements connectés à un enregistrement :

* Vous pouvez ajouter une page Enregistrements connectés à un enregistrement après avoir connecté des enregistrements ou des types d&#39;objet au type d&#39;enregistrement à partir de la vue Tableau d&#39;un type d&#39;enregistrement.

* Vous pouvez ajouter une page Enregistrements connectés à partir de la zone d&#39;aperçu d&#39;un enregistrement ou de la page de l&#39;enregistrement.

* Les pages Enregistrements connectés affichent uniquement les objets connectés ou les enregistrements d’un type d’objet ou d’enregistrement. La page n’affiche pas tous les enregistrements de ce type.

* Vous pouvez afficher les objets dans une page d’enregistrements connectés en mode Tableau.

<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>

* <span class="preview">You can create one page per one object or record type. For example, you cannot create two connected record pages for connected projects or tactics.</span>

-->

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
   <p>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Prise en main d’Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
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

1. Ajoutez le **Nom de la page**, cliquez sur **Page des enregistrements connectés**, puis sur **Créer**.

   Une nouvelle page d’enregistrements connectés est ajoutée sous la forme d’un nouvel onglet à la page d’enregistrement.

   Les enregistrements connectés à l’enregistrement actif s’affichent dans la vue Tableau.

   >[!TIP]
   >
   >Vous devez ajouter les enregistrements connectés dans la table ou la zone Détails d&#39;un enregistrement avant de pouvoir les afficher dans une page d&#39;enregistrements connectés.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   Les cinq premiers champs des enregistrements connectés s’affichent par défaut. <!--No lookup fields display by default.-->

   ![Vue du tableau connecté à l’audience sous les détails de la campagne](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Facultatif) Cliquez sur le nom d&#39;un enregistrement ou d&#39;un type d&#39;objet connecté dans la liste, ou recherchez-le, puis cliquez dessus lorsqu&#39;il s&#39;affiche dans la liste pour créer la page de cet enregistrement ou de ce type d&#39;objet.

1. (Facultatif et conditionnel) Si plusieurs champs connectés du type d’enregistrement pour lequel vous créez la page s’affichent, cliquez sur le champ dont vous souhaitez afficher les enregistrements dans la page enregistrements connectés.

   L’une des pages suivantes est ajoutée à la page des enregistrements connectés :

   * Vue Tableau d’un type d’enregistrement
   * Vue Liste d’un type d’objet de projet

1. (Facultatif et conditionnel) Lorsque vous créez une page Enregistrements connectés pour les enregistrements Planning connectés, effectuez l&#39;une des opérations suivantes : <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Cliquez sur le nom d’un enregistrement. La page de l&#39;enregistrement s&#39;ouvre alors dans un nouvel onglet.
   * Cliquez sur **Connexion** au bas de la vue Tableau pour connecter des enregistrements existants, sélectionnez-les dans la zone de connexion, puis cliquez en dehors de la zone pour la fermer. Les enregistrements sont automatiquement ajoutés à la table. Les enregistrements doivent exister avant de pouvoir les ajouter.

     Pour plus d’informations, consultez [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).
   * Modifiez toutes les informations des enregistrements connectés en ligne dans la vue Tableau.

   * Pointez sur le nom d’un enregistrement connecté, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png)

     Ou

     Sélectionnez l&#39;un des enregistrements, puis cliquez sur l&#39;une des options suivantes dans la barre bleue située en bas de la liste :

      * **Afficher** pour ouvrir la page d’enregistrement dans un nouvel onglet
      * **Copier le lien** pour copier un lien vers la page d’enregistrement
      * **Modifier la miniature** pour ouvrir la zone **Miniature d’enregistrement** et modifier l’image de la miniature de l’enregistrement
      * **Dupliquer** pour dupliquer l&#39;enregistrement connecté. L&#39;enregistrement dupliqué est également connecté à l&#39;enregistrement actif.
      * **Insérez un enregistrement au-dessus ou en dessous** pour ajouter de nouveaux enregistrements au type d’enregistrement connecté. Les nouveaux enregistrements ajoutés ici sont également connectés à l’enregistrement actif. Cette option n’est pas disponible dans la barre bleue lors de la sélection d’un enregistrement dans le tableau.
      * **Supprimer** pour supprimer l’enregistrement. La suppression d&#39;un enregistrement connecté le supprime de son type d&#39;enregistrement et de tous les endroits où l&#39;enregistrement est connecté.

        Pour plus d&#39;informations sur la modification des enregistrements en mode Tableau, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

        >[!TIP]
        >
        >Vous pouvez sélectionner plusieurs enregistrements ou objets pour les supprimer.

   * Modifiez sur la ligne l&#39;un des enregistrements Planning de la table de la page des enregistrements connectés.
   * Utilisez l’un des éléments d’affichage suivants dans la barre d’outils d’une page d’enregistrement connectée pour gérer la vue du tableau :

   * **Filtres**
   * **Trier**. Non disponible pour les projets.
   * **Regroupement**. Non disponible pour les projets.
   * **Champs**, pour afficher, masquer ou réorganiser les champs
   * **Hauteur de ligne**. Non disponible pour les projets.
   * **Rechercher**

     Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

     >[!NOTE]
     >
     >Vous ne pouvez pas créer, modifier ou supprimer des champs dans la vue Tableau de l&#39;onglet d&#39;un enregistrement connecté.

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
      >[!TIP]
      >
      >You can select more than one record or object to disconnect them.
      -->
1. (Facultatif et conditionnel) Lorsque vous créez une page d’enregistrements connectés pour des projets Workfront connectés, effectuez l’une des opérations suivantes :

   * Cliquez sur **Connecter des enregistrements** dans le coin supérieur droit de la page d’enregistrement connectée pour connecter des projets existants.

     Pour plus d’informations, consultez la section [Connecter les enregistrements](/help/quicksilver/planning/records/connect-records.md).
   * Modifiez les informations du projet sur la ligne dans le tableau.
   * Cliquez sur **Nouvelle ligne** pour créer un projet sans modèle. Le nouveau projet est immédiatement connecté à l&#39;enregistrement actuel.

     Pour plus d’informations, voir [Création d’objets Workfront à partir de Workfront Planning lorsque vous les connectez à des enregistrements](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * Pointez sur un projet et cliquez sur le menu **Plus** [Plus](assets/more-menu.png)

     Ou

     Sélectionnez un ou plusieurs projets, remarquez la barre bleue en bas de la liste, puis cliquez sur l’un des éléments suivants :

      * **Supprimer** pour supprimer le projet. La suppression d’un projet le déconnecte de l’enregistrement et le déplace vers la Corbeille de Workfront.
      * **Déconnecter** pour déconnecter le projet de l’enregistrement. La déconnexion d’un projet supprime cet enregistrement et toutes les valeurs de ses champs de recherche de l’enregistrement actif.

     >[!TIP]
     >
     >Vous pouvez sélectionner plusieurs projets à déconnecter ou à supprimer.
   * Cliquez sur le menu déroulant des vues, puis sur **Nouvelle vue** pour ajouter une nouvelle vue à la page, puis procédez comme suit :
      1. Ajoutez un **Nom de la vue**.
      1. Sélectionnez **Liste** dans la zone **Type de vue**.
      1. Cliquez sur **Créer**.
Une nouvelle vue Liste est ajoutée au menu déroulant des vues.
      1. (Facultatif) Pointez sur le nom d’une vue que vous avez créée, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur l’une des options suivantes :

         * **Renommer**, pour ajouter un nouveau nom à la vue.
         * <span class="preview">**Partager**</span>
Pour plus d’informations, voir [Partager des vues](/help/quicksilver/planning/access/share-views.md).
         * **Supprimer**
Pour plus d’informations, voir [Supprimer des vues d’enregistrement](/help/quicksilver/planning/views/delete-record-views.md).

           ![](assets/view-more-menu-projects-connected-records-page.png)
   * Cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png) et utilisez le filtre pour afficher des projets spécifiques.

     >[!TIP]
     >
     ><span class="preview">Pour les champs de type personne, tels que **Propriétaire** ou **Sponsor**, vous pouvez utiliser un caractère générique pour afficher les projets dans lesquels l’utilisateur connecté est affecté à ces rôles.</span>
     >
     >![Filtrer avec le caractère générique utilisateur pour la page des enregistrements connectés au projet](assets/filter-with-user-wildcard-project-connected-records-page.png)
     >
   * Cliquez sur l’icône **Colonnes** ![Icône Colonnes](assets/columns-icon.png) pour masquer ou afficher les colonnes de la liste.
   * Cliquez sur l’icône **+** dans le coin supérieur droit de la vue du tableau pour ajouter des champs existants au tableau. Des champs doivent exister avant de pouvoir les ajouter.

     La boîte de dialogue **Gestionnaire de colonnes** s’ouvre. Procédez comme suit :

      1. Recherchez un champ d’objet existant dans la colonne **Disponible**, puis cliquez sur **+** à droite du nom du champ pour l’ajouter à la colonne **Sélectionné**.

         Les champs que vous sélectionnez sont ajoutés à la vue Tableau dans la page enregistrements connectés.
      1. Cliquez sur **-** à droite d’un champ dans la colonne **Sélectionné** pour le supprimer de la vue Tableau.
      1. Cliquez sur **Enregistrer** pour enregistrer l’affichage du tableau de la page d’enregistrement connectée.
1. (Facultatif) Double-cliquez sur le nom de l’onglet **Page des enregistrements connectés**

   Ou

   Pointez sur le nom de l’onglet, puis cliquez sur **Plus** ![Menu Plus](assets/more-menu.png), puis cliquez sur **Renommer** pour renommer en nouvel onglet Vue connectée.


   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Facultatif) Pointez sur le nom de l’onglet Page Enregistrements connectés , cliquez sur **Plus** ![Menu Plus](assets/more-menu.png), puis cliquez sur **Supprimer** pour supprimer de l’onglet.

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->