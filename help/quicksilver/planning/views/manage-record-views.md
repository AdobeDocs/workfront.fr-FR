---
title: Gérer les vues d’enregistrement
description: Vous pouvez afficher les enregistrements dans un tableau, une chronologie ou un calendrier lors de l’utilisation d’Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: cbba9d21046d2bf05675cadea9ce706fbde6adc1
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 7%

---

# Gérer les vues d’enregistrement

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Après avoir sélectionné un type d’enregistrement dans la zone de planification Adobe Workfront, vous pouvez afficher tous les enregistrements de ce type dans les vues suivantes :

* Tableau

  Pour plus d’informations, voir [Gestion de la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

* Journal

  Pour plus d’informations, voir [Gestion du mode Chronologie](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Calendrier

  Pour plus d’informations, voir [Gestion de la vue Calendrier](/help/quicksilver/planning/views/manage-the-calendar-view.md).

Cet article décrit les informations suivantes sur les vues d’enregistrement :

* [Création et modification d’une vue](#create-or-edit-record-views)
* [Suppression d’une vue](#delete-views)
* [Dupliquer une vue](#duplicate-views)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## Conditions d’accès

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
   <p> Produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite à l’étape d’accès anticipé pour la planification Workfront </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>N’importe quelle</p> 
   <p>Les administrateurs système n’ont accès qu’aux vues qu’ils ont créées ou qui sont partagées avec eux. </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">Configuration du niveau d’accès</td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour la planification Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations pour l’affichage</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modèle de mise en page</td>
   <td> <p>L’administrateur système doit ajouter la zone Planning dans votre modèle de mise en page. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Remarques concernant l’utilisation des vues d’enregistrement

* Les vues dans Workfront Planning sont spécifiques au type d’enregistrement. Vous ne pouvez pas appliquer la même vue à deux types d’enregistrements différents.
* Les vues que vous créez sont visibles uniquement pour vous et les utilisateurs avec lesquels vous partagez les vues.
* Lorsque vous modifiez ou supprimez une vue, elle est modifiée et supprimée pour tous les utilisateurs disposant d’autorisations sur la vue.
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

Le tableau suivant présente les similitudes et les différences entre les vues de tableau, de chronologie et de calendrier :

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Fonctionnalité | Vue Tableau | Mode Chronologie | Vue Calendrier |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Afficher des enregistrements dans une liste ou une table | ✓ |              | |
| Afficher tous les champs sous forme de colonnes dans le tableau, par défaut | ✓ |              |    |
| Masquer ou afficher des champs (ou des colonnes) | ✓ |               |    |
| Modifier les valeurs de champ de chaque enregistrement | ✓ |               |             |
| Ajouter des enregistrements en tant que nouvelles lignes dans la vue | ✓ |               |        |
| Ajouter des champs en tant que nouvelles colonnes dans la vue | ✓ |               |         |
| Copier des lignes d’une liste externe et les coller dans un tableau | ✓ |               |          |
| Afficher des enregistrements dans une chronologie |            | ✓ |             |
| Filtrage des enregistrements | ✓ | ✓ | ✓ |
| Afficher des enregistrements sur un calendrier |           |              | ✓ |
| Enregistrements de groupe | ✓ | ✓ |
| Tri des enregistrements | ✓ |              |
| Enregistrements de code couleur |           | ✓ | ✓ |
| Regroupements de codes couleur |           | ✓ |
| Recherche d’enregistrements spécifiques | ✓ | ✓ |
| Partager la vue | ✓ | ✓ | ✓ |
| Ouvrez la page de l’enregistrement à partir de la vue . | ✓ | ✓ |    |


## Créer ou modifier des vues {#create-or-edit-views}

{{step1-to-planning}}


L’espace de travail que vous avez consulté pour la dernière fois s’ouvre par défaut. Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

1. Cliquez sur une carte de type enregistrement. Pour plus d’informations sur la création d’un type d’enregistrement, voir [Création de types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   Par défaut, tous les enregistrements du type sélectionné s&#39;affichent en mode Tableau.

1. Cliquez sur **+ Affichage** pour ajouter une nouvelle vue.
1. Choisissez parmi les types de vues suivants :

   * Tableau
   * Journal
   * Calendrier

   Un nouvel onglet est créé avec la vue sélectionnée.

   Selon la largeur de votre écran, d’autres vues peuvent s’afficher dans la variable **Plus** menu ![](assets/more-menu.png).


>[!TIP]
>
>Lorsque vous créez un type d’enregistrement, la vue de tableau est également créée par défaut.
>
>Pour créer une vue de chronologie ou de calendrier, le type d’enregistrement pour lequel vous créez la vue doit comporter au moins deux champs de date. Dans le cas contraire, les options Chronologie et Calendrier sont grisées.
>

![](assets/view-types-drop-down-from-record-type-list.png)

>[!NOTE]
>
>    Pour créer une vue de chronologie ou de calendrier, le type d’enregistrement pour lequel vous créez la vue doit comporter au moins deux champs de date. Dans le cas contraire, les options Chronologie ou Calendrier sont grisées.

1. (Conditionnel) Cliquez sur **Suivant**, lors de la création d’une vue de chronologie ou de calendrier.

   Par défaut, Workfront donne à la vue l’un des noms suivants :

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Le nombre est un incrément généré automatiquement.

1. (Conditionnel) Sélectionnez le **Début** et **Dates de fin** pour les enregistrements qui s’afficheront dans la vue chronologie ou calendrier.

   >[!TIP]
   >
   >    Vous pouvez sélectionner des champs de date d’enregistrement ou des champs de date de recherche à partir d’enregistrements ou d’objets connectés.

1. Cliquez sur **Créer**.

   La vue s’affiche sous la forme d’un nouvel onglet. Les vues s’affichent dans l’ordre chronologique à partir du moment où elles ont été créées ou partagées avec vous.
1. (Facultatif) Cliquez sur le **Plus** menu ![](assets/more-caret-down-icon-views.png) en regard de la dernière vue pour afficher toutes les vues pour le type d’enregistrement sélectionné.

   D’autres vues s’affichent sous **Plus** après l’onglet de la dernière vue. Le numéro en regard de la variable **Plus** affiche le nombre de vues supplémentaires.
1. (Facultatif) Pour renommer une vue après sa création, cliquez sur le menu déroulant Affichage , puis sur la variable **Plus** menu ![](assets/more-menu.png) > **Renommer** pour mettre à jour le nom de la vue

   Ou

   Double-cliquez sur le nom de la vue et commencez à saisir le nouveau nom.  <!--ensure there is not another saving step here?!-->

1. (Facultatif) Pour gérer un type de vue spécifique, consultez les articles suivants :

   * [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Gestion de la vue Calendrier](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## Suppression de vues

{{step1-to-planning}}

L’espace de travail que vous avez consulté pour la dernière fois s’ouvre par défaut. Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

1. Cliquez sur une carte de type enregistrement.

   Pour plus d’informations sur la création d’un type d’enregistrement, voir [Création de types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   Par défaut, tous les enregistrements du type sélectionné s&#39;affichent en mode Tableau.

1. Passez la souris sur l’un des noms de la vue dans l’onglet Affichage , puis cliquez sur **Plus** ![](assets/more-menu.png) à gauche du nom de la vue, puis cliquez sur **Supprimer**.
Tout d’abord, vous devrez peut-être cliquer sur **Plus** à gauche du dernier onglet pour trouver la vue que vous souhaitez supprimer.

1. Cliquez sur **Supprimer** pour confirmer. <!--ensure there is not another saving step here?!-->

   La vue est supprimée pour tous les utilisateurs qui peuvent accéder à la zone des enregistrements et elle ne peut pas être récupérée.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Dupliquer une vue

Si vous souhaitez conserver plusieurs versions d’une vue et apporter de légères modifications entre les versions, vous pouvez dupliquer une vue.

La duplication d’une vue crée des copies identiques d’une vue existante.

Les autorisations de partage de la vue d’origine ne sont pas transférées vers la vue dupliquée.

{{step1-to-planning}}

L’espace de travail que vous avez consulté pour la dernière fois s’ouvre par défaut.

Pour plus d’informations sur la création d’espaces de travail, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

1. Cliquez sur une carte de type enregistrement. Pour plus d’informations sur la création d’un type d’enregistrement, voir [Création de types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   Par défaut, tous les enregistrements du type sélectionné s&#39;affichent en mode Tableau.

1. Pointez sur l’onglet de la vue à dupliquer, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) à droite du nom de la vue, puis cliquez sur **Dupliquer**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   La vue est dupliquée et le nom de la nouvelle vue suit le modèle suivant : `Original view's name (Copy)`. Le nouvel onglet d’affichage s’affiche à la fin de tous les onglets d’affichage.

