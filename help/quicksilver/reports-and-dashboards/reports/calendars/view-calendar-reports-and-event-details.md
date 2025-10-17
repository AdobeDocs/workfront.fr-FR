---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Affichage des rapports de calendrier et des détails sur les événements
description: Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou qui ont été partagés avec vous dans Adobe Workfront.
author: Jenny
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 73%

---

# Afficher des rapports de calendrier et des détails de l’événement

Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou qui ont été partagés avec vous dans Adobe Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Contributeur</p>
       <p>Demande</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès supérieur ou égal à Rapports, Tableaux de bord et Calendriers</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations d’affichage ou supérieures pour le rapport de calendrier</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher un rapport de calendrier

<!--{{step1-to-calendars}}-->

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Calendriers]**.

   Selon votre niveau d’accès, vous pouvez voir les calendriers suivants répertoriés :

   * Votre calendrier de [!DNL Adobe Workfront] par défaut

     Workfront crée pour vous un calendrier en fonction des projets, tâches et problèmes qui vous sont attribués ou qui sont attribués à des équipes, des groupes ou des rôles qui vous sont affectés.

   * Calendriers que vous avez créés

     Pour en savoir plus sur la création de calendriers, voir [Vue d’ensemble des rapports de calendrier](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendriers que d’autres utilisateurs ont partagés avec vous

     Pour en savoir plus sur le partage de calendriers, voir [[!UICONTROL Partager un rapport] de calendrier](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Le cas échéant) Cliquez sur le bouton **[!UICONTROL Vue]**, puis sélectionnez la durée du calendrier à afficher.
   ![Durée du calendrier](assets/view-menu-calendar-report-350x189.png)
Vous pouvez choisir parmi les vues de rapports de calendrier suivantes :

   * **[!UICONTROL Mois]** : affiche quatre semaines du calendrier.
   * **[!UICONTROL Semaine]** : affiche une semaine du calendrier.
   * **[!UICONTROL Gantt]** : affiche une vue continue du calendrier

     Vous pouvez afficher davantage d’événements dans une vue **Gantt** en faisant défiler l’écran vers le bas ou sur le côté. Un symbole de chargement s’affiche lorsque des données sont renseignées pour la vue.

   >[!NOTE]
   >
   >Dans les vues **Mois** et **Semaine**, les événements actuels ou futurs (y compris les événements qui s’étendent sur plusieurs jours, à condition qu’ils contiennent le jour actuel ou un jour futur) ont un ombrage correspondant à la couleur du projet ou du regroupement de calendrier. Les événements passés ont un ombrage plus clair pour indiquer qu’ils ne sont plus actuels, mais vous pouvez toujours sélectionner et afficher ces événements.

1. (Facultatif) Si vous affichez le calendrier dans les vues **Mois** ou **Semaine**, vous pouvez modifier la vue du calendrier à l’aide des options suivantes :

   <!--   * To include or exclude weekends:
      1. On the **[!UICONTROL Calendar]** toolbar, click **[!UICONTROL Calendar Actions]**, then from the drop-down list select either **[!UICONTROL Show Weekend]** or **[!UICONTROL Hide Weekend]**.-->

   * Pour modifier rapidement les dates affichées, procédez comme suit :

      1. Dans la barre d’outils **[!UICONTROL Calendrier]**, cliquez sur la flèche gauche de l’indicateur de date pour revenir en arrière dans le calendrier ou sur la flèche droite pour avancer.

         ![Clic sur la flèche pour modifier la date](assets/click-arrows-to-change-dates-calendar-report.png)

         Les dates affichées sont ajustées selon un intervalle en fonction de votre vue Calendrier actuelle. Par exemple, si vous affichez le calendrier dans la vue **Semaine**, le calendrier affiche une semaine en avant ou une semaine en arrière, selon la flèche que vous sélectionnez.

      1. (Facultatif) Pour revenir au jour en cours, cliquez sur [!UICONTROL **Aujourd’hui**].

1. (Facultatif) Pour masquer les événements d’un regroupement de projets ou de calendriers lié au calendrier, désélectionnez-le regroupement dans la liste des projets.
   ![Masquer les événements](assets/hide-events-for-project-or-cal-grouping.png)
Vous pouvez rendre à nouveau les événements visibles en sélectionnant le regroupement [!UICONTROL projet] ou calendrier dans la liste des projets.

## Afficher des rapports de calendrier et des détails de l’événement

Vous pouvez afficher les détails d’un événement dans un calendrier, pour les événements passés et en cours.

1. Accédez à l’événement dont vous souhaitez connaître les détails, puis cliquez sur l’événement. Les détails s’ouvrent dans un panneau sur le côté droit.
1. (Facultatif) Pour ouvrir le projet, la tâche ou le problème associé, cliquez sur le titre de l’objet.
