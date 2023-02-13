---
title: 2.2 Améliorations de l’intégration
description: 2.2 Améliorations de l’intégration
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 2.2 Améliorations de l’intégration

Cette page décrit toutes les améliorations apportées à l’intégration avec la version 22.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 4 avril 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.2, voir [Présentation de la version 2.2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Intégration d’Adobe Workfront avec Anaplan désormais disponible

Pour vous offrir une meilleure flexibilité et une meilleure compréhension des aspects financiers de vos projets Workfront, Workfront peut désormais s’intégrer à votre compte Anaplan. En liant les objets Workfront aux objets Anaplan, vous pouvez mettre à jour automatiquement les informations entre les deux comptes, en vous assurant qu’elles sont à jour et identiques. Vous pouvez également déclencher des processus automatisés dans Anplan en fonction d’actions dans Workfront (ou vice versa).

Vous pouvez par exemple créer une campagne dans Anaplan, puis créer un projet ou un programme Workfront lié à la campagne. Tous les coûts suivis dans Workfront peuvent ensuite être transférés à nouveau vers Anaplan pour passer en revue les performances de la campagne.

D’autres workflows pour lesquels vous pouvez envisager d’utiliser l’intégration Workfront vers Anaplan incluent :

* Création de requêtes de budget Anplan à partir de nouveaux projets Workfront
* Création de projets Workfront à partir des nouveaux éléments de liste Anaplan
* Lancement de demandes de fournisseurs Anaplan à partir de projets Workfront

Pour plus d’informations, voir [Adobe Workfront avec Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Mises à jour du connecteur amélioré pour Workfront

Workfront pour Experience Manager Enhanced Connector comprend désormais les mises à jour suivantes :

* Vous pouvez désormais créer des dossiers liés entre Adobe Workfront et Adobe Experience Manager Assets as a Cloud Service même s’il existe plusieurs configurations de dossiers liés à un projet.
* Ajout de la prise en charge de la pagination des abonnements aux événements
* Ajout de la prise en charge d’AEM 6.4.x
* Ajout de la prise en charge des environnements proxy
* Plusieurs correctifs de bogues basés sur les commentaires des partenaires et des clients

Pour plus d’informations, voir [Présentation du connecteur amélioré pour Workfront for Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>Le déploiement et la configuration de ce connecteur nécessitent un partenaire certifié. Voir [Installation de Workfront pour Experience Manager Enhanced Connector](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) pour plus d’informations.

## Les intégrations Adobe Creative Cloud utilisent désormais OAuth2

Pour une sécurité accrue et pour offrir une expérience plus cohérente entre les intégrations, nous avons mis à jour les intégrations Adobe Creative Cloud afin d’utiliser l’authentification OAuth2, un moyen standard d’authentifier les utilisateurs. Désormais, lorsque vos utilisateurs se connectent, ils peuvent voir les actions et les zones auxquelles les intégrations ont accès et y autoriser l’accès. Après cela, il n’est plus nécessaire de se connecter aussi fréquemment.

Pour plus d’informations, voir [Utilisation de l’extension Workfront pour Illustrator et InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Voir les détails du secret client pour les intégrations OAuth2 ou JWT personnalisées

Pour garantir la transparence de l’utilisation de vos intégrations OAuth2 et JWT personnalisées, nous vous avons permis d’afficher les détails des secrets client que vos intégrations utilisent. Vous pouvez maintenant voir les dates de création et d’utilisation du secret client pour la dernière fois. Vous pouvez également ajouter et afficher vos propres notes sur le secret client.

Auparavant, ces détails n’étaient pas disponibles.

Pour plus d’informations sur les secrets client dans les intégrations personnalisées OAuth2 ou JWT, voir [Création d’applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Voir le type d’authentification dans la liste des applications OAuth2 personnalisées

Désormais, lorsque vous affichez la liste des applications OAuth2 personnalisées dans votre entreprise, vous pouvez voir si chaque application utilise l’authentification de l’utilisateur ou l’authentification du serveur.

Auparavant, vous pouviez afficher ces informations uniquement en accédant aux options de modification de chaque application.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Définition de l’expiration des jetons d’actualisation dans vos intégrations OAuth2 personnalisées

Pour mieux contrôler l’accès et la sécurité de vos intégrations OAuth2 personnalisées, vous pouvez désormais personnaliser la durée de vie des jetons d’actualisation. Une fois que le jeton d’actualisation d’un utilisateur expire, il doit se reconnecter à l’intégration.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Utilisation de clés publiques et privées dans vos intégrations OAuth2 personnalisées pour les applications serveur à serveur

Vous pouvez désormais configurer des applications OAuth2 serveur à serveur dans vos intégrations personnalisées. En configurant des clés publiques et privées, vous pouvez permettre à Workfront de communiquer avec une autre application sans utiliser d’informations de connexion.

Auparavant, toutes les authentifications de vos applications OAuth2 personnalisées utilisaient les informations de connexion de l’utilisateur.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## L’intégration de Google G Suite utilise désormais OAuth2.

Pour une plus grande sécurité et pour offrir une expérience plus cohérente entre les intégrations, nous avons mis à jour l’intégration de Google G Suite afin d’utiliser l’authentification OAuth2, un moyen standard d’authentifier les utilisateurs. Désormais, lorsque vos utilisateurs se connectent, ils peuvent voir les actions et les zones auxquelles les intégrations ont accès et y autoriser l’accès. Après cela, il n’est plus nécessaire de se connecter aussi fréquemment.

Pour plus d’informations, voir [Connexion et déconnexion d’Adobe Workfront for G Suite](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
