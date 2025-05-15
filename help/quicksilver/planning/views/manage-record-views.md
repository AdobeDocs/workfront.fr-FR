---
title: Gérer les vues d’enregistrement
description: Vous pouvez afficher les enregistrements dans une vue Tableau, Chronologie ou Calendrier lors de l'utilisation d'Adobe Workfront Planning. Cet article décrit comment créer une vue et modifier une vue existante.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: eb3db3b056cea359f77e56f77d6e9520954e2abb
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 47%

---


# Gérer les vues d’enregistrement

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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
* [Activer les indicateurs de présence en temps réel dans une vue](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Pour plus d’informations sur la gestion des vues d’enregistrement Workfront Planning, consultez également les articles suivants :

* [Supprimer les vues d’enregistrement](/help/quicksilver/planning/views/delete-record-views.md)
* [Dupliquer les vues d’enregistrement](/help/quicksilver/planning/views/duplicate-record-views.md)
* [Partager des affichages](/help/quicksilver/planning/access/share-views.md)


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
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
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
   <p>Autorisations d’affichage d’une vue pour modifier temporairement les paramètres d’affichage ou la dupliquer</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut Planning.</p>
<p><span class="preview">Dans l’environnement de Prévisualisation, les utilisateurs et utilisatrices standard et les administrateurs et administratrices système ont Planning activé par défaut.</span></p></td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant l’utilisation des vues d’enregistrement

* Les vues dans Workfront Planning sont spécifiques au type d’enregistrement. Vous ne pouvez pas appliquer la même vue à deux types d’enregistrements différents.
* Les vues que vous créez sont visibles uniquement par vous et les personnes avec lesquelles vous les partagez.
* Lorsque vous modifiez ou supprimez une vue, elle est modifiée et supprimée pour toutes les personnes disposant d’autorisations sur la vue.
* Chaque utilisateur peut créer un maximum de 100 vues. Vous pouvez afficher plus de 100 vues pour un type d’enregistrement, mais un utilisateur ne peut créer que 100 vues.
* Bien que certains éléments de vue puissent être appliqués à plusieurs vues pour le même enregistrement, ils sont propres à chaque vue d’enregistrement :

   * Filtre
   * Regroupement (pour les vues Tableau et Chronologie)
   * Apparence des barres (pour les vues Chronologie et Calendrier)

  Par exemple, lors de la création d’un filtre dans une vue Tableau, les résultats du filtre sont visibles uniquement dans la vue sélectionnée (vue Tableau) et pas dans toutes les vues associées au type d’enregistrement.

  >[!TIP]
  >
  >Certains éléments de vue ne sont pas disponibles pour toutes les vues.


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
| Filtrer des enregistrements | ✓ | ✓ | ✓ |
| Afficher des enregistrements sur un calendrier |           |              | ✓ |
| Regrouper les enregistrements | ✓ | ✓ |
| Trier les enregistrements | ✓ |              |
| <span class="preview">Enregistrements de code couleur</span> | <span class="preview">✓</span> | ✓ | ✓ |
| Attribuer des couleurs aux regroupements |           | ✓ |
| Rechercher des enregistrements spécifiques | ✓ | ✓ |
| Partager la vue avec d&#39;autres personnes | ✓ | ✓ | ✓ |
| Ouvrir la page de l’enregistrement à partir de la vue. | ✓ | ✓ |    |
| Afficher les enregistrements par année et par trimestre |           | ✓ |    |
| Afficher les enregistrements par mois |           | ✓ | ✓ |
| Afficher les enregistrements par semaine |           |               | ✓ |
| <span class="preview">Exporter des informations depuis une vue</span> | <span class="preview">✓</span> |               |    |


## Créer ou modifier des vues {#create-or-edit-views}

{{step1-to-planning}}


1. Cliquez sur la vignette d’un espace de travail.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails.

   La page de type d’enregistrement s’ouvre.

   Par défaut, tous les enregistrements du type sélectionné s&#39;affichent dans la vue de tableau.

1. Cliquez sur **+ Affichage** pour ajouter une nouvelle vue.
1. Choisissez parmi les types de vues suivants :

   * Tableau
   * Journal
   * Calendrier

   Un nouvel onglet est créé avec la vue sélectionnée.

   Selon la largeur de l’écran, d’autres vues peuvent s’afficher dans le menu **Plus** ![Plus](assets/more-menu.png).


>[!TIP]
>
>Lorsque vous créez un type d’enregistrement, la vue de tableau est également créée par défaut.
>
>Pour créer une vue de calendrier ou de chronologie, le type d’enregistrement pour lequel vous créez la vue doit comporter au moins deux champs de date.
>
>Dans le cas contraire, les options Chronologie et Calendrier sont grisées.
>

![Liste déroulante Afficher les types de la liste des types d’enregistrement](assets/view-types-drop-down-from-record-type-list.png)

1. (Le cas échéant) Cliquez sur **Suivant** lors de la création d’une vue chronologique ou de calendrier.

   Par défaut, Workfront donne à la vue l’un des noms suivants :

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Le nombre est un incrément généré automatiquement.

1. (Le cas échéant) Sélectionnez les **dates de début** et **de fin** pour les enregistrements qui s’afficheront dans la vue chronologique ou de calendrier.

   >[!TIP]
   >
   >    Vous pouvez effectuer un choix parmi les champs de date d’enregistrement ou les champs de date de recherche parmi les types d’objet ou d’enregistrement connectés. Vous devez utiliser des agrégateurs pour les champs de date (MAX ou MIN) lorsque vous sélectionnez des champs de recherche comme dates de début et de fin pour les vues chronologique et Calendrier. Pour plus d’informations, consultez la section [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Cliquez sur **Créer**.

   La vue s’affiche dans un nouvel onglet. Les vues s’affichent dans l’ordre chronologique à partir du moment où elles ont été créées ou partagées avec vous.
1. (Facultatif) Cliquez sur le menu **Plus** ![Autres vues d’icône en forme de flèche vers le bas](assets/more-caret-down-icon-views.png) en regard de la dernière vue pour afficher toutes les vues pour le type d’enregistrement sélectionné.

   D’autres vues s’affichent dans le menu **Plus** après le dernier onglet de vue. Le numéro en regard du menu **Plus** affiche le nombre de vues supplémentaires.
1. (Facultatif) Pour renommer une vue après sa création, cliquez sur le menu déroulant de la vue, puis sur le menu **Plus** ![Menu Plus](assets/more-menu.png) > **Renommer** pour mettre à jour le nom de la vue

   Ou

   Double-cliquez sur le nom de la vue et commencez à saisir le nouveau nom. <!--ensure there is not another saving step here?!-->

1. (Facultatif) Pour gérer un type de vue spécifique, consultez les articles suivants :

   * [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Gérer la vue de calendrier](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## Activation de l&#39;indicateur de présence en temps réel dans une vue

Vous pouvez voir si d’autres utilisateurs modifient des enregistrements en même temps que vous en suivant les indicateurs de présence en temps réel dans la vue.

Par défaut, les avatars d’autres utilisateurs qui modifient les informations d’enregistrement en même temps que vous s’affichent dans le coin supérieur droit de toutes les vues d’enregistrement.

Lorsque vous affichez la vue Tableau, vous pouvez également voir quel champ un autre utilisateur est en train de modifier au moment où vous affichez l’enregistrement.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).



<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->
