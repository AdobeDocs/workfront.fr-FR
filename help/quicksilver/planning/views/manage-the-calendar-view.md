---
title: Gérer la vue de calendrier
description: Vous pouvez afficher les enregistrements et leurs champs en mode Calendrier.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 27%

---

# Gérer la vue de calendrier

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Vous pouvez afficher les enregistrements et leurs champs dans une vue de calendrier, à partir de la page de type enregistrement.

Pour plus d’informations sur les vues de planification Adobe Workfront et sur la façon de les gérer, voir [Gestion des vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
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
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Nouvelle : standard</p>
   Ou
   <p>Actuelle : formule </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> Il n’existe aucun contrôle d’accès pour Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Autorisations de gestion d’une vue</p>  
   <p>Afficher les autorisations d’une vue pour modifier temporairement les paramètres d’affichage</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Vue d’ensemble des accès</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Gestion de la vue Calendrier {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Tenez compte des points suivants :

* Vous ne pouvez créer une vue Calendrier que si au moins deux champs de date sont associés à un type d’enregistrement. Lorsqu’un ou plusieurs champs de date sont associés à un type d’enregistrement, l’option Mode Calendrier est grisée.

  Vous pouvez sélectionner des champs de date d’enregistrement ou des champs de date de recherche à partir des types d’enregistrement ou d’objet connectés.
* Les scénarios suivants sont possibles :

   * Lorsque les dates de Début et de Fin n&#39;ont aucune valeur, les enregistrements ne s&#39;affichent pas dans le calendrier.
   * Lorsque les dates de début ou de fin n’ont aucune valeur, l’enregistrement s’affiche sous la forme d’un événement d’un jour.
   * Lorsque la date de début est postérieure à la date de fin, l&#39;enregistrement ne s&#39;affiche pas dans le calendrier.

Pour gérer une vue de calendrier :

1. Accédez à la page de type enregistrement pour laquelle vous souhaitez afficher le calendrier.
1. Créez une vue Calendrier, comme décrit dans l’article [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   Les enregistrements associés au type d’enregistrement que vous avez sélectionné s’affichent sous forme de barres dans un calendrier. La couleur des barres correspond à celle de l’icône d’enregistrement.

1. Pour parcourir le calendrier, effectuez l’une des opérations suivantes :

   * Cliquez sur les icônes de gauche et de droite ou utilisez le défilement horizontal pour passer d’un calendrier à l’autre.
   * Cliquez sur **Aujourd’hui** pour centrer le calendrier sur la date d’aujourd’hui.
   * Sélectionnez l’une des options suivantes dans le menu déroulant de la période pour mettre à jour les incréments de temps :

      * Mois
1. Mettez à jour les éléments de vue suivants comme décrit dans les sous-sections ci-dessous :
   * [Filtres](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Ajouter des filtres

Tirez part ides filtres pour réduire la quantité d’informations affichées à l’écran.

Tenez compte des points suivants lorsque vous utilisez des filtres dans la vue Calendrier :

<!-- this list is almost identical to the one for the table view - update both-->

* Les filtres que vous créez pour une vue Calendrier fonctionnent indépendamment des filtres de toute autre vue appliquée au même type d’enregistrement.

* Les filtres sont propres à la vue que vous sélectionnez. Deux vues calendaires du même type d&#39;enregistrement peuvent faire l&#39;objet de filtres différents.

* Deux utilisateurs qui consultent la même vue de calendrier voient le même filtre actuellement appliqué.

* Vous ne pouvez pas nommer les filtres que vous créez pour une vue Calendrier.

* La suppression d’un filtre le supprime pour toute personne accédant au même type d’enregistrement que vous et qui affiche la même vue que vous.

* L’ajout de filtres dans la vue Calendrier est identique à l’ajout de filtres dans la vue Tableau.

  Pour plus d’informations, consultez la section « Ajouter des filtres » de l’article [Gérer la vue de tableau](/help/quicksilver/planning/views/manage-the-table-view.md).

* Vous pouvez filtrer par champ d’enregistrement ou champ de recherche connecté.

* Vous pouvez filtrer par champs de recherche qui affichent plusieurs valeurs.
