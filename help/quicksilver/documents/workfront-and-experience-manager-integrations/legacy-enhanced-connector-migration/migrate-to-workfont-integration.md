---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrer à partir des connecteurs hérité ou amélioré vers Workfront pour l’intégration d’Adobe Experience Manager as a Cloud Service
description: Les informations de cette page expliquent les bonnes pratiques pour passer des connecteurs améliorés ou hérités de Workfront pour Experience Cloud à la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: f381b37e6d4537e6f83e55ed4a2f4ff7f868dd54
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 94%

---

# Migrer à partir des connecteurs hérité ou amélioré vers Workfront pour l’intégration d’Adobe Experience Manager as a Cloud Service

Les informations de cette page expliquent les bonnes pratiques pour passer des connecteurs améliorés ou hérités de Workfront pour Experience Cloud à la dernière intégration native connectant Workfront et Adobe Experience Manager Assets as a Cloud Service.

>[!IMPORTANT]
>
>Ces informations ne s‘appliquent pas aux personnes qui utilisent les environnements Adobe Experience Manager Assets On-Premise ou Managed Services.

## Déplacer votre instance Workfront vers Admin Console

>[!IMPORTANT]
>
>Comme toutes les organisations Workfront ont été migrées vers Adobe Admin Console, cette section sera supprimée prochainement.

<!--DELETE THIS SECTION MARCH 2026-->

<!--
Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

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
