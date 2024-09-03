---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Gérer votre travail et vos approbations à partir de Slack
description: Vous pouvez accéder à votre liste de travail de l’accueil, la consulter et accepter de travailler sur les tâches et les problèmes, et passer en revue ou prendre des décisions sur les approbations directement à partir de Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 100%

---

# Gérer votre travail et vos approbations à partir de [!DNL Slack]

Après avoir installé [!DNL Adobe Workfront for Slack], vous pouvez effectuer les opérations suivantes :

* Accéder aux éléments de l’[!UICONTROL Accueil] à partir de [!DNL Slack].
* Examiner et accepter de travailler sur les tâches et les problèmes à partir de [!DNL Slack].
* Examiner et prendre des décisions concernant les approbations à partir de [!DNL Slack].

Pour plus d’informations sur la configuration de [!DNL Workfront] avec [!DNL Slack], consultez la section [Configurer [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan <a href="https://www.workfront.com/plans?lang=fr" target="_blank">[!DNL Adobe Workfront]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez l’administration Workfront.

## Conditions préalables

Avant de pouvoir gérer votre travail et vos approbations à partir de [!DNL Slack], vous devez

* configurer [!DNL Workfront for Slack].\
  Pour obtenir des instructions sur la configuration de [!DNL Workfront for Slack], consultez la section [Configurer [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Gérer votre travail à partir de [!DNL Slack]

1. Connectez-vous à l’instance [!DNL Slack], puis à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section « Se connecter à [!DNL Workfront] à partir de [!DNL Slack] » sur la page [Accéder à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Choisissez un canal au choix et commencez à saisir la commande suivante dans le champ de message :

   `/workfront home`

   >[!NOTE]
   >
   >* Les commandes respectent la casse.
   >* Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.

   Les boutons à partir desquels vous pouvez accéder aux listes de vos tâches, problèmes et approbations s’affichent. Cliquez sur l’un des boutons pour afficher les 20 premiers éléments de chaque liste dans [!DNL Slack].

1. (Facultatif) Cliquez sur **[!UICONTROL Tâches]** pour afficher toutes vos tâches.

   Pour plus d’informations sur la gestion des tâches dans [!DNL Slack], consultez la section [Gérer vos tâches à partir de  [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Facultatif) Cliquez sur **[!UICONTROL Problèmes]** pour afficher tous vos problèmes.

   Pour plus d’informations sur la gestion des problèmes dans [!DNL Slack], consultez la section [Gérer vos problèmes à partir de  [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Facultatif) Cliquez sur **[!UICONTROL Approbations]** pour afficher toutes les approbations en attente de votre décision.\
   Pour plus d’informations sur la gestion de vos approbations dans [!DNL Slack], consultez la section [Gérer vos approbations à partir de  [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Gérer vos tâches à partir de [!DNL Slack] {#manage-your-tasks-from-slack}

1. Connectez-vous à l’instance [!DNL Slack], puis à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section « Se connecter à [!DNL Workfront] à partir de [!DNL Slack] » sur la page [Accéder à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Choisissez un canal et commencez à saisir l’une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Tâches]**.

   Ou

   `/workfront tasks`

   >[!NOTE]
   >
   >* Les commandes respectent la casse.
   >* Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.

   Les 20 premières tâches de votre liste s’affichent.

1. Cliquez sur **[!UICONTROL +`<remaining number>` autres]** pour afficher d’autres tâches.
1. Pensez à consulter les informations suivantes sur vos éléments de travail :

   * **[!UICONTROL Nom]**
   * **[!UICONTROL Nom du projet]** ou **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** de l’élément de travail.
   * **[!DNL Assigned By Name]** : il s’agit du nom de la personne qui vous a assigné la tâche.
   * **[!UICONTROL Statut]**

1. (Facultatif) Cliquez sur le nom d’un élément pour l’ouvrir dans Workfront dans un nouvel onglet de navigateur.
1. (Facultatif) Dans le champ **[!UICONTROL Statut]**, sélectionnez un nouveau statut.
1. (Facultatif) Cliquez sur **[!UICONTROL Consigner les heures]**, puis sélectionnez un **[!UICONTROL Type d’heure]** et un nombre d’heures pour consigner les heures passées sur l’élément.

   >[!NOTE]
   >
   >* Vous ne pouvez consigner les heures que par incréments d’une demi-heure ou d’une heure complète, avec un maximum de 12 heures et 30 minutes.
   >* La date d’entrée des heures consignées est la date du jour. Vous ne pouvez pas consigner les heures pour une date passée ou future à partir de [!DNL Slack].

   Vous recevrez une confirmation indiquant que les heures ont bien été consignées.

1. (Facultatif) Cliquez sur **[!UICONTROL Travailler sur cette tâche]** pour effectuer l’action éponyme. Le bouton [!UICONTROL Travailler sur cette tâche] disparaît.

## Gérer vos problèmes à partir de [!DNL Slack] {#manage-your-issues-from-slack}

1. Connectez-vous à votre instance [!DNL Slack], puis à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section [Se connecter à  [!DNL Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Choisissez un canal et commencez à saisir l’une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Problèmes]**.

   Ou

   `/workfront issues`

   >[!NOTE]
   >
   >* Les commandes respectent la casse.
   >* Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.

   Les 20 premiers problèmes de votre liste s’affichent.

1. Cliquez sur **[!UICONTROL + `<number>` autres restants]** pour afficher d’autres éléments.
1. Pensez à consulter les informations suivantes sur vos éléments de travail :

   * **[!UICONTROL Nom]**
   * Nom du **[!UICONTROL projet]** ou nom de l’objet parent
   * **[!UICONTROL Date d’échéance le]** : il s’agit de la date d’achèvement prévue de l’élément de travail.
   * Nom du champ **[!DNL Requested by]** : il s’agit du contact principal (pour les problèmes) ou de la personne responsable de l’affectation (pour les tâches).

1. (Facultatif) Cliquez sur le nom du problème pour l’ouvrir dans Workfront dans un nouvel onglet de navigateur.
1. (Facultatif) Cliquez sur **[!DNL Work on it]** pour commencer à travailler sur des problèmes que vous n’avez pas encore acceptés.

   Le bouton [!UICONTROL Travailler sur cette tâche] disparaît.

## Gérer vos approbations à partir de [!DNL Slack] {#manage-your-approvals-from-slack}

1. Connectez-vous à votre instance [!DNL Slack], puis à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section « Se connecter à [!DNL Workfront] à partir de [!DNL Slack] » sur la page [Accéder à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Choisissez un canal et commencez à saisir l’une des commandes suivantes dans le champ de message :

   `/workfront home`, puis cliquez sur **[!UICONTROL Approbations]**.

   Ou

   `/workfront approvals`

   >[!NOTE]
   >
   >* Les commandes respectent la casse.
   >* Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.

   Les 20 premiers éléments de votre liste d’**[!UICONTROL Approbations]** s’affichent. Des informations supplémentaires sur les éléments s’affichent également, telles que le nom de la personne qui a demandé l’approbation ou le nom du projet auquel l’élément appartient.

1. Cliquez sur **[!UICONTROL + `<number>` autres restants]** pour afficher d’autres éléments.

1. Envisagez de gérer les approbations pour les objets suivants :

   * **Projets**

     Cliquez sur **[!UICONTROL Approuver]** ou sur **[!UICONTROL Rejeter]** pour accepter ou refuser le changement de statut d’un projet.

   * **Tâches**

     Cliquez sur **[!UICONTROL Approuver]** ou sur **[!UICONTROL Rejeter]** pour accepter ou refuser le changement de statut d’une tâche.

   * **Événements**

     Cliquez sur **[!UICONTROL Approuver]** ou sur **[!DNL Reject]** pour accepter ou refuser le changement de statut d’un problème.

   * **Documents**

     Cliquez sur **[!UICONTROL Approuver]** pour approuver un document, sur **[!UICONTROL Rejeter]** pour le rejeter, ou sur **[!UICONTROL Modifications]** pour indiquer que vous l’approuvez, mais que le document nécessite des modifications supplémentaires.\
     (Facultatif) Prévisualisez le document en plaçant le pointeur de la souris sur la miniature du document, puis en cliquant sur la loupe.

   * **Épreuves** Cliquez sur le nom de l’épreuve pour l’ouvrir dans [!DNL Workfront] dans un nouvel onglet et décider de l’approbation.
   * **Demandes d’accès**

     Cliquez sur **[!UICONTROL Accorder l’accès]** pour accorder des autorisations supplémentaires à l’objet demandé, ou sur **[!UICONTROL Ignorer]** pour ignorer la demande d’accès supplémentaire.

1. (Facultatif) Cliquez sur le nom de l’objet envoyé pour approbation pour l’ouvrir dans [!DNL Workfront] dans un nouvel onglet de navigateur.
