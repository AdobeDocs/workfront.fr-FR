---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.1, version bêta 3
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.1 de Beta 3. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 7 janvier 2018. Il sera disponible dans l'environnement de production début 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# Activité Version 2018.1, version bêta 3

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.1 de Beta 3. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 7 janvier 2018. Il sera disponible dans l&#39;environnement de production début 2018.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.1, voir  [Présentation de l’activité de version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version 2018.1 de Beta 3 contient des améliorations pour les administrateurs de Workfront et d’autres utilisateurs :

**Pour les administrateurs**

* [Améliorations apportées à l’administrateur de groupe](#group-administrator-improvements)

**Pour Tous Les Utilisateurs**

* [Améliorations de la visionneuse de vérification d’HTML5](#html5-proofing-viewer-improvements)
* [ Améliorations de la vérification dans Workfront](#proofing-improvements-within-workfront)
* [Améliorations de la zone d’accueil](#home-area-improvements) 
* [Améliorations rapides](#agile-improvements)
* [Améliorations du diagramme de Gantt](#gantt-chart-improvements)
* [Améliorations du planificateur de ressources](#resource-planner-improvements)

## Améliorations apportées à l’administrateur de groupe {#group-administrator-improvements}

* [Réinitialiser l’interface utilisateur de mot de passe Mise à jour pour les administrateurs de groupe](#reset-password-ui-updated-for-group-administrators)
* [Options de configuration de niveau d’accès pour les administrateurs de groupe](#access-level-setup-options-for-group-administrators)
* [Création de profils de feuille de temps pour les groupes](#create-timesheet-profiles-for-groups)
* [Récupération des éléments supprimés pour les utilisateurs en tant qu’administrateur de groupe](#recover-deleted-items-for-users-as-a-group-administrator)

### Réinitialiser l’interface utilisateur du mot de passe Mise à jour pour les administrateurs de groupe {#reset-password-ui-updated-for-group-administrators}

En tant qu’administrateur de groupe, lorsque vous réinitialisez le mot de passe d’un autre utilisateur, vous êtes invité à saisir votre propre mot de passe avant de pouvoir modifier le leur. L’interface utilisateur a été mise à jour pour prendre en compte cette fonctionnalité. Avant cette modification, l’interface utilisateur affichait que le mot de passe administrateur de Workfront était requis.

Pour plus d’informations sur la réinitialisation des mots de passe pour d’autres utilisateurs, voir [Modification du profil d’un utilisateur](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Pour plus d’informations sur les fonctionnalités d’un administrateur de groupe, voir la section &quot;Fonctionnalités des administrateurs de groupe&quot; dans [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Options de configuration de niveau d’accès pour les administrateurs de groupe {#access-level-setup-options-for-group-administrators}

En tant qu’administrateur Workfront, vous pouvez désormais contrôler si les administrateurs de groupe peuvent se connecter en tant qu’autres utilisateurs ou s’ils peuvent réinitialiser les mots de passe des autres utilisateurs. Nous avons ajouté un nouveau paramètre au niveau d’accès pour activer ou désactiver cet accès. Avant cette modification, tous les administrateurs de groupe pouvaient se connecter en tant qu’autres utilisateurs et réinitialiser les mots de passe des autres utilisateurs par défaut. Cette modification affecte uniquement le niveau d’accès du planificateur.

Pour plus d’informations sur la configuration du niveau d’accès pour les utilisateurs, voir [Octroi de l’accès aux utilisateurs](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Pour plus d’informations sur les fonctionnalités d’un administrateur de groupe, voir la section &quot;Fonctionnalités des administrateurs de groupe&quot; dans [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Création de profils de feuille de temps pour les groupes {#create-timesheet-profiles-for-groups}

En tant qu’administrateur de groupe, vous pouvez désormais créer des profils de feuille de temps pour les groupes que vous administrez et les associer aux groupes que vous administrez, ou aux utilisateurs de ces groupes. Les profils de feuille de temps garantissent que les feuilles de temps sont automatiquement créées pour les utilisateurs qui y sont associés.

Avant cette modification, seul un administrateur Workfront pouvait créer des profils de feuille de temps.

Pour plus d’informations sur la création de profils de feuille de temps, voir [Création, modification et affectation de profils de feuille de temps](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Pour plus d’informations sur les fonctionnalités d’un administrateur de groupe, voir la section &quot;Fonctionnalités des administrateurs de groupe&quot; dans [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Récupération des éléments supprimés pour les utilisateurs en tant qu’administrateur de groupe {#recover-deleted-items-for-users-as-a-group-administrator}

Si un projet est associé à un groupe pour lequel vous êtes l’administrateur du groupe, vous pouvez récupérer le projet, ou l’une de ses tâches, problèmes ou documents supprimés dans la Corbeille. Avant cette modification, seul un administrateur Workfront pouvait récupérer les éléments de la corbeille.

Pour plus d’informations sur la récupération des éléments supprimés dans Workfront, voir [Restaurer les éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Pour plus d’informations sur les fonctionnalités d’un administrateur de groupe, voir la section &quot;Fonctionnalités des administrateurs de groupe&quot; dans [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

## Améliorations de la visionneuse de vérification d’HTML5  {#html5-proofing-viewer-improvements}

* [Mode de comparaison](#compare-mode)
* [Filtrer la liste des commentaires](#filter-the-comment-list)
* [La liste de commentaires est recherchée une fois le premier caractère saisi](#comment-list-is-searched-after-the-first-character-is-entered)

### Mode de comparaison {#compare-mode}

Vous pouvez désormais utiliser le mode de comparaison dans la visionneuse de vérification de l’HTML5 lors de l’affichage de BAT statique et vidéo. 

Le mode de comparaison dans la visionneuse de vérification d’HTML5 diffère de la visionneuse de vérification d’anciennes versions de la manière suivante :

* Lors du lancement du mode Comparer , la version la plus récente se déplace vers la droite, avec la version que vous comparez à l’ouverture sur la gauche.

  Auparavant, la version la plus récente était déplacée vers la gauche, la version que vous compariez à l’ouverture à droite.

* Vous pouvez choisir la version d’un BAT que vous souhaitez comparer directement à partir de la visionneuse de vérification. 
* Le niveau de zoom actuel et la position des bons à tirer dans la visionneuse de BAT sont conservés lors de l’accès à la navigation simultanée.
* Nouvelle option Réinitialiser lorsque vous utilisez la navigation simultanée.
* Lorsque vous quittez le mode de comparaison, vous pouvez choisir le BAT à fermer. 

  Auparavant, l’ancienne version était toujours fermée.

* Diverses améliorations de l’aspect et de la convivialité.

Pour plus d’informations, voir [Comparaison des bons à tirer dans la visionneuse de vérification de performance](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md).

### Filtrage de la liste de commentaires {#filter-the-comment-list}

Vous pouvez désormais filtrer les commentaires dans la liste des commentaires. Vous pouvez filtrer par utilisateur, action, non lu, etc.

### La liste de commentaires est recherchée une fois le premier caractère saisi {#comment-list-is-searched-after-the-first-character-is-entered}

Désormais, lors de la recherche dans la liste de commentaires, la liste est automatiquement filtrée une fois que vous avez saisi le premier caractère.

Avant cette modification, vous deviez saisir au moins 3 caractères dans le champ de recherche avant que la liste de commentaires ne soit filtrée.

Pour plus d’informations, voir .

## Améliorations de la vérification dans Workfront {#proofing-improvements-within-workfront}

* [Liaison de BAT de Workfront Proof à Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [ Ne peut plus supprimer un BAT d’un document](#can-no-longer-remove-a-proof-from-a-document)
* [Mise à jour de l’aspect lors de la génération et de l’ouverture de BAT](#updated-look-and-feel-when-generating-and-opening-proofs)

### Lier des bons à tirer de Workfront Proof à Workfront {#link-proofs-from-workfront-proof-to-workfront}

Vous pouvez désormais lier les BAT de document qui existent déjà dans votre compte Workfront Proof à Workfront.

Avant cette modification, vous ne pouviez pas accéder aux bons à tirer qui existaient déjà dans Workfront Proof dans Workfront. 

Pour plus d’informations, reportez-vous à la section [ Lier des documents à partir d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) dans [Lier des documents à partir d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Impossible de supprimer un bon à tirer d’un document {#can-no-longer-remove-a-proof-from-a-document}

Vous ne pouvez plus supprimer un BAT d’un document. Pour supprimer un BAT, vous devez supprimer l’intégralité du document.

Cette amélioration réduit le risque que les utilisateurs suppriment par inadvertance toutes les versions d’un document révisé. 

Pour plus d’informations sur la suppression d’un document, voir [Suppression d’un BAT](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) dans [Suppression d’un BAT](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md).

### Mise à jour de l’aspect lors de la génération et de l’ouverture de BAT {#updated-look-and-feel-when-generating-and-opening-proofs}

Il y a maintenant un compteur d&#39;animations mis à jour lorsqu&#39;un bon à tirer est généré.

## Améliorations de la zone d’accueil {#home-area-improvements}

Les améliorations suivantes ont été apportées à la zone d’accueil :

* [ Afficher les validations de BAT depuis la zone d’accueil](#view-proof-approvals-from-the-home-area)
* [Les champs par défaut s’affichent lors de la configuration du modèle de mise en page pour les éléments de la zone d’accueil.](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Afficher les validations de BAT depuis la zone d’accueil {#view-proof-approvals-from-the-home-area}

Vous pouvez désormais visualiser les validations de BAT dans la zone d&#39;accueil, en plus des validations standard.

Auparavant, vous pouviez afficher les approbations Workfront, mais pas les approbations pour un BAT.  

Pour plus d’informations, voir [Utilisation de la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### Les champs par défaut s’affichent lors de la configuration du modèle de mise en page pour les éléments de la zone d’accueil. {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

Auparavant, les champs par défaut n’étaient pas visibles à partir du modèle de mise en page.

Pour plus d’informations, voir &quot;Création et gestion des modèles de mise en page&quot;.

## Améliorations rapides {#agile-improvements}

* [Ajout de tâches et de problèmes à l’itération directement à partir de la page Détails de la tâche ou du problème](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [ Incluez les problèmes sur le Backlog et le Story Board pour une équipe agile ](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [Appliquer les groupes et les filtres au journal pour une équipe agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Créer une itération vierge et la mettre à jour ultérieurement](#create-a-blank-iteration-and-update-it-later)
* [Les champs &quot;Focus&quot; et &quot;Capacité&quot; sont préremplis lors de la création d’une itération](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Ajout direct de tâches et de problèmes à l’itération à partir de la page Détails de la tâche ou du problème {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

Vous pouvez désormais ajouter des tâches et des problèmes actuellement affectés à une équipe agile à une itération directement à partir de la tâche ou du problème.

Auparavant, vous pouviez ajouter des tâches à une itération uniquement à partir du journal. 

Pour plus d’informations, voir [Créer une itération](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) dans [Créer une itération](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Inclure des problèmes sur le dossier des dossiers et le tableau d’article pour une équipe agile {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

Les problèmes sont désormais inclus par défaut dans le journal de votre équipe agile lors de l’utilisation de la méthodologie Scrum agile (les problèmes ne s’affichent pas dans le journal d’une équipe agile lors de l’utilisation de la méthodologie Kanban).

Avant cette modification, seules les tâches pouvaient être ajoutées au journal. Si vous vouliez ajouter un problème, vous deviez d’abord le convertir en une tâche avant de pouvoir l’ajouter.

Pour plus d’informations sur l’utilisation des problèmes sur le journal en souffrance, voir  [Gérez le journal agile ](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Application de groupes et de filtres au journal pour une équipe agile {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

Les options Groupement et Filtre sont désormais disponibles sur le journal en souffrance agile, ce qui vous permet d&#39;organiser votre journal en souffrance par groupes, ainsi que de filtrer les tâches et problèmes spécifiques.

Avant cette modification, vous pouviez appliquer les vues au journal agile.

Pour plus d’informations, voir  [Gérer le journal en souffrance agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) dans  [Gérez le journal agile ](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Créer une itération vierge et la mettre à jour ultérieurement {#create-a-blank-iteration-and-update-it-later}

Vous n’avez plus besoin d’ajouter une tâche ou un problème à une itération pour la créer. Vous pouvez créer une itération vierge et ajouter ultérieurement des tâches et des problèmes.

Pour plus d’informations, voir [Création d’une itération](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Les champs &quot;Focus&quot; et &quot;Capacité&quot; sont préremplis lors de la création d’une itération {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

Désormais, lors de la création d’une itération, les champs &quot;Mise au point&quot; et &quot;Capacité&quot; sont prérenseignés avec les valeurs moyennes de toutes les itérations antérieures que votre équipe a créées. Si votre équipe n’a pas créé d’itérations antérieures, ces champs apparaissent comme étant 0.

Auparavant, ces champs étaient toujours définis sur 0.

Pour plus d’informations, voir [Création d’une itération](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Améliorations du diagramme de Gantt {#gantt-chart-improvements}

* [Activer le mode d’édition dans le diagramme de Gantt](#enable-edit-mode-in-the-gantt-chart)
* [Suppression des prédécesseurs lors de la modification du diagramme de Gantt](#remove-predecessors-when-editing-the-gantt-chart)

### Activation du mode d’édition dans le diagramme de Gantt {#enable-edit-mode-in-the-gantt-chart}

Lorsque vous activez le mode d’édition dans le diagramme de Gantt, vous pouvez apporter des modifications aux informations contenues dans le graphique. Avant cette modification, vous ne pouviez pas modifier les informations du diagramme de Gantt. Vous ne pouvez modifier que les informations de la tâche dans la liste des tâches.

Pour plus d’informations sur la modification du diagramme de Gantt, voir [Mise à jour d’informations dans la liste de tâches du diagramme de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Suppression des prédécesseurs lors de la modification du diagramme de Gantt {#remove-predecessors-when-editing-the-gantt-chart}

En utilisant le mode d’édition du graphique Gantt, vous pouvez désormais supprimer les relations de prédécesseur entre les tâches dans le diagramme Gantt d’un projet. Avant cette amélioration, vous ne pouviez supprimer la relation de prédécesseur que dans la liste des tâches ou au niveau de la tâche.

Pour plus d’informations sur la modification du diagramme de Gantt, voir [Mise à jour d’informations dans la liste de tâches du diagramme de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Améliorations du planificateur de ressources {#resource-planner-improvements}

* [Budget avec durée zéro dans le planificateur de ressources](#budget-with-zero-duration-in-the-resource-planner)

* [Afficher les données par coût dans le planificateur de ressources](#show-data-by-cost-in-the-resource-planner)

### Budget avec durée zéro dans le planificateur de ressources {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de l’environnement Aperçu et est en train de sortir avec la version 18.1.

Vous pouvez désormais budgéter vos ressources dans le planificateur de ressources pour n’importe quelle date, pendant ou en dehors de la période du projet. Avant cette amélioration, vous ne pouviez budgéter vos ressources que pour les dates correspondant à la période du projet.

Pour plus d’informations sur la planification des ressources dans le planificateur de ressources, consultez la section &quot;Ressources de planification budgétaire dans le planificateur de ressources&quot; dans la [présentation du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Afficher les données par coût dans le planificateur de ressources {#show-data-by-cost-in-the-resource-planner}

Vous pouvez désormais afficher les informations dans le planificateur de ressources par coût, en plus des valeurs Heures et ETR. Vous pouvez afficher les coûts dans le planificateur de ressources lorsque vous le visualisez dans les modes Affichage par projet ou Affichage par rôle . Vous ne pouvez pas afficher les coûts lorsque vous affichez le planificateur de ressources dans la vue Vue par utilisateur.

Pour plus d’informations sur l’affichage des valeurs de planificateur de ressources par heure, ETR ou Coût, consultez la [présentation de la navigation du planificateur de ressource](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
