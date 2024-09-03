---
title: 20.4 Autres améliorations
description: 20.4 Autres améliorations
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 100%

---

# 20.4 Autres améliorations

Cette page décrit toutes les autres améliorations apportées à la version 20.4 vers l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 9 novembre 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 20.4, voir [Vue d’ensemble de la version 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nouveauté pour les administrateurs et les administratrices : option Changer d’environnement Workfront disponible

Afin d’offrir une expérience plus pratique et efficace, les administrateurs et administratrices de groupes et de Workfront peuvent désormais alterner rapidement entre différents environnements Workfront à partir de n’importe quelle page Workfront, sans avoir à se déconnecter.

Dans la nouvelle expérience Workfront, l’option Basculer sur l’expérience Classique apparaît dans le menu principal.

Dans Workfront Classic, l’option Basculer sur la nouvelle expérience apparaît dans le menu qui s’affiche lorsque vous cliquez sur l’image de profil dans le coin supérieur droit de la barre de navigation globale.

Cette fonctionnalité est désormais incluse dans [Principes fondamentaux de l’administrateur et de l’administratrice, partie 1 du parcours de formation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) sur Workfront One.

## Amélioration du chiffrement de Workfront Proof

Nous apportons quelques modifications afin d’améliorer la puissance du chiffrement des données en mouvement de l’application Workfront Proof. Les algorithmes de chiffrement TLS faibles deviendront obsolètes le 11 novembre 2020.

Assurez-vous d’utiliser un navigateur pris en charge lors de l’accès à Workfront. Pour plus d’informations sur les navigateurs pris en charge, voir [Configuration requise pour le navigateur Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nouvel aspect pour 3 modèles d’e-mail

Afin d’améliorer la lisibilité et l’expérience globale, les modèles d’e-mail suivants ont un nouvel aspect :

* Nouvelle demande de travail
* Une tâche dépendante qui vous a été affectée est maintenant prête à démarrer.
* Notification par e-mail aux équipes lors de l’achèvement d’une tâche antérieure

Pour activer des e-mails à des fins de test dans votre environnement de prévisualisation, reportez-vous à la section Gérer les e-mails dans l’environnement de prévisualisation dans [Modifier vos propres notifications par e-mail](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Nouvelles notifications par e-mail pour les équipes

Nous avons ajouté la notification par e-mail suivante pour les équipes :

* Une tâche antérieure d’une tâche affectée à mon équipe est terminée : l’équipe affectée reçoit une notification par e-mail lorsqu’une tâche antérieure de l’une de ses tâches est marquée comme terminée.
* Toutes les tâches antérieures d’une tâche affectée à mon équipe sont terminées : l’équipe affectée reçoit une notification par e-mail pour chaque tâche antérieure marqué comme terminée.

Pour plus d’informations, voir [Notifications : informations sur le travail qui m’a été affecté](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Nouveauté pour les administrateurs et administratrices : améliorations apportées aux notifications par e-mail

Vous pouvez désormais activer ou désactiver en un seul clic une notification d’événement par e-mail dans Configuration. Il vous suffit de cliquer sur l’icône Activé/Désactivé en regard du nom de la notification.

Vous remarquerez également que notre style moderne améliore désormais l’expérience de configuration des notifications d’événement dans la zone Notifications par e-mail.

Pour plus d’informations sur la configuration des notifications par e-mail, voir [Configurer les notifications d’événement pour tous les utilisateurs et utilisatrices du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Cette fonctionnalité est désormais incluse dans le [parcours de formation des notifications par e-mail et in-app](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) sur Workfront One.

## Nouveaux objets API déclenchant les mises à jour d’abonnement aux événements

Deux nouveaux objets API, documentVersion et proofApproval, ont été créés et sont configurés pour déclencher des mises à jour d’abonnement à un événement lorsqu’un document est versionné ou approuvé.

Pour obtenir la liste complète des champs associés à chaque objet, voir [Champs de ressources de l’abonnement aux événements](../../../wf-api/api/event-sub-resource-fields.md).
