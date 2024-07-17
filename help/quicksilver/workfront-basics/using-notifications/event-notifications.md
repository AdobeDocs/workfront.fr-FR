---
content-type: overview
navigation-topic: notifications
title: Notifications d’événements
description: Les notifications d’événement sont des emails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches ou des problèmes. Elles sont envoyées lorsque quelque chose se produit sur le projet que les autres doivent connaître. Selon l’événement, les utilisateurs reçoivent des notifications instantanées, quotidiennes ou instantanées et quotidiennes à leur sujet.
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 16%

---

# Notifications d’événements

Les notifications d’événement sont des emails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches ou des problèmes. Elles sont envoyées lorsque quelque chose se produit sur le projet que les autres doivent connaître. Selon l’événement, les utilisateurs reçoivent des notifications instantanées, quotidiennes ou instantanées et quotidiennes à leur sujet.

>[!NOTE]
>
>Les notifications d’événement sont l’un des types de notifications [!DNL Adobe Workfront]. Pour plus d&#39;informations sur tous les types de notifications [!DNL Workfront], voir [[!DNL Adobe Workfront] notifications](../../workfront-basics/using-notifications/wf-notifications.md).

## Configuration des notifications d’événement

Les emails de notification d’événement peuvent être configurés aux niveaux suivants. La configuration d’une notification d’événement consiste à l’activer ou la désactiver.

* **Niveau du système** : un administrateur [!DNL Workfront] peut activer et désactiver des notifications d’événement au niveau du système, comme expliqué dans la section [Configurer les notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Tous les groupes héritent des notifications système par défaut, mais les administrateurs de groupe peuvent être en mesure de modifier certaines configurations au niveau du groupe, si l’administrateur [!DNL Workfront] l’autorise, comme expliqué dans l’élément de puce suivant ci-dessous.

* **Niveau de groupe** : un administrateur de groupe peut configurer une notification d’événement pour les groupes qu’il gère après qu’un administrateur [!DNL Workfront] a déverrouillé cette fonctionnalité pour les groupes. S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour les administrateurs [!DNL Workfront] (pour n&#39;importe quel groupe). Pour plus d’informations, voir [Afficher et configurer des notifications d’événement pour un groupe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Cette fonctionnalité n’est disponible dans un premier temps que pour les clientes et clients du cluster 4, dans le cadre d’un déploiement progressif. Elle sera disponible dans d’autres clusters peu de temps après. Cet article sera mis à jour au fur et à mesure.

* **Niveau utilisateur** : toutes les notifications d’événement activées à l’échelle du système sont répertoriées dans la section [!UICONTROL Notifications] de chaque utilisateur sur son profil individuel. Les utilisateurs peuvent y activer et désactiver leurs notifications d’événement individuelles.

  Les administrateurs de [!DNL Workfront] et les utilisateurs ayant accès à la modification d’autres utilisateurs peuvent également activer et désactiver des notifications dans le profil d’utilisateurs individuels.

  Pour plus d’informations, consultez [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Les notifications au niveau de l’utilisateur incluent également des notifications [!DNL Workfront Goals]. Cependant, l&#39;administrateur [!DNL Workfront] ou l&#39;administrateur de groupe ne peut pas configurer de notifications pour [!DNL Workfront Goals]. Chaque utilisateur doit configurer ses propres notifications [!DNL Workfront Goals] dans son profil. Si vous avez accès à la modification des utilisateurs, vous pouvez également modifier ces notifications pour d’autres utilisateurs. Pour activer les notifications [!DNL Workfront Goals] pour votre profil ou pour les autres utilisateurs que vous avez accès à la modification, voir [Notifications : objectifs](../../workfront-basics/using-notifications/notifications-goals.md).

  Pour plus d&#39;informations sur les notifications que l&#39;administrateur [!DNL Workfront] peut configurer, voir [Configuration des notifications d&#39;événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] sont disponibles uniquement dans la nouvelle expérience [!DNL Adobe Workfront].

## Contenu des notifications d’événement

Un email de notification d’événement contient des informations sur l’événement qui s’est produit et contient un lien vers [!DNL Workfront] où vous pouvez voir l’événement dans le système. Pour plus d’informations sur la réception de notifications par e-mail, voir [[!DNL Adobe Workfront] notifications](../../workfront-basics/using-notifications/wf-notifications.md).

Un administrateur [!DNL Workfront] ne peut pas modifier le contenu des notifications électroniques, car elles sont configurées par [!DNL Workfront]. Cependant, ils peuvent modifier l’objet des emails de notifications d’événement. Pour plus d’informations, voir [Personnalisation des sujets de courrier électronique pour les notifications d’événement](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Pour obtenir la liste de toutes les notifications d’événement [!DNL Workfront], ainsi qu’une brève description de chaque événement, et déterminer s’il est actif ou inactif par défaut, voir [Notifications d’événement disponibles dans [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
