---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Afficher les rapports de calendrier et les détails des événements
description: Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou qui ont été partagés avec vous dans Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
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
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Contributeur</p>
       <p>Demande</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Affichage ou accès supérieur aux rapports, tableaux de bord et calendriers</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Afficher ou des autorisations supérieures pour le rapport de calendrier</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher un rapport de calendrier

<!--{{step1-to-calendars}}-->

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Calendriers]**.

   Selon votre niveau d’accès, vous pouvez voir les calendriers suivants répertoriés :

   * Votre calendrier [!DNL Adobe Workfront] par défaut

     Workfront crée pour vous un calendrier en fonction des projets, tâches et problèmes qui vous sont attribués ou qui sont attribués à des équipes, des groupes ou des rôles qui vous sont affectés.

   * Calendriers que vous avez créés

     Pour en savoir plus sur la création de calendriers, voir [Vue d’ensemble des rapports de calendrier](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendriers que d&#39;autres utilisateurs ont partagés avec vous

     Pour en savoir plus sur le partage de calendriers, voir [[!UICONTROL Partager un rapport] de calendrier](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Le cas échéant) Cliquez sur le bouton **[!UICONTROL Vue]**, puis sélectionnez la durée du calendrier à afficher.
   ![Durée du calendrier](assets/view-menu-calendar-report-350x189.png)
Vous avez le choix entre les vues de rapport de calendrier suivantes :

   * **[!UICONTROL Mois]** : affiche quatre semaines du calendrier.
   * **[!UICONTROL Semaine]** : affiche une semaine du calendrier.
   * **[!UICONTROL Gantt]** : affiche une vue continue du calendrier

     Vous pouvez voir plus d&#39;événements dans une vue **Gantt** en faisant défiler vers le bas ou latéralement. Un symbole de chargement s’affiche lorsque des données sont renseignées pour la vue.

   >[!NOTE]
   >
   >Dans les vues **Mois** et **Semaine**, les événements actuels ou futurs (y compris les événements qui s’étendent sur plusieurs jours, à condition qu’ils contiennent le jour actuel ou un jour futur) ont un ombrage correspondant à la couleur du projet ou du regroupement de calendrier. Les événements passés ont un ombrage plus clair pour indiquer qu’ils ne sont plus actuels, mais vous pouvez toujours sélectionner et afficher ces événements.

1. (Facultatif) Si vous affichez le calendrier dans les vues **Mois** ou **Semaine**, vous pouvez modifier la vue du calendrier à l’aide des options suivantes :

   <!--   * To include or exclude weekends:
      1. On the **[!UICONTROL Calendar]** toolbar, click **[!UICONTROL Calendar Actions]**, then from the drop-down list select either **[!UICONTROL Show Weekend]** or **[!UICONTROL Hide Weekend]**.-->

   * Pour modifier rapidement les dates affichées, procédez comme suit :

      1. Dans la barre d&#39;outils **[!UICONTROL Calendrier]**, cliquez sur la flèche gauche de l&#39;indicateur de date pour revenir dans le calendrier ou sur la flèche droite pour avancer.

         ![Clic sur la flèche pour modifier la date](assets/click-arrows-to-change-dates-calendar-report.png)

         Les dates affichées sont ajustées selon un intervalle en fonction de votre vue Calendrier actuelle. Par exemple, si vous affichez le calendrier dans la vue **Semaine**, le calendrier affiche une semaine en avant ou une semaine en arrière, selon la flèche que vous sélectionnez.

      1. (Facultatif) Pour revenir au jour actuel, cliquez sur [!UICONTROL **Aujourd&#39;hui**].

1. (Facultatif) Pour masquer les événements d’un regroupement de projets ou de calendriers lié au calendrier, désélectionnez-le regroupement dans la liste des projets.
   ![Masquer les événements](assets/hide-events-for-project-or-cal-grouping.png)
Vous pouvez rendre les événements visibles à nouveau en sélectionnant le [!UICONTROL projet] ou le regroupement de calendriers dans la liste des projets.

## Afficher des rapports de calendrier et des détails de l’événement

Vous pouvez afficher les détails d’un événement dans un calendrier, pour les événements passés et en cours.

1. Accédez à l’événement dont vous souhaitez connaître les détails, puis cliquez sur l’événement. Les détails s’ouvrent dans un panneau sur le côté droit.
1. (Facultatif) Pour ouvrir le projet, la tâche ou le problème associé, cliquez sur le titre de l’objet.
