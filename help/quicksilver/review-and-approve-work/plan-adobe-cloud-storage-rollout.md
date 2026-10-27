---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Planification du déploiement de l’espace de stockage Adobe
description: Choisissez la manière dont l’espace de stockage dans le cloud Adobe s’affiche pour vos utilisateurs, pilotez-le avec un seul groupe et ordonnancez le travail afin qu’il n’y ait aucune surprise pour les réviseurs, les approbateurs et les propriétaires de projet.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
exl-id: b4413742-c250-4110-9097-6d38842355a4
source-git-commit: 2b5d95ed0a5c72062700bf026a18b8301e4be421
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 0%

---
# Planification du déploiement de l’espace de stockage Adobe

Vous décidez comment et quand l’espace de stockage Adobe atteint vos utilisateurs. Rien ne change tant qu’un administrateur Workfront n’a pas défini l’espace de stockage Adobe comme option de stockage par défaut dans la zone de configuration, vous avez donc le temps de tester l’expérience et de préparer vos équipes avant que quiconque ne travaille dessus.

Cet article couvre les configurations de déploiement que vous pouvez choisir, la manière de piloter avec un seul groupe et un ordre de travail suggéré.

## Choisir comment l’espace de stockage dans le cloud Adobe se déploie

Il existe deux configurations et vous pouvez en appliquer une à l’ensemble de votre organisation ou à des groupes Workfront spécifiques. Chaque projet créé dans le stockage cloud d’Adobe utilise par défaut les approbations unifiées et la visionneuse Frame.io.

Pour obtenir des instructions détaillées, voir [Activer l’espace de stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

### Options de configuration

* **Espace de stockage Adobe uniquement** : les nouveaux projets utilisent l’espace de stockage Adobe par défaut. Les utilisateurs ne peuvent pas créer de projets hérités.
* **Stockage dans le cloud Adobe et stockage Workfront hérité** : lorsque les utilisateurs créent un projet, ils choisissent entre le stockage dans le cloud Adobe (appelé « Nouveau projet ») et le stockage Workfront hérité (appelé « Stockage hérité »). Cette option est activée en cochant la case **Autoriser l’utilisateur à sélectionner le fournisseur de stockage** dans la zone de configuration.

>[!TIP]
>
>Pour placer l’espace de stockage cloud d’Adobe devant une équipe plus petite en premier, appliquez l’une des configurations à un seul groupe Workfront. Vous pouvez ainsi exécuter un pilote ciblé avant d’effectuer un déploiement plus large. Nous vous recommandons de commencer par un déploiement au niveau du groupe pour contrôler la fréquence, puis de l’étendre à l’ensemble de l’organisation une fois que le groupe pilote a validé l’expérience.

Les objets existants conservent le modèle de stockage avec lequel ils ont été créés. La modification de la préférence de stockage par défaut ne modifie aucun objet existant.

![préférences de stockage dans la configuration](assets/storage-preference-groups.png)

## Planifier le déploiement

Chaque environnement Workfront est différent. Avant de définir l’espace de stockage dans le cloud Adobe comme stockage par défaut pour vos utilisateurs, prenez le temps de planifier un déploiement réussi pour votre organisation. Les suggestions ci-dessous ne sont pas une liste de contrôle exacte, mais un point de départ pour votre propre plan.

### Choisir un groupe pilote

Un déploiement à l’échelle d’un groupe vous permet de placer l’espace de stockage cloud d’Adobe devant une équipe plus petite, de recueillir des commentaires et de procéder à des ajustements avant un déploiement plus large. Sélectionnez un groupe dont les modèles de travail sont suffisamment représentatifs pour faire apparaître rapidement les problèmes que vous souhaitez connaître.

<!--
>[!IMPORTANT]
>
>Only members of the pilot group can convert an Adobe cloud storage object, such as a request or a task, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."
-->

### Test avant la mise en ligne

L’espace de stockage dans le cloud d’Adobe est disponible dans les environnements sandbox de Workfront. Vous pouvez ainsi valider une grande partie de l’expérience avant la production. La visionneuse Frame.io n’étant pas disponible dans Sandbox, vous validez l’expérience complète de révision et d’approbation en production avec votre groupe pilote. Pour plus d’informations, voir [Activer l’espace de stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

### Communiquer le changement aux utilisateurs finaux

La plus grande modification visible pour les réviseurs, les approbateurs et les propriétaires de projet est la nouvelle zone Documents et la visionneuse Frame.io qui alimente la révision et l’approbation des projets d’espace de stockage dans le cloud Adobe. Planifiez l’introduction de ces éléments afin que les utilisateurs sachent à quoi s’attendre lorsqu’ils rencontrent leur premier projet de stockage dans le cloud Adobe. L’article [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) est un point de départ utile pour les ressources destinées aux utilisateurs finaux.

### Vérifier vos autorisations et votre gouvernance

Dans les projets de stockage dans le cloud Adobe, les options Gérer et Contribuer mappent toutes deux à Modifier et partager dans Frame.io, ce qui inclut le partage externe. Examinez vos modèles de partage et décidez s’ils correspondent à votre modèle de gouvernance avant d’intégrer des équipes dans l’espace de stockage cloud Adobe. Pour plus d’informations, voir [En quoi consiste l’espace de stockage dans le cloud d’Adobe &#x200B;](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-permissions-mapping).

### Modèles d’audit et dénomination

L’espace de stockage dans le cloud d’Adobe applique des règles de nommage strictes et Workfront renomme automatiquement les objets qui entrent en conflit avec elles. Si vous créez des projets à partir de modèles, passez en revue ces modèles afin que les noms et la structure qu’ils génèrent soient conformes aux règles. Pour plus d’informations, voir [En quoi consiste l’espace de stockage dans le cloud d’Adobe &#x200B;](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-naming-rules).

### Planifier autour de Workfront Fusion

Les scénarios Fusion existants basés sur des BAT continuent de fonctionner sur les projets hérités, mais ne fonctionnent pas automatiquement sur les projets de stockage dans le cloud Adobe. Avant d’importer des équipes qui dépendent de ces scénarios dans l’espace de stockage cloud d’Adobe, classifiez chaque scénario comme Modifier, Recréer ou Supprimer. Pour plus d’informations, voir [Mise à jour des scénarios Workfront Fusion pour une révision et une approbation unifiées](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).

### Planifier les modifications de rapports

Les données et les rapports du workflow d’approbation unifiée apparaissent dans les tableaux de bord de la zone de travail. Les anciens rapports d’approbation ne sont pas transférés automatiquement. Configurez donc un tableau de bord de remplacement avant que vos équipes pilotes n’en aient besoin. Pour plus d’informations, voir [Créer un tableau de bord de rapport pour révision et approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

## Ordre suggéré

Utilisez cet ordre comme modèle, en l’adaptant à votre environnement :

1. Testez l’expérience dans un sandbox et avec un groupe pilote en production.
2. Classez et mettez à jour vos scénarios Fusion, et créez vos rapports Tableaux de bord Canvas .
3. Contrôlez vos modèles et passez en revue vos autorisations et votre modèle de partage.
4. Communiquez la modification aux réviseurs, approbateurs et propriétaires de projet qui l’utiliseront.
5. Définissez l’espace de stockage dans le cloud Adobe comme stockage par défaut pour le groupe pilote, puis développez-le à d’autres groupes ou à l’ensemble de l’organisation une fois que le pilote a validé l’expérience.
