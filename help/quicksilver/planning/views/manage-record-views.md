---
title: Gérer les vues d’enregistrement
description: Vous pouvez afficher les enregistrements dans une vue de tableau, chronologique ou de calendrier lors de l’utilisation d’Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: f8ad026582be5b4c89939af8f135151ffaabccfe
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 76%

---


# Gérer les vues d’enregistrement

{{planning-important-intro}}

Après avoir sélectionné un type d’enregistrement dans la zone d’Adobe Workfront Planning, vous pouvez afficher tous les enregistrements de ce type dans les vues suivantes :

* Tableau

  Pour plus d’informations, voir [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

* Journal

  Pour plus d’informations, voir [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Calendrier

  Pour plus d’informations, voir [Gérer la vue de calendrier](/help/quicksilver/planning/views/manage-the-calendar-view.md).

Cet article présente les informations suivantes sur les vues d’enregistrement :

* [Créer et modifier une vue](#create-or-edit-record-views)
* [Supprimer une vue](#delete-views)
* [Dupliquer une vue](#duplicate-views)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td role="rowheader"><p>Forfait Adobe Workfront*</p></td> 
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
<p>N’importe quelle </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, voir <a href="https://business.adobe.com/products/workfront/pricing.html">Prix et package Adobe Workfront</a>. </p> 
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
   <td> <ul><li><p>Standard, Clair ou Contributeur, pour afficher les informations de la planification Workfront</p></li>
   <li><p>Standard, pour créer des espaces de travail</p></li></ul>
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
   <td>   <p>Autorisations de gestion d’une vue</p>  
   <p>Affichage d’autorisations ou d’autorisations supérieures sur une vue pour modifier temporairement les paramètres d’affichage</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, consultez les [Conditions d’accès requises dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old: 

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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->


## Remarques concernant l’utilisation des vues d’enregistrement

* Les vues dans Workfront Planning sont spécifiques au type d’enregistrement. Vous ne pouvez pas appliquer la même vue à deux types d’enregistrements différents.
* Les vues que vous créez sont visibles uniquement par vous et les personnes avec lesquelles vous les partagez.
* Lorsque vous modifiez ou supprimez une vue, elle est modifiée et supprimée pour toutes les personnes disposant d’autorisations sur la vue.
* Chaque utilisateur peut créer un maximum de 100 vues. Vous pouvez afficher plus de 100 vues pour un type d’enregistrement, mais un utilisateur ne peut créer que 100 vues.
* Vous pouvez partager les vues que vous créez avec d’autres utilisateurs. Pour plus d’informations, voir [Partage de vues](/help/quicksilver/planning/access/share-views.md).
* Les éléments suivants sont propres à chaque vue d’enregistrement :

   * Filtre
   * Regroupement 
   * Trier
   * Aspect des barres (pour le mode Chronologie)

  <!-- some of these are not available in all of the views - edit above-->

  Par exemple, lors de la création d’un filtre dans une vue de tableau, les résultats du filtre ne sont visibles que dans la vue sélectionnée et non dans toutes les vues associées au type d’enregistrement.

  >[!NOTE]
  >
  > Certains éléments d’affichage peuvent ne pas être disponibles pour toutes les vues.


## Similarités et différences entre les vues d’enregistrement

Le tableau suivant présente les similitudes et les différences entre les vues de tableau, chronologique et de calendrier :

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Fonctionnalité | Vue de tableau | Vue chronologique | Vue de calendrier |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Afficher des enregistrements dans une liste ou une table | ✓ |              | |
| Afficher tous les champs sous forme de colonnes dans le tableau, par défaut | ✓ |              |    |
| Masquer ou afficher des champs (ou des colonnes) | ✓ |               |    |
| Modifier les valeurs de champ de chaque enregistrement | ✓ |               |             |
| Ajouter des enregistrements en tant que nouvelles lignes dans la vue | ✓ |               |        |
| Ajouter des champs en tant que nouvelles colonnes dans la vue | ✓ |               |         |
| Copier des lignes d’une liste externe et les coller dans un tableau | ✓ |               |          |
| Afficher des enregistrements dans une chronologie |            | ✓ |             |
| Filtrer les enregistrements | ✓ | ✓ | ✓ |
| Afficher des enregistrements sur un calendrier |           |              | ✓ |
| Regrouper des enregistrements | ✓ | ✓ |
| Trier des enregistrements | ✓ |              |
| Attribuer des codes couleurs aux enregistrements |           | ✓ | ✓ |
| Attribuer des codes couleurs aux regroupements |           | ✓ |
| Rechercher des enregistrements spécifiques | ✓ | ✓ |
| Partager la vue avec d’autres | ✓ | ✓ | ✓ |
| Ouvrir la page de l’enregistrement à partir de la vue. | ✓ | ✓ |    |


## Créer ou modifier des vues {#create-or-edit-views}

{{step1-to-planning}}


1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’ouvre.

   Par défaut, tous les enregistrements du type sélectionné s&#39;affichent dans la vue de tableau.

1. Cliquez sur **+ Affichage** pour ajouter une nouvelle vue.
1. Choisissez parmi les types de vues suivants :

   * Tableau
   * Journal
   * Calendrier

   Un nouvel onglet est créé avec la vue sélectionnée.

   Selon la largeur de votre écran, d’autres vues peuvent s’afficher dans le menu **Plus** ![](assets/more-menu.png).


>[!TIP]
>
>Lorsque vous créez un type d’enregistrement, la vue de tableau est également créée par défaut.
>
>Pour créer une vue de chronologie ou de calendrier, le type d’enregistrement pour lequel vous créez la vue doit comporter au moins deux champs de date.
>
>Dans le cas contraire, les options Chronologie et Calendrier sont grisées.
>

![](assets/view-types-drop-down-from-record-type-list.png)

1. (Le cas échéant) Cliquez sur **Suivant** lors de la création d’une vue chronologique ou de calendrier.

   Par défaut, Workfront donne à la vue l’un des noms suivants :

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Le nombre est un incrément généré automatiquement.

1. (Le cas échéant) Sélectionnez les **dates de début** et **de fin** pour les enregistrements qui s’afficheront dans la vue chronologique ou de calendrier.

   >[!TIP]
   >
   >    Vous pouvez sélectionner des champs de date d’enregistrement ou des champs de date de recherche à partir des types d’enregistrement ou d’objet connectés. Vous devez utiliser des agrégateurs pour les champs de date (MAX ou MIN) lorsque vous sélectionnez des champs de recherche comme dates de début et de fin pour les vues de calendrier et de calendrier. Pour plus d’informations, voir [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Cliquez sur **Créer**.

   La vue s’affiche dans un nouvel onglet. Les vues s’affichent dans l’ordre chronologique à partir du moment où elles ont été créées ou partagées avec vous.
1. (Facultatif) Cliquez sur le menu **Plus** ![](assets/more-caret-down-icon-views.png) en regard de la dernière vue pour afficher toutes les vues pour le type d’enregistrement sélectionné.

   D’autres vues s’affichent dans le menu **Plus** après le dernier onglet de vue. Le numéro en regard du menu **Plus** affiche le nombre de vues supplémentaires.
1. (Facultatif) Pour renommer une vue après sa création, cliquez sur le menu déroulant Vue, puis sur le menu **Plus** ![](assets/more-menu.png) > **Renommer** pour mettre à jour le nom de la vue.

   Ou

   Double-cliquez sur le nom de la vue et commencez à saisir le nouveau nom. <!--ensure there is not another saving step here?!-->

1. (Facultatif) Pour gérer un type de vue spécifique, consultez les articles suivants :

   * [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Gérer la vue de calendrier](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## Supprimer des vues

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement.

   La page du type d’enregistrement s’ouvre.

   Par défaut, tous les enregistrements du type sélectionné s&#39;affichent dans la vue de tableau.

1. Pointez sur l’un des noms de la vue dans l’onglet Vue, cliquez sur **Plus** ![](assets/more-menu.png) à gauche du nom de la vue, puis sur **Supprimer**.
Vous devrez peut-être d’abord cliquer sur **Plus** à gauche du dernier onglet pour trouver la vue que vous souhaitez supprimer.

1. Cliquez sur **Supprimer** pour confirmer. <!--ensure there is not another saving step here?!-->

   La vue est supprimée pour l’ensemble des utilisateurs et des utilisatrices qui peuvent accéder à la zone des enregistrements et elle ne peut pas être récupérée.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Dupliquer une vue

Si vous souhaitez conserver plusieurs versions d’une vue et apporter de légères modifications entre les versions, vous pouvez dupliquer une vue.

La duplication d’une vue crée des copies identiques d’une vue existante.

Les autorisations de partage de la vue d’origine ne sont pas transférées à la vue dupliquée.

{{step1-to-planning}}

1. Cliquez sur la carte d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur une carte de type d’enregistrement.

   La page de type enregistrement s’ouvre.
Par défaut, tous les enregistrements du type sélectionné s&#39;affichent dans la vue de tableau.

1. Pointez sur l’onglet de la vue à dupliquer, cliquez sur le menu **Plus** ![](assets/more-menu.png) à droite du nom de la vue, puis sur **Dupliquer**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   La vue est dupliquée et le nom de la nouvelle vue suit le modèle suivant : `Original view's name (Copy)`. Le nouvel onglet de vue s’affiche à la fin de tous les onglets de vue.

