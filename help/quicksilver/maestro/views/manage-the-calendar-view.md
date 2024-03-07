---
title: Gestion de la vue Calendrier
description: Vous pouvez afficher les enregistrements et leurs champs en mode Calendrier.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ff52e43fc5ed5a7939b9e28b2bda195e94e81724
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Gestion de la vue Calendrier

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

{{maestro-important-intro}}

Vous pouvez afficher les enregistrements et leurs champs dans une vue de calendrier, à partir de la page de type enregistrement.

Pour plus d’informations sur les vues Maestro et leur gestion, voir [Gestion des vues d’enregistrement](../views/manage-record-views.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé Adobe Maestro. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Quelconque</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Quelconque</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Configuration du niveau d’accès</td>
   <td> <p>Il n’existe pas de contrôle de niveau d’accès pour Maestro </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations pour l’affichage</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modèle de mise en page</td>
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## Gestion de la vue Calendrier {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Tenez compte des points suivants :

* Vous ne pouvez créer une vue Calendrier que si au moins deux champs de date sont associés à un type d’enregistrement. Lorsqu’un ou plusieurs champs de date sont associés à un type d’enregistrement, l’option Mode Calendrier est grisée.
* Les scénarios suivants :

   * Lorsque les dates de début et de fin ne comportent aucune valeur, les enregistrements ne s’affichent pas dans le calendrier.
   * Lorsque les dates de début ou de fin n’ont aucune valeur, l’enregistrement s’affiche sous la forme d’un événement d’un jour.
   * Lorsque la date de début est postérieure à la date de fin, l’enregistrement ne s’affiche pas dans le calendrier.

Pour gérer une vue de calendrier :

1. Accédez à la page de type enregistrement pour laquelle vous souhaitez afficher le calendrier.
1. Créez une vue Calendrier, comme décrit dans l’article [Gestion des vues d’enregistrement](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   Les enregistrements associés au type d’enregistrement que vous avez sélectionné s’affichent sous forme de barres dans un calendrier.

1. Pour parcourir le calendrier, effectuez l’une des opérations suivantes :

   * Cliquez sur les icônes de gauche et de droite ou utilisez le défilement horizontal pour passer d’un calendrier à l’autre.
   * Cliquez sur **Aujourd&#39;hui** pour centrer le calendrier sur la date du jour.
   * Sélectionnez l’une des options suivantes dans le menu déroulant de la période pour mettre à jour les incréments de temps :

      * Mois