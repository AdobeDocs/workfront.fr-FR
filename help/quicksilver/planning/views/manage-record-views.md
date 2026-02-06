---
title: Gérer les vues d’enregistrement
description: Vous pouvez afficher les enregistrements dans une vue Tableau, Chronologie ou Calendrier lors de l'utilisation d'Adobe Workfront Planning. Cet article décrit comment créer une vue et modifier une vue existante.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 33%

---


# Gérer les vues d’enregistrement

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Après avoir sélectionné un type d&#39;enregistrement dans la zone Adobe Workfront Planning, vous pouvez afficher tous les enregistrements de ce type de différentes manières.

Vous pouvez afficher les enregistrements dans des vues de plusieurs formats qui vous donnent la possibilité d’explorer et de comprendre les informations de la manière qui vous convient le mieux. Que vous souhaitiez un aperçu structuré, une histoire chronologique, une mise en page basée sur la date ou une simple liste défilable, chaque vue offre un point de vue unique.

Les enregistrements peuvent être affichés dans les vues suivantes :

* Tableau

  Pour plus d’informations, voir [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

* Journal

  Pour plus d’informations, voir [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Calendrier

  Pour plus d’informations, voir [Gérer la vue de calendrier](/help/quicksilver/planning/views/manage-the-calendar-view.md).

* Liste

  Vous pouvez afficher les enregistrements dans une page Enregistrement connecté dans une vue Liste.

  >[!IMPORTANT]
  >
  >Vous ne pouvez pas appliquer une vue Liste à une liste d&#39;enregistrements sur une page de type d&#39;enregistrement. Vous pouvez uniquement appliquer une vue Liste dans une page Enregistrement connecté d’un enregistrement à une liste de projets connectés. <!--this will change-->

  Pour plus d’informations, consultez les articles suivants :

   * [Ajouter une page Enregistrements connectés à un enregistrement](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)
   * [Gestion de la vue Liste](/help/quicksilver/planning/views/manage-the-list-view.md)

Cet article présente les informations suivantes sur les vues d’enregistrement :

* [Créer et modifier une vue](#create-or-edit-record-views)
* [Activer les indicateurs de présence en temps réel dans une vue](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Pour plus d’informations sur la gestion des vues d’enregistrement Workfront Planning, consultez également les articles suivants :

* [Supprimer les vues d’enregistrement](/help/quicksilver/planning/views/delete-record-views.md)
* [Dupliquer les vues d’enregistrement](/help/quicksilver/planning/views/duplicate-record-views.md)
* [Partager des affichages](/help/quicksilver/planning/access/share-views.md)


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
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p> Standard pour créer et supprimer des vues</p>
   <p>Contributeur ou version ultérieure pour mettre à jour les éléments d’affichage</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations pour une vue</p>  
   <p>Autorisations d’affichage d’une vue pour modifier temporairement les paramètres d’affichage ou la dupliquer</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> Les utilisateurs disposant d'une licence light ou contributor doivent se voir attribuer un modèle de mise en page incluant Planning.
   <p>Les zones Planning sont activées par défaut pour les utilisateurs standard et les administrateurs système.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>-->

## Remarques concernant l’utilisation des vues d’enregistrement

* Les vues dans Workfront Planning sont spécifiques au type d’enregistrement. Vous ne pouvez pas appliquer la même vue à deux types d’enregistrements différents.
* Les vues que vous créez sont visibles uniquement par vous et les personnes avec lesquelles vous les partagez.
* Lorsque vous modifiez ou supprimez une vue, elle est modifiée et supprimée pour toutes les personnes disposant d’autorisations sur la vue.
* Chaque utilisateur peut créer un maximum de 100 vues. Vous pouvez afficher plus de 100 vues pour un type d’enregistrement, mais un utilisateur ne peut créer que 100 vues.
* Bien que certains éléments de vue puissent être appliqués à plusieurs vues pour le même enregistrement, ils sont propres à chaque vue d’enregistrement :

   * Filtre
   * Tri (pour la vue Tableau)
   * Couleurs des lignes (pour la vue Tableau)
   * Champs (pour la vue Tableau)
   * Répartition (pour la vue Chronologie)
   * Regroupement (pour les vues Tableau et Chronologie)
   * Apparence des barres (pour les vues Chronologie et Calendrier)
   * Hauteur de ligne (pour le tableau et la vue Calendrier mensuelle)

  Par exemple, lors de la création d’un filtre dans une vue Tableau, les résultats du filtre sont visibles uniquement dans la vue sélectionnée (vue Tableau) et pas dans toutes les vues associées au type d’enregistrement.

  >[!TIP]
  >
  >Certains éléments de vue ne sont pas disponibles pour toutes les vues.


## Similarités et différences entre les vues d’enregistrement

Le tableau suivant présente les similitudes et les différences entre les vues de tableau, chronologique et de calendrier :

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Fonctionnalité | Vue de tableau | Vue chronologique | Vue de calendrier | Vue Liste |
|-----------------------------------------------------------------------|------------|---------------|--------------|---------|
| Afficher les enregistrements sous forme de tableau | ✓ |              | | ✓ |
| Afficher tous les champs sous forme de colonnes dans un tableau ou une liste | ✓ |              |    | ✓ |
| Masquer ou afficher des champs (ou des colonnes) | ✓ |               |    | ✓ |
| Modifier les valeurs de champ de chaque enregistrement | ✓ |               |             | ✓ |
| Ajouter des enregistrements en tant que nouvelles lignes dans la vue | ✓ |               |        | ✓ |
| Ajouter des champs en tant que nouvelles colonnes dans la vue | ✓ |               |         | ✓ |
| Copier des lignes d’une liste externe et les coller dans un tableau | ✓ |               |          | ✓ |
| Afficher des enregistrements dans une chronologie |            | ✓ |             |  |
| Filtrer des enregistrements | ✓ | ✓ | ✓ | ✓ |
| Afficher des enregistrements sur un calendrier |           |              | ✓ |  |
| Regrouper les enregistrements | ✓ | ✓ |  |  |
| Trier les enregistrements | ✓ |              |  | ✓ |
| Attribuer des couleurs aux enregistrements | ✓ | ✓ | ✓ |  |
| Attribuer des couleurs aux regroupements |           | ✓ |  |  |
| Rechercher des enregistrements spécifiques | ✓ | ✓ |  | ✓ |
| Partager la vue avec d&#39;autres personnes | ✓ | ✓ | ✓ | ✓ |
| Ouvrir la page de l’enregistrement à partir de la vue. | ✓ | ✓ |    | ✓ |
| Afficher les enregistrements par année et par trimestre |           | ✓ |    |  |
| Afficher les enregistrements par mois |           | ✓ | ✓ |  |
| Afficher les enregistrements par semaine |           |               | ✓ |  |
| Exporter les informations d’une vue | ✓ |               |    |  |
| Afficher en plein écran | ✓ | ✓ | ✓ |  |
| Créer des enregistrements dans la vue | ✓ | ✓ | ✓ | ✓ |
| Répartir les enregistrements en fonction de leurs connexions |          | ✓ |    |  |

## Créer ou modifier des vues {#create-or-edit-views}

Les informations de cette section s&#39;appliquent aux types d&#39;affichage suivants :

* Tableau
* Journal
* Calendrier

Pour plus d’informations sur les vues Liste, voir [Gérer la vue Liste](/help/quicksilver/planning/views/manage-the-list-view.md).

{{step1-to-planning}}


1. Cliquez sur la vignette d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.

   Par défaut, tous les enregistrements du type sélectionné s’affichent dans la vue tableau.

1. Cliquez sur l’icône déroulante ![Icône déroulante](assets/drop-down-icon.png) en regard du nom de la vue actuelle, puis cliquez sur **+Nouvelle vue**.

1. Choisissez parmi les types de vues suivants :

   * Tableau
   * Journal
   * Calendrier

1. Choisissez un type de vue, puis cliquez sur **Créer**. Une nouvelle vue est ajoutée au menu déroulant.

   >[!TIP]
   >
   >Lorsque vous créez un type d’enregistrement, la vue de tableau est également créée par défaut.
   >
   >Pour créer une vue de calendrier ou de chronologie, le type d’enregistrement pour lequel vous créez la vue doit comporter au moins deux champs de date.
   >
   >Dans le cas contraire, les options Chronologie et Calendrier sont grisées.
   >  

   ![Créer une zone de vue](assets/create-view-box.png)

1. (Facultatif) Pour modifier une vue existante, cliquez sur le menu déroulant situé à droite du nom de la vue actuelle, puis tapez le nom d&#39;une vue dans le champ **Rechercher** et appuyez sur la touche Entrée du clavier.
1. (Facultatif) Dans le menu déroulant Affichage , faites glisser et déposez les vues dans l’ordre de votre préférence.

   ![Liste déroulante Afficher les types de la liste des types d’enregistrement](assets/view-types-drop-down-from-record-type-list.png)

1. (Le cas échéant) Cliquez sur **Suivant** lors de la création d’une vue chronologique ou de calendrier.

   Par défaut, Workfront donne à la vue l’un des noms suivants :

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Le nombre est un incrément généré automatiquement.

1. (Le cas échéant) Sélectionnez les **dates de début** et **de fin** pour les enregistrements qui s’afficheront dans la vue chronologique ou de calendrier.

   >[!NOTE]
   >
   >    Vous pouvez effectuer un choix parmi les champs de date d’enregistrement ou les champs de date de recherche parmi les types d’objet ou d’enregistrement connectés.
   >
   >Vous devez utiliser des agrégateurs pour les champs de date (MAX ou MIN) lorsque vous sélectionnez des champs de recherche lors de la connexion des types d’enregistrements. Seul l’ajout des agrégateurs vous permet d’utiliser les dates des connexions comme dates de début et de fin pour les vues chronologique et Calendrier.
   >
   >Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Cliquez sur **Créer**.

   La vue s’affiche dans un nouvel onglet. Les vues s’affichent dans l’ordre chronologique à partir du moment où elles ont été créées ou partagées avec vous.
1. (Facultatif) Cliquez sur le menu **Plus** ![Autres vues d’icône en forme de flèche vers le bas](assets/more-caret-down-icon-views.png) en regard de la dernière vue pour afficher toutes les vues pour le type d’enregistrement sélectionné.

   D’autres vues s’affichent dans le menu **Plus** après le dernier onglet de vue. Le numéro en regard du menu **Plus** affiche le nombre de vues supplémentaires.
1. (Facultatif) Pour renommer une vue après sa création, cliquez sur le menu déroulant de la vue, puis sur le menu **Plus** ![Menu Plus](assets/more-menu.png) > **Renommer** pour mettre à jour le nom de la vue

   Ou

   Double-cliquez sur le nom de la vue et commencez à saisir le nouveau nom. <!--ensure there is not another saving step here?!-->

1. (Facultatif) Cliquez sur l’icône **Plein écran** ![Icône Ouvrir le plein écran](assets/open-full-screen-icon.png) pour ouvrir un affichage en plein écran, puis sur l’icône **Quitter le plein écran** ![Icône Quitter le plein écran](assets/exit-full-screen-icon.png) ou sur la touche Échap du clavier pour quitter le plein écran.

1. (Facultatif) Pour gérer un type de vue spécifique, consultez les articles suivants :

   * [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Gérer la vue de calendrier](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## Activation de l&#39;indicateur de présence en temps réel dans une vue

Vous pouvez voir si d’autres utilisateurs modifient des enregistrements en même temps que vous en suivant les indicateurs de présence en temps réel dans la vue.

>[!NOTE]
>
>Vous ne pouvez pas afficher les indicateurs de présence en temps réel dans une vue Liste.

Par défaut, les avatars d’autres utilisateurs qui modifient les informations d’enregistrement en même temps que vous s’affichent dans le coin supérieur droit de toutes les vues d’enregistrement.

Lorsque vous affichez la vue Tableau, vous pouvez également voir quel champ un autre utilisateur est en train de modifier au moment où vous affichez l’enregistrement.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).



<!--## Add a view as a favorite - this is not possible yet-->
