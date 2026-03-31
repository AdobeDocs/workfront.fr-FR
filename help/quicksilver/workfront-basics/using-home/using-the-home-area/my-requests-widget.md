---
product-area: projects
navigation-topic: use-the-home-area
title: Utiliser le widget Mes requêtes
description: Vous pouvez envoyer des requêtes dans le widget Mes requêtes . Vous pouvez également personnaliser le widget avec des filtres et des colonnes.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 15%

---

# Utiliser le widget Mes requêtes

>[!IMPORTANT]
>
>Cet article décrit le nouveau widget Mes requêtes . La nouvelle expérience de demande doit être activée pour afficher le nouveau widget.
>Vous pouvez activer la nouvelle expérience de demande dans la zone des Demandes .

Le widget Mes requêtes affiche les requêtes que vous avez envoyées. Vous pouvez filtrer les requêtes, rechercher des requêtes spécifiques ou ajuster l’ordre et la visibilité des colonnes. Vous pouvez également créer une requête à partir du widget Mes requêtes .

>[!NOTE]
>
>* Lorsque le widget Mes requêtes se charge, il affiche jusqu’à 50 requêtes. Pour afficher davantage de requêtes, faites défiler la liste vers le bas.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Tout package de Workfront ou de workflow</p>
   <p>Tout package Workfront Planning permettant d'accéder aux demandes Workfront Planning et aux objets créés</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence</strong></td> 
   <td> <p>Contributeur ou supérieur</p>
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Configuration du niveau d’accès</strong></td> 
   <td> <p>Afficher ou accéder plus facilement à tous les objets pour lesquels vous êtes identifié(e) dans une conversation ou avez besoin de résoudre une approbation (projets, tâches, événements, documents)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations [!UICONTROL View] ou supérieures pour les projets, les tâches, les problèmes, les documents pour lesquels vous faites l’objet d’un tag dans une conversation ou pour lesquels devez résoudre une approbation.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création d’une requête

Vous pouvez créer une demande directement à partir du widget Mes demandes .

Pour obtenir des instructions, reportez-vous à la section [Créer une demande](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) de l’article [Créer des éléments de travail et des projets à partir de la zone Accueil](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Copier une requête

Vous pouvez copier une demande dans le widget Mes demandes, la modifier et l’envoyer en tant que nouvelle demande.

Pour obtenir des instructions, voir [&#x200B; Copier et envoyer des demandes &#x200B;](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Gérer les informations de la liste des requêtes dans le widget Mes requêtes

<!--
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/lines-main-menu.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Pour ajouter le widget **Mes requêtes** à votre écran d’accueil. Cliquez sur **Personnaliser** et recherchez **Mes requêtes**, puis cliquez dessus pour l’ajouter à **Accueil**.
1. (Facultatif) Pour gérer l’affichage des informations dans la liste des demandes, mettez à jour les éléments d’affichage suivants pour la liste :

   * Afficher
   * Filtre
   * Colonnes

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   Pour plus d’informations sur la gestion des informations dans la liste des demandes, voir [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


<!-- Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.


The filter is saved automatically.

-->

>[!TIP]
>
>Si votre organisation a acheté Workfront Planning en plus d’Adobe Workfront, le widget Mes demandes inclura les demandes Workfront et Workfront Planning.
> 
>* Pour filtrer uniquement les requêtes Workfront, définissez le filtre sur **Type d’objet** > **Comporte l’un des** > **Problèmes**.
>* Pour filtrer uniquement les demandes Workfront Planning, définissez le filtre sur **Type d’objet** > **N’a aucun des** > **Problèmes**.

<!--

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## Requêtes de recherche

Pour rechercher des requêtes spécifiques dans le widget Mes requêtes :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Pour ajouter le widget **Mes requêtes** à votre écran d’accueil. Cliquez sur **Personnaliser** et recherchez **Mes requêtes**, puis cliquez dessus pour l’ajouter à **Accueil**.
1. Dans la barre de recherche située en haut à droite du widget Mes requêtes , saisissez le terme que vous souhaitez rechercher.

   Les requêtes qui contiennent le terme sont surlignées en orange.

1. (Facultatif) Pour accéder directement aux requêtes en surbrillance, cliquez sur les flèches haut ou bas de la barre de recherche.

## Accéder à un objet créé par une requête

Vous trouverez des objets créés par une requête dans le widget Mes requêtes .

>[!NOTE]
>
>Les liens vers les objets créés ne sont disponibles dans la nouvelle expérience de requête que pour les requêtes Planning, dans les cas où la requête elle-même a créé un objet. Si une requête Workfront est convertie en projet ou en un autre objet, le lien vers cet objet converti n’est pas disponible dans la liste des requêtes de la nouvelle expérience de création de requêtes.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Pour ajouter le widget **Mes requêtes** à votre écran d’accueil. Cliquez sur **Personnaliser** et recherchez **Mes requêtes**, puis cliquez dessus pour l’ajouter à **Accueil**.
1. Recherchez la requête qui a créé l’objet .
1. Cliquez sur le nom de l’objet dans la colonne **Objet créé** de cette requête.

   La page de l’objet s’ouvre.

