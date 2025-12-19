---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de la version 2018.1 Beta 3
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation de la version 2018.1 Beta 3. Cette fonctionnalité a été rendue disponible dans l’environnement de prévisualisation le 7 janvier 2018. Elle sera disponible dans l’environnement de production début 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 88%

---

# Activité de la version 2018.1 Beta 3

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation de la version 2018.1 Beta 3. Cette fonctionnalité a été rendue disponible dans l’environnement de prévisualisation le 7 janvier 2018. Elle sera disponible dans l’environnement de production début 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées dans la version 2018.1, consultez [Vue d’ensemble de l’activité de la version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version 2018.1 Beta 3 contient des améliorations pour les administrateurs et administratrices Workfront et les autres personnes :

**Pour les administrateurs et administratrices**

* [Améliorations apportées à l’administration de groupes](#group-administrator-improvements)

**Pour tous les utilisateurs et utilisatrices**

* [Améliorations de la visionneuse de relecture HTML5](#html5-proofing-viewer-improvements)
* [Améliorations de la relecture dans Workfront](#proofing-improvements-within-workfront)
* [Améliorations de la zone d’accueil](#home-area-improvements)
* [Améliorations Agile](#agile-improvements)
* [Améliorations du graphique de Gantt](#gantt-chart-improvements)
* [Améliorations du planificateur de ressources](#resource-planner-improvements)

## Améliorations apportées à l’administration de groupes {#group-administrator-improvements}

* [IU de réinitialisation du mot de passe mise à jour pour les administrateurs et administratrices de groupes](#reset-password-ui-updated-for-group-administrators)
* [Options de configuration du niveau d’accès pour les administrateurs et administratrices de groupes](#access-level-setup-options-for-group-administrators)
* [Créer des profils de feuille de temps pour les groupes](#create-timesheet-profiles-for-groups)
* [Récupérer des éléments supprimés pour les utilisateurs et utilisatrices en tant qu’administrateur ou administratrice de groupes](#recover-deleted-items-for-users-as-a-group-administrator)

### IU de réinitialisation du mot de passe mise à jour pour les administrateurs et administratrices de groupes {#reset-password-ui-updated-for-group-administrators}

En tant qu’administrateur ou administratrice de groupes, lorsque vous réinitialisez le mot de passe d’une autre personne, vous recevez une invitation à saisir votre propre mot de passe avant de pouvoir modifier le sien. L’IU a été mise à jour pour prendre en compte cette fonctionnalité. Avant cette modification, l’IU affichait que le mot de passe de l’administrateur ou de l’administratrice Workfront était obligatoire.

Pour plus d’informations sur la réinitialisation des mots de passe pour d’autres personnes, voir [Modifier le profil d’une personne](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Pour plus d’informations sur les fonctionnalités d’un administrateur de groupes, consultez la section « Fonctionnalités des administrateurs de groupes » de la section [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Options de configuration de niveau d’accès pour les administrateurs et administratrices de groupes {#access-level-setup-options-for-group-administrators}

En tant qu’administrateur ou administratrice Workfront, vous pouvez désormais contrôler si les administrateurs et administrarices de groupes peuvent se connecter en tant qu’autres personnes ou s’ils peuvent réinitialiser les mots de passe d’autres personnes. Nous avons ajouté un nouveau paramètre au niveau d’accès pour activer ou désactiver cet accès. Avant cette modification, tous les administrateurs et administratrices de groupes pouvaient par défaut se connecter en tant qu’autres personnes et réinitialiser les mots de passe d’autres personnes. Cette modification affecte uniquement le niveau d’accès Planification.

Pour plus d’informations sur la configuration du niveau d’accès pour les personnes, voir [Accorder l’accès aux utilisateurs et utilisatrices](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Pour plus d’informations sur les fonctionnalités d’un administrateur de groupes, consultez la section « Fonctionnalités des administrateurs de groupes » de la section [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Créer des profils de feuille de temps pour les groupes {#create-timesheet-profiles-for-groups}

En tant qu’administrateur ou administratrice de groupes, vous pouvez désormais créer des profils de feuille de temps pour les groupes que vous administrez et les associer aux groupes que vous administrez, ou aux utilisateurs et utilisatrices de ces groupes. Les profils de feuille de temps garantissent que les feuilles de temps sont automatiquement créées pour les personnes qui y sont associées.

Avant cette modification, seulement un administrateur ou une administratrice Workfront pouvait créer des profils de feuille de temps.

Pour plus d’informations sur la création de profils de feuille de temps, voir [Créer, modifier et affecter de profils de feuille de temps](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Pour plus d’informations sur les fonctionnalités d’un administrateur de groupes, consultez la section « Fonctionnalités des administrateurs de groupes » de la section [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Récupérer des éléments supprimés pour les utilisateurs et utilisatrices en tant qu’administrateur ou administratrice de groupes {#recover-deleted-items-for-users-as-a-group-administrator}

Si un projet est associé à un groupe pour lequel vous êtes l’administrateur ou l’administratrice de groupe, vous pouvez récupérer le projet, ou l’un de ses objects (tâches, problèmes ou documents) supprimés dans la Corbeille. Avant cette modification, seulement un administrateur ou une administratrice Workfront pouvait récupérer les éléments de la corbeille.

Pour plus d’informations sur la récupération des éléments supprimés dans Workfront, voir [Restaurer des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Pour plus d’informations sur les fonctionnalités d’un administrateur de groupes, consultez la section « Fonctionnalités des administrateurs de groupes » de la section [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

## Améliorations apportées à la visionneuse de relecture HTML5 {#html5-proofing-viewer-improvements}

* [Mode de comparaison](#compare-mode)
* [Filtrer la liste de commentaires](#filter-the-comment-list)
* [La recherche dans la liste de commentaires commence une fois le premier caractère saisi.](#comment-list-is-searched-after-the-first-character-is-entered)

### Mode de comparaison {#compare-mode}

Vous pouvez désormais utiliser le mode de comparaison dans la visionneuse de relecture HTML5 lors de l’affichage d’épreuves statiques et vidéo. 

Le mode de comparaison dans la visionneuse de relecture HTML5 diffère de la visionneuse de relecture héritée sur plusieurs points :

* Lors du lancement du mode de comparaison, la version la plus récente se déplace vers la droite, et la version que vous comparez s’ouvre à gauche.

  Auparavant, la version la plus récente était déplacée vers la gauche, et la version que vous compariez s’ouvrait à droite.

* Vous pouvez choisir la version d’une épreuve que vous souhaitez comparer directement à partir de la visionneuse de relecture. 
* Le niveau de zoom actuel et la position des épreuves dans la visionneuse de relecture sont conservés lors de l’accès à la navigation simultanée.
* Nouvelle option Réinitialiser lorsque vous utilisez la navigation simultanée.
* Lorsque vous quittez le mode de comparaison, vous pouvez choisir quelle épreuve fermer. 

  Auparavant, c’était l’ancienne version qui était toujours fermée.

* Diverses améliorations de l’aspect et de la convivialité.

Pour plus d’informations, voir [Comparer des épreuves dans la visionneuse de relecture](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md).

### Filtrer la liste de commentaires {#filter-the-comment-list}

Vous pouvez désormais filtrer les commentaires dans la liste des commentaires. Vous pouvez filtrer par utilisateur ou utilisatrice, action, non lu, etc.

### La recherche dans la liste de commentaires commence une fois le premier caractère saisi. {#comment-list-is-searched-after-the-first-character-is-entered}

Désormais, lors de la recherche dans la liste de commentaires, la liste est automatiquement filtrée une fois que vous avez saisi le premier caractère.

Avant cette modification, vous deviez saisir au moins 3 caractères dans le champ de recherche avant que la liste de commentaires ne soit filtrée.

Pour plus d’informations, voir :

## Améliorations de la relecture dans Workfront {#proofing-improvements-within-workfront}

* [Lier les épreuves de Workfront Proof vers Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [Il n’est plus possible de supprimer une épreuve d’un document.](#can-no-longer-remove-a-proof-from-a-document)
* [Mise à jour de l’aspect lors de la génération et de l’ouverture d’épreuves](#updated-look-and-feel-when-generating-and-opening-proofs)

### Lier des épreuves de Workfront Proof à Workfront {#link-proofs-from-workfront-proof-to-workfront}

Vous pouvez désormais lier des épreuves de documents qui existent déjà dans votre compte Workfront Proof à Workfront.

Avant cette modification, vous ne pouviez pas accéder aux épreuves qui existaient déjà dans Workfront Proof à partir de Workfront. 

Pour plus d’informations, voir [Lier des documents d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) dans [Lier des documents d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Il n’est plus possible de supprimer une épreuve d’un document. {#can-no-longer-remove-a-proof-from-a-document}

Vous ne pouvez plus supprimer une épreuve d’un document. Pour supprimer une épreuve, vous devez supprimer l’intégralité du document.

Cette amélioration réduit le risque que les utilisateurs et utilisatrices suppriment par inadvertance toutes les versions d’un document révisé. 

Pour plus d’informations sur la suppression d’un document, voir [Supprimer une épreuve](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) dans [Supprimer une épreuve](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md).

### Mise à jour de l’aspect lors de la génération et de l’ouverture d’épreuves {#updated-look-and-feel-when-generating-and-opening-proofs}

Il y a maintenant une animation rotative mise à jour lors de la génération d’une épreuve.

## Améliorations de la zone d’accueil {#home-area-improvements}

Les améliorations suivantes ont été apportées à la zone d’accueil :

* [Afficher les approbations d’épreuves à partir de la zone d’accueil](#view-proof-approvals-from-the-home-area)
* [Les champs par défaut s’affichent lors de la configuration du modèle de mise en page pour les éléments de la zone Page de départ.](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Afficher les approbations d’épreuves à partir de la zone d’accueil {#view-proof-approvals-from-the-home-area}

Vous pouvez désormais visualiser les approbations d’épreuves dans la zone d’accueil, en plus des approbations standard.

Auparavant, vous pouviez afficher les approbations Workfront, mais pas les approbations d’une épreuve. 

Pour plus d’informations, voir [Utiliser la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### Les champs par défaut s’affichent lors de la configuration du modèle de mise en page pour les éléments de la zone Page de départ. {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

Auparavant, les champs par défaut n’étaient pas visibles à partir du modèle de mise en page.

Pour plus d’informations, voir « Créer et gérer des modèles de mise en page ».

## Améliorations de la méthode Agile {#agile-improvements}

* [Ajouter des tâches et des problèmes à l’itération directement à partir de la page Détails de la tâche ou du problème](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [Inclure des problèmes sur la liste d’attente Scrum et le storyboard pour une équipe Agile](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [Appliquer des groupes et des filtres à la liste d’attente pour une équipe Agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Créer une itération vierge et la mettre à jour ultérieurement](#create-a-blank-iteration-and-update-it-later)
* [Les champs « Thème » et « Capacité » sont préremplis lors de la création d’une itération.](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Ajouter directement des tâches et des problèmes à l’itération à partir de la page Détails de la tâche ou du problème {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

Vous pouvez désormais ajouter des tâches et des événements actuellement affectés à une équipe Agile à une itération directement à partir de la tâche ou de l’événement.

Auparavant, vous pouviez ajouter des tâches à une itération uniquement à partir de la liste d’attente. 

Pour plus d’informations, voir [Créer une itération](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) dans [Créer une itération](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Inclure des problèmes sur la liste d’attente et le storyboard Scrum d’une équipe Agile {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

Les événements sont désormais inclus par défaut dans la liste d’attente de votre équipe Agile lors de l’utilisation de la méthodologie Scrum Agile (les événements ne s’affichent pas dans la liste d’attente d’une équipe Agile lors de l’utilisation de la méthodologie Kanban).

Avant cette modification, seules les tâches pouvaient être ajoutées à la liste d’attente. Si vous vouliez ajouter un problème, vous deviez d’abord le convertir en une tâche avant de pouvoir l’ajouter.

Pour plus d’informations sur l’utilisation des événements dans la liste d’attente, voir  [Gérer la liste d’attente Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Appliquer des regroupements et des filtres à la liste d’attente d’une équipe Agile {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

Les options Regroupement et Filtre sont désormais disponibles dans la liste d’attente Agile. Vous pouvez ainsi organiser votre liste d’attente par regroupements et filtrer des tâches et des événements spécifiques.

Avant cette modification, vous pouviez appliquer des vues à la liste d’attente Agile.

Pour plus d’informations, voir  [Gérer la liste d’attente Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) dans  [Gérer la liste d’attente Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Créer une itération vierge et la mettre à jour ultérieurement {#create-a-blank-iteration-and-update-it-later}

Vous n’avez plus besoin d’ajouter une tâche ou un problème à une itération pour la créer. Vous pouvez créer une itération vierge et ajouter ultérieurement des tâches et des problèmes.

Pour plus d’informations, voir [Créer une itération](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Les champs « Thème » et « Capacité » sont préremplis lors de la création d’une itération. {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

Désormais, lors de la création d’une itération, les champs « Mise au point » et « Capacité » sont prérenseignés avec les valeurs moyennes de toutes les itérations antérieures que votre équipe a créées. Si votre équipe n’a pas créé d’itérations antérieures, ces champs apparaissent sur 0.

Auparavant, ces champs étaient toujours définis sur 0.

Pour plus d’informations, voir [Créer une itération](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Améliorations du graphique de Gantt {#gantt-chart-improvements}

* [Activer le mode de modification dans le graphique de Gantt](#enable-edit-mode-in-the-gantt-chart)
* [Supprimer les tâches antérieures lors de la modification du graphique de Gantt](#remove-predecessors-when-editing-the-gantt-chart)

### Activer le mode de modification dans le graphique de Gantt {#enable-edit-mode-in-the-gantt-chart}

Lorsque vous activez le mode de modification dans le graphique de Gantt, vous pouvez apporter des modifications aux informations contenues dans le graphique. Avant cette modification, vous ne pouviez pas modifier les informations du graphique de Gantt. Vous ne pouviez modifier que les informations de la tâche dans la liste des tâches.

Pour plus d’informations sur la modification du graphique de Gantt, voir [Mettre à jour des informations dans le graphique de Gantt de la liste des tâches](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Supprimer les tâches antérieures lors de la modification du graphique de Gantt {#remove-predecessors-when-editing-the-gantt-chart}

En utilisant le mode de modification du graphique Gantt, vous pouvez désormais supprimer les relations antérieures entre les tâches dans le graphique Gantt d’un projet. Avant cette amélioration, vous ne pouviez supprimer la relation antérieure que dans la liste des tâches ou au niveau de la tâche.

Pour plus d’informations sur la modification du graphique de Gantt, voir [Mettre à jour des informations dans le graphique de Gantt de la liste des tâches](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Améliorations du planificateur de ressources {#resource-planner-improvements}

* [Budget avec une durée nulle dans le planificateur de ressources](#budget-with-zero-duration-in-the-resource-planner)

* [Afficher les données par coût dans le planificateur de ressources](#show-data-by-cost-in-the-resource-planner)

### Budget avec une durée nulle dans le planificateur de ressources {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de l’environnement de prévisualisation et est publiée avec la version 18.1.

Vous pouvez désormais budgéter vos ressources dans le planificateur de ressources pour n’importe quelle date, pendant ou en dehors de la période du projet. Avant cette amélioration, vous ne pouviez budgéter vos ressources que pour les dates correspondant à la période du projet.

Pour plus d’informations sur l’établissement du budget des ressources dans le planificateur de ressources, voir la section « Établir un budget des ressources dans le planificateur de ressources » dans [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Afficher les données par coût dans le planificateur de ressources {#show-data-by-cost-in-the-resource-planner}

Vous pouvez désormais afficher les informations dans le planificateur de ressources par coût, en plus des valeurs Heures et FTE. Vous pouvez afficher les coûts dans le planificateur de ressources lorsque vous le consultez dans les vues Par projet ou Par rôle. Vous ne pouvez pas afficher les coûts lorsque vous affichez le planificateur de ressources dans la vue Par utilisateur et utilisatrice.

Pour plus d’informations sur l’affichage du planificateur de ressources par valeurs d’heures, de FTE ou de coûts, voir [Vue d’ensemble de la navigation dans le planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
