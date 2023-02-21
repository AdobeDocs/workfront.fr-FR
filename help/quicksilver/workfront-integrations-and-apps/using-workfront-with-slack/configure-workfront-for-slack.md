---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: Configurer [!DNL Adobe Workfront] pour le Slack
description: Intégration [!DNL Adobe Workfront] avec Slack vous permet d’accéder à et de créer [!DNL Workfront] tâches, approbations, favoris, éléments récents du Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Configurer [!DNL Adobe Workfront for Slack]

Intégration [!DNL Adobe Workfront] avec [!DNL Slack] vous permet d’effectuer les opérations suivantes :

* Accédez à [!DNL Workfront] tâches, validations, favoris, éléments récents de [!DNL Slack].
* S’abonner, approuver ou attribuer une tâche à partir de [!DNL Slack].
* Création de tâches et de problèmes à partir de [!DNL Slack].
* Recevez quelques [!DNL Workfront] notifications dans [!DNL Slack].

Selon la manière dont votre [!DNL Slack] environnement est configuré, vous pouvez installer et configurer [!DNL Workfront for Slack] vous-même, ou votre [!DNL Workfront] l’administrateur doit l’installer et le configurer avant de pouvoir le configurer vous-même.

Lorsque vous intégrez votre [!DNL Slack] instance avec [!DNL Workfront] les utilisateurs peuvent utiliser [!DNL Workfront] en collaborant au sein de leur [!DNL Slack] canaux. L’intégration peut être utilisée à partir de n’importe quel [!DNL Slack] , y compris le [!DNL Slack] application mobile.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrator.\

## Conditions préalables à l’utilisation [!DNL Workfront] avec [!DNL Slack]

* Vous devez disposer d’un [!DNL Slack] instance.
* Votre [!DNL Slack] l’administrateur système doit autoriser tous les [!DNL Slack] utilisateurs à installer [!DNL Workfront for Slack].
* Vous devez disposer d’un [!DNL Workfront] pour pouvoir utiliser les fonctionnalités intégrées dans [!DNL Workfront].

   >[!NOTE]
   >
   >Utilisateurs avec tout [!DNL Workfront] type de licence accessible [!DNL Workfront] de [!DNL Slack]. Actions que vous pouvez effectuer à partir de [!DNL Slack] sont limitées à vos [!DNL Workfront] niveaux de licence et d’autorisation.

Pour plus d’informations sur la gestion des applications dans [!DNL Slack], voir [Gestion des applications pour votre espace de travail.](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## Installer [!DNL Workfront for Slack]

Chaque [!DNL Slack] l’utilisateur doit installer la variable [!DNL Workfront] pour utiliser [!DNL Workfront] de [!DNL Slack].

Vous pouvez installer l’application de la manière suivante :

* [Installez le [!DNL Workfront] application externe [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [Installez le [!DNL Workfront] in [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### Installez le [!DNL Workfront] application externe [!DNL Slack] {#install-the-workfront-app-outside-slack}

Suivez les étapes ci-dessous pour exécuter le processus d’installation et autoriser [!DNL Workfront for Slack] sur votre [!DNL Slack] instance.

>[!IMPORTANT]
>
>Lorsqu’une nouvelle version de [!DNL Workfront] pour que Slack soit publié, vous devez réautoriser l’application afin de continuer à l’utiliser.

1. Recherchez la variable [!DNL Adobe Workfront] module complémentaire dans le [[!DNL Slack] store](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. Cliquez sur **[!UICONTROL Ouvrir dans[!DNL Slack]]**.

1. Connectez-vous à votre espace de travail en spécifiant votre [!DNL Slack] URL et clic **[!UICONTROL Continuer]**.\

1. Examiner l’accès qui [!DNL Slack] demande. Si vous acceptez cet accès, cliquez sur **[!UICONTROL Autoriser l’accès]** pour autoriser le [!DNL Workfront] application.

Vous pouvez désormais accéder à [!DNL Workfront] de [!DNL Slack], comme décrit dans la section [Accès [!DNL Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### Installez le [!DNL Workfront] in [!DNL Slack] {#install-the-workfront-app-within-slack}

Vous pouvez installer le [!DNL Workfront] directement depuis l’application [!DNL Slack] application :

1. Accédez à [!DNL Slack] URL.

   Par exemple : *`<YourTeamName>`.slack.com/apps*.

   Ou

   Cliquez sur le bouton **[!UICONTROL Ajout d’applications]** dans votre [!DNL Slack] instance.

1. Commencez à taper *[!DNL Workfront]* dans le champ de recherche.
1. Appuyez sur Entrée.
1. Sélectionnez la **[!DNL Workfront]** application.
1. Cliquez sur **[!UICONTROL Paramètres]**.

   La page Répertoire de l’application s’affiche.

1. Cliquez sur **[!UICONTROL Visite du site de l’application]**.
1. Cliquez sur **[!UICONTROL Ajouter à[!DNL Slack]]**.
1. Suivez les étapes pour terminer l’installation.
1. Une fois l’installation terminée, vous pouvez accéder à [!DNL Workfront] de [!DNL Slack], comme décrit dans la section [Accès à [!UICONTROL [!DNL Workfront] de [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
