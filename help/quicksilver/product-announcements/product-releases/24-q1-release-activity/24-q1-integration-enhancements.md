---
title: Améliorations de l’intégration au premier trimestre 2024
description: Améliorations de l’intégration au premier trimestre 2024
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 100%

---

# Améliorations de l’intégration au premier trimestre 2024

Cette page décrit toutes les améliorations d’intégration apportées dans la version du premier trimestre 2024 à l’environnement de prévisualisation. Si indiqué, ces améliorations seront disponibles dans l’environnement de production avec la version du premier trimestre 2024.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du premier trimestre 2024, consultez l’article [Vue d’ensemble de la version du premier trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## Le mappage des métadonnées dans Experience Manager Assets Essentials utilise désormais `xcm:keywords` au lieu de `dc:subject`.

Nous avons mis à jour l’intégration d’Experience Manager Assets Essentials afin qu’elle corresponde à l’expérience de l’intégration d’Experience Manager Assets as a Cloud Service. Désormais, lorsque vous mappez plusieurs champs de texte d’une seule ligne à un seul champ dans Experience Manager Assets, les deux services utilisent le champ `xcm:keywords`.

Auparavant, ces champs étaient mappés au champ `dc:subject` dans Experience Manager Assets Essentials. La fonctionnalité Experience Manager Assets as a Cloud Service reste inchangée.

Toutes les métadonnées Experience Manager Assets Essentials actuellement mappées sur `dc:subject` doivent être remappées sur `xcm:keywords`.

Pour plus d’informations sur le mappage des métadonnées sur Experience Manager Assets Essentials, voir [Mot-clé AEM](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Champs de saisie semi-automatique désormais disponibles dans l’intégration Adobe Experience Manager

Afin de faciliter la liaison des champs entre Workfront et Adobe Experience Manager, nous avons ajouté la prise en charge des champs de saisie semi-automatique dans le mappage des métadonnées. Vous pouvez maintenant mapper des champs de saisie semi-automatique sur des champs correspondants dans Adobe Experience Manager.

Si une personne sélectionne une autre valeur pour un champ dans Workfront, cette modification est immédiatement répercutée dans Adobe Experience Manager. En outre, si une option de valeur de champ change (par exemple, si une équipe prend un nouveau nom), cette modification est également répercutée dans Adobe Experience Manager.

Pour plus d’informations et d’instructions sur le mappage des métadonnées dans l’intégration Adobe Experience Manager, voir [Configurer des métadonnées](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Publier automatiquement des ressources dans Adobe Experience Manager

Nous avons ajouté un autre workflow à l’intégration Adobe Experience Manager. Désormais, vous pouvez définir vos ressources afin qu’elles soient automatiquement publiées lorsqu’elles sont envoyées à Adobe Experience Manager. L’intégration peut être configurée pour la publication sur le service de publication Adobe Experience Manager ou sur Adobe Experience Manager Brand Portal.

Le workflow Publication automatique peut être activé et configuré dans l’intégration d’Adobe Experience Manager. Une fois activé, le workflow peut être modifié au niveau du modèle de projet ou du projet.

Pour plus d’informations, voir la section [Publier des ressources](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) dans [Utiliser des workflows dans l’intégration d’Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
