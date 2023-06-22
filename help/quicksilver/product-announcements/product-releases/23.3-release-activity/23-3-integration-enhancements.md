---
title: 23.3 Améliorations de l’intégration
description: 23.3 Améliorations de l’intégration
author: Lisa
feature: Product Announcements
source-git-commit: 3ebf408bb03a97de78600ab771834a7d7f29e2e0
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# 23.3 Améliorations de l’intégration

Cette page décrit toutes les améliorations de l’intégration apportées à la version 23.3 de l’environnement Aperçu. Ces améliorations seront rendues disponibles dans l’environnement de production avec la version 23.3.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication 23.3, voir [Présentation de la version 23.3](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Les intégrations Adobe Creative Cloud prennent désormais en charge plusieurs utilisateurs affectés.

L’intégration de Adobe Creative Cloud prend désormais en charge la possibilité de choisir entre &quot;Terminé avec ma part&quot; et &quot;Terminé&quot; (ou &quot;Résolu&quot;) lorsqu’une tâche ou un problème comporte plusieurs utilisateurs affectés.

Auparavant, l’intégration permettait aux utilisateurs de marquer une tâche comme étant terminée, sans spécifier &quot;Terminé avec ma part&quot; ou &quot;Terminé&quot;/&quot;Résolu&quot;.

Pour tirer parti de cette fonctionnalité, téléchargez et installez les modules externes les plus récents de Workfront for Creative Cloud.

Pour plus d’informations sur cette fonctionnalité, voir [Marquer les tâches terminées à l’aide du module externe Adobe Workfront](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Pour plus d’informations sur l’installation des modules externes Workfront for Creative Cloud, voir [Installation du module externe Adobe Workfront pour les applications Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Affichage et gestion des notifications Workfront à partir de Workfront pour les modules externes Creative Cloud

Afin de vous permettre de recevoir plus facilement les notifications dont vous avez besoin, nous avons rendu possible l’affichage et la gestion des notifications Workfront sans quitter Adobe Creative Cloud. Vous pouvez désormais afficher des notifications, ainsi que accéder aux tâches et aux commentaires associés à ces notifications, directement depuis la fenêtre du module externe Workfront dans l’application du Creative Cloud.

Auparavant, les notifications n’étaient disponibles que dans Workfront et par courrier électronique.

Pour tirer parti de cette fonctionnalité, téléchargez et installez les modules externes les plus récents de Workfront for Creative Cloud.

Pour plus d’informations, voir [Affichage et gestion [!DNL Adobe Workfront] notifications de Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Pour plus d’informations sur l’installation des modules externes Workfront for Creative Cloud, voir [Installation du module externe Adobe Workfront pour les applications Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Expérience améliorée lors du déplacement d’un document vers un dossier lié à l’aide du glisser-déposer

Nous avons ajouté une certaine transparence au processus de glisser-déposer d’un document dans un dossier lié. Désormais, le document que vous avez déplacé vers un dossier lié reste dans la liste des documents jusqu’à ce qu’il ait été complètement déplacé. Les options du document sont désactivées, mais vous pouvez toujours ouvrir le document pour l’afficher pendant son déplacement. Une fois le transfert terminé, le document disparaît de la liste des documents, car il se trouve désormais entièrement dans le dossier lié.

Auparavant, les documents disparaissaient immédiatement de la liste des documents avant d’être déplacés vers le dossier lié.

Pour plus d’informations, voir [Liaison de documents à partir d’applications externes](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Création automatique de dossiers liés à Adobe Experience Manager Assets lors de la création d’un projet

Avec le nouveau workflow Créer un dossier lié pour l’intégration d’Adobe Experience Manager, vous pouvez configurer l’intégration avec un chemin d’accès à un dossier Adobe Experience Manager Assets. Lorsque l’intégration est ajoutée à un modèle de projet, tout projet créé à partir du modèle crée automatiquement un sous-dossier lié dans Experience Manager Assets dans le dossier spécifié.

Auparavant, la création de dossiers liés nécessitait une action de la part de l’utilisateur.

Cette fonctionnalité est disponible uniquement avec une intégration Adobe Experience Manager as a Cloud Service dans Workfront. Cette option n’est pas disponible dans le connecteur amélioré d’Adobe Experience Manager.

Pour plus d’informations, voir [Utilisation des workflows dans l’intégration Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Mappage des valeurs de champ Workfront aux balises dans Experience Manager Assets

Vous pouvez désormais classer et rechercher rapidement des ressources en fonction des données de Workfront. Vous pouvez mapper ces données dans le cadre de votre configuration de métadonnées dans l’intégration de Workfront for Experience Manager Assets.

Auparavant, le mappage des données Workfront aux balises Experience Manager Assets n’était pas disponible.

Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets as a Cloud Service, voir [Configurez la variable [!UICONTROL Experience Manager Assets as a Cloud Service] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets Essentials, voir [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Mappage des champs Workfront aux champs de métadonnées Experience Manager Assets personnalisés

Avec l’intégration native, vous pouvez désormais mapper des champs Workfront natifs et intégrés aux champs de schéma de métadonnées personnalisés dans Experience Manager Assets as a Cloud Service.

Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets as a Cloud Service, voir [Configurez la variable [!UICONTROL Experience Manager Assets as a Cloud Service] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Pour plus d’informations sur cette fonctionnalité dans Experience Manager Assets Essentials, voir [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Ajuster les paramètres du modèle de workflow de BAT automatisé à l’aide d’Adobe Workfront pour Creative Cloud

Vous pouvez désormais ajuster les paramètres de modèle de workflow automatisé existants directement dans le Creative Cloud. Une fois que vous avez choisi un modèle de workflow automatisé existant, vous pouvez :

* Désactivation des étapes
* Ajouter des destinataires supplémentaires
* Modification des rôles de BAT
* Ajuster la date limite
* Mettre à jour les notifications par email
* Et plus encore !

Pour plus d’informations, voir [Téléchargement de documents et de BAT avec le [!DNL Adobe Workfront] module externe pour [!DNL Creative Cloud] Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Ces améliorations sont disponibles pour les applications de Creative Cloud suivantes :

* Photoshop
* XD
* InDesign
* Illustrator
