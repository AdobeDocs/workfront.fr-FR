---
content-type: release-notes
title: Activité de mise à jour du troisième trimestre 2026 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le troisième trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: f11daa69f72c32418298ac75f81b0fb64835d99b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 4%

---

# Activité de mise à jour du troisième trimestre 2026 pour Adobe Workfront Planning

<!--take the next sentence out when we start listing features-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du troisième trimestre 2026.

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

<!--

## List view updates 

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

Multiple field types on the list view have been updated to include keyboard navigation and other enhancements. 

Multi-, Single-select, and Assignee fields now offer keyboard navigation in the list view: 

* Use the up and down arrows on your keyboard to move through the list of people. 

* Press the space bar to select a person or to remove a selected person. 

On single and multi-select fields in the list view:  

* You can add new options directly from the editor when no results are found. Note that this feature may not be available on all lists. 

* The field interaction is now keyboard accessible. This includes navigation between the tags, search options, and list using the up and down arrows. Press the space bar to select an item or remove a selected item. 

Reference fields such as typeahead and external lookup fields, have received some interface enhancements. 

Also, where available, the experience of dragging and dropping columns has been improved visually. 

For more information, see [Manage the list view in Adobe Workfront Planning](/help/quicksilver/planning/views/manage-the-list-view.md). 

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}


You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

## Workfront reference fields are enabled as lookup fields for Planning connections

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026  
>Production for everyone: July 16, 2026 

You can now add Workfront reference fields as lookup fields when connecting a Planning record type with a Workfront object type. 

For example, you can add the Portfolio, Program, Group or Company information from the Project object to a project connection field of a campaign in Planning.  

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

## Edit submitted Planning requests

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

Users can now edit Planning requests after they submitted them. The following users can edit a submitted request: 

* The request creator 
* Workspace managers for the workspace where the request was submitted 
* System administrators 

For more information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md). 

## Synchronize Metadata from Planning to AEM Content Fragments  

>[!NOTE]
>
>Preview: May 28 , 2026
>Production fast release: May 28, 2026
>Production for everyone: May 28, 2026
>[!BADGE Off schedule]{type=Neutral}

***************TO ADD MORE INFO AFTER TALKING WITH SYUZANNA**********

To improve data integrity, we've released seamless metadata synchronization between Planning record types in the GenStudio workspace and AEM Content Fragments when Content Fragments are linked to GenStudio campaigns.  

GenStudio campaign information now displays in the Metadata tab of a Content Fragment in AEM.  

With this release key metadata is consistent across both platforms and reflects updates in near real-time, reducing manual reconciliation. 

For information, see [Get Started with Adobe Workfront Planning and GenStudio for Performance Marketing integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).  

## Synchronize Metadata from Planning to AEM Assets (title)
 
>[!NOTE]
>
>Preview: May 28 , 2026
>Production fast release: May 28, 2026
>Production for everyone: May 28, 2026
>[!BADGE Off schedule]{type=Neutral} 

To improve data integrity, we've released seamless metadata synchronization between  GenStudio record types and AEM Assets when AEM Assets are linked to GenStudio record types in Workfront Planning. The following GenStudio for Performance Marketing record types can be connected to AEM Assets: Campaign, Product, Persona, Region, and Channel. 

Information added to a GenStudio record type in Workfront Planning displays in a separate Campaign tab of an AEM Asset in AEM. 

For information, see [Get Started with Adobe Workfront Planning and GenStudio for Performance Marketing integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## New filters for the timeline view breakdown feature 

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

You can now filter information in the timeline view based on criteria that match items included in the breakdown of the records.  

Prior to this enhancement, you could only apply filters for the main records in the timeline view. 

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

## Grant permissions to records

***********CHECKING WITH LILIT ABOUT PREVIEW************ 

>[!NOTE]
>
>Preview: Not available
>Production fast release: May 28, 2026
>Production for everyone: May 28, 2026
>[!BADGE Off schedule]{type=Neutral}

You can now share individual records with users.  

By default, users inherit permissions from the workspace and the record type.  

You can give users the following permissions levels: 

* View 
* Manage 

>[!NOTE]
>
>* You cannot remove a user's permissions from a record at this time. If they have at least View permissions to the record type, they can view all the records of that type.  
>* Sharing records is not available in the Preview environment. It is only available in the Production environment.  

For information, see [Share records](/help/quicksilver/planning/access/share-records.md).

## New indication that edited and deleted fields impact request forms 

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added a reminder that record fields that you edit or delete might impact request forms that contain those fields. Now, you will have a chance to review the affected forms and ensure the changes you want to make to the fields will not impact existing information.  

For information, see [Edit field settings](/help/quicksilver/planning/fields/edit-fields.md). 

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

<!--

API new version delayed till May 21, 2026

## Workfront Planning API version 2 

>[!NOTE]
>
>Available for all customers: May 28, 2026

Version 2 of Workfront Planning API is now available and it significantly expands the capabilities of Version 1.  

The following enhancements are included in Version 2: 

* Create, update, and delete workspaces, record types, and fields programmatically. 

* Fully manage records. 
* Improvements to URL structure, error handling, pagination, filtering, and permissions. 
* Includes partial updates via PATCH 
* Includes bulk record operations. 

Version 1 remains available, although we recommend that you switch to using Version 2.  

>[!NOTE]
>
>The Workfront Planning connector for Fusion has not been updated to API Version 2 and it will continue to use Version 1 until further notice.   

For information, see [Adobe Workfront Planning API basics](/help/quicksilver/planning/general/planning-api-basics.md).  

For Workfront Planning API specifications, see the [Workfront Planning API](https://developer.adobe.com/wf-planning/) developer documentation. 

-->



## Nouvelle fenêtre d’aperçu pour les fragments de contenu AEM

>[!NOTE]
>
>Aperçu : 14 mai 2026>Version rapide de production : 14 mai 2026>Production pour tous : 14 mai 2026>[!BADGE Hors planning]{type=Neutral}

Pour une meilleure visibilité lorsque vous utilisez des fragments de contenu AEM connectés à des enregistrements Workfront Planning, nous avons ajouté une fenêtre d’aperçu qui affiche des informations sur les fragments dans Workfront Planning.

Cette fonctionnalité était auparavant disponible pour les ressources AEM et nous l’avons maintenant ajoutée aux fragments de contenu.

Pour plus d’informations, consultez [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

## Champs de recherche désormais disponibles pour les fragments de contenu AEM dans Workfront Planning

>[!NOTE]
>
>Aperçu : 14 mai 2026>Version rapide de production : 14 mai 2026>Production pour tous : 14 mai 2026>[!BADGE Hors planning]{type=Neutral}

Vous pouvez désormais ajouter les champs de recherche suivants lorsque vous connectez un type d’enregistrement Planning à un fragment de contenu AEM :

* Créé par
* Date de création
* Modifié par
* Modifié le

Avant cette amélioration, les champs de recherche n’étaient disponibles que pour les ressources et dossiers AEM.

Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).



## Vues personnalisées pour la page Détails d&#39;un enregistrement

>[!NOTE]
>
>Aperçu : 14 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Pour une meilleure flexibilité de visualisation de vos informations dans la page de détails d&#39;un enregistrement, nous avons introduit la possibilité de créer des vues personnalisées pour cette page.

Outre l&#39;ajout de deux vues de page de détails déjà créées, qui contiennent tous les champs d&#39;enregistrement ou uniquement les champs visibles en mode Tableau, vous pouvez désormais créer des vues personnalisées pour les pages de détails d&#39;un enregistrement. Les vues que vous créez sont visibles par tous ceux qui peuvent accéder à l&#39;enregistrement.

Cette mise à jour supprime le paramètre **Afficher tous les champs** et le remplace par des vues détaillées personnalisées.

Pour plus d’informations, voir [&#x200B; Gérer la page d’enregistrement &#x200B;](/help/quicksilver/planning/records/manage-the-record-page.md).

## Ajouter des regroupements à une page d’enregistrement connecté Projets

>[!NOTE]
>
>Aperçu : 14 mai 2026\
>Production rapide : 11 juin 2026>Production pour tous : 16 juillet 2026

Vous pouvez désormais regrouper vos informations dans la page Enregistrements connectés à des projets d’un enregistrement dans Workfront Planning. Cette fonctionnalité n&#39;existait pas dans ce domaine avant cette amélioration.

Pour plus d’informations, voir [&#x200B; Gérer la vue Liste &#x200B;](/help/quicksilver/planning/views/manage-the-list-view.md).
