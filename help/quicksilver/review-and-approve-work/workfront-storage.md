---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Passer à Workfront sur l’espace de stockage dans le cloud Adobe
description: Planifiez votre déplacement vers Workfront sur l’espace de stockage cloud Adobe. Découvrez ce qui se passe lorsque votre organisation est activée, ce qui est différent sur les objets de stockage dans le cloud Adobe et comment la déployer à votre propre rythme.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---
# Passer à Workfront sur l’espace de stockage dans le cloud Adobe

Workfront sur le stockage cloud Adobe offre une expérience de révision et d’approbation entièrement unifiée : révisions dans la visionneuse Frame.io, workflows d’approbation puissants, visibilité des ressources sur l’ensemble des produits, etc.

Cet article est le point de départ pour les administrateurs Workfront qui passent à l’espace de stockage dans le cloud Adobe. Il explique ce qui se passe lorsque vous activez l’espace de stockage dans le cloud d’Adobe, vous donne des détails sur les différences et fournit des liens vers les articles qui vous aident à planifier et à déployer la modification.

## C’est vous qui décidez quand l’espace de stockage Adobe dans le cloud sera activé

Votre environnement Workfront ne change que lorsqu’un administrateur Workfront active l’espace de stockage Adobe dans le cloud en tant qu’option de stockage par défaut dans **Configuration** > **Système** > **Préférences**. D’ici là, vos projets existants et les nouveaux projets que vous créez resteront sur l’ancien stockage Workfront et conserveront le service d’approbation que vous utilisez aujourd’hui.

Lorsqu’un administrateur active l’espace de stockage Adobe dans le cloud en tant qu’option de stockage par défaut :

* Les nouveaux projets utilisent l’espace de stockage Adobe dans le cloud.
* Frame.io est la visionneuse par défaut
* Les validations unifiées constituent le service de validation par défaut

Les projets existants ne changent pas.

Étant donné que vous contrôlez le minutage, vous pouvez tester l’expérience, mettre à jour vos scénarios Workfront Fusion et planifier les modifications des rapports avant que quiconque n’y travaille. Pour obtenir des instructions détaillées, voir [Activer l’espace de stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

## Fonctionnement des approbations dans l’espace de stockage cloud d’Adobe

Les projets de stockage dans le cloud Adobe utilisent par défaut les approbations unifiées, avec révision et approbation dans la visionneuse Frame.io. Les objets qui restent sur l’espace de stockage Workfront hérité conservent le service d’approbation qu’ils utilisent déjà : approbations de documents hérités ou approbations unifiées.

>[!NOTE]
>
>Définir l’espace de stockage dans le cloud d’Adobe comme valeur par défaut ne modifie pas le service d’approbation déjà utilisé sur vos objets de stockage Workfront hérités. Le paramètre Approbations unifiées est la valeur par défaut uniquement pour les nouveaux objets créés dans l’espace de stockage cloud d’Adobe.

Avant de déployer l’espace de stockage dans le cloud d’Adobe, assurez-vous que les personnes qui gèrent les validations savent à quoi s’attendre. Pour plus d&#39;informations, voir [Passer des approbations de documents hérités aux approbations unifiées](/help/quicksilver/review-and-approve-work/move-to-unified-approvals.md).

## Planifier votre déménagement

Parcourez ces articles dans l’ordre au fur et à mesure que vous préparez :

* [En quoi consiste l’espace de stockage dans le cloud d’Adobe &#x200B;](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md) : principales différences entre les objets de stockage dans le cloud d’Adobe, de la nouvelle zone Documents à la visionneuse Frame.io, en passant par les règles de nommage, le quota de stockage et Fusion.
* [Planifiez le déploiement de votre espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md) : choisissez une configuration de déploiement, pilotez avec un seul groupe et ordonnancez le travail afin d’éviter les surprises pour vos utilisateurs.
* [Activer l’espace de stockage Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md) : étapes de définition de l’option de stockage par défaut pour l’ensemble de l’organisation ou pour des groupes spécifiques.
* [Conversion d’objets hérités en espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md) : les trois cas où vous pouvez convertir un objet hérité en espace de stockage dans le cloud Adobe, et ce qui se déplace au cours de chaque conversion.


## Articles connexes

* [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Aperçu de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [La zone Documents](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)
