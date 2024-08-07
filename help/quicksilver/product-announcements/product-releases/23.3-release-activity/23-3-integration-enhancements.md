---
title: Améliorations apportées aux intégrations (version 23.3)
description: Améliorations apportées aux intégrations (version 23.3)
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 4%

---

# Améliorations apportées aux intégrations (version 23.3)

Cette page décrit toutes les améliorations apportées à l’intégration avec la version 23.3. Ces améliorations ont été apportées à l’environnement de production avec la version 23.3 des 20 et 21 juillet 2023.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version 23.3, voir l’article [Vue d’ensemble de la version 23.3](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Nouvelle intégration de Google Workspace désormais disponible

Une nouvelle intégration Google Workspace est désormais disponible dans Google Marketplace. La nouvelle intégration s’authentifie à l’aide d’OAuth2 et remplace l’intégration précédente.

L’intégration précédente de Google Workspace est désormais obsolète et sera automatiquement désinstallée.

Pour obtenir des instructions sur l’installation de la nouvelle intégration, voir [Installation [!DNL Adobe Workfront for Google Workspace]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Pour plus d’informations sur Workfront pour Google Workspace, voir [Workfront pour Google Workspace](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Les intégrations Adobe Creative Cloud prennent désormais en charge plusieurs utilisateurs affectés.

L’intégration de Adobe Creative Cloud prend désormais en charge la possibilité de choisir entre &quot;Terminé avec ma part&quot; et &quot;Terminé&quot; (ou &quot;Résolu&quot;) lorsqu’une tâche ou un problème comporte plusieurs utilisateurs affectés.

Auparavant, l’intégration permettait aux utilisateurs de marquer une tâche comme étant terminée, sans spécifier &quot;Terminé avec ma part&quot; ou &quot;Terminé&quot;/&quot;Résolu&quot;.

Pour tirer parti de cette fonctionnalité, téléchargez et installez les modules externes les plus récents de Workfront for Creative Cloud.

Pour plus d’informations sur la fonctionnalité, voir [Marquer les tâches terminées à l’aide du module externe Adobe Workfront](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Pour plus d’informations sur l’installation des modules externes Workfront for Creative Cloud, voir [Installation du module externe Adobe Workfront pour les applications Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Affichage et gestion des notifications Workfront à partir de Workfront pour les modules externes Creative Cloud

Afin de vous permettre de recevoir plus facilement les notifications dont vous avez besoin, nous avons rendu possible l’affichage et la gestion des notifications Workfront sans quitter Adobe Creative Cloud. Vous pouvez désormais afficher des notifications, ainsi que accéder aux tâches et aux commentaires associés à ces notifications, directement depuis la fenêtre du module externe Workfront dans l’application du Creative Cloud.

Auparavant, les notifications n’étaient disponibles que dans Workfront et par courrier électronique.

Pour tirer parti de cette fonctionnalité, téléchargez et installez les modules externes les plus récents de Workfront for Creative Cloud.

Pour plus d’informations, voir [Affichage et gestion [!DNL Adobe Workfront] des notifications de Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Pour plus d’informations sur l’installation des modules externes Workfront for Creative Cloud, voir [Installation du module externe Adobe Workfront pour les applications Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Création automatique de dossiers liés à Adobe Experience Manager Assets lors de la création d’un projet

Avec le nouveau workflow Créer un dossier lié pour l’intégration de Adobe Experience Manager, vous pouvez configurer l’intégration avec un chemin d’accès à un dossier Adobe Experience Manager Assets. Lorsque l’intégration est ajoutée à un modèle de projet, tout projet créé à partir du modèle crée automatiquement un sous-dossier lié dans Experience Manager Assets dans le dossier spécifié.

Auparavant, la création de dossiers liés nécessitait une action de la part de l’utilisateur.

Cette fonctionnalité est disponible uniquement avec une intégration Adobe Experience Manager as a Cloud Service dans Workfront. Cette option n’est pas disponible dans le connecteur amélioré de Adobe Experience Manager.

Pour plus d’informations, voir [Utilisation des workflows dans l’intégration Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Mappage des valeurs de champ Workfront aux balises dans Experience Manager Assets

Vous pouvez désormais classer et rechercher rapidement des ressources en fonction des données de Workfront. Vous pouvez mapper ces données dans le cadre de votre configuration de métadonnées dans l’intégration de Workfront for Experience Manager Assets.

Auparavant, le mappage des données Workfront aux balises Experience Manager Assets n’était pas disponible.

Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets as a Cloud Service, voir [Configuration de l’ [!UICONTROL intégration Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets Essentials, voir [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Mappage des champs Workfront aux champs de métadonnées Experience Manager Assets personnalisés

Avec l’intégration native, vous pouvez désormais mapper les champs Workfront natifs et intégrés aux champs de schéma de métadonnées personnalisés as a Cloud Service Experience Manager Assets.

Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets as a Cloud Service, voir [Configuration de l’ [!UICONTROL intégration Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets Essentials, voir [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Ajuster les paramètres du modèle de workflow de BAT automatisé à l’aide d’Adobe Workfront pour Creative Cloud

Vous pouvez désormais ajuster les paramètres de modèle de workflow automatisé existants directement dans le Creative Cloud. Une fois que vous avez choisi un modèle de workflow automatisé existant, vous pouvez :

* Désactiver les étapes
* Ajouter des destinataires supplémentaires
* Modification des rôles de BAT
* Ajuster la date limite
* Mettre à jour les notifications par email
* Et plus encore !

Pour plus d’informations, voir [Téléchargement de documents et de BAT avec le  [!DNL Adobe Workfront] module externe pour [!DNL Creative Cloud] Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Ces améliorations sont disponibles pour les applications de Creative Cloud suivantes :

* Photoshop
* XD
* InDesign
* Illustrator
