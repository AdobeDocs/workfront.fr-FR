---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Accéder à [!DNL Adobe Workfront] à partir de [!DNL Slack]
description: L'intégration de  [!DNL Adobe Workfront] à [!DNL Slack] vous permet d'accéder à [!DNL Workfront] à partir de Slack ou d'effectuer certaines actions dans  [!DNL Workfront] à l'aide d'une commande de barre oblique. L'intégration peut être utilisée à partir de n'importe quel environnement  [!DNL Slack] , y compris l'application mobile  [!DNL Slack] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

---

# Accès à [!DNL Adobe Workfront] à partir de [!DNL Slack]

L&#39;intégration de [!DNL Adobe Workfront] à [!DNL Slack] vous permet d&#39;accéder à [!DNL Workfront] à partir de [!DNL Slack] ou d&#39;effectuer certaines actions dans [!DNL Workfront] à l&#39;aide d&#39;une commande de barre oblique. L&#39;intégration peut être utilisée à partir de n&#39;importe quel environnement [!DNL Slack], y compris l&#39;application mobile [!DNL Slack].

Vous ou votre administrateur [!DNL Slack] devez installer l&#39;application [!DNL Workfront] dans votre instance [!DNL Slack] avant de pouvoir utiliser [!DNL Workfront] à partir de [!DNL Slack]. Pour plus d’informations, voir [Configuration d’Adobe Workfront pour Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## A propos des commandes de barre oblique {#about-slash-commands}

Lorsque vous utilisez [!DNL Slack], vous saisissez des messages dans un champ de message. Lorsque vous lancez votre message avec une barre oblique, il devient une commande et il se comporte différemment d’un simple message. La commande indique à [!DNL Slack] d&#39;effectuer une action.

Vous pouvez accéder à votre instance [!DNL Workfront] à partir de [!DNL Slack] en saisissant une commande de barre oblique dans n’importe quel canal [!DNL Slack].

Souvenez-vous des points suivants lorsque vous utilisez une commande de barre oblique dans [!DNL Slack] pour accéder à [!DNL Workfront] :

* Les commandes Flash sont sensibles à la casse.
* Les commandes de [!DNL Workfront] ne sont visibles que par vous, quel que soit le canal dans lequel vous les saisissez.
* La commande doit toujours commencer par `/workfront` ou `/wf`, suivie d’un espace et du nom d’une action que vous souhaitez effectuer dans [!DNL Workfront].

  Cela indique que votre commande est destinée à l’application [!DNL Workfront]. Les commandes de [!DNL Workfront] ne fonctionnent que si vous avez déjà configuré l’application [!DNL Workfront] avec votre instance [!DNL Slack].

Pour obtenir la liste de toutes les commandes que vous pouvez exécuter à partir de Slack pour [!DNL Workfront], voir [Accès [!DNL Workfront] à partir d&#39;une commande de barre oblique dans [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Connectez-vous à [!DNL Workfront] depuis [!DNL Slack] {#log-in-to-workfront-from-slack}

Lorsque vous tapez une commande dans le champ de message de Slack, vous serez d’abord invité à vous connecter à [!DNL Workfront].\
Pour obtenir la liste complète des commandes [!DNL Workfront] de [!DNL Slack], reportez-vous à la section [Accès [!DNL Workfront]  à partir d&#39;une commande de barre oblique dans [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) de cet article.

Pour vous connecter à [!DNL Workfront] à partir de [!DNL Slack] :

1. Connectez-vous à votre instance [!DNL Slack].
1. Depuis n’importe quel canal, saisissez l’une des commandes suivantes :\
   `/workfront log in`

   Ou

   `/wf log in`

1. Cliquez sur le lien [!DNL Workfront] **[!UICONTROL Se connecter]** affiché dans la réponse.\
   Un nouvel onglet s’ouvre avec des champs pour les informations d’identification [!DNL Workfront].

1. Suivez les invites pour vous connecter à [!DNL Workfront] à l’aide de l’authentification améliorée, d’OAuth 2.0 ou de l’URL SAML (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* Lorsque vous êtes invité à saisir l’hôte de votre compte [!DNL Workfront], saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre société correspond généralement au nom de votre société.
   >* L’authentification améliorée n’est pas disponible tant qu’un administrateur [!DNL Workfront] ne l’a pas activée pour cette intégration.


   La page de configuration des notifications [!DNL Workfront] dans [!DNL Slack] s’ouvre.

1. (Facultatif) Désactivez toutes les notifications [!DNL Workfront] que vous ne souhaitez pas recevoir dans [!DNL Slack].

   Pour plus d&#39;informations sur la configuration des paramètres [!DNL Workfront] pour [!DNL Slack], consultez la section [Configurer les paramètres](#configure-settings-configure-settings) de cet article.

1. Revenez à votre canal [!DNL Slack].

   Vous êtes connecté à [!DNL Workfront] à partir de votre instance [!DNL Slack].

## Accès à [!DNL Workfront] à partir de [!DNL Slack]

* [A propos des commandes de barre oblique](#about-slash-commands-about-slash-commands)
* [Accéder à  [!DNL Workfront]  à partir d&#39;un lien partagé dans  [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Accéder à [!DNL Workfront] à partir d&#39;une commande de barre oblique dans [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] depuis [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], voir [Connexion à [!DNL Workfront] à partir de [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Depuis n&#39;importe quel canal, commencez à saisir la commande suivante dans le champ de message :

   `/workfront help`

   Ou

   `/wf help`

1. Sélectionnez l’une des commandes suivantes :

   * `/wf home`

     Affiche des boutons à partir desquels vous pouvez accéder aux listes de vos tâches, problèmes et validations. Cliquez sur l’un des boutons pour afficher les 20 premiers éléments de chaque liste dans [!DNL Slack].

     Pour plus d&#39;informations sur la gestion des [!DNL Workfront] tâches à partir de [!DNL Slack], voir [Gérer votre travail et vos validations à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

     Insérez le nom de la tâche tel qu&#39;il apparaîtra dans l&#39;interface [!DNL Workfront].

     Ajoute une tâche à [!DNL Workfront].

     Pour plus d’informations sur l’ajout de tâches à [!DNL Workfront] à partir du Slack, voir la section &quot;Création de tâches à partir de [!DNL Slack]&quot; dans [Création de tâches et de problèmes à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

     Insérez le nom du problème tel qu&#39;il apparaîtra dans l&#39;interface [!DNL Workfront].

     Ajoute un problème à [!DNL Workfront].

     Pour plus d’informations sur l’ajout de problèmes à [!DNL Workfront] à partir de [!DNL Slack], voir la section &quot;Création de problèmes à partir de [!DNL Slack]&quot; dans [Création de tâches et de problèmes à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

     Affiche la liste de vos favoris [!DNL Workfront].

     Pour plus d’informations sur l’accès à vos favoris à partir de [!DNL Slack], reportez-vous à la section [Accès à votre liste [!UICONTROL Favoris] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) de l’article [Accès à vos favoris et aux éléments récents à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) .

   * `/wf recent`

     Affiche la liste de vos éléments récemment consultés dans [!DNL Workfront].

     Pour plus d’informations sur l’accès à vos éléments récents à partir de [!DNL Slack], consultez les articles [Accès à votre liste d’ [!UICONTROL  éléments récents] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites]  et [!UICONTROL éléments récents à partir de [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `wf tasks`

     Affiche une liste de vos tâches.

     Pour plus d’informations sur la gestion de vos tâches à partir de [!DNL Slack], consultez la section &quot;Gestion de vos tâches à partir de [!DNL Slack]&quot; dans la section [Gestion de votre travail et approbations à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Affiche une liste de vos problèmes.

     Pour plus d’informations sur la gestion de vos problèmes à partir de [!DNL Slack], consultez la section &quot;Gestion de vos problèmes à partir de [!DNL Slack]&quot; dans la section [Gestion de votre travail et approbations à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Affiche vos [!DNL Workfront] validations.\

     Pour plus d&#39;informations sur la gestion de vos approbations depuis [!DNL Slack], consultez la section &quot;Gestion de vos approbations depuis [!DNL Slack]&quot; dans [Gérer votre travail et vos approbations depuis [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

     Inclure le mot-clé.

     Recherchez un mot-clé spécifique. Vous pouvez rechercher les types d’objets suivants :

      * Projet
      * Tâche
      * Problème
      * Rapport
      * Personnes
      * Modèle
      * Document
      * Portfolio
      * Programme
      * Tableau de bord
      * Entreprise
      * Remarque \

        Pour plus d&#39;informations sur la recherche dans [!DNL Slack], voir [Recherche d&#39;éléments  [!DNL Adobe Workfront] à partir de Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Connectez-vous à [!DNL Workfront] à partir de [!DNL Slack].

   * `/wf log out `

     Déconnecte-toi de [!DNL Workfront] à partir de [!DNL Slack]. Vous restez connecté à [!DNL Workfront] si une instance [!DNL Workfront] distincte est ouverte dans un autre onglet du navigateur sur une autre application.
   * `/wf settings`

     Vous donne accès à la configuration de vos paramètres [!DNL Workfront] dans [!DNL Slack].

     Pour plus d&#39;informations sur la configuration des paramètres [!DNL Workfront] dans Slack, voir [Configuration des paramètres](#configure-settings-configure-settings).

   * `/wf help`
Affiche une liste complète des commandes pour [!DNL Workfront].


   * `Visit Workfront Help` : ouvre la section [!UICONTROL Slack] sur le site d’aide [!DNL Workfront] dans un nouvel onglet du navigateur.


1. (Facultatif) Pour supprimer le message d’une commande, placez le pointeur de la souris dans le coin supérieur droit du message du Slack contenant la commande, puis cliquez sur &#x200B;**[!UICONTROL Afficher les actions du message]**, puis cliquez sur **[!UICONTROL Supprimer le message]**.

1. (Facultatif et conditionnel) Cliquez sur **[!UICONTROL Supprimer]** pour confirmer que vous souhaitez supprimer ce message.

### Accéder à [!DNL Workfront] à partir d&#39;un lien partagé dans [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Vous pouvez accéder aux objets [!DNL Workfront] à partir d’un lien vers les objets partagés avec vous dans [!DNL Slack].

Pour plus d&#39;informations sur l&#39;accès à [!DNL Workfront] à partir d&#39;un lien partagé, voir [Accès [!DNL Adobe Workfront] aux objets à partir d&#39;un lien partagé dans [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Configuration des paramètres {#configure-settings}

1. Dans un champ de message [!DNL Slack], saisissez la commande suivante :

   `/workfront settings`

   Ou

   `/wf settings`

   Tous les paramètres sont activés par défaut.

1. Désélectionnez l’une des options suivantes pour désactiver vos paramètres pour Workfront :

   * Dans la zone **[!UICONTROL Paramètres généraux]**, désactivez le paramètre **[!UICONTROL lors du collage d&#39;une URL [!DNL Workfront] dans un canal [!DNL Slack], affichez une description supplémentaire, l&#39;échéance ou le nom du demandeur]** &#x200B; si vous ne souhaitez pas que [!DNL Slack] ajoute des informations supplémentaires sur vos objets [!DNL Workfront] lorsque vous partagez une URL vers l&#39;objet dans [!UICONTROL Slack].

   * Dans la zone **[!UICONTROL Paramètres des notifications]**, désactivez les notifications que vous souhaitez arrêter de recevoir de Workfront.\

     Pour plus d&#39;informations sur la réception de [!DNL Workfront] notifications dans [!DNL Slack], voir [Recevoir [!DNL Adobe Workfront] les notifications dans [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Déconnectez-vous de [!DNL Workfront] depuis [!DNL Slack]

1. Dans un champ de message [!DNL Slack], saisissez la commande suivante :\
   `/workfront log out` Or\
   `/wf log out`\
   Vous recevez une confirmation que vous avez été déconnecté de [!DNL Workfront].\
   Vous restez connecté à [!DNL Workfront] si une instance [!DNL Workfront] distincte est ouverte dans un autre onglet du navigateur sur une autre application.
