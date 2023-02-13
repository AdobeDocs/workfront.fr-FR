---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Désinstallation du connecteur hérité
description: text
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Désinstallation de Workfront avec Adobe Experience Manager legacy connector

Vous devez désinstaller Workfront avec le connecteur hérité Adobe Experience Manager vers la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.

## Désabonnement de Workfront

1. Ouvrez Adobe Experience Manager.
1. En Experience Manager, accédez à **Outils** > **Cloud Services** > **Configuration de l’intégration Workfront**.
1. Sélectionnez votre configuration (global-workfront par défaut), puis cliquez sur **Propriétés**.
   ![se désabonner de workfront](assets/unsubscribe-from-workfront.png)
1. Désactivez la synchronisation du document, des commentaires et des métadonnées. Le libellé doit être désactivé le jour.
Cela supprime les abonnements dans Workfront et permet à l’utilisateur de créer un abonnement à l’aide de l’URL définie dans Day CQ Link Externalizer.

## Suppression de la configuration de l’intégration Workfront

Après la suppression de l’abonnement, il est désormais possible de supprimer la configuration de l’intégration Workfront en toute sécurité.

1. Ouvrez la configuration, puis sélectionnez **Supprimer**.
   ![configuration de suppression](assets/delete-wf-configuration.png)

## Suppression du mappage

Ensuite, vous devez supprimer le mappage des propriétés Workfront.

1. En Experience Manager, accédez à **Outils** > **Ressources** > **Mappage des propriétés Workfront**.

1. Sélectionnez tous les mappages, puis cliquez sur **Supprimer**.

## Autorisations des utilisateurs

Tous les utilisateurs qui ont accès à AEM Dam à partir de Workfront ont reçu des autorisations de lecture pour `/content/dam`. Si un utilisateur n’en a plus besoin, vous pouvez supprimer les autorisations accordées à ces utilisateurs.

Le connecteur fonctionne à l’aide du service front-service de l’utilisateur système. Cette opération est désinstallée lors de la désinstallation du connecteur.

>[!NOTE]
>
>Si vous utilisez la version 2.0.3 du connecteur et que vous avez ajouté le groupe `workfront-aem-connector-group`, il doit également être supprimé en accédant à **Outils** > **Sécurité** > **Groupes**.

## Externalisateur de lien Day CQ

Si vous n’avez pas besoin de l’externaliseur de liens Day CQ, vous pouvez rétablir cette valeur sur `localhost:4502` en accédant à `/system/console/configMgr` et recherchez &quot;Day CQ Link Externalizer&quot;.

>[!NOTE]
>
>Si vous utilisez Adobe Experience Manager as a Cloud Service, vous pouvez modifier ce paramètre en accédant à votre projet et en localisant le fichier . _com.day.cq.commons.impl.ExternalizerImpl.xml_ inside _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Externalisateur de lien Day CQ](assets/Day-CQ-Link-Externalizer.png)

## Désinstallation du module Connector

Les étapes requises pour désinstaller le package connecteur diffèrent selon la version d’Adobe Experience Manager dont vous disposez.

### Adobe Experience Manager On-Premise

Si vous utilisez Adobe Experience Manager on-premise, accédez à _crx/packmgr/index.jsp_, puis recherchez le `workfront-aem-connector.all-<version>.zip`, cliquez sur **Plus** puis **Désinstaller**.

Veuillez vérifier `/conf` pour vous assurer que tous les fichiers créés par Workfront ont été supprimés.

### Adobe Experience Manager as a Cloud Service

Pour Adobe Experience Manager as a Cloud Service, vous pouvez supprimer les dépendances du connecteur du fichier pom.files du projet.

## Pare-feu et Dispatcher

N’oubliez pas de supprimer vos URL Workfront placées sur la liste autorisée si la communication n’est plus nécessaire. En outre, le connecteur utilise l’apiKey des en-têtes et le nom d’utilisateur qui ont été définis sur Dispatcher. Ils peuvent également être supprimés.
