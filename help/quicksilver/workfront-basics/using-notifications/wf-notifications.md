---
content-type: overview;reference
navigation-topic: notifications
title: Présentation des notifications
description: Adobe Workfront envoie des notifications par courrier électronique, des notifications in-app et des notifications sur votre périphérique mobile.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# Présentation des notifications

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] envoie des notifications par e-mail, des notifications in-app et des notifications sur votre appareil mobile.

## Notifications par e-mail

[!DNL Workfront] envoie des notifications par courrier électronique pour alerter les utilisateurs sur l’activité dans Workfront et fournit des informations et des liens utiles.

Pour modifier les préférences de vos notifications par e-mail, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Si vous souhaitez recevoir des notifications par courrier électronique de l’environnement Sandbox, vous devez activer les courriers électroniques de votre profil utilisateur dans cet environnement.

Vous pouvez recevoir les notifications par e-mail suivantes de [!DNL Workfront]:

* [Notifications d’événements](#event-notifications)
* [Notifications de condensation quotidiennes](#daily-digest-notifications)
* [Notification des commentaires publiés](#notification-of-posted-comments)
* [Rappels automatiques](#automatic-reminders)
* [Notifications de rappel](#reminder-notifications)
* [Notifications des panoramas](#boards-notifications)
* [Autre [!DNL Workfront] emails](#other-workfront-emails)

### Notifications d’événements

Les notifications d’événement sont généralement déclenchées par certains événements prédéfinis, par exemple lorsqu’une tâche vous est affectée ou qu’une réponse est reçue sur un commentaire.

Une fois les notifications d’événement activées dans votre [!DNL Workfront] par votre [!DNL Workfront] administrateur ou administrateur de groupe, vous pouvez sélectionner ceux que vous souhaitez recevoir en modifiant votre [!UICONTROL Notifications] préférences dans votre profil utilisateur. Vous pouvez également choisir de recevoir des notifications au fur et à mesure des événements ou de recevoir des événements résumés dans un courrier électronique de résumé quotidien.

Il se peut que vous ne voyiez qu’un sous-ensemble de ces notifications dans vos paramètres, selon la manière dont la variable [!DNL Workfront] l’administrateur a configuré des notifications d’événement pour votre [!DNL Workfront] système. Pour plus d’informations, voir [Configuration des notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

L’état par défaut indique les notifications (quotidiennes, instantanées ou les deux) activées par défaut pour les nouveaux utilisateurs lorsque vous créez les nouveaux utilisateurs.

Pour obtenir la liste complète des notifications d’événement et des informations sur leur activation et leur configuration au niveau du système, du groupe ou de l’utilisateur, voir [Notifications d’événements disponibles dans [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Pour plus d’informations sur le choix des notifications d’événement que vous souhaitez recevoir, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Les notifications d’événement sont les seules notifications qui peuvent être configurées pour être diffusées dans des mises à jour de résumé quotidiennes.

### Notifications de condensation quotidiennes

Une notification condensée quotidienne est un email contenant toutes les notifications d’un certain type que vous avez reçues dans les 24 heures précédant l’e-mail.

Pour obtenir la liste complète des notifications électroniques qui ont été activées pour une diffusion de courrier électronique condensé quotidienne, ainsi que des informations sur toutes les catégories de notifications électroniques, voir [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] n’envoie aucune notification de résumé quotidien pour la variable [!UICONTROL Divers] et [!DNL Goals] catégories d’événements. Vous ne pouvez pas désactiver les notifications quotidiennes pour ces catégories.

Plusieurs éléments doivent être pris en compte lors de la réception de notifications de résumé quotidiennes :

* Chaque [!UICONTROL notifications] dans votre section **[!UICONTROL Mes paramètres]** génère son propre courrier électronique de résumé quotidien. Vous pouvez avoir autant d’emails de résumé quotidiens par jour que de paramètres de notification activés pour les emails de résumé quotidiens.\
   Par exemple, si vous avez choisi de recevoir un courrier électronique de résumé quotidien pour plusieurs actions sous le **[!UICONTROL Informations sur les projets I] À lui,** vous recevez une notification par e-mail répertoriant tous les événements rencontrés pour cette zone.

* Les notifications d’un email de résumé quotidien sont regroupées selon différents critères. Par exemple, dans le cas de **[!UICONTROL Informations sur les projets que je possède]**, les événements sont regroupés par nom de projet.

  Pour le **[!UICONTROL Communication]** , les notifications sont regroupées par objet sur lequel la communication a eu lieu.

  >[!NOTE]
  >
  >Pour la catégorie Communication , vous ne pouvez sélectionner que des notifications individuelles pour une diffusion instantanée. Pour que les notifications soient diffusées dans un résumé quotidien, vous devez tous les sélectionner.

* Le courrier électronique de résumé quotidien répertorie les événements qui se sont produits pour les actions dans un domaine particulier (comme **Informations sur les projets que je possède**) dans les 24 heures précédant le moment choisi pour la diffusion.
* Le fuseau horaire de l’heure sélectionnée pour la diffusion condensée quotidienne correspond à votre fuseau horaire, tel qu’il est configuré sur votre navigateur.
* Le nom de la section de l’objet est indiqué dans les messages de résumé quotidiens, ainsi que la date de leur diffusion.
* Au moins un événement doit déclencher une notification pour que le résumé quotidien soit diffusé. Les digestifs quotidiens ne sont pas envoyés si aucun événement marqué pour les emails de résumé quotidien n’est satisfait.

### Notification des commentaires publiés

Les notifications de la variable [!UICONTROL Communication] catégorie vous alerte aux commentaires qui ont été publiés dans la [!UICONTROL Mettre à jour] flux d’un élément spécifique.

Courriers électroniques de résumé quotidiens pour [!UICONTROL Communication] sont sélectionnées pour toutes les notifications disponibles.

Les informations sont résumées pour l’objet sur lequel la communication a eu lieu et un nombre total de messages de communication s’affiche pour chaque objet.

Pour répondre au commentaire ou l’afficher dans Workfront :

1. Cliquez sur le bouton **[!UICONTROL Commentaire]** dans l’email.

   La variable [!UICONTROL Mises à jour] s’ouvre, avec le commentaire spécifique indiqué en bleu.

   Une boîte de réponse est ouverte, que vous pouvez utiliser pour répondre au commentaire.

Pour plus d’informations sur la configuration des notifications par e-mail, y compris l’activation des notifications de résumé quotidiennes, voir [Afficher et modifier vos paramètres de notification électronique](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) in [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Rappels automatiques

Les rappels automatiques sont activés par votre [!DNL Workfront] l’administrateur pour vous alerter des tâches et des problèmes qui sont dus, en retard ou près de la date d’achèvement prévue. Pour les notifications en retard, l’email est envoyé de nuit jusqu’à ce que la tâche ou le problème soit terminé. Une fois que l’administrateur les a configurés, vous ne pouvez pas les désactiver. En outre, vous ne pouvez pas modifier le contenu ou l’objet d’un email déclenché par un rappel automatique.

Ils peuvent être envoyés à l’une ou plusieurs des ressources suivantes :

* Utilisateurs affectés à une tâche ou à un problème
* Gestionnaire immédiat de l’utilisateur
* Le responsable du responsable immédiat

Les courriers électroniques de rappel automatiques sont envoyés à partir de l’adresse électronique que votre [!DNL Workfront] administrateur sélectionné pour gérer les emails sortants.

Selon le type de rappel automatique activé, les informations suivantes sont disponibles dans l&#39;email de rappel automatique :

* Date de création de la tâche ou du problème
* Nom de la tâche ou du problème
* Nom du projet dans lequel réside la tâche ou le problème.
* Description de la tâche ou du problème
* Liste des utilisateurs affectés à la tâche ou au problème
* Nom de l’utilisateur qui a saisi la tâche ou le problème
* Priorité de la tâche ou du problème
* Date à laquelle la tâche ou le problème est arrivé en retard

Pour plus d’informations sur l’activation des rappels automatiques, voir [Configuration de rappels automatiques](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Notifications de rappel

A [!DNL Workfront] (ou un utilisateur disposant d’un [!UICONTROL Planificateur] niveau d’accès et accès administratif aux notifications de rappel) peut concevoir des notifications de rappel sur l’approche des échéances et les associer manuellement aux projets, tâches, problèmes et feuilles de temps.

>[!IMPORTANT]
>
>Si l’échéance change après qu’un utilisateur a reçu une notification de rappel pour l’un des objets mentionnés ci-dessus, il ne reçoit aucune autre notification de rappel.

Les notifications de rappel sont envoyées à partir de l’adresse électronique que la variable [!DNL Workfront] administrateur sélectionné pour gérer les emails sortants.

Pour plus d’informations sur la configuration et l’activation des notifications de rappel, voir [Configuration des notifications de rappel](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Pour plus d’informations sur la manière d’obtenir l’accès administratif requis, voir [Octroi aux utilisateurs un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Notifications des panoramas

[!DNL Adobe Workfront] [!UICONTROL Panoramas] vous envoie un courrier électronique lorsque vous êtes ajouté à un panorama et lorsqu’une carte vous est attribuée. Vous pouvez sélectionner les e-mails que vous souhaitez recevoir dans les préférences de vos panoramas.

Pour plus d’informations, voir [Forums de notification électronique et préférences](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Autre [!DNL Workfront] emails

Il existe d’autres courriers électroniques que vous pourriez recevoir [!DNL Workfront] qui ne peut pas être configuré.

Les emails suivants sont automatiquement envoyés par [!DNL Workfront] lorsque ces conditions sont remplies :

* Restaurer un élément : lorsque la variable [!DNL Workfront] L’administrateur restaure un objet à partir de la fonction [!UICONTROL Recycler] Bin, un email est envoyé au [!DNL Workfront] administrateur.
* Échec de la restauration : lorsque la variable [!DNL Workfront] L’administrateur tente de restaurer un objet à partir de la corbeille. En cas d’échec de la restauration, un email est envoyé au [!DNL Workfront] administrateur.

Les emails suivants ne peuvent être configurés qu’au niveau du profil utilisateur. Ils ne peuvent pas être activés ni désactivés au niveau du système :

* Fin de la tâche personnelle : lorsqu’une tâche personnelle que vous avez assignée à une autre est terminée, vous recevrez un email.
* Commentaire ajouté à l’utilisateur : lorsque quelqu’un commente votre profil utilisateur, vous recevrez un e-mail.

## Notifications in-app

Vous pouvez recevoir des notifications dans le [!DNL Workfront] application web, lorsque certains événements se produisent.

Pour plus d’informations sur les notifications in-app, voir [Affichage et gestion des notifications in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Notifications par e-mail dans l’application de messagerie mobile

Vous pouvez recevoir [!DNL Workfront] notifications par e-mail dans votre application de messagerie mobile, sur votre appareil mobile.

Si vous avez le [!DNL Workfront] L’application mobile installée sur votre téléphone, en appuyant sur les liens du courrier électronique, les ouvre dans la variable [!DNL Workfront] Application mobile. Vous pouvez notamment appuyer sur l’un des boutons d’action suivants :

* [!UICONTROL Travailler dessus]
* [!UICONTROL Commentaire]
* [!UICONTROL Rendre une décision d’approbation]
* [!UICONTROL Voir Toutes les notifications]
* [!UICONTROL Ajouter]
* [!UICONTROL Prise en main]
* [!UICONTROL Voir Plus de détails]

Pour plus d’informations sur la variable [!DNL Workfront] Application mobile, voir [Utilisez la variable [!DNL Adobe Workfront] application mobile](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
