---
title: Améliorations de l’intégration au premier trimestre 2024
description: Améliorations de l’intégration au premier trimestre 2024
author: Becky
feature: Product Announcements
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 44dd48b72e798b8967c4a4e3dc7d523fe9b130d2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Améliorations de l’intégration au premier trimestre 2024

Cette page décrit toutes les améliorations de l’intégration apportées à la version du premier trimestre 2024 de l’environnement Aperçu. Ces améliorations seront rendues disponibles dans l’environnement de production avec la version du premier trimestre 2024.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du premier trimestre 2024, voir [Présentation de la version du premier trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## Le mappage des métadonnées dans Experience Manager Assets Essentials utilise désormais `xcm:keywords` au lieu de `dc:subject`

Nous avons mis à jour l’intégration de Experience Manager Assets Essentials afin qu’elle corresponde à l’expérience de l’intégration as a Cloud Service de Experience Manager Assets. Désormais, lorsque vous mappez plusieurs champs de texte d’une seule ligne à un seul champ dans Experience Manager Assets, les deux services utilisent la variable `xcm:keywords` champ .

Auparavant, ces champs étaient mappés à la variable `dc:subject` dans Experience Manager Assets Essentials. La fonctionnalité as a Cloud Service d’Experience Manager Assets reste inchangée.

Toutes les métadonnées Experience Manager Assets Essentials actuellement mises en correspondance avec `dc:subject` doit être mappé sur `xcm:keywords`.

Pour plus d’informations sur le mappage des métadonnées sur Experience Manager Assets Essentials, voir [Mot-clé AEM](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Champs de saisie anticipée désormais disponibles dans l’intégration Adobe Experience Manager

Afin de faciliter la liaison des champs entre Workfront et Adobe Experience Manager, nous avons ajouté la prise en charge des champs de saisie anticipée dans le mappage des métadonnées. Vous pouvez maintenant mapper des champs de type anticipé aux champs correspondants dans Adobe Experience Manager.

Si un utilisateur sélectionne une autre valeur pour un champ dans Workfront, cette modification est immédiatement répercutée dans Adobe Experience Manager. En outre, si une option de valeur de champ change (par exemple si une équipe remplace son nom par un nouveau nom), cette modification est également répercutée dans Adobe Experience Manager.

Pour plus d’informations et d’instructions sur le mappage des métadonnées dans l’intégration Adobe Experience Manager, voir [Configuration des métadonnées](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Publication automatique de ressources dans Adobe Experience Manager

Nous avons ajouté un autre workflow à l’intégration Adobe Experience Manager. Désormais, vous pouvez définir vos ressources pour qu’elles soient automatiquement publiées lorsqu’elles sont envoyées à Adobe Experience Manager. L’intégration peut être configurée pour la publication sur le service de publication Adobe Experience Manager ou sur un portail de marque Adobe Experience Manager.

Le workflow Publication automatique peut être activé et configuré dans l’intégration de Adobe Experience Manager. Une fois activé, le workflow peut être modifié au niveau du modèle de projet ou du projet.

Pour plus d’informations, voir [Publication de ressources](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) in [Utilisation des workflows dans l’intégration Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
