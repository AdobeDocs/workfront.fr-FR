---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Configurer les paramètres de la vue Calendrier d’accueil
description: Vous pouvez configurer les paramètres du calendrier d’accueil pour les intégrer à une version web d’Outlook et vous aider à suivre votre charge de travail par rapport à vos heures de travail disponibles.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 100%

---

# Configurer les paramètres de la vue [!UICONTROL Calendrier d’accueil]

<!--Audited: 01/2024-->

Vous pouvez configurer les paramètres du [!UICONTROL Calendrier d’accueil] pour effectuer les opéations suivantes :

* Effectuer l’intégration à une version web d’[!DNL Outlook] dans [!DNL Office 365] hébergé dans le cloud ou [!DNL Outlook Live]. Vous pouvez afficher tous les événements de votre calendrier Outlook et les calendriers associés que vous sélectionnez dans votre [!UICONTROL Calendrier d’accueil] dans Adobe Workfront.
* Suivez plus facilement votre charge de travail par rapport à vos heures de travail disponibles dans la barre [!UICONTROL Allocation].

Pour en savoir plus sur le calendrier d’accueil, voir [[!UICONTROL Vue Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

Cet article décrit comment configurer les paramètres du calendrier d’accueil et l’intégrer à votre calendrier Outlook externe.

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
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>Actuelle : [!UICONTROL Work] ou niveau supérieur</p> 
   Ou
   <p>Nouvelle : [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

* Pour connaître le plan ou le type de licence dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront]. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## À propos de l’intégration de calendriers [!DNL Microsoft Outlook]

Tenez compte des points suivants lorsque vous configurez votre calendrier d’accueil avec votre calendrier [!DNL Microsoft Outlook] :

* Vous pouvez effectuer l’intégration à une version web d’[!DNL Outlook] dans [!DNL Office 365] hébergé dans le cloud ou à [!DNL Outlook Live].

  [!DNL Outlook] On-Premise et [!DNL Outlook] sur un serveur [!DNL Exchange] d’entreprise cloud ne sont pas pris en charge.

  Si votre entreprise utilise l’authentification unique, vous avez besoin de [!DNL Microsoft 365 E3] ou [!DNL E5].

* Les pièces jointes associées à vos événements [!DNL Outlook] ne sont pas jointes aux événements [!DNL Outlook] dans votre calendrier d’accueil.
* Intégration avec un calendrier [!DNL Outlook] effectuée individuellement pour chaque utilisateur ou utilisatrice.
* Les événements qui apparaissent dans la barre [!UICONTROL Échéance] n’apparaissent pas dans votre calendrier [!DNL Microsoft], sauf si vous les avez déplacés depuis la [!UICONTROL Liste de travail] vers votre calendrier [!DNL Adobe Workfront]. Pour plus d’informations, voir [[!UICONTROL Barre Échéance]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) et [Liste de travail dans le [!UICONTROL Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) dans la vue [[!UICONTROL Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Lorsque vous activez l’intégration avec [!DNL Outlook], seuls les éléments de travail qui ont été déplacés vers le [!UICONTROL Calendrier d’accueil] à partir de ce moment se synchroniseront. Les éléments qui se trouvaient sur le calendrier d’accueil avant d’activer l’intégration ne s’affichent pas. Vous devez les faire glisser à nouveau sur le calendrier d’accueil si vous souhaitez qu’ils apparaissent dans [!DNL Outlook].
* Lorsque vous partagez (ou annulez le partage) un calendrier [!DNL Outlook] avec d’autres personnes ou lorsque vous modifiez le niveau d’autorisation d’un calendrier que vous partagez avec d’autres personnes, cette modification n’a aucune incidence sur leurs calendriers pendant environ 30 minutes. Pour plus d’informations, consultez la documentation [!DNL Microsoft Outlook].\
   Par conséquent, lorsque vous intégrez un calendrier [!DNL Workfront] avec un calendrier [!DNL Outlook] que vous partagez avec d’autres personnes, elles ne verront pas vos éléments de calendrier [!DNL Workfront] pendant environ 30 minutes.

>[!NOTE]
>
>La configuration du calendrier [!DNL Outlook] est complètement différente du module complémentaire [!DNL Outlook] (Intégration [!UICONTROL [!DNL Outlook]] ou [!DNL Workfront Outlook]). Aucune installation n’est nécessaire pour configurer le calendrier, mais une installation est nécessaire pour le module complémentaire [!DNL Outlook]. Pour plus d’informations sur le module complémentaire [!DNL Outlook], voir [Configurer  [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configurer les paramètres de la vue [!UICONTROL Calendrier d’accueil] et les intégrer aux calendriers Outlook

1. Dans la vue [!UICONTROL Calendrier d’accueil], cliquez sur l’icône d’engrenage **[!UICONTROL Paramètres]** ![Calendar_Settings_engr_icon.png](assets/calendar-settings-gear-icon.png) dans le coin supérieur droit pour ouvrir le panneau **[!UICONTROL Paramètres du calendrier]** sur la droite.

   Si vous avez besoin d’informations sur l’accès à la vue [!UICONTROL Calendrier d’accueil], voir [Afficher le [!UICONTROL Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Facultatif) Pour intégrer votre calendrier [!DNL Microsoft Outlook], cliquez sur **[!UICONTROL Ajouter un compte]** dans le coin supérieur droit du panneau **[!UICONTROL Paramètres du calendrier]**. Ensuite, si on vous le demande, saisissez vos informations de connexion [!DNL Microsoft Outlook]. Vous pouvez répéter cette étape pour ajouter plusieurs comptes [!DNL Outlook].

   >[!NOTE]
   >
   >Vous devez donner l’autorisation [!DNL Workfront] pour accéder à votre calendrier [!DNL Outlook]. Accorder l’autorisation permet à [!DNL Workfront] de conserver l’accès aux données du calendrier, de lire votre profil [!DNL outlook] et de lire et mettre à jour votre calendrier [!DNL Microsoft].

1. Actualisez la fenêtre du navigateur pour afficher les informations de votre compte [!DNL Outlook] dans le calendrier et dans le panneau [!UICONTROL Paramètres du calendrier].
1. Cliquez à nouveau sur l’icône d’engrenage **[!UICONTROL Paramètres]** dans le coin supérieur droit pour ouvrir le panneau **[!UICONTROL Paramètres du calendrier]**. ![Calendar_Settings_engr_icon.png](assets/calendar-settings-gear-icon.png)

1. (Facultatif) Sous chaque compte [!DNL Microsoft] ajouté à l’étape précédente, sélectionnez **[!UICONTROL Afficher]** ou **[!UICONTROL Synchroniser]** :

   * **[!UICONTROL Afficher]** : il s’agit d’une option en lecture seule qui affiche les événements du calendrier [!DNL Microsoft] sur votre [!UICONTROL Calendrier d’accueil].
   * **[!UICONTROL Synchroniser]** : cette option permet une synchronisation bidirectionnelle entre votre calendrier [!DNL Microsoft] et votre [!UICONTROL Calendrier d’accueil]. En d’autres termes, les éléments du [!UICONTROL Calendrier d’accueil] [!DNL Workfront] s’exportent vers votre calendrier [!DNL Microsoft] et les éléments du calendrier [!DNL Microsoft] s’importent dans le [!UICONTROL Calendrier d’accueil] Workfront en temps réel.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Facultatif) Sous votre compte [!DNL Workfront] ou un compte intégré, sélectionnez les calendriers associés à afficher dans votre [!UICONTROL Calendrier d’accueil] (comme votre calendrier de congés payés, d’anniversaire ou de congés), puis cliquez sur le bouton [!UICONTROL Actualiser] ou [!UICONTROL Recharger] pour consulter vos modifications.

1. (Facultatif) Dans la section **[!UICONTROL Général]** sous **[!UICONTROL Démarrer la semaine le]**, sélectionnez le jour que vous souhaitez afficher comme premier jour de la semaine de travail dans le calendrier d’accueil.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configurez les options suivantes :

   * **[!UICONTROL Mes jours ouvrables] :** sélectionnez les jours où vous travaillez.
   * **[!UICONTROL Mon heure de début habituelle] :** sélectionnez l’heure à laquelle vous commencez votre journée de travail.
   * **[!UICONTROL Mon heure de fin habituelle] :** sélectionnez l’heure à laquelle vous terminez votre journée de travail.

   [!DNL Workfront] utilise ces trois paramètres pour calculer le nombre d’heures que vous effectuez au cours d’une semaine. Ce nombre affecte la barre [!UICONTROL Allocation] qui vous aide à suivre votre charge de travail par rapport à vos heures de travail disponibles. Pour plus d’informations, voir la barre [[!UICONTROL Allocation] ](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) dans l’article [[!UICONTROL vue du calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Cliquez en dehors de la zone **[!UICONTROL Paramètres du calendrier]** pour la fermer.

   [!DNL Workfront] enregistre automatiquement vos modifications.

Pour plus d’informations sur l’utilisation de la vue [!UICONTROL Calendrier] pour gérer vos affectations de travail et les événements de calendrier intégrés, voir [Utiliser la vue [!UICONTROL Calendrier d’accueil]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
