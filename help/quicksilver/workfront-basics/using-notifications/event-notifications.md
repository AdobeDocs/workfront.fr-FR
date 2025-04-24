---
content-type: overview
navigation-topic: notifications
title: Notifications d’événements
description: Les notifications d’événement sont des e-mails déclenchés par différents types d’événements sur des objets tels que des projets, des tâches ou des problèmes. Elles sont envoyées lorsqu’il se passe quelque chose sur le projet et que d’autres personnes doivent en être informées. En fonction de l’événement, les personnes reçoivent des notifications instantanées, quotidiennes ou à la fois instantanées et quotidiennes par e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 67%

---

# Notifications d’événements

<!-- Audited: 4/2025 -->

Les notifications d’événement sont des e-mails déclenchés par différents types d’événements sur des objets tels que des projets, des tâches ou des problèmes. Elles sont envoyées lorsqu’il se passe quelque chose sur le projet et que d’autres personnes doivent en être informées. En fonction de l’événement, les personnes reçoivent des notifications instantanées, quotidiennes ou à la fois instantanées et quotidiennes par e-mail.

>[!NOTE]
>
>Les notifications d’événement sont l’un des nombreux types de notifications d’[!DNL Adobe Workfront]. Pour plus d’informations sur tous les types de notification [!DNL Workfront], voir [Présentation des notifications](../../workfront-basics/using-notifications/wf-notifications.md).

## Configurer des notifications d’événement

Les e-mails de notification d’événement peuvent être configurés aux niveaux suivants :

* **Au niveau du système** : un administrateur ou une administratrice [!DNL Workfront] peut activer et désactiver les notifications d’événements au niveau du système, comme expliqué dans [Configurer les notifications d’événement pour toutes les personnes du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Tous les groupes héritent des notifications système par défaut, mais les administrateurs peuvent modifier certaines configurations au niveau du groupe s’ils sont autorisés par l’administrateur [!DNL Workfront].

* **Au niveau du groupe** : une personne chargée de l’administration de groupes peut configurer une notification d’événement pour les groupes qu’elle gère après qu’un administrateur ou une administratrice [!DNL Workfront] a débloqué cette possibilité pour les groupes. S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices [!DNL Workfront] (pour n’importe quel groupe). Pour plus d’informations, voir [Afficher et configurer les notifications d’événement pour un groupe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

* **Au niveau des personnes** : toutes les notifications d’événement activées à l’échelle du système sont répertoriées dans la section [!UICONTROL Notifications] de chaque profil individuel. Les personnes peuvent y activer et désactiver leurs notifications d’événement individuelles.

  [!DNL Workfront] administrateurs et les utilisateurs autorisés à modifier d’autres utilisateurs peuvent également activer et désactiver les notifications dans le profil d’un utilisateur individuel.

  Pour plus d’informations, voir [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Les notifications au niveau des personnes comprennent également les notifications [!DNL Workfront Goals]. Cependant, l’administrateur ou l’administratrice [!DNL Workfront] ou de groupes ne peut pas configurer de notifications pour [!DNL Workfront Goals]. Chaque personne doit configurer ses propres notifications [!DNL Workfront Goals] dans son profil. Si vous avez accès à la modification d’utilisateurs et d’utilisatrices, vous pouvez également modifier ces notifications pour d’autres personnes. Pour activer les notifications [!DNL Workfront Goals] pour votre profil ou pour d’autres personnes que vous avez le droit de modifier, voir [Notifications : objectifs](../../workfront-basics/using-notifications/notifications-goals.md).

  Pour plus d’informations sur les notifications que l’administrateur [!DNL Workfront] peut configurer, voir [Configurer des notifications d’événement pour tous les utilisateurs du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Contenu de la notification d’événement

Un e-mail de notification d’événement contient des informations sur l’événement qui a eu lieu et un lien vers [!DNL Workfront] où vous pouvez voir l’événement dans le système. Pour plus d’informations sur la réception de notifications par e-mail, voir [Présentation des notifications](../../workfront-basics/using-notifications/wf-notifications.md).

Un administrateur [!DNL Workfront] ne peut pas modifier le contenu des notifications par e-mail tel qu’il est configuré par [!DNL Workfront], mais il peut modifier l’objet des notifications par e-mail. Pour plus d’informations, voir [Personnaliser les sujets des e-mails pour les notifications d’événement](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Pour obtenir la liste de toutes les notifications d’événement [!DNL Workfront], ainsi qu’une brève description de chaque événement, et savoir s’il est actif ou inactif par défaut, voir [Types de notification d’événement](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
