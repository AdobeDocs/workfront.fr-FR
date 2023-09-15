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
source-wordcount: '553'
ht-degree: 0%

---

# Notifications d’événements

Les notifications d’événement sont des emails déclenchés par divers types d’événements sur des objets tels que des projets, des tâches ou des problèmes. Elles sont envoyées lorsque quelque chose se produit sur le projet que les autres doivent connaître. Selon l’événement, les utilisateurs reçoivent des notifications instantanées, quotidiennes ou instantanées et quotidiennes à leur sujet.

>[!NOTE]
>
>Les notifications d’événement sont de plusieurs types : [!DNL Adobe Workfront] notifications. Pour plus d’informations sur tous les [!DNL Workfront] types de notification, voir [[!DNL Adobe Workfront] notifications](../../workfront-basics/using-notifications/wf-notifications.md).

## Configuration des notifications d’événement

Les emails de notification d’événement peuvent être configurés aux niveaux suivants. La configuration d&#39;une notification d&#39;événement consiste à l&#39;activer ou la désactiver.

* **Niveau système**: A [!DNL Workfront] l’administrateur peut activer et désactiver des notifications d’événement au niveau du système, comme expliqué dans la section [Configuration des notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

  Tous les groupes héritent des notifications système par défaut, mais les administrateurs de groupe peuvent modifier certaines configurations au niveau du groupe, si le [!DNL Workfront] administrateur, comme expliqué dans l’élément de puce suivant ci-dessous.

* **Niveau de groupe**: un administrateur de groupe peut configurer une notification d’événement pour les groupes qu’il gère après un événement [!DNL Workfront] L’administrateur déverrouille cette fonctionnalité pour les groupes. S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour [!DNL Workfront] administrateurs (pour n’importe quel groupe). Pour plus d’informations, voir [Affichage et configuration des notifications d’événement pour un groupe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

  >[!NOTE]
  >
  >Cette fonctionnalité est initialement disponible uniquement pour les clients du cluster 4 dans le cadre d’un déploiement échelonné. Il sera disponible dans d&#39;autres grappes peu de temps après. Cet article sera mis à jour au fur et à mesure.

* **Niveau d’utilisateur**: toutes les notifications d’événement qui sont activées à l’échelle du système sont répertoriées dans les [!UICONTROL Notifications] sur leur profil individuel. Les utilisateurs peuvent y activer et désactiver leurs notifications d’événement individuelles.

  [!DNL Workfront] les administrateurs et les utilisateurs ayant accès à la modification d’autres utilisateurs peuvent également activer et désactiver des notifications dans le profil d’utilisateurs individuels.

  Pour plus d’informations, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >Les notifications au niveau de l’utilisateur incluent également [!DNL Workfront Goals] notifications. Toutefois, la variable [!DNL Workfront] L’administrateur ou l’administrateur de groupe ne peut pas configurer de notifications pour [!DNL Workfront Goals]. Chaque utilisateur doit configurer ses propres [!DNL Workfront Goals] notifications dans leur profil. Si vous avez accès à la modification des utilisateurs, vous pouvez également modifier ces notifications pour d’autres utilisateurs. Pour activer [!DNL Workfront Goals] notifications de votre profil ou d’autres utilisateurs que vous avez accès à la modification, voir [Notifications : objectifs](../../workfront-basics/using-notifications/notifications-goals.md).

  Pour plus d’informations sur les notifications de la variable [!DNL Workfront] l’administrateur peut configurer, voir [Configuration des notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] sont disponibles uniquement dans la nouvelle [!DNL Adobe Workfront] expérience.

## Contenu des notifications d’événement

Un email de notification d’événement contient des informations sur l’événement qui s’est produit et contient un lien vers [!DNL Workfront] où vous pouvez voir l’événement dans le système. Pour plus d’informations sur la réception de notifications par courrier électronique, voir [[!DNL Adobe Workfront] notifications](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] L’administrateur ne peut pas modifier le contenu des notifications électroniques, car elles sont configurées par [!DNL Workfront]. Cependant, ils peuvent modifier l’objet des emails de notifications d’événement. Pour plus d’informations, voir [Personnalisation des sujets des emails pour les notifications d’événement](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

Pour une liste, tous les [!DNL Workfront] notifications d’événement, ainsi qu’une brève description de chaque événement, et indiquant s’il est actif ou inactif par défaut, voir [Notifications d’événements disponibles dans [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
