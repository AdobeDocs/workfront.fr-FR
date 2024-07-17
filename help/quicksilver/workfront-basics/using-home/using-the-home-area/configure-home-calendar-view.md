---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Configurer les paramètres d’affichage du calendrier de l’accueil
description: Vous pouvez configurer les paramètres du calendrier d’accueil pour les intégrer à une version Web d’Outlook et vous aider à suivre votre charge de travail par rapport à vos heures de travail disponibles.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 5%

---

# Configuration des paramètres de la vue [!UICONTROL Calendrier d’accueil]

<!--Audited: 01/2024-->

Vous pouvez configurer les paramètres [!UICONTROL Home Calendar] pour effectuer les opérations suivantes :

* Effectuer l’intégration à une version web d’[!DNL Outlook] dans [!DNL Office 365] hébergé dans le cloud ou [!DNL Outlook Live]. Vous pouvez afficher tous les événements de votre calendrier Outlook et les calendriers associés que vous sélectionnez dans votre [!UICONTROL calendrier d’accueil] dans Adobe Workfront.
* Vous aider à suivre votre charge de travail par rapport à vos heures de travail disponibles sur la barre [!UICONTROL Affectation].

Pour en savoir plus sur le calendrier d’accueil, consultez la [[!UICONTROL vue Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

Cet article décrit comment configurer les paramètres du calendrier d’accueil et intégrer le calendrier d’accueil à votre calendrier Outlook externe.

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> 
   Ou
   <p>Nouvelle : [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur [!DNL Workfront]. Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## A propos de l&#39;intégration de [!DNL Microsoft Outlook] calendriers

Tenez compte des points suivants lorsque vous configurez votre calendrier d’accueil avec votre calendrier [!DNL Microsoft Outlook] :

* Vous pouvez intégrer uniquement une version web de [!DNL Outlook] dans le cloud [!DNL Office 365] ou [!DNL Outlook Live] hébergé.

  Sur site [!DNL Outlook] et [!DNL Outlook] sur un serveur d’entreprise [!DNL Exchange] basé sur le cloud ne sont pas pris en charge.

  Si votre entreprise utilise l’authentification unique, vous avez besoin de [!DNL Microsoft 365 E3] ou de [!DNL E5].

* Les pièces jointes associées à vos événements [!DNL Outlook] ne sont pas jointes aux événements [!DNL Outlook] de votre calendrier d’accueil.
* L’intégration à un calendrier [!DNL Outlook] doit être effectuée individuellement pour chaque utilisateur.
* Les événements qui apparaissent dans la barre [!UICONTROL Échéance] n’apparaissent pas sur votre calendrier [!DNL Microsoft], sauf si vous les avez déplacés de la [!UICONTROL liste de travail] vers votre calendrier [!DNL Adobe Workfront]. Pour plus d’informations, voir [[!UICONTROL due] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) et [liste de travail sur le [!UICONTROL calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) dans la [[!UICONTROL vue Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Lorsque vous activez l’intégration avec [!DNL Outlook], seules les tâches qui sont glissées sur le [!UICONTROL calendrier d’accueil] à partir de ce moment-là se synchronisent. Les éléments qui se trouvaient sur le calendrier d’accueil avant d’activer l’intégration n’apparaîtront pas et vous devez les faire glisser de nouveau sur le calendrier d’accueil si vous souhaitez qu’ils apparaissent dans [!DNL Outlook].
* Lorsque vous partagez (ou annulez le partage) un calendrier [!DNL Outlook] avec d’autres personnes, ou lorsque vous modifiez le niveau d’autorisation d’un calendrier que vous partagez avec d’autres personnes, cette modification n’a aucune incidence sur leurs calendriers pendant environ 30 minutes. Pour plus d&#39;informations, consultez la documentation [!DNL Microsoft Outlook].\
   Par conséquent, lorsque vous intégrez le calendrier [!DNL Workfront] à un calendrier [!DNL Outlook] que vous partagez avec d’autres utilisateurs, vos éléments de calendrier [!DNL Workfront] ne s’affichent pas pendant environ 30 minutes.

>[!NOTE]
>
>La configuration du calendrier [!DNL Outlook] est complètement distincte du module complémentaire [!DNL Outlook] ([!UICONTROL [!DNL Outlook] Intégration] ou [!DNL Workfront Outlook]). Aucune installation n’est requise pour configurer le calendrier, mais une installation est nécessaire pour le module complémentaire [!DNL Outlook]. Pour plus d’informations sur le [!DNL Outlook] module complémentaire, voir [Configuration [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configurez vos paramètres d’affichage [!UICONTROL Calendrier d’accueil] et intégrez-les aux calendriers Outlook

1. Dans la vue [!UICONTROL  Home Calendar], cliquez sur l’icône d’engrenage **[!UICONTROL Settings]** ![Calendar_Settings_engrenage_icon.png](assets/calendar-settings-gear-icon.png) dans le coin supérieur droit pour ouvrir le panneau **[!UICONTROL Calendar settings]** sur la droite.

   Si vous avez besoin d’informations sur l’accès à la vue [!UICONTROL Home Calendar], voir [Affichage du [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Facultatif) Pour intégrer votre calendrier [!DNL Microsoft Outlook], cliquez sur **[!UICONTROL Ajouter un compte]** dans le coin supérieur droit du panneau **[!UICONTROL Paramètres du calendrier]**. Ensuite, si vous êtes invité à le faire, saisissez vos informations de connexion [!DNL Microsoft Outlook]. Vous pouvez répéter cette étape pour ajouter plusieurs comptes [!DNL Outlook].

   >[!NOTE]
   >
   >Vous devez autoriser [!DNL Workfront] à accéder à votre calendrier [!DNL Outlook]. L&#39;attribution d&#39;une autorisation permet à [!DNL Workfront] de conserver l&#39;accès aux données du calendrier, de lire votre profil [!DNL outlook] et de lire et de mettre à jour votre calendrier [!DNL Microsoft].

1. Actualisez la fenêtre du navigateur pour afficher les informations de votre compte [!DNL Outlook] dans le calendrier et dans le panneau [!UICONTROL Paramètres du calendrier].
1. Cliquez à nouveau sur l’icône d’engrenage **[!UICONTROL Settings]** dans le coin supérieur droit pour ouvrir le panneau **[!UICONTROL Calendar settings]** . ![Calendar_Settings_engrenage_icon.png](assets/calendar-settings-gear-icon.png)

1. (Facultatif) Sous chaque compte [!DNL Microsoft] que vous avez ajouté à l’étape précédente, sélectionnez **[!UICONTROL Afficher]** ou **[!UICONTROL Synchroniser]** :

   * **[!UICONTROL Affichage]** : il s’agit d’une option en lecture seule qui affiche [!DNL Microsoft] événements de calendrier sur votre [!UICONTROL  calendrier d’accueil ].
   * **[!UICONTROL Synchronisation]** : cette option permet une synchronisation bidirectionnelle entre vos calendriers [!DNL Microsoft] et [!UICONTROL Accueil]. En d’autres termes, les éléments [!DNL Workfront] [!UICONTROL Calendrier d’accueil] sont exportés vers votre calendrier [!DNL Microsoft] et les éléments de calendrier [!DNL Microsoft] sont importés dans votre [!UICONTROL Calendrier d’accueil] Workfront en temps réel.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Facultatif) Sous votre compte [!DNL Workfront] ou un compte intégré, sélectionnez les calendriers associés à afficher dans le [!UICONTROL calendrier d’accueil] (comme votre calendrier PTO, Anniversaire ou Jours fériés), puis cliquez sur le bouton [!UICONTROL Actualiser] ou [!UICONTROL Recharger] de votre navigateur pour afficher vos modifications.

1. (Facultatif) Dans la section **[!UICONTROL Général]** sous **[!UICONTROL Semaine de début le]**, sélectionnez le jour que vous souhaitez afficher comme premier jour de la semaine de travail dans le calendrier d’accueil.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configurez les options suivantes :

   * **[!UICONTROL Mes jours de travail] :** sélectionnez les jours de travail.
   * **[!UICONTROL Mon heure de début habituelle] :** sélectionnez l’heure à laquelle vous commencez votre journée de travail.
   * **[!UICONTROL Mon heure de fin habituelle] :** sélectionnez l’heure à laquelle vous mettez fin à votre journée de travail.

   [!DNL Workfront] utilise ces trois paramètres pour calculer le nombre d’heures que vous travaillez au cours d’une semaine. Ce nombre affecte la barre [!UICONTROL Affectation], qui vous aide à suivre votre charge de travail par rapport à vos heures de travail disponibles. Pour plus d’informations, voir [[!UICONTROL Affectation] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) dans l’article [[!UICONTROL Vue Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Cliquez en dehors de la zone **[!UICONTROL Paramètres du calendrier]** pour la fermer.

   [!DNL Workfront] enregistre automatiquement vos modifications.

Pour plus d’informations sur l’utilisation de la vue [!UICONTROL Calendar] pour gérer vos affectations de travail et vos événements de calendrier intégrés, voir [ Utilisation de la vue [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
