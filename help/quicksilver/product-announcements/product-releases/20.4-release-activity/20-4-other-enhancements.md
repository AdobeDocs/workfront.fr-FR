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
ht-degree: 0%

---

# 20.4 Autres améliorations

Cette page décrit toutes les autres améliorations apportées à la version 20.4 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production durant la semaine du 9 novembre 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 20.4, voir [Présentation de la version 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nouveau pour les administrateurs : option Changement d’environnement Workfront disponible

Pour une expérience plus efficace et plus pratique, les administrateurs de groupe et les administrateurs de Workfront peuvent désormais basculer rapidement entre différents environnements Workfront à partir de n’importe quelle page de Workfront sans avoir à se déconnecter.

Dans la nouvelle expérience Workfront, l’option Passer à Classic apparaît dans le menu principal.

Dans Workfront Classic, l’option Basculer vers la nouvelle expérience apparaît dans le menu qui s’affiche lorsque vous cliquez sur l’image de profil dans le coin supérieur droit de la barre de navigation globale.

Cette fonctionnalité est désormais incluse dans la variable [Principes fondamentaux de l’administrateur, partie 1 du parcours d’apprentissage](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) sur Workfront One.

## Amélioration du chiffrement du BAT Workfront

Nous apportons quelques modifications afin d’améliorer la force du chiffrement des données en mouvement de l’application de vérification de Workfront. Les chiffrements TLS faibles seront abandonnés le 11 novembre 2020.

Assurez-vous d’utiliser un navigateur pris en charge lors de l’accès à Workfront. Pour plus d’informations sur les navigateurs pris en charge, voir [Configuration requise pour le navigateur Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).

## Nouvelle apparence pour 3 modèles d’email

Pour améliorer la lisibilité et l’expérience globale, les modèles d’email suivants ont une nouvelle apparence :

* Nouvelle demande de travail
* Une tâche dépendante à laquelle vous êtes affecté est maintenant prête à démarrer
* Notification par e-mail de l’équipe avec le prédécesseur terminé

Pour activer les emails à des fins de test dans votre environnement Aperçu, reportez-vous à la section Gestion des emails dans l’aperçu dans la section [Modifier vos propres notifications électroniques](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Nouvelles notifications électroniques pour les équipes

Nous avons ajouté la notification électronique suivante pour les équipes :

* Un prédécesseur d&#39;une tâche affectée à mon équipe est terminé : l&#39;équipe affectée reçoit une notification par email lorsqu&#39;un prédécesseur de l&#39;une de ses tâches est marqué comme terminé.
* Tous les prédécesseurs d&#39;une tâche affectée à mon équipe sont terminés : l&#39;équipe affectée reçoit une notification par email pour chaque prédécesseur marqué comme terminé.

Pour plus d’informations, voir [Notifications : informations sur le travail qui m’est assigné](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Nouveautés pour les administrateurs : améliorations apportées aux notifications électroniques

Désormais, en un seul clic, vous pouvez activer ou désactiver une notification électronique d’événement dans Configuration. Il vous suffit de cliquer sur l’icône Activé/Désactivé en regard du nom de la notification.

Notez également notre mise en forme moderne qui améliore désormais l’expérience de configuration des notifications d’événement dans la zone Notifications par e-mail .

Pour plus d’informations sur la configuration des notifications par courrier électronique, voir [Configuration des notifications d’événement pour tous les membres du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Cette fonctionnalité est désormais incluse dans la variable [Chemin d’apprentissage des notifications par e-mail et in-app](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) sur Workfront One.

## Nouveaux objets API qui déclenchent les mises à jour d’abonnement aux événements

Deux nouveaux objets API, documentVersion et BATApproval, ont été créés et sont configurés pour déclencher des mises à jour d’abonnement à un événement lorsqu’un document est versionné ou approuvé.

Pour obtenir la liste complète des champs associés à chaque objet, voir [Champs de ressource d’abonnement à un événement](../../../wf-api/api/event-sub-resource-fields.md).
