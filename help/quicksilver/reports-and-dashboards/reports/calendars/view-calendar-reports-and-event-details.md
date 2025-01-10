---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Affichage des rapports de calendrier et des détails sur les événements
description: Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou qui ont été partagés avec vous dans Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: d90459cb4f6fb1960552f0ab174e963582312b5c
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 78%

---

# Afficher des rapports de calendrier et des détails de l’événement

Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou qui ont été partagés avec vous dans Adobe Workfront.

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
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouveau : contributeur</p>
       <p>ou</p>
       <p>Actuel : demande</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>[!UICONTROL View] ou un accès supérieur à [!UICONTROL Reports], [!UICONTROL Dashboards] et [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations [!UICONTROL View] ou de niveau supérieur au rapport de calendrier</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher un rapport de calendrier

{{step1-to-calendars}}

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

     ![[!UICONTROL Gantt] rapport de calendrier](assets/gantt-calendar-report.png)

     Vous pouvez afficher davantage d’événements dans une vue [!UICONTROL Gantt] en faisant défiler l’écran vers le bas ou sur le côté. Un symbole de chargement s’affiche lorsque des données sont renseignées pour la vue.

   >[!NOTE]
   >
   >Dans les vues [!UICONTROL Mois] et [!UICONTROL Semaine], les événements actuels ou futurs (y compris les événements qui s’étendent sur plusieurs jours, à condition qu’ils contiennent le jour actuel ou un jour futur) ont un ombrage correspondant à la couleur du projet ou du regroupement de calendrier. Les événements passés ont un ombrage plus clair pour indiquer qu’ils ne sont plus actuels, mais vous pouvez toujours sélectionner et afficher ces événements.

1. (Facultatif) Si vous affichez le calendrier dans les vues [!UICONTROL Mois] ou [!UICONTROL Semaine], vous pouvez modifier la vue du calendrier à l’aide des options suivantes :

   * Pour inclure ou exclure les week-ends, procédez comme suit :

      1. Sur la barre d’outils **[!UICONTROL Calendrier]**, cliquez sur **[!UICONTROL Actions du calendrier]**, puis, dans la liste déroulante, sélectionnez **[!UICONTROL Afficher le week-end]** ou **[!UICONTROL Masquer le week-end]**.

   * Pour modifier rapidement les dates affichées, procédez comme suit :

      1. Dans la barre d’outils **[!UICONTROL Calendrier]**, cliquez sur la flèche gauche de l’indicateur de date pour revenir en arrière dans le calendrier ou sur la flèche droite pour avancer.

         ![Clic sur la flèche pour modifier la date](assets/click-arrows-to-change-dates-calendar-report.png)\
         Les dates affichées sont ajustées selon un intervalle en fonction de votre vue Calendrier actuelle. Par exemple, si vous affichez le calendrier dans la vue [!UICONTROL Semaine], le calendrier affiche une semaine en avant ou une semaine en arrière, selon la flèche que vous sélectionnez.

      1. (Facultatif) Pour revenir au jour en cours, cliquez sur [!UICONTROL **Aujourd’hui**].


1. (Facultatif) Pour afficher un calendrier en plein écran, cliquez sur les flèches du mode plein écran situées dans la partie droite de la barre d’outils **[!UICONTROL Calendrier]**.
   ![Clic sur la flèche pour modifier la date](assets/click-arrows-to-change-dates-calendar-report.png)\
   Appuyez sur Échap pour revenir à la vue normale du calendrier.

1. (Facultatif) Pour masquer les événements d’un regroupement de projets ou de calendriers lié au calendrier, désélectionnez-le regroupement dans la liste des projets.
   ![Masquer les événements](assets/hide-events-for-project-or-cal-grouping.png)
Vous pouvez rendre à nouveau les événements visibles en sélectionnant le regroupement [!UICONTROL projet] ou calendrier dans la liste des projets.

## Afficher des rapports de calendrier et des détails de l’événement

Vous pouvez afficher les détails d’un événement dans un calendrier, pour les événements passés et en cours.

1. Accédez à l’événement dont vous souhaitez connaître les détails, puis cliquez sur l’événement.
Une page de détails de l’événement s’ouvre.
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (Facultatif) Pour afficher des détails supplémentaires sur l’objet :

   1. Pointez sur le projet, la tâche ou le nom du problème.

      Une page de détails s’ouvre pour l’objet.
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (Facultatif) Pour ouvrir le projet, la tâche ou le problème associé, cliquez sur le titre de l’objet.
   1. (Facultatif) Pour fermer toutes les pages de détails ouvertes, cliquez n’importe où en dehors des pages de détails de l’événement.
