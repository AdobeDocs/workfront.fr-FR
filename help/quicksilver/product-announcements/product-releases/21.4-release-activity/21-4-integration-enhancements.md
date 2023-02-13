---
title: 21.4 Améliorations de l’intégration
description: 21.4 Améliorations de l’intégration
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 21.4 Améliorations de l’intégration

Cette page décrit toutes les améliorations apportées à l’intégration avec la version 21.4 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 4 octobre 2021.

Pour obtenir la liste de toutes les modifications disponibles avec la version 21.4, voir [Présentation de la version 21.4](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Liaison de documents à partir de Dropbox Business

Nous avons ajouté Dropbox Business en tant qu’intégration de document disponible. Vous pouvez désormais accéder aux documents que vous avez stockés dans Dropbox Business directement depuis Workfront.

Dropbox Business vous permet de lier des documents partagés et de télécharger des documents vers des dossiers partagés. Dropbox (et non Dropbox Business) permet uniquement au propriétaire des documents d’afficher le document dans Workfront.

Votre administrateur Workfront peut activer cette intégration pour votre organisation.

Pour plus d’informations, voir [Liaison de documents à partir d’applications externes](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Pour plus d’informations sur la façon dont un administrateur Workfront peut activer cette option, voir [Configuration des intégrations de documents](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Mises à jour de Workfront pour Slack

Les mises à jour suivantes sont désormais visibles dans l’intégration Workfront for Slack :

* Workfront for Slack a une nouvelle apparence.
* Vous recevez maintenant votre Workfront pour les notifications de Slack en temps réel.

   Par exemple, si vous êtes affecté à une tâche, vous recevez cette notification dès que vous êtes affecté. Auparavant, il pouvait y avoir un délai avant que la notification n’apparaisse en Slack.

Cette mise à jour nécessite que vous réautorisiez votre intégration Workfront for Slack. Pour plus d’informations sur l’autorisation de l’intégration, voir [Configuration d’Adobe Workfront pour Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Pour plus d’informations sur Workfront pour les notifications de Slack, voir [Réception de notifications Adobe Workfront dans Slack](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Pour plus d’informations, voir les détails de l’accès au compte lors de l’obtention du consentement aux intégrations Adobe Workfront

Les écrans de consentement pour les intégrations Adobe Workfront sont désormais mis à jour. Vous pouvez désormais voir les actions et les zones spécifiques auxquelles les intégrations ont accès, afin de mieux comprendre ce à quoi vous accordez l’accès à l’intégration ou à l’application.

Ce nouvel écran de consentement s’applique à toute intégration Adobe Workfront qui utilise OAuth 2.0.

Pour plus d’informations sur des intégrations spécifiques, consultez la documentation de cette intégration.

## L’authentification par clé API n’est plus nécessaire pour les intégrations

Les intégrations Workfront ont récemment commencé à utiliser OAuth2 pour une sécurité et une convivialité plus grandes. Dans le cadre de ce déplacement, Workfront ne nécessite plus de clés d’API pour l’authentification des intégrations.
