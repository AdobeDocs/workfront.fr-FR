---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.1, version bêta 4
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.1 de Beta 4. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 24 janvier 2018. Il sera disponible dans l’environnement de production en mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 1%

---

# Activité Version 2018.1, version bêta 4

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.1 de Beta 4. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 24 janvier 2018. Il sera disponible dans l’environnement de production en mars 2018.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.1, voir  [Présentation de l’activité de version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version 2018.1 de Beta 4 contient des améliorations pour les administrateurs de Workfront et d’autres utilisateurs :

**Pour les administrateurs**

* [Planifications gérées par les administrateurs de groupe](#schedules-managed-by-group-administrators)

**Pour Tous Les Utilisateurs**

* [ Améliorations de la vérification dans Workfront](#proofing-improvements-within-workfront)
* [Création de BAT dans Workfront Proof - Expérience utilisateur améliorée et fonctionnalité supplémentaire](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [ Améliorations de la vérification dans Workfront et Workfront Proof](#proofing-improvements-within-workfront-and-workfront-proof)
* [Mise à jour de l’intégration Look and Feed avec Basecamp dans Workfront Proof](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [Coller des images vers Workfront à partir du Presse-papiers](#paste-images-to-workfront-from-the-clipboard)
* [Améliorations du rapport d’utilisation](#utilization-report-improvements)
* [Supprimer l’objet Resource Budget Hour de Workfront](#remove-the-resource-budgeted-hour-object-from-workfront)
* [Statistiques d’utilisation des rapports](#report-usage-statistics)
* [Mises à jour du graphique Gantt](#gantt-chart-updates)
* [New Portfolio Optimizer](#new-portfolio-optimizer)
* [Option d’ajustement de date de budget dans le planificateur de ressources](#budget-date-adjustment-option-in-the-resource-planner)
* [Planification des ressources : restreindre les affectations aux utilisateurs en fonction de l’appartenance à un groupe](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [Planification des ressources : autoriser les affectations aux utilisateurs, quel que soit leur rôle](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Prise en charge d’Emoji](#emoji-support)

## Améliorations de la vérification dans Workfront {#proofing-improvements-within-workfront}

Les améliorations suivantes ont été apportées à la liste de documents dans Workfront : 

* [Afficher la progression du BAT à partir de la liste de documents](#view-proof-progress-from-the-document-list)
* [Nouvelle option pour afficher le résumé d’impression à partir de la liste de documents](#new-option-to-view-the-print-summary-from-the-document-list)
* [ Représentation mise à jour de la génération ou de l’ouverture du BAT à partir de la liste de documents ](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [Divers liens supprimés des documents dans la liste de documents](#various-links-removed-from-documents-on-the-document-list)
* [Afficher les noms de fichier sur les bons à tirer combinés](#view-file-names-on-combined-proofs)
* [Affichage de l’étape active actuelle d’un bon à tirer à partir de la liste de documents](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### Affichage de la progression du BAT à partir de la liste des documents {#view-proof-progress-from-the-document-list}

Les indicateurs de progression du BAT s’affichent désormais pour tous les BAT lors de l’affichage de la liste de documents. (Cela inclut les envois, les ouvertures, les commentaires effectués et la décision.)

Avant cette modification, vous deviez sélectionner un BAT dans la liste des documents pour afficher la progression du BAT dans le panneau de droite. 

Pour plus d’informations, voir [Proof progress and status overview](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

### Nouvelle option pour afficher le résumé d’impression à partir de la liste des documents {#new-option-to-view-the-print-summary-from-the-document-list}

Vous pouvez désormais afficher la synthèse d’impression d’un BAT directement à partir de la liste des documents.

Avant cette modification, vous ne pouviez afficher le résumé imprimé qu’à partir de la visionneuse de vérification. 

Pour plus d’informations sur l’affichage de la synthèse d’impression à partir de la liste de documents, voir [Imprimer une synthèse de BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Mise à jour de l’aspect pour la génération ou l’ouverture du BAT à partir de la liste de documents {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

Désormais, lorsque vous placez le pointeur de la souris sur un document dans la liste des documents, les options de génération du BAT ou d’ouverture du BAT ont été mises à jour. Ces options apparaissent désormais sous la forme de boutons.

Avant cette modification, ces options étaient disponibles sous forme de liens sous le nom du document.

Pour plus d’informations, voir les sections suivantes :

* .
* dans .

### Divers liens supprimés des documents de la liste de documents {#various-links-removed-from-documents-on-the-document-list}

Les actions suivantes ne sont plus disponibles en tant que liens sur des documents individuels dans la liste de documents :

* Créer une épreuve
* Épreuve
* Détails
* Partager
* Extraction/archivage

Les actions suivantes sont désormais disponibles sous forme de bouton dans le document au sein de la liste de documents :

* BAT ouvert (disponible après la génération du BAT) 
* Générer un bon à tirer (disponible lorsque le BAT n’est pas encore généré)

Les actions suivantes sont désormais disponibles dans le menu déroulant en regard du bouton Ouvrir le bon à tirer ou Générer le bon à tirer :

* Détails de l&#39;épreuve
* Détails du document
* Imprimer le résumé

Pour plus d’informations, voir les sections suivantes :

* .
* dans .

### Affichage des noms de fichier sur les bons à tirer combinés {#view-file-names-on-combined-proofs}

Vous pouvez désormais afficher les noms de fichiers individuels qui constituent un BAT combiné. Ces informations s&#39;affichent dans l&#39;onglet Détails lorsque le BAT est sélectionné dans la liste des documents.

Pour plus d’informations, voir Affichage de tous les fichiers contenus dans un BAT combiné. 

### Affichage de l’étape active actuelle d’un bon à tirer à partir de la liste de documents {#view-the-current-active-stage-of-a-proof-from-the-document-list}

Désormais, lorsque vous sélectionnez un BAT dans la liste des documents, les étapes actives actuelles s’affichent dans la colonne de droite de l’onglet Détails. 

Pour plus d’informations, voir [Affichage des étapes actives sur un BAT](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md).  

## Création de BAT dans Workfront Proof - Expérience utilisateur améliorée et fonctionnalité supplémentaire {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

Outre une meilleure expérience utilisateur lors de la création de BAT dans Workfront Proof, les fonctionnalités supplémentaires suivantes sont désormais disponibles :

* Fusionnez plusieurs images en un seul BAT.
* Les sites web de BAT de plusieurs résolutions (plusieurs résolutions peuvent être créées sous la forme de BAT individuels ou combinées en un seul BAT).
* Modifiez le nom du fichier pendant le processus de chargement.
* Incluez des champs personnalisés dans le formulaire de création de BAT.
* Ajoutez un message personnalisé pour les notifications électroniques de BAT.
* Paramètres de BAT supplémentaires 
* Validation des erreurs en temps réel lors de la vérification d’une URL (auparavant, vous deviez attendre plusieurs minutes avant qu’une erreur ne s’affiche)

>[!NOTE]
>
>Cette nouvelle page de création de BAT dans Workfront Proof correspond désormais à la page de création de BAT récemment mise à disposition lors de la création de BAT dans Workfront. 

Pour plus d’informations, voir  [Générer des bons à tirer dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Améliorations de la vérification dans Workfront et Workfront Proof {#proofing-improvements-within-workfront-and-workfront-proof}

Les modifications suivantes s’appliquent lors de l’ajout de documents à Workfront et à Workfront Proof :

* [Redimensionner la liste des commentaires lors de la révision des bons à tirer](#resize-the-comment-list-when-reviewing-proofs)
* [Les Hyperliens Sont Actifs Lors De La Vérification De Bons À Tirer Statiques](#hyperlinks-are-active-when-reviewing-static-proofs)
* [Améliorations de l’ajout de bons à tirer](#improvements-when-adding-proofs)

### Redimensionner la liste des commentaires lors de la révision des bons à tirer {#resize-the-comment-list-when-reviewing-proofs}

Vous pouvez désormais redimensionner la liste de commentaires lors de la révision de BAT dans la visionneuse de BAT.

Pour plus d’informations, voir .

### Les Hyperliens Sont Actifs Lors De La Révision De Bons À Tirer Statiques {#hyperlinks-are-active-when-reviewing-static-proofs}

Les hyperliens sont désormais actifs lors de la révision d’un BAT statique dans la visionneuse de vérification. Cliquez sur un lien hypertexte pour accéder à la page liée.

Cette fonctionnalité est prise en charge dans tous les types de fichiers qui contiennent du texte, tels que PDF, DOC, etc. Les fichiers image ne sont pas pris en charge.

### Améliorations de l’ajout de bons à tirer {#improvements-when-adding-proofs}

Les améliorations suivantes sont disponibles lors de l’ajout de documents à vérifier. 

* Les informations contenues dans la liste des destinataires sont désormais disponibles dans une vue à 3 colonnes, ce qui facilite l&#39;affichage et la modification des informations. 

  Auparavant, les informations s’affichaient dans une seule colonne, ce qui nécessitait plus de clics lorsque des modifications étaient requises. 

  Pour plus d’informations, voir .

* Faites glisser un ou plusieurs destinataires d’une étape de workflow vers une autre lors de l’utilisation du workflow automatisé. Vous pouvez faire glisser directement sur une scène ou sur une scène du diagramme, situé en haut de la page.

  Pour plus d’informations, voir .

* Le diagramme de workflow reste visible en haut de la page, même lors du défilement. Par défaut, le diagramme est réduit ; développez-le pour afficher le diagramme complet.

  Pour plus d’informations, voir .

* Lors de l’ajout d’un modèle à un workflow automatisé dans un BAT, une animation de chargement s’affiche, indiquant que le modèle est en cours de chargement.

  Pour plus d’informations, voir .

* Les paramètres suivants ont été déplacés de la section Paramètres du BAT vers la section Processus de la page Nouveau BAT :

   * Principal Decision Maker
   * Exiger une seule décision

## Mise à jour de l’aspect et du ressenti avec l’intégration Basecamp dans Workfront Proof {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

L’aspect de l’intégration de Basecamp à Workfront Proof est désormais mis à jour. La fonctionnalité reste la même.

## Coller des images dans Workfront à partir du Presse-papiers {#paste-images-to-workfront-from-the-clipboard}

Vous pouvez désormais ajouter des fichiers image à Workfront en collant une image à partir du Presse-papiers du système.

La possibilité de coller du presse-papiers a été supprimée de Workfront dans une version précédente ; elle est réintroduite avec cette version. La nouvelle méthode est plus simple et intuitive.

Pour plus d’informations, voir [Coller des images à partir du Presse-papiers](../../../../documents/managing-documents/paste-image-clipboard.md). 

## Améliorations des rapports d’utilisation {#utilization-report-improvements}

Le rapport Utilisation contient les améliorations suivantes :

* Afficher les recettes dans le rapport Utilisation d’un projet

  Permet d’afficher les recettes budgétaires, les recettes prévues, les recettes réelles, l’écart budgétaire et l’écart planifié.

* Comparaison des recettes et des coûts prévus et réels

  Permet d&#39;afficher le Coût planifié ou réel à côté du Revenu planifié. La marge (%) est également affichée (la marge est calculée en tant que Recettes - Coût / Recettes).

* Les recettes s’affichent lors de l’affichage du graphique.
* Les en-têtes restent visibles lors du défilement.

  Désormais, lorsque vous parcourez les informations du rapport Utilisation , l’en-tête situé en haut du rapport Utilisation est toujours visible, ce qui vous permet de comprendre plus facilement les données du rapport.

  Auparavant, l’en-tête situé en haut du rapport Utilisation ne s’affichait pas lors du défilement.

* Rapport d’utilisation sur le chargement automatique d’un projet individuel

  Lors de l’affichage du rapport Utilisation sur un projet, le rapport se charge automatiquement.

  Avant cette modification, vous deviez cliquer sur &quot;Exécuter&quot; avant l’exécution du rapport.

* Amélioration des performances

Pour plus d’informations sur le rapport Utilisation, voir [Présentation du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Suppression de l’objet Resource Budget Hour de Workfront {#remove-the-resource-budgeted-hour-object-from-workfront}

Pour résoudre les problèmes de performances, le champ Resource Budget Hour a été temporairement supprimé de Workfront.

Pour rappel, les heures budgétées de la ressource sont les heures que vous estimez prévues pour vos ressources ou vos projets dans le planificateur de ressources. Pour l’instant, vous ne pouvez plus générer de rapports sur ce champ dans l’application web ni via l’API. Le champ sera rétabli dans une version ultérieure, une fois les problèmes de performances résolus.

Pour plus d’informations sur la planification des heures dans le planificateur de ressources, consultez la [présentation du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Statistiques d’utilisation des rapports {#report-usage-statistics}

Vous pouvez désormais afficher les informations d’utilisation suivantes pour vos rapports Workfront dans une liste de rapports :

* Affiché en dernier par
* Date de dernière vue
* 10 derniers observateurs
* Affichages ce mois/trimestre/année
* Affichages le mois/trimestre/année dernier
* Toutes les vues

Avant cette mise à jour, les informations d’utilisation que vous pouviez afficher dans vos rapports étaient limitées.

Pour plus d’informations sur l’utilisation des rapports, voir [Affichage de l’utilisation des rapports](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)

## Planifications gérées par les administrateurs de groupe {#schedules-managed-by-group-administrators}

En tant qu’administrateur de groupe, vous pouvez créer et modifier des plannings associés aux groupes que vous administrez, ainsi que leurs sous-groupes. Avant cette modification, seuls les administrateurs Workfront pouvaient créer et modifier des plannings.

Pour plus d’informations sur la gestion des plannings, voir [Créer un planning](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

## Mises à jour du graphique Gantt {#gantt-chart-updates}

Le diagramme de Gantt est maintenant modifiable. Le diagramme de Gantt vous permet d’effectuer les mises à jour suivantes sur vos tâches :

* Créer des relations de prédécesseur
* Modifier la durée de la tâche
* Mettre à jour le pourcentage de la tâche terminé
* Appliquer le niveau de ressource

Avant cette modification, vous pouviez uniquement supprimer les relations de prédécesseur dans le diagramme de Gantt et vous pouviez modifier les tâches uniquement dans la liste des tâches.

Pour plus d’informations sur le graphique Gantt, voir [Mise à jour d’informations dans la liste des tâches Graphique Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)

## Nouvel Portfolio Optimizer {#new-portfolio-optimizer}

La zone Portfolio Optimizer de Workfront est désormais mise à jour avec un nouvel aspect. La fonctionnalité n’a pas été modifiée.

Pour plus d’informations sur Portfolio Optimizer, consultez la [présentation de Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## Option d’ajustement de date du budget dans le planificateur de ressources {#budget-date-adjustment-option-in-the-resource-planner}

Nous avons ajouté une option permettant une visibilité rapide des délais sans conflit de budget. Une fois que vous avez vu le moment où les périodes sans conflit de budget se produisent, vous pouvez déplacer manuellement vos Heures budgétées vers ces heures. Les dates budgétisées des heures seront également ajustées. Avant cette mise à jour, il n’était pas possible d’afficher les conflits de budget pour un projet en un coup d’oeil.

Pour plus d’informations sur l’ajustement des dates budgétées dans le planificateur de ressources, consultez la section &quot;Ajustement des dates de budget&quot; dans la [présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)

## Planification des ressources : restreindre les affectations aux utilisateurs en fonction de l’appartenance à un groupe {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Lors de l’attribution d’affectations d’utilisateurs dans la zone Planification (comme décrit dans la section &quot;Affecter manuellement des tâches et des problèmes non attribués dans les zones Planification&quot;), vous pouvez maintenant configurer Workfront pour limiter les affectations de tâches et de problèmes uniquement aux utilisateurs qui sont membres du groupe défini sur le projet à l’origine de la tâche ou du problème. 

Cela s’applique lorsque vous effectuez des affectations de la manière suivante :

* Lors de l’affectation d’un utilisateur à toutes les tâches et problèmes pour un rôle spécifique, comme décrit dans la section &quot;Affecter manuellement des tâches et des problèmes non attribués dans les zones de planification&quot;.

  Avant cette modification, une tâche ou un problème pouvait toujours être affecté à n’importe quel utilisateur, quel que soit son appartenance à un groupe. 

* Lors de la permutation d’affectations avec un autre utilisateur, comme décrit dans la section &quot;Affecter manuellement des tâches non affectées et des problèmes dans les zones Planification&quot;.

  Avant cette modification, une tâche ou un problème pouvait toujours être affecté à n’importe quel utilisateur, quel que soit son appartenance à un groupe. 

* Lors de l’affectation manuelle d’une tâche ou d’un problème dans la chronologie de planification, comme décrit dans la section &quot;Affecter manuellement des tâches non affectées et des problèmes dans les zones de planification&quot;.

  Avant cette modification, une tâche ou un problème pouvait toujours être affecté à n’importe quel utilisateur, quel que soit son appartenance à un groupe. 

* Lorsque vous autorisez Workfront à affecter automatiquement des utilisateurs, comme décrit dans la section &quot;Affectation manuelle de tâches non affectées et de problèmes dans les zones Planification&quot;.

  Avant cette modification, Workfront attribuait des tâches et des problèmes aux utilisateurs, quel que soit leur appartenance à un groupe.

Pour plus d’informations sur la configuration de cette option, voir &quot;Prise en main de la planification des ressources&quot;.

## Planification des ressources : autorisation des affectations aux utilisateurs, quel que soit leur rôle {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

Lors de l’attribution d’affectations d’utilisateurs dans la zone Planification (comme décrit dans la section &quot;Affecter manuellement des tâches et des problèmes non attribués dans les zones Planification&quot;), vous pouvez maintenant configurer Workfront pour autoriser l’affectation de tâches et de problèmes à un utilisateur, que ce dernier ait ou non un rôle défini dans son profil utilisateur correspondant à l’affectation du rôle de la tâche ou au problème qui lui est assigné.

Cela s’applique lorsque vous effectuez des affectations de la manière suivante :

* Lors de l’affectation d’un utilisateur à toutes les tâches et problèmes pour un rôle spécifique, comme décrit dans &quot;Affecter manuellement des tâches et des problèmes non attribués dans les zones Planification&quot; dans &quot;Affecter manuellement des tâches et des problèmes non attribués dans les zones Planification&quot;.

  Avant cette modification, le rôle principal de l’utilisateur que vous affectez devait correspondre au rôle déjà défini dans le champ Sélectionner un rôle .

* Lors de la permutation d’affectations avec un autre utilisateur, comme décrit dans la section &quot;Affecter manuellement des tâches non affectées et des problèmes dans les zones Planification&quot;.

  Avant cette modification, le rôle principal de l’utilisateur que vous affectez devait correspondre au rôle déjà défini dans le champ Sélectionner un rôle .

* Lors de l’affectation manuelle d’une tâche ou d’un problème dans la chronologie de planification, comme décrit dans la section &quot;Affecter manuellement des tâches non affectées et des problèmes dans les zones de planification&quot;.

  Avant cette modification, seuls les utilisateurs dont le rôle correspondait au rôle de la tâche ou du problème que vous assignez s’affichaient dans la chronologie de planification.

>[!NOTE]
>
>Cela ne s’applique pas lorsque vous autorisez Workfront à affecter automatiquement des utilisateurs, comme décrit dans la section &quot;Affecter manuellement des tâches non affectées et des problèmes dans les zones de planification&quot;. Lors de l’affectation automatique d’utilisateurs, les tâches et les problèmes ne peuvent être affectés qu’aux utilisateurs disposant d’un rôle correspondant.

Pour plus d’informations sur la configuration de cette option, voir &quot;Prise en main de la planification des ressources&quot;.

## Prise en charge d’Emoji {#emoji-support}

Vous pouvez maintenant donner le ton aux commentaires et aux mises à jour que vous effectuez dans Workfront en insérant des émoticônes. Les émoticônes ajoutées aux commentaires sur l’onglet Mises à jour s’affichent également dans la notification électronique de mise à jour. 

Pour plus d’informations, voir [Mise à jour du travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
