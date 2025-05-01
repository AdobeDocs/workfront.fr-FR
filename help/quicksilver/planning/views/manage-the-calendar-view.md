---
title: Gérer la vue de calendrier
description: Vous pouvez afficher les enregistrements et leurs champs dans une vue Calendrier. Cet article décrit comment créer une vue de calendrier et modifier ou supprimer une vue existante.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 22%

---

# Gérer la vue de calendrier

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Vous pouvez afficher les enregistrements et leurs champs dans une vue Calendrier, à partir de la page Type d’enregistrement.

Pour plus d’informations sur les vues Adobe Workfront Planning et leur gestion, voir [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

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
   <p>Autorisations d’affichage d’une vue pour modifier temporairement les paramètres d’affichage</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut Planning.</p>
<p><span class="preview">Dans l’environnement de Prévisualisation, les utilisateurs et utilisatrices standard et les administrateurs et administratrices système ont Planning activé par défaut.</span></p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gérer une vue Calendrier {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Tenez compte des points suivants :

* Vous ne pouvez créer une vue Calendrier que si au moins deux champs de date sont associés à un type d’enregistrement. Lorsqu’un type d’enregistrement est associé à un ou à aucun champ de date, l’option Vue Calendrier est grisée.

  Vous pouvez effectuer un choix parmi les champs de date d’enregistrement ou les champs de date de recherche parmi les types d’objet ou d’enregistrement connectés.
* Les scénarios suivants sont possibles :

   * Lorsque les dates de début et de fin ne comportent aucune valeur, les enregistrements ne s’affichent pas dans le calendrier
   * Lorsque les dates de début et de fin n’ont aucune valeur, l’enregistrement s’affiche sous la forme d’un événement d’un jour
   * Lorsque la date de début est postérieure à la date de fin, l&#39;enregistrement ne s&#39;affiche pas dans le calendrier.

Pour gérer une vue Calendrier :

1. Accédez à la page de type d’enregistrement pour laquelle vous souhaitez afficher le calendrier.
1. Créez une vue Calendrier, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   ![Exemple de vue Calendrier](assets/calendar-view-example.png)

   Les enregistrements associés au type d&#39;enregistrement que vous avez sélectionné s&#39;affichent sous forme de barres dans un calendrier. La couleur des barres correspond à celle de l’icône d’enregistrement.

1. Effectuez l’une des opérations suivantes pour parcourir le calendrier :

   * Cliquez sur les icônes de gauche et de droite ou utilisez le défilement horizontal pour vous déplacer dans le calendrier.
   * Cliquez sur **Aujourd&#39;hui** pour centrer le calendrier sur la date d&#39;aujourd&#39;hui.
   * Sélectionnez l’une des options suivantes dans le menu déroulant de la période pour mettre à jour les incréments de temps :

      * **Mois** : les enregistrements s’affichent dans un calendrier mensuel.


      * **Semaine** : les enregistrements s’affichent dans les zones suivantes :

         * Les enregistrements qui s&#39;étendent sur plusieurs jours s&#39;affichent en haut du calendrier.
         * Les enregistrements d&#39;une durée inférieure ou égale à un jour s&#39;affichent dans la moitié inférieure de la vue Calendrier. Si vous avez choisi d&#39;afficher l&#39;heure des dates de début et de fin, l&#39;enregistrement s&#39;affiche à l&#39;heure appropriée dans la journée où il se produit.


1. Mettez à jour les éléments de vues suivants, comme décrit dans les sous-sections ci-dessous :
   * [Filtres](#add-filters)
   * [Paramètres](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Ajouter des filtres

Vous pouvez réduire la quantité d’informations affichées à l’écran en utilisant des filtres.

Tenez compte des points suivants lorsque vous utilisez des filtres dans la vue Calendrier :

<!-- this list is almost identical to the one for the table view - update both-->

* Les filtres que vous créez pour une vue Calendrier fonctionnent indépendamment des filtres de toute autre vue appliquée au même type d&#39;enregistrement.

* Les filtres sont propres à la vue que vous sélectionnez. Des filtres différents peuvent être appliqués à deux vues de calendrier du même type d’enregistrement.

* Deux utilisateurs qui consultent le même affichage Calendrier verront le même filtre qui est actuellement appliqué.

* Vous ne pouvez pas nommer les filtres que vous créez pour une vue Calendrier.

* En supprimant les filtres, vous les supprimez pour toutes les personnes qui accèdent au même type d’enregistrement que vous et qui consultent la même vue que vous.

* L’ajout de filtres dans la vue Calendrier est identique à l’ajout de filtres dans la vue Tableau.

  Pour plus d’informations, consultez la section « Ajout de filtres » dans l’article [Gestion de la vue tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

* Vous pouvez filtrer par champs d’enregistrement connectés ou champs de recherche.

* Vous pouvez filtrer par champs de recherche qui affichent plusieurs valeurs.

### Modifier les paramètres de la vue Calendrier

La modification des paramètres de la vue Calendrier est similaire à la modification des paramètres d’une vue Chronologie.

Pour plus d’informations, consultez la section « Modifier les paramètres de la vue chronologique » de l’article [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).
