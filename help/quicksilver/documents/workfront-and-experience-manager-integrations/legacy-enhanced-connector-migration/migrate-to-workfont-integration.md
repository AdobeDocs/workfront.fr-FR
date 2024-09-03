---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrer à partir des connecteurs hérité ou amélioré vers Workfront pour l’intégration d’Adobe Experience Manager as a Cloud Service
description: Les informations de cette page expliquent les bonnes pratiques pour passer des connecteurs améliorés ou hérités de Workfront pour Experience Cloud à la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 100%

---

# Migrer à partir des connecteurs hérité ou amélioré vers Workfront pour l’intégration d’Adobe Experience Manager as a Cloud Service

Les informations de cette page expliquent les bonnes pratiques pour passer des connecteurs améliorés ou hérités de Workfront pour Experience Cloud à la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Ces informations ne s‘appliquent pas aux personnes qui utilisent les environnements Adobe Experience Manager Assets On-Premise ou Managed Services.

## Déplacer votre instance Workfront vers Admin Console

Les personnes qui souhaitent utiliser la nouvelle intégration native entre Workfront et Adobe Experience Manager Assets as a Cloud Service doivent s’assurer que leur environnement Workfront est lié à une console Adobe Admin Console. Pour les environnements Workfront existants, cela nécessitera probablement une migration de l’environnement vers une console Adobe Admin Console connectée. Pour plus d’informations sur cette migration et la liste de contrôle associée, voir [Préparer l’intégration de votre organisation à Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe doit aider à réaliser cette migration. Pour demander de l’aide, procédez comme suit :

* Si vous avez accès à Workfront Hub, soumettez votre demande à [Migration de Workfront vers Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Si vous n&#39;avez pas accès à Workfront Hub, vous pouvez soumettre votre demande à [File d’attente des demandes de migration anticipée de Workfront vers Adobe Admin Console](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## Configurer votre nouvelle intégration Workfront pour Adobe Experience Manager Assets as a Cloud Service

Une fois que votre environnement Workfront a été migré vers une console Adobe Admin Console, les administrateurs et administratices Workfront peuvent configurer la nouvelle intégration native. Pour obtenir de l’aide pour la configuration, voir [Configurer l&#39;intégration d’Experience Manage Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Déplacer les ressources existantes vers votre intégration Workfront pour Adobe Experience Manager Assets as a Cloud Service

Une fois votre environnement configuré, vous pouvez déplacer les ressources et dossiers liés existants vers Adobe Experience Manager. Cette étape est facultative, mais elle garantit que les dossiers et les ressources précédemment liés par le connecteur hérité ou amélioré resteront accessibles une fois que ces connecteurs auront été désinstallés.

Pour plus d’informations sur le déplacement de vos ressources, voir [Migrer des dossiers et des documents liés](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Valider tous les cas d’utilisation critiques destinés à être utilisés

Il sera important de valider tous les cas d’utilisation importants destinés à être utilisés par l’intégration native avant de désinstaller le connecteur hérité ou amélioré.

## Désinstaller le connecteur hérité ou amélioré

Enfin, vous devez désinstaller le connecteur hérité ou amélioré. L’intégration native n’est pas conçue pour fonctionner en parallèle avec l’un ou l’autre des connecteurs.

Pour les désinstaller, voir

* Instructions de désinstallation du connecteur hérité : [désinstaller Workfront avec le connecteur hérité Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* Instructions de désinstallation du connecteur amélioré : [désinstaller Workfront avec le connecteur amélioré Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
