---
title: Améliorations de l’intégration dans la version 23.3
description: Améliorations de l’intégration dans la version 23.3
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 94%

---

# Améliorations de l’intégration dans la version 23.3

Cette page décrit toutes les améliorations apportées à l’intégration avec la version 23.3. Ces améliorations ont été mises à disposition dans l’environnement de production avec la version 23.3 les 20 et 21 juillet 2023.

Pour une liste de tous les changements disponibles à ce stade du cycle de publication de la version 23.3, voir [Vue d’ensemble de la version 23.3](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Nouvelle intégration de Google Workspace désormais disponible

Une nouvelle intégration Google Workspace est désormais disponible dans Google Marketplace. La nouvelle intégration s’authentifie à l’aide d’OAuth2 et remplace l’intégration précédente.

L’intégration précédente de Google Workspace est désormais obsolète et sera automatiquement désinstallée.

Pour plus d’informations sur l’installation de la nouvelle intégration, voir [Installer [!DNL Adobe Workfront for Google Workspace]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Pour plus d’informations sur Workfront pour Google Workspace, voir [Workfront pour Google Workspace](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Les intégrations Adobe Creative Cloud prennent désormais en charge plusieurs personnes affectées.

L&#39;intégration d’Adobe Creative Cloud permet désormais de choisir entre « J’ai fait ma part » et « Terminé » (ou « Résolu ») lorsque plusieurs personnes sont affectées à une tâche ou un problème.

Auparavant, l’intégration permettait aux personnes de marquer une tâche comme étant terminée, sans spécifier « J’ai fait ma part » ou « Terminé »/« Résolu ».

Pour tirer parti de cette fonctionnalité, téléchargez et installez les plug-ins les plus récents de Workfront pour Creative Cloud.

Pour plus d’informations sur cette fonctionnalité, voir [Marquer les éléments de travail comme terminés à l’aide du plug-in Adobe Workfront](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Pour plus d’informations sur l’installation des plug-ins Workfront pour Creative Cloud, voir [Installer le plug-in Adobe Workfront pour les applications Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Afficher et gérer des notifications Workfront à partir de Workfront pour les plug-ins Creative Cloud

Afin de vous permettre de recevoir plus facilement les notifications dont vous avez besoin, nous avons rendu possible l’affichage et la gestion des notifications Workfront sans quitter Adobe Creative Cloud. Vous pouvez désormais afficher des notifications, ainsi qu’accéder aux éléments de travail et aux commentaires associés à ces notifications, directement à partir de la fenêtre du plug-in Workfront dans l’application Creative Cloud.

Auparavant, les notifications n’étaient disponibles que dans Workfront et par e-mail.

Pour tirer parti de cette fonctionnalité, téléchargez et installez les plug-ins les plus récents de Workfront pour Creative Cloud.

Pour plus d’informations, voir [Afficher et gérer les notifications [!DNL Adobe Workfront] d’Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Pour plus d’informations sur l’installation des plug-ins Workfront pour Creative Cloud, voir [Installer le plug-in Adobe Workfront pour les applications Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Créer automatiquement des dossiers liés à Adobe Experience Manager Assets lors de la création d’un projet

Avec le nouveau workflow Créer un dossier lié pour l’intégration d’Adobe Experience Manager, vous pouvez configurer l’intégration avec un chemin d’accès à un dossier Adobe Experience Manager Assets. Lorsque l’intégration est ajoutée à un modèle de projet, tout projet créé à partir du modèle crée automatiquement un sous-dossier lié dans Experience Manager Assets dans le dossier spécifié.

Auparavant, la création de dossiers liés nécessitait une action de la part de l’utilisateur ou de l’utilisatrice.

Cette fonctionnalité est disponible uniquement avec une intégration Adobe Experience Manager as a Cloud Service dans Workfront. Cette option n’est pas disponible dans le connecteur amélioré d’Adobe Experience Manager.

Pour plus d’informations, voir [Utiliser des workflows dans l’intégration Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Mapper les valeurs des champs Workfront aux balises dans Experience Manager Assets

Vous pouvez désormais classer et rechercher rapidement des ressources en fonction des données de Workfront. Vous pouvez mapper ces données dans le cadre de votre configuration de métadonnées dans l’intégration Workfront pour Experience Manager Assets.

Auparavant, le mappage des données Workfront aux balises Experience Manager Assets n’était pas disponible.

Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets as a Cloud Service, voir [Configurer l’intégration [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets Essentials, voir [Configurer l’intégration Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Mapper des champs Workfront aux champs de métadonnées Experience Manager Assets personnalisés

Avec l’intégration native, vous pouvez désormais mapper des champs Workfront natifs et intégrés aux champs de schéma de métadonnées personnalisés dans Experience Manager Assets as a Cloud Service.

Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets as a Cloud Service, voir [Configurer l’intégration [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets Essentials, voir [Configurer l’intégration Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Ajuster les paramètres du modèle de workflow d’épreuve automatisé à l’aide d’Adobe Workfront pour Creative Cloud

Vous pouvez désormais ajuster les paramètres des modèles de workflow automatisé existants directement dans Creative Cloud. Une fois que vous avez choisi un modèle de workflow automatisé existant, vous pouvez effectuer ce qui suit :

* Désactiver les étapes
* Ajouter des personnes destinataires supplémentaires
* Modifier les rôles d’épreuve
* Ajuster l’échéance
* Mettre à jour les notifications par e-mail
* et plus...

Pour plus d’informations, voir [Charger des documents et des épreuves à l’aide du plug-in  [!DNL Adobe Workfront]  pour les applications  [!DNL Creative Cloud] ](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Ces améliorations sont disponibles pour les applications Creative Cloud suivantes :

* Photoshop
* XD
* InDesign
* Illustrator
