---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migration du connecteur hérité vers le connecteur amélioré
description: Le processus suivant décrit les bonnes pratiques à suivre pour quitter le connecteur hérité d’Adobe Experience Manager vers le connecteur amélioré pour intégrer Adobe Workfront à AEM Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Migration du connecteur hérité vers le connecteur amélioré

Le processus suivant décrit les bonnes pratiques à suivre pour quitter le connecteur hérité d’Adobe Experience Manager vers le connecteur amélioré pour intégrer Adobe Workfront à AEM Assets.

>[!IMPORTANT]
>
>Cette documentation s’applique uniquement aux clients utilisant des environnements Adobe Experience Manager Assets On-Premise ou Managed Services.


Pour les clients sur Adobe Experience Manager Assets as a Cloud Service, le chemin de migration du connecteur hérité vers la nouvelle intégration native au sein de Workfront. Pour en savoir plus sur ce processus de migration, voir [Migration du connecteur hérité ou amélioré vers Workfront pour l’intégration Adobe Experience Manager as a Cloud Service](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## Mise en oeuvre du connecteur amélioré

>[!IMPORTANT]
>
>Un partenaire certifié ou des services de conseil en Adobe sont nécessaires pour l’implémentation du connecteur amélioré.
>
> Pour les partenaires qui souhaitent certifier sur le connecteur amélioré, consultez l’article suivant : [Workfront pour les séries d’experts du connecteur amélioré pour Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

Pour mettre en oeuvre le connecteur amélioré, voir [Configuration de Workfront pour Experience Manager Enhanced Connector](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## Déplacement de ressources existantes

Une fois votre environnement configuré, vous pouvez déplacer les ressources et dossiers liés existants vers Adobe Experience Manager. Il s’agit d’une étape facultative, mais qui garantit que les dossiers et ressources précédemment liés par le biais du connecteur hérité seront toujours accessibles une fois le connecteur hérité désinstallé.

Pour plus d’informations sur le déplacement de vos ressources, voir [Migration des dossiers et documents liés](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## Validation de tous les cas d’utilisation critiques prévus

Il est important de valider tous les cas d’utilisation critiques destinés à être utilisés par le connecteur amélioré avant de désinstaller le connecteur hérité.

## Désinstallation du connecteur hérité

Enfin, vous devez désinstaller le connecteur hérité. Le connecteur hérité n’est pas conçu pour s’exécuter en parallèle avec le connecteur amélioré.

Pour désinstaller, voir [Désinstallation de Workfront avec Adobe Experience Manager legacy connector](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
