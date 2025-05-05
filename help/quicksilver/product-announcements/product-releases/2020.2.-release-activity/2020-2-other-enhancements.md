---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Autres améliorations (version 2020.2)
description: Cette page décrit toutes les autres améliorations apportées par la version 2020.2 à l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 99%

---

# Autres améliorations (version 2020.2)

Cette page décrit toutes les autres améliorations apportées par la version 2020.2 à l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.2, consultez l’article [Présentation de la version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Pour les administrateurs et administratrices de Workfront : les nouveaux modèles de disposition créés dans Workfront Classic sont désormais disponibles dans la nouvelle expérience Workfront.

Les modèles de disposition créés dans Workfront Classic après l’automne 2019 sont désormais disponibles dans la nouvelle expérience Workfront. Il est conseillé de mettre à jour ces modèles de disposition dans la nouvelle expérience Workfront afin de profiter des nouvelles fonctionnalités et de les rendre aussi utiles que possible aux utilisateurs et utilisatrices de cet environnement.

Pour plus d’informations, voir [Modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Disponibles dans ces environnements :**

* La nouvelle expérience Adobe Workfront

## Des processus d’approbation spécifiques aux groupes sont disponibles pour tous les objets

Pour utiliser pleinement les processus d’approbation spécifiques aux groupes, vous pouvez désormais les ajouter aux tâches, problèmes et projets lorsque vous modifiez ces objets.

Vous pouvez également associer automatiquement un processus d’approbation spécifique aux groupes à une tâche dans la zone Tâches de la zone Modifier le projet , ainsi qu’à des problèmes, lors de la configuration des files d’attente des demandes ou des rubriques de file d’attente sur un projet.

Pour plus d’informations sur l’ajout de processus d’approbation aux projets, tâches et problèmes, consultez les articles suivants :

* [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Modifier des tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Modifier des problèmes](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Créer des processus d’approbation pour les groupes utilisant des statuts personnalisés

Afin qu’il soit plus facile pour les groupes de gérer leurs propres workflows uniques, vous pouvez désormais utiliser des statuts personnalisés spécifiques aux groupes dans les processus d’approbation.

Auparavant, un groupe ne pouvait pas utiliser ses propres statuts personnalisés avec ses processus d’approbation spécifiques aux groupes. Seuls les statuts à l’échelle du système étaient disponibles et ceux-ci ne correspondaient pas toujours aux processus d’approbation des groupes.

Les statuts personnalisés peuvent désormais être utilisés dans les processus d’approbation à usage unique et à l’échelle du système :

* Créez un processus d’approbation à usage unique pour un objet (projet, tâche ou problème) et basez-le sur les statuts associés au groupe travaillant sur cet objet. Cela inclut tous les statuts personnalisés associés au groupe.
* Créez un processus d’approbation global et rendez-le disponible pour le groupe uniquement ou pour toutes les personnes du système.

Pour les utilisateurs et utilisatrices disposant d’un accès administratif aux processus d’approbation, des informations sur la configuration des processus d’approbation sont disponibles dans [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (ou, si vous utilisez Adobe Workfront Classic, consultez [Créer un processus d’approbation](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

Pour les utilisateurs et utilisatrices, des informations sur l’association des processus d’approbation aux éléments de travail sont disponibles dans [Associer un processus d’approbation nouveau ou existant à un travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (ou, si vous utilisez Adobe Workfront Classic, consultez [Associer un processus d’approbation nouveau ou existant à un travail](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponibles dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Nouvelles pages de superposition pour la recherche

Pour permettre aux utilisateurs et aux utilisatrices de naviguer plus facilement entre les pages de recherche et les pages précédentes dans la nouvelle expérience Workfront, nous avons ajouté une page de superposition de recherche qui couvre partiellement l’écran.

Désormais, lorsque vous cliquez sur Recherche avancée dans le menu Rechercher ou que vous effectuez une recherche de base, une page s’ouvre dans la partie droite de l’écran.

Pour plus d’informations, consultez [Rechercher dans Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Disponibles dans ces environnements :**

* La nouvelle expérience Adobe Workfront

## Mises à jour des abonnements aux événements

Pour permettre aux utilisateurs et utilisatrices de mieux trier, dépanner et résoudre les problèmes, nous avons modifié le comportement et ajouté plus de données à l’API des abonnements aux événements. Nous avons également apporté les modifications suivantes :

* Technologies de messagerie sous-jacentes migrées
* Reconstruisez le service pour avoir des dépendances moins complexes et pour le dimensionner ainsi plus efficacement.
* Améliorations apportées à la surveillance et aux alertes

Pour en savoir plus, consultez [Questions fréquentes - Abonnements aux événements](../../../wf-api/general/event-subs-faq.md) et [Bonnes pratiques relatives aux abonnements aux événements](../../../wf-api/general/event-sub-best-practice.md).
