---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migration du connecteur hérité ou amélioré vers Workfront pour l’intégration Adobe Experience Manager as a Cloud Service
description: Les informations de cette page expliquent les bonnes pratiques à appliquer pour passer de Workfront pour les connecteurs hérités ou améliorés Experience Cloud à la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Migration du connecteur hérité ou amélioré vers Workfront pour l’intégration Adobe Experience Manager as a Cloud Service

Les informations de cette page expliquent les bonnes pratiques à appliquer pour passer de Workfront pour les connecteurs hérités ou améliorés Experience Cloud à la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Ces informations ne s’appliquent pas aux clients qui utilisent des environnements Adobe Experience Manager Assets On-Premise ou Managed Services.

## Déplacez votre instance Workfront vers le Admin Console

Les clients qui ont l’intention d’utiliser la nouvelle intégration native entre Workfront et Adobe Experience Manager Assets as a Cloud Service doivent s’assurer que leur environnement Workfront est lié à un Adobe Admin Console. Pour les environnements Workfront existants, cela nécessitera probablement une migration de l’environnement vers un Adobe Admin Console connecté. Pour plus d’informations sur cette migration et la liste de contrôle associée, voir [Préparation à l’intégration de votre organisation à Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe doit contribuer à cette migration. Pour demander de l’aide, effectuez l’une des opérations suivantes :

* Si vous disposez d’un accès à Workfront Hub, envoyez votre demande à l’ [Migration de Workfront vers Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Si vous ne disposez pas d’un accès à Workfront Hub, vous pouvez envoyer votre demande à la variable [File d’attente des demandes de migration anticipée de Workfront vers Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Configuration de votre nouvelle intégration Workfront pour Adobe Experience Manager Assets as a Cloud Service

Une fois la migration de votre environnement Workfront vers un Adobe Admin Console effectuée, les administrateurs Workfront peuvent configurer la nouvelle intégration native. Pour obtenir de l’aide sur la configuration, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Déplacer des ressources existantes vers votre intégration Workfront pour Adobe Experience Manager Assets as a Cloud Service

Une fois votre environnement configuré, vous pouvez déplacer les ressources et dossiers liés existants vers Adobe Experience Manager. Il s’agit d’une étape facultative, mais qui garantit que les dossiers et les ressources précédemment liés par le biais du connecteur hérité ou amélioré seront toujours accessibles une fois ces connecteurs désinstallés.

Pour plus d’informations sur le déplacement de vos ressources, voir [Migration des dossiers et documents liés](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validation de tous les cas d’utilisation critiques prévus

Il sera important de valider tous les cas d’utilisation critiques destinés à être utilisés via l’intégration native avant de désinstaller l’ancien connecteur ou le connecteur amélioré.

## Désinstaller le connecteur hérité ou amélioré

Enfin, vous devez désinstaller le connecteur hérité ou amélioré. L’intégration native n’est pas destinée à s’exécuter en parallèle avec l’un ou l’autre des connecteurs.

Pour désinstaller, voir

* Instructions de désinstallation du connecteur hérité : [Désinstallation de Workfront avec Adobe Experience Manager legacy connector](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Instructions de désinstallation du connecteur améliorées : [Désinstallation de Workfront avec Adobe Experience Manager Enhanced Connector](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
