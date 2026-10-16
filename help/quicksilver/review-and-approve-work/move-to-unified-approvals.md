---
product-area: documents
navigation-topic: approvals
title: Passer des approbations de documents hérités aux approbations unifiées
description: Découvrez ce qui se passe avec vos workflows d’approbation de documents existants lorsque votre entreprise passe à une version de Workfront qui prend en charge les approbations unifiées.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 4f63b6c4f4c73bedba707aed6b02c9046f9b356c
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%
---
# Passer des approbations de documents hérités aux approbations unifiées

Par défaut, les projets de stockage dans le cloud Adobe utilisent les approbations unifiées. Cet article décrit les fonctionnalités disponibles dans les approbations unifiées par rapport aux approbations de documents hérités.


>[!NOTE]
>
>Le paramètre Approbations unifiées est la valeur par défaut uniquement pour les nouveaux objets créés dans l’espace de stockage cloud d’Adobe. Les objets de stockage Workfront hérités conservent leur service d’approbation actuel.<br>
>Pour plus d’informations, voir [Déplacer vers Workfront sur l’espace de stockage cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Comprendre ce qui change des approbations de documents héritées en approbations unifiées

|  | Approbations de documents hérités | Validations unifiées |
| --- | --- | --- |
| Approbateurs et réviseurs | Approbation par des utilisateurs individuels uniquement | Approbation ou révision par des utilisateurs ou des équipes individuels |
| Échéances et rappels | Aucun rappel automatisé | Rappels automatisés 72 heures après, 24 heures après et à la date d’échéance |
| Étapes et chemins de validation | Une étape d’approbation, pas de chemins parallèles | [Étapes d’approbation multiples et chemins de révision parallèles](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| Modèles d’approbation | Chaque approbation configurée à partir de zéro | [Modèles réutilisables](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) disponibles dans la configuration de Workfront |
| Révision et balisage | Visionneuse de relecture | [Visionneuse de relecture](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) sur les objets de stockage Workfront hérités ou [visionneuse Frame.io](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) sur les objets de stockage dans le cloud Adobe |
| Révision assistée par l’IA | Non disponible | Contrôles de conformité de marque automatiques avec [Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md) |
| Rapports | Rapports hérités | Widgets des indicateurs de performance clés d’accueil et [tableaux de bord de la zone de travail](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### Qu’advient-il des approbations déjà en cours ?

Les approbations en vol créées dans les approbations de documents héritées continuent de fonctionner comme avant. Les nouvelles approbations des objets d’espace de stockage dans le cloud Adobe utilisent les approbations unifiées. Les nouvelles approbations sur les objets de stockage Workfront hérités conservent le service d’approbation que ces objets utilisent déjà.


## Préparer le déménagement

* Partagez avec vos utilisateurs finaux l’article [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).
* Examinez vos scénarios Workfront Fusion existants. Si vous utilisez les approbations de documents hérités avec la relecture, consultez [Mise à jour des scénarios Workfront Fusion pour une révision et une approbation unifiées](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) avant d’importer des équipes dans l’espace de stockage cloud Adobe.
* Configurez un tableau de bord de révision et d’approbation dans les tableaux de bord de la zone de travail pour remplacer les anciens rapports d’approbation. Voir [Créer un tableau de bord de révision et d’approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) pour plus d’informations.


### Articles d’aide pour les utilisateurs finaux

* [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Fonctionnalité disponible pour les approbations de documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Aperçu de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Vérifier et approuver avec la visionneuse Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Utiliser conjointement les approbations unifiées et la relecture](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Vue d’ensemble du statut de décision des documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Prise en main du Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
