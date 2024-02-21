---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 autres améliorations
description: Cette page décrit toutes les autres améliorations apportées à la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 2020.2 autres améliorations

Cette page décrit toutes les autres améliorations apportées à la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.2, voir [Présentation de la version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Pour les administrateurs de Workfront : les nouveaux modèles de mise en page créés dans Workfront Classic sont désormais disponibles dans la nouvelle expérience Workfront.

Les modèles de mise en page créés dans Workfront Classic après l’automne 2019 sont désormais disponibles dans la nouvelle expérience Workfront. Il est conseillé de mettre à jour ces modèles de mise en page dans la nouvelle expérience Workfront afin de profiter des nouvelles fonctionnalités et de les rendre aussi utiles que possible aux utilisateurs de cet environnement.

Pour plus d’informations, voir [Modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Disponible dans ces environnements :**

* Nouvelle expérience Adobe Workfront

## Des processus d’approbation spécifiques à un groupe sont disponibles pour tous les objets.

Pour utiliser pleinement les processus d’approbation spécifiques à un groupe, vous pouvez désormais les ajouter aux tâches, problèmes et projets lorsque vous modifiez ces objets.

Vous pouvez également associer automatiquement un processus d’approbation spécifique à un groupe à une tâche dans la zone Tâches de la zone Modifier le projet , ainsi qu’à des problèmes, lors de la configuration des files d’attente de requête ou des rubriques de file d’attente sur un projet.

Pour plus d’informations sur l’ajout de processus de validation aux projets, tâches et problèmes, consultez les articles suivants :

* [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Modification des problèmes](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Créer des processus d’approbation pour les groupes utilisant des états personnalisés

Afin de faciliter la gestion de leurs propres workflows uniques par les groupes, vous pouvez désormais utiliser des états personnalisés spécifiques aux groupes dans les processus d’approbation.

Auparavant, un groupe ne pouvait pas utiliser ses propres états personnalisés avec ses processus d’approbation spécifiques au groupe. Seuls les états à l’échelle du système étaient disponibles et ceux-ci ne correspondaient pas toujours aux processus d’approbation de groupe.

Les états personnalisés peuvent désormais être utilisés dans les processus d’approbation à usage unique et à l’échelle du système :

* Créez un processus d’approbation à usage unique pour un objet (projet, tâche ou problème) et basez-le sur les états associés au groupe travaillant sur cet objet. Cela inclut tous les états personnalisés associés au groupe.
* Créez un processus d’approbation globale et rendez-le disponible uniquement pour le groupe ou pour toutes les personnes du système.

Pour les utilisateurs disposant d’un accès administratif aux processus de validation, des informations sur la configuration des processus de validation sont disponibles dans [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (ou si vous utilisez Adobe Workfront Classic, voir [Création de processus de validation](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

Pour les utilisateurs, des informations sur l’association des processus d’approbation aux tâches sont disponibles dans [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (ou si vous utilisez Adobe Workfront Classic, voir [Association d’un processus d’approbation nouveau ou existant à un travail](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Nouvelles pages de superposition pour la recherche

Pour permettre aux utilisateurs de naviguer plus facilement entre les pages de recherche et les pages précédentes dans la nouvelle expérience Workfront, nous avons ajouté une page de recouvrement de recherche qui couvre partiellement l’écran.

Désormais, lorsque vous cliquez sur Recherche avancée dans le menu Rechercher ou que vous effectuez une recherche de base, une page s’ouvre dans la partie droite de l’écran.

Pour plus d’informations, voir [Rechercher dans Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Disponible dans ces environnements :**

* Nouvelle expérience Adobe Workfront

## Mises à jour des abonnements à un événement

Pour permettre aux utilisateurs de mieux trier, résoudre les problèmes et les problèmes, nous avons modifié le comportement et ajouté plus de données à l’API des abonnements à un événement. Nous avons également apporté les modifications suivantes :

* Technologies de messagerie sous-jacentes migrées
* Reconstruisez le service pour avoir des dépendances moins complexes et ainsi le dimensionner plus efficacement.
* Améliorations apportées à la surveillance et aux alertes

Pour en savoir plus, voir [Questions fréquentes - Abonnements à un événement](../../../wf-api/general/event-subs-faq.md) et [Bonnes pratiques relatives à l’abonnement aux événements](../../../wf-api/general/event-sub-best-practice.md).
