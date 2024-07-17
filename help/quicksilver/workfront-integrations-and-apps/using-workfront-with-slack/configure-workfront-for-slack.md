---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configurer [!DNL Adobe Workfront] pour le Slack
description: L'intégration de  [!DNL Adobe Workfront]  avec Slack vous permet d'accéder aux  [!DNL Workfront] tâches, approbations, favoris, éléments récents de Slack et d'en créer.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 4%

---

# Configurer [!DNL Adobe Workfront for Slack]

L&#39;intégration de [!DNL Adobe Workfront] à [!DNL Slack] vous permet d&#39;effectuer les opérations suivantes :

* Accédez à vos [!DNL Workfront] tâches, validations, favoris, éléments récents de [!DNL Slack].
* Abonnez-vous, approuvez et affectez une tâche à partir de [!DNL Slack].
* Créez des tâches et des problèmes à partir de [!DNL Slack].
* Recevez quelques [!DNL Workfront] notifications dans [!DNL Slack].

Selon la configuration de votre environnement [!DNL Slack], vous pouvez installer et configurer vous-même [!DNL Workfront for Slack] ou votre administrateur [!DNL Workfront] doit l’installer et le configurer avant de pouvoir le configurer vous-même.

Lorsque vous intégrez votre instance [!DNL Slack] avec des utilisateurs [!DNL Workfront], vous pouvez utiliser [!DNL Workfront] tout en collaborant au sein de leurs canaux [!DNL Slack]. L&#39;intégration peut être utilisée à partir de n&#39;importe quel environnement [!DNL Slack], y compris l&#39;application mobile [!DNL Slack].

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans?lang=fr" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur [!DNL Workfront].\

## Conditions préalables pour l’utilisation de [!DNL Workfront] avec [!DNL Slack]

* Vous devez avoir une instance [!DNL Slack].
* Votre administrateur système [!DNL Slack] doit autoriser tous les utilisateurs [!DNL Slack] à installer [!DNL Workfront for Slack].
* Vous devez disposer d’une licence [!DNL Workfront] pour pouvoir utiliser les fonctionnalités intégrées de [!DNL Workfront].

  >[!NOTE]
  >
  >Les utilisateurs avec n&#39;importe quel type de licence [!DNL Workfront] peuvent accéder à [!DNL Workfront] à partir de [!DNL Slack]. Les actions que vous pouvez effectuer à partir de [!DNL Slack] sont limitées à vos niveaux de licence et d’autorisation [!DNL Workfront].

Pour plus d’informations sur la gestion des applications dans [!DNL Slack], voir [Gestion des applications pour votre Workspace.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installer [!DNL Workfront for Slack]

Chaque utilisateur [!DNL Slack] doit installer l’application [!DNL Workfront] lui-même pour utiliser [!DNL Workfront] à partir de [!DNL Slack].

Vous pouvez installer l’application de la manière suivante :

* [Installation de l’application  [!DNL Workfront] en dehors de [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installation de l’application  [!DNL Workfront] dans [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installez l&#39;application [!DNL Workfront] en dehors de [!DNL Slack] {#install-the-workfront-app-outside-slack}

Suivez les étapes ci-dessous pour exécuter le processus d’installation et autoriser [!DNL Workfront for Slack] sur votre instance [!DNL Slack].

>[!IMPORTANT]
>
>Lorsqu’une nouvelle version de [!DNL Workfront] pour Slack est publiée, vous devez réautoriser l’application pour continuer à l’utiliser.

1. Localisez le module complémentaire [!DNL Adobe Workfront] dans le [[!DNL Slack] magasin](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Cliquez sur **[!UICONTROL Ouvrir dans[!DNL Slack]]**.

1. Connectez-vous à votre espace de travail en spécifiant votre URL [!DNL Slack] et en cliquant sur **[!UICONTROL Continuer]**.\

1. Examinez l’accès demandé par [!DNL Slack]. Si vous acceptez cet accès, cliquez sur **[!UICONTROL Autoriser l’accès]** pour autoriser l’application [!DNL Workfront].

Vous pouvez désormais accéder à [!DNL Workfront] à partir de [!DNL Slack], comme décrit dans la section [Accès [!DNL Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installez l’application [!DNL Workfront] dans [!DNL Slack] {#install-the-workfront-app-within-slack}

Vous pouvez installer l’application [!DNL Workfront] directement à partir de l’application [!DNL Slack] :

1. Accédez à votre URL [!DNL Slack].

   Par exemple : *`<YourTeamName>`.slack.com/apps*.

   Ou

   Cliquez sur l&#39;icône **[!UICONTROL Ajouter des applications]** dans votre instance [!DNL Slack].

1. Commencez à saisir *[!DNL Workfront]* dans le champ de recherche.
1. Appuyez sur Entrée.
1. Sélectionnez l’application **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Paramètres]**.

   La page Répertoire de l’application s’affiche.

1. Cliquez sur **[!UICONTROL Visiter le site de l’application]**.
1. Cliquez sur **[!UICONTROL Ajouter à[!DNL Slack]]**.
1. Suivez les étapes pour terminer l’installation.
1. Une fois l’installation terminée, vous pouvez accéder à [!DNL Workfront] à partir de [!DNL Slack], comme décrit dans la section [[!UICONTROL Accès [!DNL Workfront] à partir de [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
