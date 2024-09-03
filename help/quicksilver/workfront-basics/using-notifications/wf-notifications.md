---
content-type: overview;reference
navigation-topic: notifications
title: Vue d’ensemble des notifications
description: Adobe Workfront envoie des notifications par e-mail, des notifications in-app et des notifications sur votre appareil mobile.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 100%

---

# Vue d’ensemble des notifications

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] envoie des notifications par e-mail, des notifications in-app et des notifications sur votre appareil mobile.

## Notifications par e-mail

[!DNL Workfront] envoie des notifications par e-mail afin d’alerter les utilisateurs et les utilisatrices de l’activité de Workfront et de fournir des informations et des liens utiles.

Pour modifier les préférences de vos notifications par e-mail, consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Pour recevoir des notifications par e-mail de l’environnement sandbox, vous devez activer les e-mails dans votre profil d’utilisateur ou d’utilisatrice dans cet environnement.

Vous pouvez recevoir les notifications suivantes par e-mail de [!DNL Workfront] :

* [Notifications d’événements](#event-notifications)
* [Notifications de synthèse quotidienne](#daily-digest-notifications)
* [Notifications de commentaires postés](#notification-of-posted-comments)
* [Rappels automatiques](#automatic-reminders)
* [Notifications de rappel](#reminder-notifications)
* [Notifications des panoramas](#boards-notifications)
* [Autres e-mails  [!DNL Workfront] ](#other-workfront-emails)

### Notifications d’événements

Généralement, les notifications d’événements sont déclenchées par certains événements prédéfinis, comme l’affectation d’une tâche ou la réception d’une réponse à un commentaire que vous avez fait.

Une fois que votre équipe d’administration [!DNL Workfront] ou de groupes active les notifications d’événements dans votre système [!DNL Workfront], vous pouvez sélectionner celles que vous souhaitez recevoir en modifiant vos préférences de [!UICONTROL notifications] dans votre profil d’utilisateur ou d’utilisatrice. Vous avez également le choix de recevoir des notifications au fur et à mesure des événements, ou de recevoir une synthèse des événements dans un e-mail quotidien.

En fonction de la configuration des notifications d’événements par votre équipe d’administration [!DNL Workfront], il se peut que vous ne voyiez qu’un sous-ensemble de ces notifications dans vos paramètres système [!DNL Workfront]. Pour plus d’informations, consultez la section [Configurer les notifications d’événements pour tous les utilisateurs et les utilisatrices du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Le statut par défaut indique quelles notifications (quotidiennes, instantanées ou les deux) sont activées par défaut pour les nouveaux utilisateurs ou les nouvelles utilisatrices lorsque vous les créez.

Pour consulter une liste complète des notifications d’événements ainsi que des informations sur leur activation et leur configuration au niveau du système, du groupe ou de l’utilisateur ou de l’utilisatrice, consultez la section [Notifications d’événements disponibles dans  [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Pour plus d’informations sur la manière de choisir les notifications d’événements que vous souhaitez recevoir, consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Seules les notifications d’événements peuvent être configurées pour être diffusées sous forme de mises à jour quotidiennes.

### Notifications de synthèse quotidienne

Une notification de synthèse quotidienne est un e-mail contenant toutes les notifications d’un certain type que vous avez reçues au cours des 24 heures précédant l’envoi de l’e-mail.

Pour obtenir une liste complète des notifications par e-mail qui ont été activées pour l’envoi d’une synthèse quotidienne par e-mail, ainsi que des informations sur toutes les catégories de notifications par e-mail, consultez la section [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] n’envoie pas une synthèse quotidienne des notifications pour les catégories d’événements [!UICONTROL Divers] et d’[!DNL Goals]. Vous ne pouvez pas désactiver les notifications quotidiennes pour ces catégories.

Plusieurs points méritent une attention particulière lors de la réception de notifications de synthèse quotidienne :

* Chaque section de [!UICONTROL notifications] de votre panneau **[!UICONTROL Mes paramètres]** génère son propre e-mail quotidien. Vous pouvez recevoir autant d’e-mails quotidiens que le permettent les paramètres de notification activés pour les e-mails quotidiens.\
   Si, par exemple, vous avez opté pour la réception d’une synthèse quotidienne par e-mail concernant plusieurs actions sous la catégorie **[!UICONTROL Informations sur les projets dont je suis propriétaire]**, vous recevrez un e-mail de notification répertoriant tous les événements rencontrés dans cette catégorie.

* Les notifications contenues dans une synthèse quotidienne par e-mail sont regroupées en fonction de différents critères. Par exemple, dans le cas de la catégorie **[!UICONTROL Informations sur les projets dont je suis propriétaire]**, les événements sont regroupés par nom de projet.

  Les notifications pour la catégorie **[!UICONTROL Communication]** sont regroupées en fonction de l’objet concerné par la communication.

  >[!NOTE]
  >
  >Pour la catégorie Communication, vous pouvez sélectionner des notifications individuelles pour une diffusion instantanée uniquement. Pour que les notifications soient diffusées dans une synthèse quotidienne, vous devez toutes les sélectionner.

* La synthèse quotidienne par e-mail répertorie les événements survenus pour les actions dans une catégorie spécifique (comme **Informations sur les projets dont je suis propriétaire**) au cours des 24 heures précédant l’heure sélectionnée pour la diffusion.
* Le fuseau horaire de l’heure sélectionnée pour la diffusion de la synthèse quotidienne par e-mail correspond à celui configuré dans votre navigateur.
* Les e-mails de la synthèse quotidienne contiennent le nom de la catégorie dans la ligne d’objet, ainsi que la date de livraison.
* Pour que la synthèse quotidienne soit diffusée, il faut qu’au moins un événement déclenche une notification. Les synthèses quotidiennes ne sont pas envoyées si aucun des événements pour lesquels des e-mails de synthèses quotidiennes ont été définis n’existe.

### Notifications de commentaires postés

Les notifications de la catégorie [!UICONTROL Communication] vous alertent des commentaires qui ont été publiés dans le flux [!UICONTROL Mettre à jour] d’un élément spécifique.

Les e-mails de synthèse quotidienne de la catégorie [!UICONTROL Communication] sont sélectionnés pour toutes les notifications disponibles.

Les informations sont résumées pour l’objet concerné par la communication et le nombre total de messages de communication est affiché pour chaque objet.

Pour répondre au commentaire ou le consulter dans Workfront :

1. Cliquez sur le bouton **[!UICONTROL Commenter]** dans l’e-mail.

   La zone [!UICONTROL Mises à jour] de l’objet s’ouvre avec le commentaire spécifique souligné en bleu.

   Une zone de réponse s’ouvre, que vous pouvez utiliser pour répondre au commentaire.

Pour plus d’informations sur la configuration des notifications par e-mail, y compris l’activation des notifications de synthèse quotidiennes, voir [Afficher et modifier vos paramètres de notification par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) dans [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Rappels automatiques

Des rappels automatiques sont activés par votre administrateur ou administratrice [!DNL Workfront] pour vous avertir des tâches et des problèmes qui sont dus, en retard ou proches de la date d’achèvement prévue. Pour les notifications de retard, l’e-mail est envoyé chaque nuit jusqu’à ce que la tâche ou le problème soit terminé. Une fois que l’administrateur ou l’administratrice les a configurés, vous ne pouvez pas les désactiver. Vous ne pouvez pas non plus modifier le contenu ou l’objet d’un e-mail déclenché par un rappel automatique.

Ils peuvent être envoyés à un ou plusieurs des destinataires suivants :

* La personne affectée à une tâche ou à un problème.
* La personne responsable directe ou de cette personne.
* La personne responsable de la personne responsable directe.

Les e-mails de rappel automatique sont envoyés à partir de l’adresse e-mail que votre administrateur ou administratrice [!DNL Workfront] a sélectionnée pour traiter les e-mails sortants.

Selon le type de rappel automatique activé, les informations suivantes sont disponibles dans l’e-mail de rappel automatique :

* Date de création de la tâche ou du problème
* Nom de la tâche ou du problème
* Nom du projet dans lequel se trouve la tâche ou le problème
* Description de la tâche ou du problème
* Liste des utilisateurs et utilisatrices affectés à la tâche ou au problème
* Nom de l’utilisateur ou utilisatrice qui a saisi la tâche ou le problème
* Priorité de la tâche ou du problème
* Date à laquelle la tâche ou le problème est devenu en retard

Pour plus d’informations sur l’activation des rappels automatiques, voir [Configurer des rappels automatiques](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Notifications de rappel

Un administrateur ou une administratrice [!DNL Workfront] (ou un utilisateur ou une utilisatrice ayant un niveau d’accès [!UICONTROL Planificateur ou planificatrice] et un accès administratif aux notifications de rappel) peut concevoir des notifications de rappel concernant les échéances proches et les associer manuellement à des projets, des tâches, des problèmes et des feuilles de temps.

>[!IMPORTANT]
>
>Si l’échéance change après qu’un utilisateur ou une utilisatrice a reçu une notification de rappel pour l’un des objets mentionnés ci-dessus, l’utilisateur ou utilisatrice ne reçoit pas de nouvelle notification de rappel.

Les notifications de rappel sont envoyées à partir de l’adresse e-mail que l’administrateur ou administratrice [!DNL Workfront] a sélectionnée pour traiter les e-mails sortants.

Pour plus d’informations sur la configuration et l’activation des notifications de rappel, voir [Configurer des notifications de rappel](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Pour plus d’informations sur la manière d’obtenir l’accès administratif requis, voir [Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Notifications des panoramas

Les [!UICONTROL panoramas] [!DNL Adobe Workfront] vous envoient un e-mail lorsque vous intégrez un panorama et lorsqu’une carte vous est attribuée. Vous pouvez sélectionner les e-mails que vous souhaitez recevoir dans vos préférences de panoramas.

Pour plus d’informations, voir [Notifications par e-mail et préférences des panoramas](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Autres e-mails [!DNL Workfront]

Vous pouvez recevoir d’autres e-mail de [!DNL Workfront] qui ne peuvent pas être configurés.

Les e-mails suivants sont automatiquement envoyés par [!DNL Workfront] lorsque ces conditions sont remplies :

* Restaurer un élément : lorsque l’administrateur ou administratrice [!DNL Workfront] restaure un objet de la [!UICONTROL corbeille], un e-mail est envoyé à l’administrateur ou administratrice [!DNL Workfront].
* Échec de la restauration : lorsque l’administrateur ou administratrice [!DNL Workfront] tente de restaurer un objet de la corbeille et que la restauration échoue, un e-mail est envoyé à l’administrateur ou administratrice [!DNL Workfront].

Les e-mails suivants ne peuvent être configurés qu’au niveau du profil de l’utilisateur ou de l’utilisatrice. Ils ne peuvent pas être activés ou désactivés au niveau du système :

* Achèvement d’une tâche personnelle : lorsqu’une tâche personnelle que vous avez confiée à quelqu’un d’autre est achevée, vous recevez un e-mail.
* Commentaire ajouté à l’utilisateur ou utilisatrice : lorsque quelqu’un commente votre profil d’utilisateur ou d’utilisatrice, vous recevrez un e-mail.

## Notifications in-app

Vous pouvez recevoir des notifications dans l’application web [!DNL Workfront] lorsque certains événements se produisent.

Pour plus d’informations sur les notifications in-app, voir [Afficher et gérer les notifications in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Notifications par e-mail dans l’application de messagerie mobile.

Vous pouvez recevoir des notifications par e-mail [!DNL Workfront] dans votre application de messagerie sur votre appareil mobile.

Si l’application mobile [!DNL Workfront] est installée sur votre téléphone, les liens contenus dans l’e-mail s’ouvrent dans l’application mobile [!DNL Workfront] en tapant dessus. Il s’agit notamment d’appuyer sur l’un des boutons d’action suivants :

* [!UICONTROL Travailler sur ce projet]
* [!UICONTROL Commenter]
* [!UICONTROL Prendre une décision d’approbation]
* [!UICONTROL Afficher toutes les notifications]
* [!UICONTROL Ajouter]
* [!UICONTROL Démarrer]
* [!UICONTROL Voir plus de détails]

Pour plus d’informations sur l’application mobile [!DNL Workfront], voir [Utiliser l’application mobile  [!DNL Adobe Workfront] ](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
