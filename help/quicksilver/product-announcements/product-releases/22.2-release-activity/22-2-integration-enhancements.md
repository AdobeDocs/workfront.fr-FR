---
title: Améliorations apportées aux intégrations (version 22.2)
description: Améliorations apportées aux intégrations (version 22.2)
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 93%

---

# Améliorations apportées aux intégrations (version 22.2)

Cette page décrit toutes les améliorations apportées aux intégrations pour l&#39;environnement de prévisualisation de la version 22.2. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

La semaine du 4 avril 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.2, voir [Présentation de la version 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront avec intégration d’Anaplan désormais disponible

Pour vous donner plus de flexibilité et de visibilité sur les aspects financiers de vos projets Workfront, Workfront peut désormais s’intégrer à votre compte Anaplan. En reliant les objets Workfront à ceux d’Anaplan, vous pouvez mettre à jour automatiquement les informations entre les deux comptes, ce qui garantit que les informations contenues dans les deux comptes sont à jour et identiques.
Vous pouvez également déclencher des processus automatisés dans Anaplan sur la base d’actions dans Workfront (et vice versa).

Par exemple, vous pouvez créer une campagne dans Anaplan, puis créer un projet ou un programme Workfront lié à la campagne. Tous les coûts suivis dans Workfront peuvent ensuite être chargés dans Anaplan pour examiner les performances de la campagne.

Voici d’autres workflows pour lesquels vous pourriez envisager d’utiliser l’intégration de Workfront à Anaplan :

* Créer des demandes de budget Anaplan à partir de nouveaux projets Workfront
* Créer des projets Workfront à partir de nouveaux éléments de liste Anaplan
* Initier des demandes de fournisseurs Anaplan à partir de projets Workfront

Pour plus d&#39;informations, voir [Adobe Workfront avec Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Mises à jour du connecteur amélioré de Workfront pour Experience Manager

Le connecteur amélioré de Workfront for Experience Manager comprend désormais les mises à jour suivantes :

* Vous pouvez désormais créer des dossiers liés entre Adobe Workfront et Adobe Experience Manager Assets as a Cloud Service, même s’il existe plusieurs configurations de dossiers liés à un projet.
* Ajout de la prise en charge de la pagination des abonnements aux événements
* Ajout de la prise en charge d’AEM 6.4.x
* Ajout de la prise en charge des environnements proxy
* Plusieurs corrections de bugs basées sur les commentaires des partenaires et de la clientèle

Pour plus d&#39;informations, voir [Vue d’ensemble du connecteur amélioré de Workfront pour Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>Le déploiement et la configuration de ce connecteur nécessitent un partenaire certifié. Pour plus d’informations, voir [Installer le connecteur amélioré de Workfront pour Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install).

## Les intégrations d’Adobe Creative Cloud utilisent désormais OAuth2.

Pour plus de sécurité et une expérience plus cohérente entre les intégrations, nous avons mis à jour les intégrations d’Adobe Creative Cloud pour utiliser l’authentification OAuth2, une méthode standard d’authentification des utilisateurs et utilisatrices. Désormais, lorsque vos utilisateurs et utilisatrices se connectent, ils peuvent voir les actions et les zones spécifiques auxquelles les intégrations ont accès, et en autoriser l’accès. Ensuite, il n’est plus nécessaire de se connecter aussi fréquemment.

Pour plus d’informations, voir [Utiliser l’extension Workfront pour Illustrator et InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Voir les détails du secret client pour les intégrations OAuth2 ou JWT personnalisées.

Afin d’assurer la transparence de l’utilisation de vos intégrations OAuth2 et JWT personnalisées, nous vous avons donné la possibilité de consulter les détails des secrets clients utilisés par vos intégrations. Vous pouvez maintenant voir les dates de création et de dernière utilisation du secret client. Vous pouvez également ajouter et consulter vos propres notes sur le secret client.

Ces informations n’étaient pas disponibles auparavant.

Pour plus d’informations sur les secrets clients dans les intégrations personnalisées OAuth2 ou JWT, voir [Créer des applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Voir le type d’authentification dans la liste des applications OAuth2 personnalisées.

Désormais, lorsque vous consultez la liste des applications OAuth2 personnalisées de votre organisation, vous pouvez voir si chaque application utilise l’authentification de l’utilisateur ou de l’utilisatrice ou l’authentification du serveur.

Auparavant, vous ne pouviez consulter ces informations qu’en accédant aux options de modification de chaque application.

Pour plus d’informations, voir [Créer des applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Définir l’expiration des jetons d’actualisation dans vos intégrations OAuth2 personnalisées

Pour mieux contrôler l’accès et la sécurité de vos intégrations OAuth2 personnalisées, vous pouvez désormais personnaliser la durée de vie des jetons d’actualisation. Après l’expiration du jeton d’actualisation, vous devrez vous reconnecter à l’intégration.

Pour plus d’informations, voir [Créer des applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Utiliser des clés publiques et privées dans vos intégrations OAuth2 personnalisées pour les applications serveur à serveur

Vous pouvez désormais configurer des applications OAuth2 de serveur à serveur dans vos intégrations personnalisées. En configurant des clés publiques et privées, vous pouvez permettre à Workfront de communiquer avec une autre application sans utiliser d’identifiants de connexion.

Auparavant, toutes les authentifications dans vos applications OAuth2 personnalisées utilisaient les identifiants de connexion de l’utilisateur ou utilisatrice.

Pour plus d’informations, voir [Créer des applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## L’intégration de Google Google Workspace utilise désormais OAuth2

Pour plus de sécurité et une expérience plus cohérente entre les intégrations, nous avons mis à jour l’intégration de Google Google Workspace afin d’utiliser l’authentification OAuth2, une méthode d’authentification standard des utilisateurs. Désormais, lorsque vos utilisateurs et utilisatrices se connectent, ils peuvent voir les actions et les zones spécifiques auxquelles les intégrations ont accès, et en autoriser l’accès. Ensuite, il n’est plus nécessaire de se connecter aussi fréquemment.

Pour plus d’informations, voir [Connexion et déconnexion à Adobe Workfront for Google Workspace](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
