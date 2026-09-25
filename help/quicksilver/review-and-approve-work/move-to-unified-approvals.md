---
product-area: documents
navigation-topic: approvals
title: Passer des approbations de documents hérités aux approbations unifiées
description: Découvrez ce qui se passe avec vos workflows d’approbation de documents existants lorsque votre entreprise passe à une version de Workfront qui prend en charge les approbations unifiées.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%
---
# Passer des approbations de documents hérités aux approbations unifiées

Le passage à une version de Workfront qui prend en charge l’espace de stockage dans le cloud Adobe fait également passer votre organisation des approbations de documents héritées aux approbations unifiées. Cet article fournit des informations sur les fonctionnalités qui seront disponibles dans les approbations unifiées, ainsi que des recommandations destinées aux administrateurs Workfront afin de déplacer les utilisateurs des approbations de documents hérités.


>[!IMPORTANT]
>
>Cette modification s’applique à l’ensemble de l’entreprise dès que vous passez à une version de Workfront prenant en charge l’espace de stockage dans le cloud Adobe. Il n’existe aucune option de groupe pilote ou de déploiement progressif pour passer des approbations de documents héritées aux approbations unifiées.<br>
>Pour plus d’informations sur les modifications apportées à l’espace de stockage dans le cloud d’Adobe, voir [Déplacer vers Workfront sur l’espace de stockage dans le cloud d’Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Comprendre ce qui change des approbations de documents héritées en approbations unifiées

|  | Approbations de documents hérités | Validations unifiées |
| --- | --- | --- |
| Approbateurs et réviseurs | Approbation par des utilisateurs individuels uniquement | Approbation ou révision par des utilisateurs ou des équipes individuels |
| Échéances et rappels | Aucun rappel automatisé | Rappels automatisés 72 heures après, 24 heures après et à la date d’échéance |
| Étapes et chemins de validation | Une étape d’approbation, pas de chemins parallèles | [Étapes d’approbation multiples et chemins de révision parallèles](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| Modèles d’approbation | Chaque approbation configurée à partir de zéro | [Modèles réutilisables](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) disponibles dans la configuration de Workfront |
| Révision et balisage | Visionneuse de relecture | [Visionneuse de relecture](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) sur les objets de stockage Workfront hérités ou [visionneuse Frame.io](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) sur les objets de stockage dans le cloud Adobe |
| Révision assistée par l’IA | Non disponible | Contrôles de conformité de marque automatiques avec [AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md) |
| Rapports | Rapports hérités | Widgets des indicateurs de performance clés d’accueil et [tableaux de bord de la zone de travail](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### Qu’advient-il des approbations déjà en cours ?

Les approbations en cours créées dans les approbations de documents héritées continueront à fonctionner comme avant la mise à niveau. Toutefois, toutes les nouvelles approbations créées après la mise à niveau utiliseront les approbations unifiées.


## Préparation de la mise à niveau

* Partagez avec vos utilisateurs finaux l’article [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).
* Examinez vos scénarios Workfront Fusion existants. Si vous utilisez les approbations de documents hérités avec la relecture, consultez [Mise à jour des scénarios Workfront Fusion pour une révision et une approbation unifiées](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) avant les mises à niveau de votre organisation.
* Configurez un tableau de bord de révision et d’approbation dans les tableaux de bord de la zone de travail pour remplacer les anciens rapports d’approbation. Voir [Créer un tableau de bord de révision et d’approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) pour plus d’informations.


### Articles d’aide pour les utilisateurs finaux

* [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Fonctionnalité disponible pour les approbations de documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Aperçu de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Vérifier et approuver avec la visionneuse Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Utiliser conjointement les approbations unifiées et la relecture](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Vue d’ensemble du statut de décision des documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Prise en main du réviseur de l’IA dédiée à Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)