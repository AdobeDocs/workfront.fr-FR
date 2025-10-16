---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Accédez à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]
description: Intégrer  [!DNL Adobe Workfront]  avec  [!DNL Slack]  vous permet d’accéder à  [!DNL Workfront]  à partir de Slack ou d’effectuer certaines actions dans  [!DNL Workfront]  à l’aide d’une commande de barre oblique. L’intégration peut être utilisée à partir de n’importe quel environnement  [!DNL Slack] , notamment l’application mobile  [!DNL Slack] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 99%

---

# Accédez à [!DNL Adobe Workfront] à partir de [!DNL Slack]

L’intégration de [!DNL Adobe Workfront] à [!DNL Slack] vous permet d’accéder à [!DNL Workfront] à partir de [!DNL Slack] ou d’effectuer certaines actions dans [!DNL Workfront] à l’aide d’une commande de barre oblique. L’intégration peut être utilisée à partir de n’importe quel environnement [!DNL Slack], notamment l’application mobile [!DNL Slack].

Vous ou votre administrateur ou administratrice [!DNL Slack] devez installer l’application [!DNL Workfront] dans votre instance [!DNL Slack] avant de pouvoir utiliser [!DNL Workfront] à partir de [!DNL Slack]. Pour plus d’informations, consultez la section [Configurer Adobe Workfront pour Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Tous</p>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## À propos des commandes de barre oblique {#about-slash-commands}

Lorsque vous utilisez [!DNL Slack], vous saisissez des messages à l’intérieur d’un champ de message. Quand vous commencez votre message par une barre oblique, il se transforme en commande et fonctionne différemment d’un simple message. La commande indique à [!DNL Slack] d’effectuer une action.

Vous pouvez accéder à votre instance [!DNL Workfront] à partir de [!DNL Slack] en saisissant une commande de barre oblique dans n’importe quel canal [!DNL Slack].

Rappelez-vous ce qui suit lorsque vous utilisez une commande de barre oblique dans [!DNL Slack] pour accéder à [!DNL Workfront] :

* Les commandes de barre oblique sont sensibles à la casse.
* Les commandes pour [!DNL Workfront] ne sont visibles que par vous, quel que soit le canal dans lequel vous les saisissez.
* La commande doit toujours commencer par `/workfront` ou `/wf`, suivie d’un espace et du nom de l’action que vous souhaitez effectuer dans [!DNL Workfront].

  Cela indique que votre commande est destinée à l’application [!DNL Workfront]. Les commandes pour [!DNL Workfront] ne fonctionnent que si vous avez déjà configuré l’application [!DNL Workfront] avec votre instance [!DNL Slack].

Pour une liste de toutes les commandes que vous pouvez exécuter à partir de Slack pour [!DNL Workfront], consultez la section [Accéder à  [!DNL Workfront]  à partir d’une commande de barre oblique dans  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Se connecter à [!DNL Workfront] à partir de [!DNL Slack] {#log-in-to-workfront-from-slack}

Dans le champ de message de Slack, lorsque vous saisissez une commande, il vous est demandé de vous connecter d’abord à [!DNL Workfront].\
Pour une liste complète des commandes [!DNL Workfront] à partir de [!DNL Slack], consultez dans cet article la section [Accéder à  [!DNL Workfront]  à partir d’une commande de barre oblique dans  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

Se connecter à [!DNL Workfront] à partir de [!DNL Slack] :

1. Connectez-vous à votre instance [!DNL Slack].
1. À partir de n’importe quel canal, saisissez l’une des commandes suivantes :\
   `/workfront log in`

   Ou

   `/wf log in`

1. Cliquez sur le lien **[!UICONTROL Connexion]** [!DNL Workfront] affiché dans la réponse.\
   Un nouvel onglet s’ouvre avec des champs pour les informations d’identification [!DNL Workfront].

1. Suivez les invites pour vous connecter à [!DNL Workfront] en utilisant l’authentification améliorée, OAuth 2.0, ou votre URL SAML (Security Assertion Markup Language).

   >[!NOTE]
   >
   >* Pour saisir l’hôte de votre compte [!DNL Workfront], saisissez-le au format suivant : *domaineDeVotreEntreprise.my.workfront.com*. Le domaine de votre entreprise est généralement le nom de votre entreprise.
   >* Tant qu’un administrateur ou une administratrice [!DNL Workfront] n’a pas activé l’authentification améliorée pour cette intégration, celle-ci n’est pas disponible.


   La page de configuration des notifications [!DNL Workfront] dans [!DNL Slack] s’ouvre.

1. (Facultatif) Désactivez les notifications [!DNL Workfront] que vous ne souhaitez pas recevoir dans [!DNL Slack].

   Pour plus d’informations sur la configuration des paramètres [!DNL Workfront] pour [!DNL Slack], consultez dans cet article la section [Configurer les paramètres](#configure-settings-configure-settings).

1. Retournez à votre canal [!DNL Slack].

   À partir de votre instance [!DNL Slack], la connexion à [!DNL Workfront] est établie.

## Accéder à [!DNL Workfront] à partir de [!DNL Slack]

* [À propos des commandes de barre oblique](#about-slash-commands-about-slash-commands)
* [Accéder à  [!DNL Workfront]  à partir d’un lien partagé dans  [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Accéder à [!DNL Workfront] à partir d’une commande de barre oblique dans [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section [Se connecter à  [!DNL Workfront]  à partir de  [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack).

1. Choisissez un canal au choix et commencez à saisir la commande suivante dans le champ de message :

   `/workfront help`

   Ou

   `/wf help`

1. Sélectionnez l’une des commandes suivantes :

   * `/wf home`

     Affiche les boutons à partir desquels vous pouvez accéder aux listes de vos tâches, problèmes et approbations. En cliquant sur l’un des boutons, les 20 premiers éléments de chaque liste s’affichent dans [!DNL Slack].

     Pour plus d’informations sur la gestion des éléments de travail [!DNL Workfront] à partir de [!DNL Slack], consultez la section [Gérer votre travail et vos approbations à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

     Indiquez le nom de la tâche tel qu’il apparaîtra dans l’interface [!DNL Workfront].

     Ajoute une tâche à [!DNL Workfront].

     Pour plus d’informations sur l’ajout de tâches à [!DNL Workfront] à partir de Slack, consultez la section « Créer des tâches à partir de [!DNL Slack] » dans [Créer des tâches et des problèmes à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

     Indiquez le nom du problème tel qu’il apparaîtra dans l’interface [!DNL Workfront].

     Ajoute une question à [!DNL Workfront].

     Pour plus d’informations sur l’ajout de problèmes à [!DNL Workfront] à partir de [!DNL Slack], consultez la section « Créer des problèmes à partir de [!DNL Slack] » dans [Créer des tâches et des problèmes à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

     Affiche la liste de vos favoris [!DNL Workfront].

     Pour plus d’informations sur la manière d’accéder à vos favoris à partir de [!DNL Slack], consultez la section [Accéder à la liste de vos [!UICONTROL favoris] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) dans l’article [Accéder à vos favoris et à vos éléments récents à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `/wf recent`

     Affiche la liste des derniers éléments auxquels vous avez accédé dans [!DNL Workfront].

     Pour plus d’informations sur la manière d’accéder à vos éléments récents à partir de [!DNL Slack], consultez la section [Accéder à la liste de vos [!UICONTROL éléments récents] à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites]  dans l’article [!UICONTROL Accéder à vos favoris et à vos éléments récents à partir de  [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md).

   * `wf tasks`

     Affiche une liste de vos tâches.

     Pour plus d’informations sur la gestion de vos tâches à partir de [!DNL Slack], consultez la section « Gérer vos tâches à partir de [!DNL Slack] » dans [Gérer votre travail et vos approbations à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Affiche une liste de vos problèmes.

     Pour plus d’informations sur la gestion de vos problèmes à partir de [!DNL Slack], consultez la section « Gérer vos questions à partir de [!DNL Slack] » dans [Gérer votre travail et vos approbations à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Affiche vos approbations [!DNL Workfront].

     Pour plus d’informations sur la gestion de vos approbations à partir de [!DNL Slack], consultez la section « Gérer vos approbations à partir de [!DNL Slack] » dans [Gérer votre travail et vos approbations à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

     Inclure un mot-clé.

     Rechercher un mot-clé spécifique. Vous pouvez rechercher les types d’objets suivants :

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
      * Note

        Pour plus d’informations sur la recherche dans [!DNL Slack], consultez [Rechercher des éléments  [!DNL Adobe Workfront]  à partir de Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Vous connecte à [!DNL Workfront] à partir de [!DNL Slack].

   * `/wf log out `

     Vous déconnecte de [!DNL Workfront] à partir de [!DNL Slack]. Votre connexion à [!DNL Workfront] reste ouverte même si vous avez une autre instance de [!DNL Workfront] ouverte dans un autre onglet du navigateur ou dans une autre application.
   * `/wf settings`

     Vous permet de configurer vos paramètres [!DNL Workfront] dans [!DNL Slack].

     Pour plus d’informations sur la configuration des paramètres [!DNL Workfront] dans Slack, consultez [Configurer les paramètres](#configure-settings-configure-settings).

   * `/wf help`
Affiche une liste complète des commandes pour [!DNL Workfront].


   * `Visit Workfront Help` : ouvre la section [!UICONTROL Slack] sur le site d’aide [!DNL Workfront] dans un nouvel onglet du navigateur.


1. (Facultatif) Pour supprimer le message d’une commande, passez la souris sur le coin supérieur droit du message Slack contenant la commande et cliquez sur **[!UICONTROL Afficher les actions de message]**, puis cliquez sur **[!UICONTROL Supprimer le message]**.

1. (Facultatif et le cas échéant) Cliquez sur **[!UICONTROL Supprimer]** pour confirmer que vous souhaitez supprimer ce message.

### Accéder à [!DNL Workfront] à partir d’un lien partagé dans [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

Vous pouvez accéder aux objets [!DNL Workfront] à partir d’un lien vers ces objets qui est partagé avec vous dans [!DNL Slack].

Pour plus d’informations sur l’accès à [!DNL Workfront] à partir d’un lien partagé, consultez [Accéder aux objets  [!DNL Adobe Workfront]  à partir d’un lien partagé dans  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Configurer les paramètres {#configure-settings}

1. Dans un champ de message [!DNL Slack], entrez la commande suivante :

   `/workfront settings`

   Ou

   `/wf settings`

   Tous les paramètres sont activés par défaut.

1. Désélectionnez les options suivantes pour désactiver vos paramètres pour Workfront :

   * Dans la zone **[!UICONTROL Paramètres généraux]**, désactivez le paramètre **[!UICONTROL Lors du collage d’une URL [!DNL Workfront] dans un canal [!DNL Slack], afficher une description, une date d’échéance ou un nom de demandeur ou de demandeuse supplémentaire]** si vous ne souhaitez pas que [!DNL Slack] ajoute des informations supplémentaires sur vos objets [!DNL Workfront] lorsque vous partagez une URL vers l’objet dans [!UICONTROL Slack].

   * Dans la zone **[!UICONTROL Paramètres des notifications]**, désactivez les notifications que vous souhaitez ne plus recevoir de Workfront.

     Pour plus d’informations sur la réception de notifications [!DNL Workfront] dans [!DNL Slack], consultez [Recevoir des notifications  [!DNL Adobe Workfront]  dans  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Se déconnecter de [!DNL Workfront] à partir de [!DNL Slack]

1. Dans un champ de message [!DNL Slack], tapez la commande suivante :\
   `/workfront log out` Ou\
   `/wf log out`\
   Vous recevez une confirmation de déconnexion de [!DNL Workfront].\
   Votre connexion à [!DNL Workfront] est maintenue si vous avez une autre instance [!DNL Workfront] ouverte dans un autre onglet du navigateur ou dans une autre application.
