---
product-area: documents
navigation-topic: approvals
title: Mettre à jour les scénarios Workfront Fusion pour une révision et une approbation unifiées
description: inventoriez, classez et corrigez les scénarios Workfront Fusion basés sur la relecture Workfront héritée lorsque votre entreprise adopte l’espace de stockage dans le cloud Adobe et la révision et l’approbation unifiées.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: a3ef3b4ea00298e23ebc8b6196c951417e75eebe
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 1%

---

# Mettre à jour les scénarios Workfront Fusion pour une révision et une approbation unifiées

Les scénarios Workfront Fusion reposant sur la relecture Workfront héritée ne fonctionnent pas automatiquement avec les projets de stockage dans le cloud Adobe. Les modules, webhooks et points d’entrée d’API spécifiques à une épreuve ont des équivalents directs dans certains cas et des changements significatifs dans d’autres. Cet article vous aide à inventorier les scénarios affectés, à les classer et à décider d’un chemin de correction avant d’importer les équipes qui dépendent de ces scénarios dans votre déploiement de l’espace de stockage dans le cloud Adobe.

Les scénarios étendus aux projets Workfront hérités continuent de fonctionner comme aujourd’hui. Le travail de correction décrit dans cet article s’applique aux scénarios que vous avez l’intention d’exécuter sur des projets de stockage dans le cloud Adobe.

>[!IMPORTANT]
>
>Le connecteur Adobe Workfront Unified Review and Approvals est désormais disponible dans Workfront Fusion. Nous vous recommandons d’utiliser ce connecteur pour des scénarios plus simples et plus fiables lors de l’utilisation de Fusion avec le stockage dans le cloud Adobe.
>
>Pour plus d’informations et d’instructions, consultez [Modules de révision et d’approbation unifiés d’](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-review-and-approvals-modules) dans la documentation de Workfront Fusion.

Utilisez cet article pour inventorier et classer les scénarios afin de comprendre la meilleure façon de mettre à niveau vos scénarios Fusion pour tenir compte de l’espace de stockage cloud Adobe.

Pour un résumé général des changements qui surviennent lorsque votre organisation passe à Workfront sur l’espace de stockage dans le cloud Adobe, voir [Déplacer vers Workfront sur l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).


## Changements pour Fusion dans les projets de stockage dans le cloud Adobe

Les scénarios Fusion existants créés sur Workfront Proof reposent sur des modules spécifiques aux épreuves, des déclencheurs webhook et des points d’entrée API qui ne font pas partie du modèle de données de révision et d’approbation unifiées. Le tableau ci-dessous met en correspondance les types de scénario courants avec leur impact attendu et leur cheminement :

| Type de scénario | Impact | Chemin à suivre |
|---|---|---|
| Création et routage d&#39;un BAT | Pauses | Reconstruction à l’aide de l’API d’approbations unifiées au 3e trimestre 2026 |
| Webhooks de statut des épreuves | Pauses | Recréer avec de nouveaux déclencheurs d’événement d’approbation au 3e trimestre 2026 |
| Déclencheurs de chargement de document | Partiel : nouveau test requis | Audit et retest après la migration au T3 2026 |
| Notifications de rappel de validation | Pauses | Remplacer par les dates limites du modèle d&#39;approbation |
| Acheminement des décisions d&#39;approbation | Pauses | Recréer à l&#39;aide de nouveaux champs de statut de décision |
| Rapports d’approbation personnalisés | Partiel : les noms de champ peuvent changer | Mapper les champs hérités au nouveau schéma |


## Classer chaque scénario en tant que Modifier, Recréer ou Supprimer

Le travail requis par chaque scénario dépend de sa fonction et de ce qui est disponible dans l’examen et l’approbation unifiés. Utilisez les classifications suivantes :

* **Modifier** : l’action existante liée à l’épreuve possède un équivalent direct en matière de révision et d’approbation unifiées. Vous pouvez mettre à jour le scénario pour utiliser la nouvelle action.
* **Reconstruire** : les étapes sous-jacentes ont considérablement changé ou de nouvelles fonctionnalités sont disponibles que le scénario doit utiliser. Il doit donc être reconstruit à partir de zéro.
* **Retirer** : la fonctionnalité native de révision et d’approbation unifiée, telle que les modèles d’approbation à plusieurs étapes avec des rappels d’échéance, remplace l’objectif du scénario qui avait été conçu.

Examinez chaque scénario par rapport à votre logique commerciale spécifique pour décider de sa classification.

## Approche de remédiation

Utilisez l’approche suivante pour planifier et exécuter la remédiation de Fusion :

1. **Inventaire immédiat.** Extrayez une liste complète des scénarios Fusion actifs et balisez chacun d’eux qui fait référence à la création d’épreuves, au statut de l’épreuve, aux approbations de documents ou au routage d’approbation. N’attendez pas que l’espace de stockage dans le cloud d’Adobe soit activé.
1. **Classez chaque scénario** en tant que Modifier, Recréer ou Mettre hors service selon les critères de la section précédente.
1. **Mettez en pause les scénarios basés sur des épreuves** avant d’intégrer les équipes qui en dépendent dans votre projet pilote de stockage dans le cloud Adobe. L’exécution d’automatisations obsolètes basées sur des BAT par rapport au nouveau modèle peut produire des échecs silencieux ou des actions en double.
1. **Utilisez des modèles d’approbation pour remplacer la logique de routage simple.** Les modèles d’approbation natifs en plusieurs étapes avec automatisation des dates limites peuvent gérer de nombreux cas d’utilisation qui nécessitaient auparavant Fusion. Pour plus d’informations, voir [Créer un modèle d’approbation pour les ressources et les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Utiliser le connecteur Adobe Workfront Unified Review and Approvals lors de la reconstruction.** Les connecteurs mis à jour exposent les modules créés spécifiquement pour la révision et l’approbation unifiées, et rendent les reconstructions beaucoup plus simples et plus fiables. Il est déconseillé de reconstruire avec l’API Workfront version 22 avant.
1. **Testez de bout en bout les scénarios reconstruits dans une instance sandbox** avant de les activer en production. Accordez une attention particulière aux payloads d’abonnement aux événements : les noms de champ et le schéma diffèrent des événements de BAT hérités.

>[!TIP]
>
>De nombreuses entreprises ont accumulé des scénarios Fusion qui constituaient des solutions de contournement pour les lacunes en matière de relecture héritée. Les fonctionnalités natives de révision et d’approbation unifiées, notamment les modèles d’approbation, les rappels d’échéance et le routage en plusieurs étapes, éliminent entièrement la nécessité de certains de ces scénarios. Au fur et à mesure que vous classez chaque scénario, évaluez si une fonctionnalité native peut le remplacer. Le retrait d&#39;un scénario est souvent un résultat à long terme plus propre que sa reconstruction.

## Articles connexes

* [Passer à Workfront sur l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [Aperçu de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Créer un modèle d’approbation pour les ressources et les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
