---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Afficher des rapports de calendrier et des détails de l’événement
description: Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou qui ont été partagés avec vous dans Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 100%

---

# Afficher des rapports de calendrier et des détails de l’événement

Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou qui ont été partagés avec vous dans Adobe Workfront.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Accès [!UICONTROL View] ou de niveau supérieur aux [!UICONTROL Reports], [!UICONTROL Dashboards] et [!UICONTROL Calendars]</p> <p>Remarque : si vous n’avez toujours pas accès, demandez à votre administrateur ou à votre administratrice [!DNL Workfront] si des restrictions supplémentaires ont été définies pour votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations [!UICONTROL View] ou de niveau supérieur au rapport de calendrier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou votre administratrice [!DNL Workfront].

## Afficher un rapport de calendrier

1. Cliquez sur l’icône **[!UICONTROL Menu principal]**![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Calendriers]**.

   Selon votre niveau d’accès, vous pouvez voir les calendriers suivants répertoriés :

   * Votre calendrier [!DNL Adobe Workfront] par défaut

     Workfront crée pour vous un calendrier en fonction des projets, tâches et problèmes qui vous sont attribués ou qui sont attribués à des équipes, des groupes ou des rôles qui vous sont affectés.
   * Calendriers que vous avez créés.

     Pour en savoir plus sur la création de calendriers, voir [Vue d’ensemble des rapports de calendrier](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendriers que d’autres personnes ont partagés avec vous.

     Pour en savoir plus sur le partage de calendriers, voir [[!UICONTROL Partager un rapport] de calendrier](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Le cas échéant) Cliquez sur le bouton **[!UICONTROL Vue]**, puis sélectionnez la durée du calendrier à afficher.\
   ![Durée du calendrier](assets/view-menu-calendar-report-350x189.png)\
   Vous pouvez choisir parmi les vues de rapports de calendrier suivantes :

   * **[!UICONTROL Mois]** : affiche quatre semaines du calendrier.
   * **[!UICONTROL Semaine]** : affiche une semaine du calendrier.
   * **[!UICONTROL Gantt]** : affiche une vue continue du calendrier.

     Rapport de calendrier ![[!UICONTROL Gantt]](assets/gantt-calendar-report.png)
Vous pouvez voir d’autres événements dans une vue [!UICONTROL Gantt] en faisant défiler la page vers le bas ou sur les côtés. Un symbole de chargement s’affiche lorsque des données sont renseignées pour la vue.
   >[!NOTE]
   >
   >Dans les vues [!UICONTROL Mois] et [!UICONTROL Semaine], les événements actuels ou futurs (y compris les événements qui s’étendent sur plusieurs jours, à condition qu’ils contiennent le jour actuel ou un jour futur) ont un ombrage correspondant à la couleur du projet ou du regroupement de calendrier. Les événements passés ont un ombrage plus clair pour indiquer qu’ils ne sont plus actuels, mais vous pouvez toujours sélectionner et afficher ces événements.

1. (Facultatif) Si vous affichez le calendrier dans les vues [!UICONTROL Mois] ou [!UICONTROL Semaine], vous pouvez modifier la vue du calendrier à l’aide des options suivantes :

   * Pour inclure ou exclure les week-ends, procédez comme suit :

      1. Sur la barre d’outils **[!UICONTROL Calendrier]**, cliquez sur **[!UICONTROL Actions du calendrier]**, puis, dans la liste déroulante, sélectionnez **[!UICONTROL Afficher le week-end]** ou **[!UICONTROL Masquer le week-end]**.
   * Pour modifier rapidement les dates affichées, procédez comme suit :

      1. Sur la barre d’outils **[!UICONTROL Calendrier]** cliquez sur la flèche gauche de l’indicateur de date pour reculer dans le temps ou sur la flèche droite pour avancer.

         ![Clic sur la flèche pour modifier la date](assets/click-arrows-to-change-dates-calendar-report.png)\
         Les dates affichées sont ajustées selon un intervalle en fonction de votre vue Calendrier actuelle. Par exemple, si vous affichez le calendrier dans la vue [!UICONTROL Semaine], le calendrier affiche une semaine en avant ou une semaine en arrière, selon la flèche que vous sélectionnez.

      1. (Facultatif) Pour revenir au jour actuel, cliquez sur **Aujourd’hui**.


1. (Facultatif) Pour afficher un calendrier en plein écran, cliquez sur les flèches du mode plein écran situées dans la partie droite de la barre d’outils **[!UICONTROL Calendrier]**.
   ![Clic sur la flèche pour modifier la date](assets/click-arrows-to-change-dates-calendar-report.png)\
   Appuyez sur Échap pour revenir à la vue normale du calendrier.

1. (Facultatif) Pour masquer les événements d’un regroupement de projets ou de calendriers lié au calendrier, désélectionnez-le regroupement dans la liste des projets.
   ![Masquer les événements](assets/hide-events-for-project-or-cal-grouping.png)\
   Vous pouvez rendre les événements visibles à nouveau en sélectionnant le [!UICONTROL projet] ou regroupement de calendriers dans la liste des projets.

## Afficher des rapports de calendrier et des détails de l’événement

Vous pouvez afficher les détails d’un événement dans un calendrier, pour les événements passés et en cours.

1. Accédez à l’événement dont vous souhaitez connaître les détails, puis cliquez dessus.\
   Une page de détails de l’événement s’ouvre.\
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (Facultatif) Pour afficher des détails supplémentaires sur l’objet :

   1. Pointez sur le projet, la tâche ou le nom du problème.

      Une page de détails s’ouvre pour l’objet.\
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (Facultatif) Pour ouvrir le projet, la tâche ou le problème associé, cliquez sur le titre de l’objet.
   1. (Facultatif) Pour fermer toutes les pages de détails ouvertes, cliquez n’importe où en dehors des pages de détails de l’événement.
