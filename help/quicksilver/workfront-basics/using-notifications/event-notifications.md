---
content-type: overview
navigation-topic: notifications
title: Notifications d’événements
description: Les notifications d’événement sont des e-mails déclenchés par différents types d’événements sur des objets tels que des projets, des tâches ou des problèmes. Elles sont envoyées lorsqu’il se passe quelque chose sur le projet et que d’autres personnes doivent en être informées. En fonction de l’événement, les personnes reçoivent des notifications instantanées, quotidiennes ou à la fois instantanées et quotidiennes par e-mail.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 100%

---

# Notifications d’événements

Les notifications d’événement sont des e-mails déclenchés par différents types d’événements sur des objets tels que des projets, des tâches ou des problèmes. Elles sont envoyées lorsqu’il se passe quelque chose sur le projet et que d’autres personnes doivent en être informées. En fonction de l’événement, les personnes reçoivent des notifications instantanées, quotidiennes ou à la fois instantanées et quotidiennes par e-mail.

>[!NOTE]
>
>Les notifications d’événement sont l’un des nombreux types de notifications d’[!DNL Adobe Workfront]. Pour plus d’informations sur tous les types de notification [!DNL Workfront], voir Notifications [[!DNL Adobe Workfront] ](../../workfront-basics/using-notifications/wf-notifications.md).

## Configurer des notifications d’événement

Les e-mails de notification d’événements peuvent être configurés aux niveaux suivants. La configuration d’une notification d’événement consiste à l’activer ou à la désactiver.

* **Au niveau du système** : un administrateur ou une administratrice [!DNL Workfront] peut activer et désactiver les notifications d’événements au niveau du système, comme expliqué dans [Configurer les notifications d’événement pour toutes les personnes du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Tous les groupes héritent par défaut des notifications du système, mais les administrateurs et administratrices de groupes peuvent être en mesure de modifier certaines configurations au niveau du groupe, si l’administrateur ou l’administratrice [!DNL Workfront] l’autorise, comme l’explique le point suivant.

* **Au niveau du groupe** : une personne chargée de l’administration de groupes peut configurer une notification d’événement pour les groupes qu’elle gère après qu’un administrateur ou une administratrice [!DNL Workfront] a débloqué cette possibilité pour les groupes. S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices [!DNL Workfront] (pour n’importe quel groupe). Pour plus d’informations, voir [Afficher et configurer les notifications d’événement pour un groupe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Cette fonctionnalité n’est disponible dans un premier temps que pour les clientes et clients du cluster 4, dans le cadre d’un déploiement progressif. Elle sera disponible dans d’autres clusters peu de temps après. Cet article sera mis à jour au fur et à mesure.

* **Au niveau des personnes** : toutes les notifications d’événement activées à l’échelle du système sont répertoriées dans la section [!UICONTROL Notifications] de chaque profil individuel. Les personnes peuvent y activer et désactiver leurs notifications d’événement individuelles.

  Les administrateurs et administratrices [!DNL Workfront] et les personnes ayant accès à la modification d’autres utilisateurs et utilisatrices peuvent également activer et désactiver les notifications dans le profil des personnes individuelles.

  Pour plus d’informations, voir [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Les notifications au niveau des personnes comprennent également les notifications [!DNL Workfront Goals]. Cependant, l’administrateur ou l’administratrice [!DNL Workfront] ou de groupes ne peut pas configurer de notifications pour [!DNL Workfront Goals]. Chaque personne doit configurer ses propres notifications [!DNL Workfront Goals] dans son profil. Si vous avez accès à la modification des utilisateurs et utilisatrices, vous pouvez également modifier ces notifications pour d’autres personnes. Pour activer les notifications [!DNL Workfront Goals] pour votre profil ou pour d’autres personnes que vous avez le droit de modifier, voir [Notifications : objectifs](../../workfront-basics/using-notifications/notifications-goals.md).

  Pour plus d’informations sur les notifications que l’administrateur ou l’administratrice [!DNL Workfront] peut configurer, voir [Configurer les notifications d’événements pour toutes les personnes du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Le produit [!DNL Workfront Goals] n’est disponible que dans la nouvelle expérience [!DNL Adobe Workfront].

## Contenu de la notification d’événement

Un e-mail de notification d’événement contient des informations sur l’événement qui a eu lieu et un lien vers [!DNL Workfront] où vous pouvez voir l’événement dans le système. Pour plus d’informations sur la réception de notifications par e-mail, voir Notifications [[!DNL Adobe Workfront] ](../../workfront-basics/using-notifications/wf-notifications.md).

Un administrateur ou une administratrice [!DNL Workfront] ne peut pas modifier le contenu des notifications par e-mail, car elles sont configurées par [!DNL Workfront]. Toutefois, la personne chargée de l’administration peut modifier l’objet des e-mails de notification d’événement. Pour plus d’informations, voir [Personnaliser les sujets des e-mails pour les notifications d’événement](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Pour obtenir une liste de toutes les notifications d’événement sur [!DNL Workfront], ainsi qu’une brève description de chaque événement et savoir s’il est actif ou inactif par défaut, voir [Notifications d’événement disponibles dans  [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
