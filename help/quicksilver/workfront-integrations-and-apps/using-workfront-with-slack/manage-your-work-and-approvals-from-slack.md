---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Gérer votre travail et vos validations depuis Slack
description: Vous pouvez accéder à votre liste de tâches à domicile, la consulter et accepter de travailler sur les tâches et les problèmes, et passer en revue ou prendre des décisions sur les validations directement depuis Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 1%

---

# Gérez votre travail et vos approbations à partir de [!DNL Slack]

Une fois que vous avez installé [!DNL Adobe Workfront for Slack], vous pouvez effectuer les opérations suivantes :

* Accédez aux listes de vos [!UICONTROL Accueil] éléments de [!DNL Slack]
* Révisez et acceptez de travailler sur les tâches et les problèmes de [!DNL Slack]
* Examiner et prendre des décisions concernant les approbations [!DNL Slack]

Pour plus d’informations sur la configuration [!DNL Workfront] avec [!DNL Slack], voir [Configurer [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir gérer votre travail et vos validations depuis [!DNL Slack], vous devez

* Configurer [!DNL Workfront for Slack]\
   Pour obtenir des instructions sur la configuration [!DNL Workfront for Slack], voir [Configurer [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Gérer votre travail à partir de [!DNL Slack]

1. Connectez-vous à [!DNL Slack] et connectez-vous à [!DNL Workfront] de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] de [!DNL Slack], voir &quot;Connexion à [!DNL Workfront] de [!DNL Slack]&quot; dans la section [Accès [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir la commande suivante dans le champ de message :

   `/workfront home`

   >[!NOTE]
   >
   >* Les commandes sont sensibles à la casse.
   >* Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.


   Les boutons à partir desquels vous pouvez accéder aux listes de vos tâches, problèmes et validations s’affichent. Cliquez sur l’un des boutons pour afficher les 20 premiers éléments de chaque liste dans la [!DNL Slack].

1. (Facultatif) Cliquez sur **[!UICONTROL Tâches]** pour afficher toutes vos tâches.

   Pour plus d’informations sur la gestion des tâches dans [!DNL Slack], voir [Gestion de vos tâches à partir de [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Facultatif) Cliquez sur **[!UICONTROL Problèmes]** pour afficher tous vos problèmes.

   Pour plus d’informations sur la gestion des problèmes dans [!DNL Slack], voir [Gestion de vos problèmes à partir de [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Facultatif) Cliquez sur **[!UICONTROL Approbations]** pour afficher toutes les validations en attente de votre décision.\
   Pour plus d’informations sur la gestion de vos validations dans [!DNL Slack], voir [Gérez vos approbations depuis [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Gérez vos tâches depuis [!DNL Slack] {#manage-your-tasks-from-slack}

1. Connectez-vous à [!DNL Slack] et connectez-vous à [!DNL Workfront] de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] de [!DNL Slack], voir &quot;Connexion à [!DNL Workfront] de [!DNL Slack]&quot; dans la section [Accès [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir l&#39;une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Tâches]**

   Ou

   `/workfront tasks`

   >[!NOTE]
   >
   >* Les commandes sont sensibles à la casse.
   >* Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.


   Les 20 premières tâches de votre liste s’affichent.

1. Cliquez sur **[!UICONTROL +`<remaining number>` more]** pour afficher d’autres tâches.
1. Pensez à consulter les informations suivantes sur vos tâches :

   * **[!UICONTROL Nom]**
   * **[!UICONTROL Nom du projet]** ou **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** de l’élément de travail.
   * **[!DNL Assigned By Name]**: il s’agit du nom de l’utilisateur qui vous a assigné la tâche.
   * **[!UICONTROL Statut]**

1. (Facultatif) Cliquez sur le nom d’un élément pour l’ouvrir dans Workfront dans un onglet de navigateur distinct.
1. (Facultatif) Dans le **[!UICONTROL État]** , sélectionnez un nouvel état.
1. (Facultatif) Cliquez sur **[!UICONTROL Temps journal]**, puis sélectionnez une **[!UICONTROL Type d’heure]** et une heure pour le temps de connexion de l’élément.

   >[!NOTE]
   >
   >* Vous ne pouvez consigner les heures que par incréments d’une demi-heure ou complète, jusqu’à 12 heures et 30 minutes.
   >* Les heures que vous enregistrez ont une date d’entrée d’aujourd’hui. Vous ne pouvez pas consigner l’heure pour une date passée ou future à partir de [!DNL Slack].


   Vous recevez une confirmation que l’heure a été enregistrée.

1. (Facultatif) Cliquez sur **[!UICONTROL Travailler dessus]** accepter de travailler sur une tâche. Le [!UICONTROL Travailler dessus] disparaît.

## Gérez vos problèmes depuis [!DNL Slack] {#manage-your-issues-from-slack}

1. Connectez-vous à [!DNL Slack] et connectez-vous à [!DNL Workfront] de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] de [!DNL Slack], reportez-vous à la section [Connexion à [!DNL Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir l&#39;une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Problèmes]**

   Ou

   `/workfront issues`

   >[!NOTE]
   >
   >* Les commandes sont sensibles à la casse.
   >* Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.


   Les 20 premiers problèmes de votre liste s’affichent.

1. Cliquez sur **[!UICONTROL + restant `<number>` more]** pour afficher d’autres éléments.
1. Pensez à consulter les informations suivantes sur vos tâches :

   * **[!UICONTROL Nom]**
   * **[!UICONTROL Projet]** Nom ou nom de l’objet parent
   * **[!UICONTROL Échéance le]** Date : Il s’agit de la date d’achèvement planifiée de l’élément de travail.
   * **[!DNL Requested by]** Nom : Il s’agit du contact Principal (pour les problèmes) ou de l’utilisateur qui a effectué l’affectation (pour les tâches).

1. (Facultatif) Cliquez sur le nom du problème pour l’ouvrir dans Workfront dans un onglet de navigateur distinct.
1. (Facultatif) Cliquez sur **[!DNL Work on it]** pour commencer à travailler sur des problèmes que vous n’avez pas encore acceptés.

   Le [!UICONTROL Travailler dessus] disparaît.

## Gérez vos approbations depuis [!DNL Slack] {#manage-your-approvals-from-slack}

1. Connectez-vous à [!DNL Slack] et connectez-vous à [!DNL Workfront] de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] de [!DNL Slack], voir &quot;Connexion à [!DNL Workfront] de [!DNL Slack]&quot; dans la section [Accès [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir l&#39;une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Approbations]**

   Ou

   `/workfront approvals`

   >[!NOTE]
   >
   >* Les commandes sont sensibles à la casse.
   >* Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.


   Les 20 premiers éléments de votre **[!UICONTROL Approbations]** affichage de la liste. Des informations supplémentaires sur les éléments s’affichent également, telles que le nom de l’utilisateur qui l’a demandé ou le nom du projet auquel l’élément appartient.

1. Cliquez sur **[!UICONTROL + restant `<number>` more]** pour afficher d’autres éléments.

1. Envisagez de gérer les validations pour les objets suivants :

   * **Projets**

      Cliquez sur **[!UICONTROL Approuver]** ou **[!UICONTROL Rejeter]** pour accepter ou refuser le changement d’état d’un projet.

   * **Tâches**

      Cliquez sur **[!UICONTROL Approuver]** ou **[!UICONTROL Rejeter]** pour accepter ou refuser le changement d’état d’une tâche.

   * **Événements**

      Cliquez sur **[!UICONTROL Approuver]** ou **[!DNL Reject]** pour accepter ou refuser le changement d’état d’un problème.

   * **Documents**

      Cliquez sur **[!UICONTROL Approuver]** pour approuver un document, **[!UICONTROL Rejeter]** pour le rejeter, ou **[!UICONTROL Modifications]** pour indiquer que vous l’approuvez, mais que le document nécessite des modifications supplémentaires.\
      (Facultatif) Placez le pointeur de la souris sur la miniature du document pour cliquer sur la loupe et prévisualiser le document.

   * **Bons à tirer**&#x200B; Cliquez sur le nom du BAT pour l’ouvrir dans [!DNL Workfront] dans un onglet distinct et gérez la validation.
   * **Demandes d&#39;accès**

      Cliquez sur **[!UICONTROL Accorder l’accès]** pour accorder des autorisations améliorées à l’objet demandé, ou **[!UICONTROL Ignorer]** pour ignorer la demande d’accès supplémentaire.

1. (Facultatif) Cliquez sur le nom de l’objet soumis à validation pour l’ouvrir dans [!DNL Workfront] dans un nouvel onglet du navigateur.
