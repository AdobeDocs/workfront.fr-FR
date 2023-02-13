---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Affichage des rapports de calendrier et des détails sur les événements
description: Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou que vous avez partagés avec vous dans Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 0%

---

# Affichage des rapports de calendrier et des détails sur les événements

Vous pouvez afficher les rapports de calendrier et les détails des événements que vous avez créés ou que vous avez partagés avec vous dans Adobe Workfront.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur à [!UICONTROL Reports], [!UICONTROL Tableaux de bord] et [!UICONTROL Calendriers]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations d’[!UICONTROL Affichage] ou supérieures au rapport Calendrier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Affichage d’un rapport de calendrier

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Calendriers]**.

   Selon votre niveau d’accès, vous pouvez voir les calendriers suivants répertoriés :

   * Votre valeur par défaut [!DNL Adobe Workfront] calendar\

      Workfront crée pour vous un calendrier en fonction des projets, tâches et problèmes qui vous sont affectés ou qui sont affectés à des équipes, des groupes ou des rôles auxquels vous êtes affecté.
   * Calendriers que vous avez créés\

      Pour en savoir plus sur la création de calendriers, voir [Présentation des rapports sur les calendriers](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendriers que d’autres utilisateurs ont partagés avec vous\

      Pour en savoir plus sur le partage de calendriers, voir [[!UICONTROL Partage d’un calendrier] rapport](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Conditionnel) Cliquez sur le bouton **[!UICONTROL Affichage]** , puis sélectionnez la durée du calendrier à afficher.\
   ![Durée du calendrier](assets/view-menu-calendar-report-350x189.png)\
   Vous pouvez choisir parmi les vues de rapports de calendrier suivantes :

   * **[!UICONTROL Mois]**: Affiche quatre semaines du calendrier
   * **[!UICONTROL Semaine]**: Affiche une semaine du calendrier
   * **[!UICONTROL Gantt]**: Affiche une vue continue du calendrier\

      ![[!UICONTROL Gantt] rapport de calendrier](assets/gantt-calendar-report.png)
Vous pouvez voir d’autres événements dans une [!UICONTROL Gantt] en faisant défiler la page vers le bas ou vers le bas. Un symbole de chargement s’affiche lorsque des données sont renseignées pour la vue.
   >[!NOTE]
   >
   >Dans le [!UICONTROL Mois] et [!UICONTROL Semaine] vues, événements actuels ou futurs (y compris les événements qui s’étendent sur plusieurs jours, à condition qu’ils contiennent aujourd’hui ou un jour futur) ont un ombrage correspondant à la couleur du projet ou du regroupement de calendrier. Les événements passés ont un ombrage plus clair pour indiquer qu’ils ne sont plus en cours, mais vous pouvez toujours sélectionner et afficher ces événements.

1. (Facultatif) Si vous affichez le calendrier dans la variable [!UICONTROL Mois] ou [!UICONTROL Semaine] vous pouvez modifier la vue Calendrier à l’aide des options suivantes :

   * Pour inclure ou exclure les week-ends :

      1. Sur le **[!UICONTROL Calendrier]** barre d’outils, cliquez sur **[!UICONTROL Actions du calendrier]**, puis, dans la liste déroulante, sélectionnez l’une des options suivantes : **[!UICONTROL Afficher le week-end]** ou **[!UICONTROL Masquer le week-end]**.
   * Pour modifier rapidement les dates affichées :

      1. Sur le **[!UICONTROL Calendrier]** cliquez sur la flèche gauche de l’indicateur de date pour revenir au calendrier ou sur la flèche droite pour avancer.\

         ![Cliquez sur la flèche pour modifier la date](assets/click-arrows-to-change-dates-calendar-report.png)\
         Les dates affichées sont ajustées selon un intervalle en fonction de votre vue Calendrier actuelle. Par exemple, si vous affichez le calendrier dans la variable [!UICONTROL Semaine] le calendrier affiche une semaine en avant ou une semaine en arrière, selon la flèche que vous sélectionnez.

      1. (Facultatif) Pour revenir au jour en cours, cliquez sur **Today**.


1. (Facultatif) Pour afficher un calendrier en plein écran, cliquez sur les flèches du mode Plein écran situées dans la partie droite du **[!UICONTROL Calendrier]** de la barre d’outils.
   ![Cliquez sur la flèche pour modifier la date](assets/click-arrows-to-change-dates-calendar-report.png)\
   Appuyez sur Échap pour revenir à la vue normale du calendrier.

1. (Facultatif) Pour masquer les événements d’un projet ou d’un groupe de calendrier lié au calendrier, désélectionnez le groupe de projet ou de calendrier dans la liste des projets.
   ![Masquer les événements](assets/hide-events-for-project-or-cal-grouping.png)\
   Vous pouvez rendre les événements visibles à nouveau en sélectionnant l’option [!UICONTROL project] ou regroupement calendaire dans la liste des projets.

## Affichage des détails d’un événement de rapport de calendrier

Vous pouvez afficher les détails d’un événement dans un calendrier, pour les événements en cours et précédents.

1. Accédez à l’événement pour lequel vous souhaitez connaître les détails, puis cliquez sur l’événement .\
   Une page de détails de l’événement s’ouvre.\
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (Facultatif) Pour afficher des détails supplémentaires sur l’objet :

   1. Passez la souris sur le projet, la tâche ou le nom du problème.

      Une page de détails s’ouvre pour l’objet.\
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (Facultatif) Pour ouvrir le projet, la tâche ou le problème associé, cliquez sur le titre de l’objet.
   1. (Facultatif) Pour fermer toutes les pages de détails ouvertes, cliquez n’importe où en dehors des pages de détails de l’événement.
