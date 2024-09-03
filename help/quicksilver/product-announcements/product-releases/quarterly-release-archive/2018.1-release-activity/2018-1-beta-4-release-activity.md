---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.1 bêta 4
description: Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version 2018.1 bêta 4. La fonctionnalité a été mise à disposition dans l’environnement de prévisualisation le 24 janvier 2018. Elles seront disponibles dans l’environnement de production en mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 100%

---

# Activité Version 2018.1 bêta 4

Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version 2018.1 bêta 4.La fonctionnalité a été mise à disposition dans l’environnement de prévisualisation le 24 janvier 2018. Elles seront disponibles dans l’environnement de production en mars 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées dans la version 2018.1, consultez [Vue d’ensemble de l’activité de la version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version 2018.1 bêta 4 contient des améliorations pour les administrateurs et administratrices Workfront et les autres personnes :

**Pour les administrateurs et administratrices**

* [Plannings gérés par les administrateurs et administratrices de groupes](#schedules-managed-by-group-administrators)

**Pour tous les utilisateurs et utilisatrices**

* [Améliorations de la relecture dans Workfront](#proofing-improvements-within-workfront)
* [Création des épreuves dans Workfront Proof - Amélioration de l’expérience client et fonctionnalités supplémentaires](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [Améliorations de la relecture dans Workfront et Workfront Proof](#proofing-improvements-within-workfront-and-workfront-proof)
* [Aspect mis à jour avec l’intégration de Basecamp dans Workfront Proof](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [Coller des images dans Workfront à partir du presse-papiers](#paste-images-to-workfront-from-the-clipboard)
* [Améliorations du rapport d’utilisation](#utilization-report-improvements)
* [Suppression de l’objet Heures budgétées pour les ressources de Workfront](#remove-the-resource-budgeted-hour-object-from-workfront)
* [Rapport sur les statistiques d’utilisation](#report-usage-statistics)
* [Mises à jour du graphique de Gantt](#gantt-chart-updates)
* [Nouvel optimisateur de portfolio](#new-portfolio-optimizer)
* [Option de réglage de la date du budget dans le planificateur de ressources](#budget-date-adjustment-option-in-the-resource-planner)
* [Planification des ressources : restreindre les affectations aux personnes en fonction de leur appartenance à un groupe](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [Planification des ressources : autoriser les affectations aux personnes indépendamment de leur rôle](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Prise en charge d’émoticônes](#emoji-support)

## Améliorations de la relecture dans Workfront {#proofing-improvements-within-workfront}

Les améliorations suivantes ont été apportées à la liste des documents dans Workfront :

* [Afficher la progression de la relecture à partir de la liste des documents](#view-proof-progress-from-the-document-list)
* [Nouvelle option pour afficher le résumé de l’impression à partir de la liste des documents](#new-option-to-view-the-print-summary-from-the-document-list)
* [Aspect mis à jour pour la génération ou l’ouverture de l’épreuve à partir de la liste des documents](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [Divers liens supprimés des documents de la liste des documents](#various-links-removed-from-documents-on-the-document-list)
* [Afficher les noms de fichiers sur les épreuves combinées](#view-file-names-on-combined-proofs)
* [Afficher l’étape active actuelle d’une épreuve à partir de la liste de documents](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### Afficher la progression de la relecture à partir de la liste des documents {#view-proof-progress-from-the-document-list}

Les indicateurs de progression de la relecture sont désormais affichés pour toutes les épreuves lors de l’affichage de la liste des documents. (Cela comprend Ies messages envoyés, ouverts, les commentaires formulés et la décision.)

Avant cette modification, vous deviez sélectionner une épreuve dans la liste des documents pour voir la progression de la relecture dans le panneau de droite. 

Pour plus d’informations, voir [Vue d’ensemble de la progression de la relecture et du statut des épreuves](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

### Nouvelle option pour afficher le résumé de l’impression à partir de la liste des documents {#new-option-to-view-the-print-summary-from-the-document-list}

Vous pouvez désormais afficher le résumé de l’impression d’une épreuve directement à partir de la liste des documents.

Avant cette modification, vous ne pouviez afficher le résumé de l’impression qu’à partir de la visionneuse de relecture. 

Pour plus d’informations sur l’affichage du résumé de l’impression à partir de la liste des documents, voir [Imprimer un résumé de l’épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Aspect mis à jour pour la génération ou l’ouverture des épreuves à partir de la liste des documents {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

Maintenant, lorsque vous pointez sur un document dans la liste des documents, les options de génération ou d’ouverture d’épreuve ont été mises à jour. Ces options sont maintenant plus visibles et apparaissent sous la forme de boutons.

Avant cette modification, ces options étaient disponibles sous forme de liens sous le nom du document.

Pour plus d’informations, consultez les sections suivantes :

* .
* dans .

### Divers liens supprimés des documents dans la liste de documents {#various-links-removed-from-documents-on-the-document-list}

Les actions suivantes ne sont plus disponibles en tant que liens sur des documents individuels dans la liste de documents :

* Créer une épreuve
* Épreuve
* Détails
* Partager
* Extraire/Archiver

Les actions suivantes sont désormais disponibles sous forme de bouton dans le document au sein de la liste de documents :

* Ouvrir une épreuve (disponible après la génération de l’épreuve)
* Générer une épreuve (disponible lorsque l’épreuve n’est pas encore générée)

Les actions suivantes sont désormais disponibles dans le menu déroulant en regard du bouton Ouvrir une épreuve ou Générer une épreuve :

* Détails de l&#39;épreuve
* Détails du document
* Imprimer le résumé

Pour plus d’informations, consultez les sections suivantes :

* .
* dans .

### Afficher les noms de fichier sur les épreuves combinées {#view-file-names-on-combined-proofs}

Vous pouvez désormais afficher les noms de fichiers individuels qui constituent une épreuve combinée. Ces informations s’affichent dans l’onglet Détails lorsque l’épreuve est sélectionnée dans la liste des documents.

Pour plus d’informations, voir Afficher tous les fichiers contenus dans une épreuve combinée. 

### Afficher l’étape active actuelle d’une épreuve à partir de la liste de documents {#view-the-current-active-stage-of-a-proof-from-the-document-list}

Désormais, lorsque vous sélectionnez une épreuve dans la liste de documents, les étapes actives actuelles s’affichent dans la colonne de droite de l’onglet Détails. 

Pour plus d’informations, voir [Afficher les étapes actives sur une épreuve](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md).

## Création d’épreuves dans Workfront Proof - Expérience d’utilisation améliorée et fonctionnalités supplémentaires {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

Outre une meilleure expérience d’utilisation lors de la création d’épreuves dans Workfront Proof, les fonctionnalités supplémentaires suivantes sont désormais disponibles :

* Combiner plusieurs images en une seule épreuve.
* Relire des sites web en plusieurs résolutions (plusieurs résolutions peuvent être créées sous la forme d’épreuves individuelles ou combinées en une seule épreuve).
* Modifier le nom du fichier pendant le processus de chargement.
* Inclure des champs personnalisés dans le formulaire de création d’épreuve.
* Ajouter un message personnalisé pour les notifications d’épreuves par e-mail.
* Paramètres supplémentaires d’épreuves
* Validation des erreurs en temps réel lors de la relecture d’une URL (auparavant, vous deviez attendre plusieurs minutes avant qu’une erreur ne s’affiche)

>[!NOTE]
>
>Cette nouvelle page de création d’épreuves dans Workfront Proof correspond désormais à la page de création d’épreuves récemment mise à disposition lors de la création d’épreuves dans Workfront. 

Pour plus d’informations, voir [Générer une épreuve dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Améliorations de la relecture dans Workfront et Workfront Proof {#proofing-improvements-within-workfront-and-workfront-proof}

Les modifications suivantes s’appliquent lors de l’ajout de documents à Workfront et à Workfront Proof :

* [Redimensionner la liste des commentaires lors de la révision des épreuves](#resize-the-comment-list-when-reviewing-proofs)
* [Hyperliens actifs lors de la révision d’épreuves statiques](#hyperlinks-are-active-when-reviewing-static-proofs)
* [Améliorations de l’ajout d’épreuves](#improvements-when-adding-proofs)

### Redimensionner la liste des commentaires lors de la révision des épreuves {#resize-the-comment-list-when-reviewing-proofs}

Vous pouvez désormais redimensionner la liste de commentaires lors de la révision d’épreuves dans la visionneuse de relecture.

Pour plus d’informations, voir :

### Les hyperliens sont actifs lors de la révision des épreuves statiques. {#hyperlinks-are-active-when-reviewing-static-proofs}

Les liens hypertextes sont désormais actifs lors de la révision d’une épreuve statique dans la visionneuse de relecture. Cliquez sur un lien hypertexte pour accéder à la page liée.

Cette fonctionnalité est prise en charge dans tous les types de fichiers qui contiennent du texte, tels que PDF, DOC, etc. Les fichiers image ne sont pas pris en charge.

### Améliorations de l’ajout d’épreuves {#improvements-when-adding-proofs}

Les améliorations suivantes sont disponibles lorsque des documents à réviser sont ajoutés. 

* Les informations contenues dans la liste des personnes destinataires sont désormais disponibles dans une vue à 3 colonnes, ce qui facilite l’affichage et la modification des informations. 

  Auparavant, les informations étaient affichées dans une seule colonne, obligeant à multiplier les clics pour effectuer des modifications. 

  Pour plus d’informations, voir :

* Faites glisser une ou plusieurs personnes destinataires d’une étape du workflow vers une autre lorsque vous utilisez la fonction de workflow automatisé. Vous pouvez glisser directement vers une étape ou vers une étape du diagramme, situé en haut de la page.

  Pour plus d’informations, voir :

* Le diagramme de workflow reste visible en haut de la page même lorsque vous faites défiler la page. Le diagramme est réduit par défaut ; développez le pour l’afficher dans son intégralité.

  Pour plus d’informations, voir :

* Lorsque vous ajoutez un modèle à un workflow automatisé dans une épreuve, une animation de chargement s’affiche, indiquant que le modèle est en train de se charger.

  Pour plus d’informations, voir :

* Les paramètres suivants ont été déplacés de la section des paramètres de l’épreuve à la section du workflow sur la page de la nouvelle épreuve :

   * Décisionnaire principal
   * Exiger une seule décision

## Aspect actualisé de l’intégration Basecamp dans Workfront Proof {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

L’aspect de l’intégration Basecamp dans Workfront Proof a été actualisé. La fonctionnalité reste la même.

## Coller des images dans Workfront à partir du presse-papiers {#paste-images-to-workfront-from-the-clipboard}

Vous pouvez désormais ajouter des fichiers images à Workfront en collant une image à partir du presse-papiers de votre système.

La possibilité de coller à partir du presse-papiers avait été supprimée de Workfront dans une version précédente ; elle est réintroduite dans cette version. La nouvelle méthode est plus simple et intuitive.

Pour plus d’informations, consultez la section [Coller des images à partir du presse-papiers](../../../../documents/managing-documents/paste-image-clipboard.md).

## Améliorations des rapports d’utilisation {#utilization-report-improvements}

Le rapport d’utilisation contient les améliorations suivantes :

* Afficher les revenus dans le rapport d’utilisation d’un projet

  Permet d’afficher les revenus budgétés, les revenus prévus, les revenus réels, la variance budgétée et la variance prévue.

* Comparer les revenus aux coûts prévus et réels

  Permet d’afficher le coût prévu ou réel à côté des revenus prévus. La marge (%) est également affichée (la marge est calculée comme suit : revenus - coût / revenus).

* Les revenus s’affichent lors de l’affichage du graphique.
* Les en-têtes restent visibles lors du défilement.

  Désormais, lorsque vous faites défiler les informations dans le rapport d’utilisation, l’en-tête en haut du rapport est toujours visible, vous permettant ainsi de comprendre plus facilement les données du rapport.

  Auparavant, l’en-tête en haut du rapport d’utilisation était masqué lors du défilement.

* Rapport d’utilisation sur le chargement automatique d’un projet individuel

  Lorsque vous consultez le rapport d’utilisation d’un projet, le rapport se charge automatiquement.

  Avant cette modification, il fallait cliquer sur « Exécuter » pour que le rapport s’exécute.

* Amélioration des performances

Pour plus d’informations sur le rapport d’utilisation, consultez la section [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Suppression de l’objet des heures budgétées pour les ressources de Workfront {#remove-the-resource-budgeted-hour-object-from-workfront}

Pour résoudre les problèmes de performances, le champ des heures budgétées pour les ressources a été temporairement supprimé de Workfront.

Pour rappel, les heures budgétées pour les ressources sont les heures que vous budgétisez pour vos ressources ou vos projets dans le planificateur de ressources. Pour l’instant, vous ne pouvez plus générer de rapports sur ce champ dans l’application web ni via l’API. Le champ sera rétabli dans une version ultérieure, une fois les problèmes de performances résolus.

Pour plus d’informations sur la budgétisation des heures dans le planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Statistiques d’utilisation des rapports {#report-usage-statistics}

Vous pouvez désormais afficher les informations d’utilisation suivantes pour vos rapports Workfront dans une liste de rapports :

* Affiché en dernier par
* Date du dernier affichage
* 10 derniers observateurs
* Vues le mois / le trimestre / l’année en cours
* Vues le mois / le trimestre / l’année en cours
* Toutes les vues

Avant cette mise à jour, les informations d’utilisation que vous pouviez afficher dans vos rapports étaient limitées.

Pour plus d’informations sur l’utilisation des rapports, voir [Afficher l’utilisation des rapports](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md).

## Plannings gérés par les administrateurs et administratrices de groupes {#schedules-managed-by-group-administrators}

En tant qu’administrateur ou administratrice de groupes, vous pouvez créer et modifier des plannings associés aux groupes que vous administrez, ainsi que leurs sous-groupes. Avant cette modification, seuls les administrateurs et administratrices Workfront pouvaient créer et modifier des plannings.

Pour plus d’informations sur la gestion des plannings, voir [Créer un planning](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Mises à jour du graphique de Gantt {#gantt-chart-updates}

Le graphique de Gantt est maintenant modifiable. Le graphique de Gantt vous permet d’effectuer les mises à jour suivantes sur vos tâches :

* Créer des relations d’antériorité
* Modifier la durée de la tâche
* Mettre à jour le pourcentage terminé de la tâche
* Appliquer le nivellement des ressources

Avant cette modification, vous pouviez uniquement supprimer les relations de tâche antérieure dans le graphique de Gantt et vous pouviez modifier les tâches uniquement dans la liste des tâches.

Pour plus d’informations sur le graphique de Gantt, voir [Mettre à jour des informations dans le graphique de Gantt de la liste des tâches](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Nouvel optimisateur de portfolio {#new-portfolio-optimizer}

La zone Optimisateur de portfolio de Workfront est désormais mise à jour avec un nouvel aspect. La fonctionnalité n’a pas été modifiée.

Pour plus d’informations sur l’optimisateur de portfolio, voir [Vue d’ensemble de l’optimisateur de portfolio](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Option d’ajustement de date du budget dans le planificateur de ressources {#budget-date-adjustment-option-in-the-resource-planner}

Nous avons ajouté une option permettant une visibilité rapide des périodes sans conflit de budget. Une fois que vous avez vu le moment où les périodes sans conflit de budget se produisent, vous pouvez déplacer manuellement vos Heures budgétées vers ces heures. Les dates budgétées des heures seront également ajustées. Avant cette mise à jour, il n’était pas possible d’afficher les conflits de budget pour un projet en un coup d’oeil.

Pour plus d’informations sur l’ajustement des dates budgétées dans le planificateur de ressources, voir la section « Ajuster les dates de budget » dans la section [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Planification des ressources : restreindre les affectations aux utilisateurs et utilisatrices en fonction de l’appartenance à un groupe {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Lors de la création d’affectations de personnes dans la zone Planification (comme décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification »), vous pouvez maintenant configurer Workfront pour limiter les affectations de tâches et de problèmes uniquement aux personnes qui sont membres du groupe défini sur le projet à l’origine de la tâche ou du problème. 

Cela concerne les cas où vous effectuez des affectations des manières suivantes :

* Lors de l’affectation d’une personne à toutes les tâches et problèmes pour un rôle spécifique, comme décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification ».

  Avant cette modification, il était toujours possible d’affecter une tâche ou un problème à n’importe quelle personne, indépendamment de son appartenance à un groupe. 

* Lors de la permutation d’affectations avec une autre personne, tel que décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification ».

  Avant cette modification, il était toujours possible d’affecter une tâche ou un problème à n’importe quelle personne, indépendamment de son appartenance à un groupe. 

* Lors de l’affectation manuelle d’une tâche ou d’un problème du journal de planification, tel que décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification ».

  Avant cette modification, il était toujours possible d’affecter une tâche ou un problème à n’importe quelle personne, indépendamment de son appartenance à un groupe. 

* Lorsque vous autorisez Workfront à affecter automatiquement des personnes, comme décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones de planification ».

  Avant cette modification, Workfront attribuait des tâches et des problèmes aux personnes, indépendamment de leur appartenance à un groupe.

Pour plus d’informations sur la configuration de cette option, voir la section « Commencer avec la planification des ressources ».

## Planification des ressources : autoriser les affectations aux personnes, indépendamment de leur rôle {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

Lors des affectations de personnes dans la zone Planification (tel que décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification »), vous pouvez désormais configurer Workfront pour que l’affectation de tâches et de problèmes à une personne soit possible, que cette personne ait ou non un rôle défini dans son profil, correspondant à l’affectation du rôle de la tâche ou du problème qui lui est affecté.

Cela concerne les cas où vous effectuez des affectations des manières suivantes :

* Lors de l’affectation d’une personne à toutes les tâches et tous les problèmes d’un rôle spécifique, tel que décrit dans « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification » dans « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification ».

  Avant cette modification, le rôle principal de la personne que vous affectiez devait correspondre au rôle déjà défini dans le champ Sélectionner un rôle.

* Lors de la permutation d’affectations avec une autre personne, tel que décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification ».

  Avant cette modification, le rôle principal de la personne que vous affectiez devait correspondre au rôle déjà défini dans le champ Sélectionner un rôle.

* Lors de l’affectation manuelle d’une tâche ou d’un problème du journal de planification, tel que décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification ».

  Avant cette modification, seules les personnes dont le rôle correspondait à celui de la tâche ou du problème que vous affectiez s’affichaient dans le journal de planification.

>[!NOTE]
>
>Cela ne concerne pas les cas où vous autorisez Workfront à affecter automatiquement des personnes, tel que décrit dans la section « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification ». Lors de l’affectation automatique de personnes, les tâches et les problèmes ne peuvent être affectés qu’aux personnes disposant d’un rôle correspondant.

Pour plus d’informations sur la configuration de cette option, voir la section « Commencer avec la planification des ressources ».

## Prise en charge d’émoticônes {#emoji-support}

Vous pouvez maintenant donner le ton des commentaires et des mises à jour que vous effectuez dans Workfront en insérant des émoticônes. Les émoticônes ajoutées aux commentaires de l’onglet Mises à jour s’affichent également dans la notification électronique de mise à jour. 

Pour plus d’informations, voir la section [Mettre à jour un travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
