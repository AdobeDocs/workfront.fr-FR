---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Configuration des paramètres de la vue Calendrier d’accueil
description: Vous pouvez configurer les paramètres du calendrier d’accueil pour les intégrer à une version Web d’Outlook et vous aider à suivre votre charge de travail par rapport à vos heures de travail disponibles.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 3b3ba7cc6a975af71205f7f524e1a9a91a9d3810
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Configurez vos [!UICONTROL Calendrier d’accueil] paramètres d’affichage

<!--Audited: 01/2024-->

Vous pouvez configurer la variable [!UICONTROL Calendrier d’accueil] pour effectuer les opérations suivantes :

* Intégration à une version web d’ [!DNL Outlook] dans le cloud hébergé [!DNL Office 365] ou [!DNL Outlook Live]. Vous pouvez afficher tous les événements de votre calendrier Outlook et les calendriers associés que vous sélectionnez dans votre [!UICONTROL Calendrier d’accueil] dans Adobe Workfront.
* vous aider à effectuer le suivi de votre charge de travail par rapport à vos heures de travail disponibles sur la [!UICONTROL Affectation] de la barre

Pour en savoir plus sur le calendrier d’accueil, voir [[!UICONTROL Calendrier d’accueil] view](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

Cet article décrit comment configurer les paramètres du calendrier d’accueil et intégrer le calendrier d’accueil à votre calendrier Outlook externe.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Actuel : [!UICONTROL Travail] ou version ultérieure</p> 
   Ou
   <p>Nouveau : [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*Pour savoir quel plan ou type de licence vous disposez, contactez votre [!DNL Workfront] administrateur. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## A propos de l&#39;intégration [!DNL Microsoft Outlook] calendriers

Tenez compte des points suivants lorsque vous configurez votre calendrier d’accueil avec votre [!DNL Microsoft Outlook] calendar :

* Vous ne pouvez intégrer qu’une version web de [!DNL Outlook] dans le cloud hébergé [!DNL Office 365] ou [!DNL Outlook Live].

  On-premise [!DNL Outlook] et [!DNL Outlook] sur une entreprise cloud [!DNL Exchange] ne sont pas pris en charge.

  Si votre entreprise utilise l’authentification unique, vous devez [!DNL Microsoft 365 E3] ou [!DNL E5].

* Pièces jointes associées à vos [!DNL Outlook] Les événements ne sont pas associés à la variable [!DNL Outlook] événements dans votre calendrier d’accueil.
* Intégration avec une [!DNL Outlook] Le calendrier doit être renseigné individuellement pour chaque utilisateur.
* Événements qui apparaissent dans la variable [!UICONTROL Échéance] n’apparaît pas sur votre [!DNL Microsoft] calendrier , sauf si vous les avez déplacés depuis [!UICONTROL Liste de tâches] à votre [!DNL Adobe Workfront] Calendrier. Pour plus d’informations, voir [[!UICONTROL Échéance] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) et [Liste de travail sur la [!UICONTROL Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL Calendrier d’accueil] view](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Lorsque vous activez l’intégration avec [!DNL Outlook], uniquement les tâches qui sont glissées sur le [!UICONTROL Calendrier d’accueil] à partir de ce moment, se synchronisera. Les éléments qui se trouvaient sur le calendrier d’accueil avant d’activer l’intégration ne s’affichent pas. Vous devez les faire glisser à nouveau sur le calendrier d’accueil si vous souhaitez qu’ils apparaissent dans [!DNL Outlook].
* Lorsque vous partagez (ou annulez le partage) une [!DNL Outlook] calendrier avec d’autres personnes ou lorsque vous modifiez le niveau d’autorisation d’un calendrier que vous partagez avec d’autres personnes, cette modification n’a aucune incidence sur leurs calendriers pendant environ 30 minutes. Pour plus d’informations, consultez la [!DNL Microsoft Outlook] la documentation.\
   Par conséquent, lorsque vous intégrez [!DNL Workfront] Calendrier avec un [!DNL Outlook] calendrier que vous partagez avec d’autres utilisateurs, il ne verra pas vos [!DNL Workfront] Calendrier des éléments pendant environ 30 minutes.

>[!NOTE]
>
>La variable [!DNL Outlook] la configuration du calendrier est complètement différente de [!DNL Outlook] Module complémentaire ([!UICONTROL [!DNL Outlook] Intégration] ou [!DNL Workfront Outlook]). Aucune installation n’est nécessaire pour configurer le calendrier, mais une installation est nécessaire pour que la variable [!DNL Outlook] Module complémentaire. Pour plus d’informations sur la variable [!DNL Outlook] Pour plus d’informations, voir [Configuration [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configurez vos [!UICONTROL Calendrier d’accueil] afficher les paramètres et les intégrer aux calendriers Outlook ;

1. Dans le [!UICONTROL Calendrier d’accueil] , cliquez sur le bouton **[!UICONTROL Paramètres]** icône d’engrenage ![Calendar_Settings_engr_icon.png](assets/calendar-settings-gear-icon.png) dans le coin supérieur droit pour ouvrir le **[!UICONTROL Paramètres du calendrier]** sur la droite.

   Si vous avez besoin d’informations sur l’accès au [!UICONTROL Calendrier d’accueil] vue, voir [Afficher la variable [!UICONTROL Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Facultatif) Pour intégrer votre [!DNL Microsoft Outlook] calendrier, cliquez sur **[!UICONTROL Ajouter un compte]** dans le coin supérieur droit du **[!UICONTROL Paramètres du calendrier]** du panneau. Ensuite, si vous êtes invité à le faire, saisissez votre [!DNL Microsoft Outlook] informations de connexion. Vous pouvez répéter cette étape pour ajouter plusieurs [!DNL Outlook] comptes.

   >[!NOTE]
   >
   >Vous devez donner [!DNL Workfront] l’autorisation d’accéder à [!DNL Outlook] calendrier. Octroi d’autorisations [!DNL Workfront] pour conserver l’accès aux données du calendrier, lisez votre [!DNL outlook] et lisez et mettez à jour votre [!DNL Microsoft] calendrier.

1. Actualisez la fenêtre du navigateur pour afficher les informations de votre [!DNL Outlook] dans le calendrier et dans la variable [!UICONTROL Paramètres du calendrier] du panneau.
1. Cliquez sur le bouton **[!UICONTROL Paramètres]** icône d’engrenage à nouveau dans le coin supérieur droit pour ouvrir la **[!UICONTROL Paramètres du calendrier]** du panneau. ![Calendar_Settings_engr_icon.png](assets/calendar-settings-gear-icon.png)

1. (Facultatif) Sous chaque [!DNL Microsoft] compte ajouté à l’étape précédente, sélectionnez **[!UICONTROL Affichage]** ou **[!UICONTROL Synchronisation]**:

   * **[!UICONTROL Affichage]**: il s’agit d’une option en lecture seule qui affiche [!DNL Microsoft] événements du calendrier sur votre [!UICONTROL Calendrier d’accueil].
   * **[!UICONTROL Synchronisation]**: cette option permet une synchronisation bidirectionnelle entre votre [!DNL Microsoft] et [!UICONTROL Accueil] les calendriers. En d&#39;autres termes, [!DNL Workfront] [!UICONTROL Calendrier d’accueil] d’éléments à exporter vers votre [!DNL Microsoft] calendrier et [!DNL Microsoft] importation des éléments du calendrier dans Workfront [!UICONTROL Calendrier d’accueil] en temps réel.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Facultatif) Sous [!DNL Workfront] , ou un compte intégré, sélectionnez les calendriers associés à afficher dans votre [!UICONTROL Calendrier d’accueil] (comme votre calendrier PTO, Anniversaire ou Jours fériés), puis cliquez sur le [!UICONTROL Actualiser] ou [!UICONTROL Recharger] pour afficher vos modifications.

1. (Facultatif) Dans la variable **[!UICONTROL Général]** section sous **[!UICONTROL Commencer la semaine]**, sélectionnez le jour que vous souhaitez afficher comme premier jour de la semaine de travail dans le calendrier d’accueil.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configurez les options suivantes :

   * **[!UICONTROL Mes journées de travail]:** Sélectionnez les jours de travail.
   * **[!UICONTROL Mon heure de début habituelle]:** Sélectionnez l’heure à laquelle vous commencez votre journée de travail.
   * **[!UICONTROL Mon heure de fin habituelle]:** Sélectionnez l’heure à laquelle vous mettez fin à votre journée de travail.

   [!DNL Workfront] utilise ces trois paramètres pour calculer le nombre d’heures que vous travaillez au cours d’une semaine. Ce nombre affecte le [!UICONTROL Affectation] qui vous aide à suivre votre charge de travail par rapport à vos heures de travail disponibles. Pour plus d’informations, voir [[!UICONTROL Affectation] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) dans l’article [[!UICONTROL Calendrier d’accueil] view](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Cliquez en dehors du **[!UICONTROL Paramètres du calendrier]** pour la fermer.

   [!DNL Workfront] enregistre automatiquement vos modifications.

Pour plus d’informations sur l’utilisation de la variable [!UICONTROL Calendrier] pour afficher la gestion de vos affectations de travail et des événements de calendrier intégrés, voir [Utilisez la variable [!UICONTROL Calendrier d’accueil] view](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
