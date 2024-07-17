---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Gérer votre travail et vos approbations à partir de Slack
description: Vous pouvez accéder à votre liste de tâches à domicile, la consulter et accepter de travailler sur les tâches et les problèmes, et passer en revue ou prendre des décisions sur les validations directement depuis Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 4%

---

# Gérer votre travail et vos validations depuis [!DNL Slack]

Après avoir installé [!DNL Adobe Workfront for Slack], vous pouvez effectuer les opérations suivantes :

* Accédez aux listes de vos éléments [!UICONTROL Home] depuis [!DNL Slack]
* Révisez et acceptez de travailler sur les tâches et problèmes de [!DNL Slack].
* Examiner et prendre des décisions concernant les approbations de [!DNL Slack]

Pour plus d&#39;informations sur la configuration de [!DNL Workfront] avec [!DNL Slack], voir [Configuration [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans?lang=fr" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Avant de pouvoir gérer votre travail et vos validations depuis [!DNL Slack], vous devez :

* Configurer [!DNL Workfront for Slack]\
  Pour obtenir des instructions sur la configuration de [!DNL Workfront for Slack], voir [Configuration [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Gérer votre travail depuis [!DNL Slack]

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] depuis [!DNL Slack].\
   Pour plus d&#39;informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section &quot;Connexion à [!DNL Workfront] à partir de [!DNL Slack]&quot; dans [Accès [!DNL Adobe Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir la commande suivante dans le champ de message :

   `/workfront home`

   >[!NOTE]
   >
   >* Les commandes respectent la casse.
   >* Vous pouvez démarrer votre commande avec `/wf` au lieu de `/workfront`.

   Les boutons à partir desquels vous pouvez accéder aux listes de vos tâches, problèmes et validations s’affichent. Cliquez sur l’un des boutons pour afficher les 20 premiers éléments de chaque liste dans [!DNL Slack].

1. (Facultatif) Cliquez sur **[!UICONTROL Tâches]** pour afficher toutes vos tâches.

   Pour plus d’informations sur la gestion des tâches dans [!DNL Slack], voir [Gestion de vos tâches à partir de [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Facultatif) Cliquez sur **[!UICONTROL Problèmes]** pour afficher tous vos problèmes.

   Pour plus d’informations sur la gestion des problèmes dans [!DNL Slack], voir [Gestion de vos problèmes à partir de [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Facultatif) Cliquez sur **[!UICONTROL Validations]** pour afficher toutes les approbations en attente de votre décision.\
   Pour plus d&#39;informations sur la gestion de vos approbations dans [!DNL Slack], voir [Gestion de vos approbations depuis [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Gérer vos tâches depuis [!DNL Slack] {#manage-your-tasks-from-slack}

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] depuis [!DNL Slack].\
   Pour plus d&#39;informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section &quot;Connexion à [!DNL Workfront] à partir de [!DNL Slack]&quot; dans [Accès [!DNL Adobe Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir l&#39;une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Tâches]**

   Ou

   `/workfront tasks`

   >[!NOTE]
   >
   >* Les commandes respectent la casse.
   >* Vous pouvez démarrer votre commande avec `/wf` au lieu de `/workfront`.

   Les 20 premières tâches de votre liste s’affichent.

1. Cliquez sur **[!UICONTROL +`<remaining number>` more]** pour afficher d’autres tâches.
1. Pensez à consulter les informations suivantes sur vos tâches :

   * **[!UICONTROL Nom]**
   * **[!UICONTROL Nom du projet]** ou **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** de la tâche.
   * **[!DNL Assigned By Name]** : nom de l’utilisateur qui vous a assigné la tâche.
   * **[!UICONTROL Statut]**

1. (Facultatif) Cliquez sur le nom d’un élément pour l’ouvrir dans Workfront dans un onglet de navigateur distinct.
1. (Facultatif) Dans le champ **[!UICONTROL Status]**, sélectionnez un nouvel état.
1. (Facultatif) Cliquez sur **[!UICONTROL Temps du journal]**, puis sélectionnez un **[!UICONTROL Type d’heure]** et une durée d’heure pour consigner l’heure sur l’élément.

   >[!NOTE]
   >
   >* Vous ne pouvez consigner les heures que par incréments d’une demi-heure ou complète, jusqu’à 12 heures et 30 minutes.
   >* Les heures que vous enregistrez ont une date d’entrée d’aujourd’hui. Vous ne pouvez pas consigner l’heure d’une date passée ou future à partir de [!DNL Slack].

   Vous recevez une confirmation que l’heure a été enregistrée.

1. (Facultatif) Cliquez sur **[!UICONTROL Travailler dessus]** pour accepter de travailler sur une tâche. Le bouton [!UICONTROL Travailler dessus] disparaît.

## Gérer vos problèmes depuis [!DNL Slack] {#manage-your-issues-from-slack}

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] depuis [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], voir [Connexion à [!DNL Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir l&#39;une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Issues]**

   Ou

   `/workfront issues`

   >[!NOTE]
   >
   >* Les commandes respectent la casse.
   >* Vous pouvez démarrer votre commande avec `/wf` au lieu de `/workfront`.

   Les 20 premiers problèmes de votre liste s’affichent.

1. Cliquez sur **[!UICONTROL + `<number>` plus]** pour afficher des éléments supplémentaires.
1. Pensez à consulter les informations suivantes sur vos tâches :

   * **[!UICONTROL Nom]**
   * **[!UICONTROL Nom du projet]** ou nom de l’objet parent
   * **[!UICONTROL Date d’échéance le]** : il s’agit de la date d’achèvement planifiée de l’élément de travail.
   * **[!DNL Requested by]** Nom : il s’agit du contact de Principal (pour les problèmes) ou de l’utilisateur qui a effectué l’affectation (pour les tâches).

1. (Facultatif) Cliquez sur le nom du problème pour l’ouvrir dans Workfront dans un onglet de navigateur distinct.
1. (Facultatif) Cliquez sur **[!DNL Work on it]** pour commencer à travailler sur les problèmes que vous n’avez pas encore acceptés.

   Le bouton [!UICONTROL Travailler dessus] disparaît.

## Gérer vos approbations depuis [!DNL Slack] {#manage-your-approvals-from-slack}

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] depuis [!DNL Slack].\
   Pour plus d&#39;informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section &quot;Connexion à [!DNL Workfront] à partir de [!DNL Slack]&quot; dans [Accès [!DNL Adobe Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir l&#39;une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Approbations]**

   Ou

   `/workfront approvals`

   >[!NOTE]
   >
   >* Les commandes respectent la casse.
   >* Vous pouvez démarrer votre commande avec `/wf` au lieu de `/workfront`.

   Les 20 premiers éléments de votre liste **[!UICONTROL Approbations]** s’affichent. Des informations supplémentaires sur les éléments s’affichent également, telles que le nom de l’utilisateur qui l’a demandé ou le nom du projet auquel l’élément appartient.

1. Cliquez sur **[!UICONTROL + `<number>` plus]** pour afficher des éléments supplémentaires.

1. Envisagez de gérer les validations pour les objets suivants :

   * **Projets**

     Cliquez sur **[!UICONTROL Approve]** ou **[!UICONTROL Reject]** pour accepter ou rejeter le changement d’état d’un projet.

   * **Tâches**

     Cliquez sur **[!UICONTROL Approve]** ou **[!UICONTROL Reject]** pour accepter ou rejeter le changement d’état d’une tâche.

   * **Événements**

     Cliquez sur **[!UICONTROL Approuver]** ou **[!DNL Reject]** pour accepter ou refuser le changement d’état d’un problème.

   * **Documents**

     Cliquez sur **[!UICONTROL Approuver]** pour approuver un document, sur **[!UICONTROL Rejeter]** pour le rejeter ou sur **[!UICONTROL Modifications]** pour indiquer que vous l’approuvez, mais que le document nécessite des modifications supplémentaires.\
     (Facultatif) Placez le pointeur de la souris sur la miniature du document pour cliquer sur la loupe et prévisualiser le document.

   * **BAT** &#x200B; cliquez sur le nom du BAT pour l’ouvrir dans [!DNL Workfront] dans un onglet distinct et gérer la validation.
   * **Demandes d’accès**

     Cliquez sur **[!UICONTROL Accorder l’accès]** pour accorder des autorisations améliorées à l’objet demandé ou sur **[!UICONTROL Ignorer]** pour ignorer la demande d’accès supplémentaire.

1. (Facultatif) Cliquez sur le nom de l’objet soumis à approbation pour l’ouvrir dans [!DNL Workfront] dans un nouvel onglet du navigateur.
