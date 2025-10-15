---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configurer  [!DNL Adobe Workfront]  pour Slack
description: L’intégration d’ [!DNL Adobe Workfront]  avec Slack vous permet d’accéder et de créer des éléments de travail, des approbations, des favoris et des éléments récents  [!DNL Workfront]  à partir de Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 100%

---

# Configurer [!DNL Adobe Workfront for Slack]

Intégrer [!DNL Adobe Workfront] avec [!DNL Slack] permet de faire ce qui suit :

* Accéder à vos éléments de travail, approbations, favoris et éléments récents [!DNL Workfront] à partir de [!DNL Slack].
* S’abonner, approuver, affecter du travail à partir de [!DNL Slack].
* Créer des tâches et des problèmes à partir de [!DNL Slack].
* Recevoir des notifications [!DNL Workfront] dans [!DNL Slack].

En fonction de la configuration de votre environnement [!DNL Slack], vous pouvez soit installer et configurer vous-même [!DNL Workfront for Slack], soit l’administration [!DNL Workfront] doit d’abord l’installer et le configurer avant que vous ne puissiez le faire vous-même.

Lorsque vous intégrez votre instance [!DNL Slack] à [!DNL Workfront], les utilisateurs et les utilisatrices peuvent utiliser [!DNL Workfront] tout en collaborant dans leurs canaux [!DNL Slack]. L’intégration peut être utilisée à partir de n’importe quel environnement [!DNL Slack], y compris l’application mobile [!DNL Slack].

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/fr/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

## Conditions préalables à l’utilisation de [!DNL Workfront] avec [!DNL Slack]

* Vous devez disposer d’une instance [!DNL Slack].
* L’administration du système [!DNL Slack] doit autoriser tous les utilisateurs et toutes les utilisatrices de [!DNL Slack] à installer [!DNL Workfront for Slack].
* Vous devez disposer d’une licence [!DNL Workfront] pour pouvoir utiliser les fonctionnalités intégrées dans [!DNL Workfront].

  >[!NOTE]
  >
  >Les utilisateurs et les utilisatrices disposant de n’importe quel type de licence [!DNL Workfront] peuvent accéder à [!DNL Workfront] à partir de [!DNL Slack]. Les actions que vous pouvez effectuer à partir de [!DNL Slack] dépendent de votre licence [!DNL Workfront] et de vos niveaux d’autorisation.

Pour plus d’informations sur la gestion des applications dans [!DNL Slack], consultez la section [Gérer les applications de votre espace de travail.](https://get.slack.help/hc/fr-fr/articles/222386767-Manage-apps-for-your-workspace)

## Installer [!DNL Workfront for Slack]

Chaque utilisateur ou utilisatrice [!DNL Slack] doit installer l’application [!DNL Workfront] par ses propres moyens pour pouvoir utiliser [!DNL Workfront] à partir de [!DNL Slack].

Vous pouvez installer l’application des manières suivantes :

* [Installer l’application  [!DNL Workfront]  en dehors de  [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installer l’application  [!DNL Workfront]  dans  [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installer l’application [!DNL Workfront] en dehors de [!DNL Slack] {#install-the-workfront-app-outside-slack}

Suivez les étapes ci-dessous pour exécuter le processus d’installation et autoriser [!DNL Workfront for Slack] sur votre instance [!DNL Slack].

>[!IMPORTANT]
>
>Lorsqu’une nouvelle version de [!DNL Workfront] pour Slack est publiée, vous devez réautoriser l’application pour pouvoir continuer à l’utiliser.

1. Localisez le module complémentaire [!DNL Adobe Workfront] dans la boutique [[!DNL Slack] ](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Cliquez sur **[!UICONTROL Ouvrir dans[!DNL Slack]]**.

1. Connectez-vous à votre espace de travail en spécifiant votre URL [!DNL Slack] et en cliquant sur **[!UICONTROL Continuer]**.

1. Examinez l’accès demandé par [!DNL Slack]. Si vous acceptez cette demande d’accès, cliquez sur **[!UICONTROL Autoriser l’accès]** pour autoriser l’application [!DNL Workfront].

Vous pouvez maintenant accéder à [!DNL Workfront] à partir de [!DNL Slack], comme décrit dans [Accéder à  [!DNL Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installer l’application [!DNL Workfront] à partir de [!DNL Slack] {#install-the-workfront-app-within-slack}

Vous pouvez installer l’application [!DNL Workfront] directement à partir de l’application [!DNL Slack] :

1. Accédez à l’URL de votre site [!DNL Slack].

   Par exemple : *`<YourTeamName>`.slack.com/apps*.

   Ou

   Cliquez sur l’icône **[!UICONTROL Ajouter des applications]** dans votre instance [!DNL Slack].

1. Commencez à saisir *[!DNL Workfront]* dans le champ de recherche.
1. Appuyez sur « Entrée ».
1. Sélectionnez l’application **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Paramètres]**.

   La page App Directory s’affiche.

1. Cliquez sur **[!UICONTROL Visiter le site de l’application]**.
1. Cliquez sur **[!UICONTROL Ajouter à[!DNL Slack]]**.
1. Suivez les étapes pour terminer l’installation.
1. Une fois l’installation terminée, vous pouvez accéder à [!DNL Workfront] à partir de [!DNL Slack], comme décrit dans [[!UICONTROL Access [!DNL Workfront]  à partir de  [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront]  à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
