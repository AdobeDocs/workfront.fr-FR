---
product-area: requests
navigation-topic: create-requests
title: Créer et gérer des vues dans la zone Requêtes
description: Si vous utilisez la nouvelle expérience de demande, vous pouvez créer et enregistrer des vues pour la zone des Demandes.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 59a9725e7697a81be2a827a902ee3d23085a2ecd
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 11%

---


# Créer et gérer des vues dans la zone Requêtes

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Si vous utilisez la nouvelle expérience de demande dans Adobe Workfront, vous pouvez créer et enregistrer des vues pour la zone des Demandes . Ces vues incluent des filtres et des dispositions de colonnes, des <span class="preview"> et des regroupements.</span>


>[!IMPORTANT]
>
>* Cette fonctionnalité n’est disponible que dans la nouvelle expérience de demande de la zone des Demandes .
>* Les paramètres d’affichage sont également disponibles dans le widget Mes requêtes de l’Accueil. Toutefois, les vues de la zone des Demandes sont distinctes de celles du widget Mes demandes .
>* La liste des demandes de la zone des Demandes et du widget Mon travail utilise la liste améliorée de Workfront. Pour plus d’informations, voir [Utilisation de listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package de Workfront ou de workflow</p>
   <p>Toute licence Workfront Planning, pour afficher les demandes Workfront Planning dans les listes de demandes</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Contributeur ou supérieur</p>
   <p>Requête ou supérieure</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p>  <p>Vous devez être un administrateur Workfront pour ajouter des vues aux modèles de disposition</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<div class="preview">

## Vues système pour les requêtes

>[!NOTE]
>
>Les vues système peuvent ne pas être disponibles dans votre environnement de prévisualisation. Ils seront disponibles en production pour tous les clients le 16 avril 2026.

Outre les vues que vous pouvez créer vous-même, Workfront propose les vues système suivantes pour la zone des Requêtes et le widget Mes requêtes dans l’Accueil :

* **Toutes les requêtes** : toutes les requêtes que vous ou une autre personne avez envoyées dans les files d’attente ou les espaces de travail que vous êtes autorisé à afficher. Cette option n’est pas disponible pour le widget Mes requêtes .
* **Mes demandes** : les demandes que vous avez envoyées, quel que soit leur statut.
* **Mes demandes ouvertes** : les demandes que vous avez envoyées sont toujours ouvertes.
* **Mes brouillons** : des brouillons de vos requêtes qui n&#39;ont pas encore été soumis.
* **Demandes ouvertes** : demandes que vous ou toute autre personne avez envoyées dans les files d’attente ou pour les espaces de travail que vous êtes autorisé à afficher et qui sont toujours ouverts. Cette option n’est pas disponible pour le widget Mes requêtes .

Vous ne pouvez pas modifier les vues système. Vous pouvez modifier leurs éléments, puis copier la vue et modifier ou partager la copie.

</div>

## Création d’une vue pour les requêtes

Vous pouvez créer une vue dans la zone des Demandes de Workfront lorsque vous utilisez la nouvelle expérience de demandes. Après avoir activé et ajouté une nouvelle expérience de requêtes, vous pouvez également créer des vues pour le widget Mes requêtes dans l’Accueil.

1. Pour accéder à la liste **Demandes** :

   {{step1-to-requests}}

   1. Assurez-vous que le paramètre **Utiliser une nouvelle expérience** est activé.

1. Pour accéder au widget **Mes requêtes** dans l’accueil :

   {{step1-to-home}}

   1. Ajoutez ou accédez au widget **Mes requêtes**.

1. Dans la liste des requêtes, cliquez sur le menu déroulant **Vues** ![Liste déroulante Vues](assets/view-icon-requests.png) et cliquez sur **Nouvelle vue**.

   <!-- 
   
   replace the screen shot with release
   ![New view](assets/create-new-view.png)

   -->

1. Saisissez le nom de la nouvelle vue, puis cliquez sur **Créer**.
1. Passez à [Modifier une vue pour les demandes](#edit-a-view-for-requests).

## Modification d’une vue pour les requêtes

Vous pouvez modifier des vues existantes, y compris les vues que vous venez de créer dans la zone des Demandes ou le widget Mes demandes dans l’Accueil.

En modifiant une vue, vous pouvez modifier les éléments suivants de la vue :

* Nom
* Filtres
* Colonnes

<div class="preview">

* Regroupement
* Formater les cellules
* Hauteur de ligne

</div>

Pour plus d’informations, voir [Utilisation de listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Les modifications apportées aux vues sont enregistrées automatiquement.
> * Toute personne qui utilise la vue peut voir les modifications apportées aux vues <span class="preview">uniquement lorsque vous partagez une nouvelle copie de la vue après y avoir apporté des modifications.</span>
> * Utilisez le caractère générique de filtre **Moi (utilisateur connecté)** dans tout champ ayant des utilisateurs comme valeur.

## Ajout de la vue des requêtes à un modèle de mise en page

Un administrateur Workfront peut ajouter une nouvelle vue aux modèles de mise en page pour la zone des Demandes .

Pour obtenir des instructions, voir [Personnaliser des filtres, des vues et des regroupements à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Partager une vue

Vous pouvez partager les vues que vous créez avec d&#39;autres utilisateurs, équipes, groupes ou sociétés.

Après avoir partagé une vue, d’autres utilisateurs peuvent afficher les éléments de vue mis à jour que vous avez modifiés pour la vue avant de la partager.

<span class="preview">S&#39;ils mettent à jour la vue, leurs modifications ne seront pas visibles par les autres utilisateurs, à moins qu&#39;ils ne fassent une copie de la même vue et conservent leurs modifications avant de partager la copie.

Pour plus d&#39;informations, voir [Utiliser des listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->