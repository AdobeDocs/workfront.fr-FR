---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrer à partir des connecteurs hérité ou amélioré
description: Le processus suivant décrit les bonnes pratiques à suivre pour passer du connecteur hérité d’Adobe Experience Manager au connecteur amélioré pour intégrer Adobe Workfront à AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 100%

---

# Migrer à partir des connecteurs hérité ou amélioré

Le processus suivant décrit les bonnes pratiques à suivre pour passer du connecteur hérité d’Adobe Experience Manager au connecteur amélioré pour intégrer Adobe Workfront à AEM Assets.

>[!IMPORTANT]
>
>Cette documentation s’applique uniquement aux clientes et clients utilisant des environnements Adobe Experience Manager Assets On-Premise ou Managed Services.


Pour les clientes et clients sur Adobe Experience Manager Assets as a Cloud Service, le chemin de migration du connecteur hérité sera vers la nouvelle intégration native dans Workfront. Pour en savoir plus sur ce processus de migration, voir [Migrer du connecteur hérité ou amélioré vers Workfront pour l’intégration Adobe Experience Manager as a Cloud Service](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Mettre en œuvre le connecteur amélioré

>[!IMPORTANT]
>
>Un partenaire certifié ou des services de conseil Adobe sont nécessaires pour mettre en œuvre le connecteur amélioré.
>
> Pour les partenaires qui souhaitent se certifier sur le connecteur amélioré, consultez l’article suivant : [Expert Series Workfront pour le connecteur amélioré pour Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=fr).

Pour mettre en œuvre le connecteur amélioré, voir [Configurer Workfront pour le connecteur amélioré Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=fr).


## Déplacer des ressources existantes

Une fois votre environnement configuré, vous pouvez déplacer les ressources et dossiers liés existants vers Adobe Experience Manager. Il s’agit d’une étape facultative, mais qui garantit que les dossiers et ressources précédemment liés par le biais du connecteur hérité seront toujours accessibles une fois le connecteur hérité désinstallé.

Pour plus d’informations sur le déplacement de vos ressources, voir [Migrer des dossiers et des documents liés](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Valider tous les cas d’utilisation critiques destinés à être utilisés

Il est important de valider tous les cas d’utilisation critiques destinés à être utilisés par le biais du connecteur amélioré avant de désinstaller le connecteur hérité.

## Désinstaller le connecteur hérité

Enfin, vous devez désinstaller le connecteur hérité. Le connecteur hérité n’est pas conçu pour s’exécuter en parallèle avec le connecteur amélioré.

Pour le désinstaller, voir [Désinstaller le connecteur hérité Workfront avec Adobe Experience Manager](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
