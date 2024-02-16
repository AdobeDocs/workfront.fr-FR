---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version finale de la version 2017.3 bêta
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version finale de la version bêta 2017.3. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 12 septembre 2017. Il sera disponible dans l’environnement de production début novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3821'
ht-degree: 0%

---

# Activité Version finale de la version 2017.3 bêta

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version finale de la version bêta 2017.3. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 12 septembre 2017. Il sera disponible dans l’environnement de production début novembre 2017.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.3, voir  [Présentation de l’activité de la version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La version finale de la version bêta 2017.3 contient des améliorations pour les administrateurs de Workfront et d’autres utilisateurs :

**Pour les administrateurs**

* [Nouvelle configuration pour les requêtes d’appel dans la zone Paramètres d’approbation](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Configuration des rôles de BAT par défaut](#configure-default-proof-roles)

**Pour tous les utilisateurs**

* [Zone d’accueil (mise à jour de ma zone de travail)](#home-area-updated-my-work-area)

* [Mise à jour du modèle de mise en page pour prendre en charge la zone d’accueil](#updated-layout-template-to-support-the-home-area)

* [Kanban pour Agile](#kanban-for-agile)
* [Inclure des problèmes sur le journal de démarrage d’une équipe agile](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [Inclure des problèmes sur le panorama d’articles agiles sur Scrum](#include-issues-on-the-scrum-agile-story-board)
* [Application de groupes et de filtres au journal pour une équipe agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Amélioration des @Tagging Fonctionnalités de retour dans l’environnement de prévisualisation](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [Les mises à jour du système de filtrage dans le flux de mise à jour sont maintenant persistantes dans tous les objets](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Visualiser les données dans le rapport d’utilisation](#visualize-data-in-the-utilization-report)
* [Amélioration des performances des rapports d’utilisation](#utilization-report-performance-improvement)
* [Améliorations des documents : interface rationalisée](#document-enhancements-streamlined-interface)
* [Améliorations de la vérification dans Workfront](#proofing-enhancements-within-workfront)
* [Améliorations de la vérification dans Workfront Proof et Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [Formatage de texte enrichi pour les mises à jour et les emails](#rich-text-formatting-for-updates-and-emails)
* [Nouvelle reconception du diagramme de Gantt](#new-gantt-chart-redesign)
* [Les rapports natifs contiennent des descriptions mises à jour](#built-in-reports-contain-updated-descriptions)
* [Marque dans les rapports, listes et tableaux de bord exportés](#branding-in-exported-reports-lists-and-dashboards)
* [Améliorations apportées à la copie de tâches et au déplacement de tâches ou de problèmes](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [Nouveau groupement pour les rapports d’heure budgétés de ressources : Date d’affectation](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [Améliorations du planificateur de ressources](#resource-planner-improvements)
* [Améliorations des périphériques mobiles](#mobile-improvements)
* [Intégration de Workfront avec Slack](#workfront-integration-with-slack)
* [Améliorations d’Outlook 365](#outlook-365-improvements)
* [Modifications des API](#api-changes)

## Zone d’accueil (mise à jour de ma zone de travail) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Cette fonctionnalité ne sera pas publiée dans l’environnement de production avec la version 17.3 ; elle restera dans Aperçu avant début 2018.

La nouvelle zone d’accueil offre une autre vue améliorée des mêmes données actuellement disponibles dans la zone Mon travail. La zone Accueil offre les avantages suivants par rapport à la zone Mon travail :

* Interface plus simple et intuitive
* Amélioration des performances

Les fonctionnalités suivantes sont disponibles dans la zone Mon travail, mais ne sont pas encore mises en oeuvre dans la zone Accueil :

* Afficher votre calendrier personnel
* Mettre à jour les tâches et les problèmes liés au formatage de texte enrichi
* Approuver les bons à tirer
* Afficher la liste des tâches que vous avez soumises pour approbation
* Création d’un problème ad hoc sur un projet
* Afficher uniquement les autorisations qui vous ont été déléguées

Pour plus d’informations sur l’utilisation de la nouvelle zone d’accueil, voir [Utilisation de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Mise à jour du modèle de mise en page pour prendre en charge la zone d’accueil {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Cette fonctionnalité ne sera pas publiée dans l’environnement de production avec la version 17.3 ; elle restera dans Aperçu avant début 2018.

En tant qu’administrateur Workfront, vous pouvez déterminer si les utilisateurs de votre entreprise ont accès à la zone d’accueil en configurant le modèle de mise en page auquel ils sont affectés. Les utilisateurs qui n’ont pas de modèle de mise en page peuvent toujours accéder à la zone Accueil.

Pour plus d’informations, voir &quot;Personnalisation de l’accueil&quot; dans &quot;Création et gestion des modèles de mise en page&quot;.

## Kanban pour Agile  {#kanban-for-agile}

Les équipes agiles peuvent désormais utiliser une méthodologie Kanban dans Workfront, en plus de la méthodologie Scrum agile déjà prise en charge.

Les méthodologies agiles Scrum et Kanban de Workfront diffèrent comme suit :

**Avantages de l’utilisation de Kanban dans Workfront**

* Afficher le journal des logs sur le tableau de bord agile de Kanban.

  Pour plus d’informations, voir .

* Configurez les éléments sur le journal en attente pour qu’ils soient automatiquement ajoutés au tableau de bord agile de Kanban lorsque d’autres éléments sont déplacés vers un état correspondant à Terminé.

  Pour plus d’informations, voir [Configurer des articles à ajouter automatiquement à partir du journal](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in [Configurer Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configurez une limite de travail en cours (WIP) à afficher sur le tableau de bord agile de Kanban.

  Pour plus d’informations, voir [Configuration de la limite de travail en cours (WIP)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) in [Configurer Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Avantages de Scrum dans Workfront**

* Ajoutez un ensemble d’articles à une itération agile et créez un panorama pour cette itération.
* Incluez les problèmes sur le tableau de bord Scrum.
* Incluez des problèmes sur le journal des tâches d’une équipe agile.

  Pour plus d’informations, voir [Configurer l’application des dates lors de l’ajout d’éléments de travail à une itération](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Configuration de Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Les sous-tâches peuvent être affichées sur le tableau de bord de Scrum.
* Affichez un graphique de condensation pour voir la progression par rapport aux histoires lors de l’itération.

  Pour plus d’informations, voir [Présentation du graphique en décharge agile](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Pour plus d’informations sur l’activation et la configuration de Kanban pour une équipe agile, voir [Choix d’une méthodologie agile](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) in [Créer une équipe agile](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Inclure des problèmes sur le journal de démarrage d’une équipe agile {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de l’environnement de production le 14 novembre 2017. Il devrait être réintroduit dans l’environnement Aperçu début 2018 avec une conception améliorée et une stabilité accrue. Il sera disponible dans l’environnement de production avec la version 2018.1.

Vous pouvez désormais inclure des problèmes sur le journal de votre équipe agile lors de l’utilisation de la méthodologie Scrum agile (les problèmes ne s’affichent pas sur le journal de l’équipe agile lors de l’utilisation de la méthodologie Kanban). Les équipes agiles de Scrum existantes doivent activer cette fonctionnalité pour que les problèmes soient inclus. Les problèmes sont automatiquement inclus dans le journal des travaux des équipes dynamiques Scrum créées après la version 2017.3.

Avant cette modification, seules les tâches pouvaient être ajoutées au journal. Si vous vouliez ajouter un problème, vous deviez d’abord le convertir en une tâche avant de pouvoir l’ajouter.

Comme vous avez désormais accès à plus de tâches que les tâches du journal, toutes les tâches personnalisées disponibles précédemment dans le journal sont copiées et ajoutées au journal en tant que vues d’élément de travail du journal personnalisées.

Pour plus d’informations sur l’utilisation des problèmes sur le journal en souffrance, voir  [Gestion du journal en souffrance agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Pour plus d’informations sur l’activation des problèmes à mettre à disposition sur le journal d’une équipe Scrum agile, voir  [Configurer l’application des dates lors de l’ajout d’éléments de travail à une itération](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) in [Configuration de Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Inclure des problèmes sur le panorama d’articles agiles sur Scrum {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de l’environnement de production le 14 novembre 2017. Il devrait être réintroduit dans l’environnement Aperçu début 2018 avec une conception améliorée et une stabilité accrue. Il sera disponible dans l’environnement de production avec la version 2018.1.

Vous pouvez désormais inclure des problèmes sur le panorama lorsque vous utilisez la méthodologie agile de Scrum.

Pour plus d’informations, voir [Configuration des colonnes d’état sur le tableau de bord agile](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) in [Configuration de Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Application de groupes et de filtres au journal pour une équipe agile {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de l’environnement de production le 14 novembre 2017. Il devrait être réintroduit dans l’environnement Aperçu début 2018 avec une conception améliorée et une stabilité accrue. Il sera disponible dans l’environnement de production avec la version 2018.1.

Les options Groupement et Filtre sont désormais disponibles sur le journal en souffrance agile, ce qui vous permet d&#39;organiser votre journal en souffrance par groupes, ainsi que de filtrer les tâches et problèmes spécifiques.

Avant cette modification, vous pouviez appliquer les vues au journal agile.

Pour plus d’informations, voir  [Gestion du journal en souffrance agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) in  [Gestion du journal en souffrance agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Formatage de texte enrichi pour les mises à jour et les emails {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>Les modifications apportées à la mise en forme dans l’environnement Aperçu peuvent revenir à l’état non formaté.

Vous pouvez maintenant mettre l’accent sur les informations importantes en formatant les commentaires et les mises à jour que vous apportez aux objets Workfront. 

Les outils Texte enrichi vous permettent d’appliquer des attributs de mise en forme au texte, de créer des listes à puces et numérotées et d’ajouter des liens hypertexte à des ressources supplémentaires.

La mise en forme appliquée aux commentaires dans le flux de mise à jour s’affiche également dans les notifications par courrier électronique de mise à jour. Pour en savoir plus sur le formatage de vos commentaires, voir [Mise à jour du travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Amélioration des @Tagging Fonctionnalités de retour dans l’environnement de prévisualisation {#enhanced-tagging-functionality-returns-in-the-preview-environment}

Vous pouvez à nouveau utiliser le symbole @ pour baliser d’autres utilisateurs dans le flux de mise à jour de tous les objets de l’environnement Aperçu. Dans le passé, @tagging avait placé le prénom et le nom de l’utilisateur balisé dans le flux de mise à jour. Désormais, la fonctionnalité améliorée de @tagging affiche uniquement le prénom de l’utilisateur. Pour en savoir plus sur le balisage des utilisateurs dans les mises à jour, voir [Balisage des autres sur les mises à jour](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Les mises à jour du système de filtrage dans le flux de mise à jour sont maintenant persistantes dans tous les objets {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

L’option Filtrer les mises à jour du système est désormais persistante sur tous les objets du site Workfront. Vous pouvez ainsi masquer les mises à jour du système et afficher uniquement les commentaires des utilisateurs dans le flux de mise à jour sur un objet. Ce paramètre reste conservé lorsque vous accédez à d’autres objets.

Avant cette modification, vous deviez choisir de filtrer les mises à jour du système pour chaque objet lorsque vous parcourez le site Workfront.

Pour plus d’informations, voir [Mise à jour du travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Visualiser les données dans le rapport d’utilisation {#visualize-data-in-the-utilization-report}

 Vous pouvez désormais afficher les informations d’utilisation dans un graphique. 

Pour plus d’informations, voir [Présentation du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Présentation du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Amélioration des performances des rapports d’utilisation {#utilization-report-performance-improvement}

>[!NOTE]
>
>Cette fonctionnalité a été publiée dans un correctif après la version finale bêta.

Désormais, lors de l’exécution d’un rapport d’utilisation, vous êtes invité à appliquer un filtre avant l’exécution du rapport. Cette modification garantit que les informations les plus pertinentes sont générées dans le rapport Utilisation aussi rapidement que possible.

Pour plus d’informations sur l’exécution d’un rapport d’utilisation, voir [Présentation du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) in [Présentation du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Améliorations des documents : interface rationalisée {#document-enhancements-streamlined-interface}

L’expérience utilisateur de l’ajout de documents à Workfront est désormais plus simple et intuitive. Vous pouvez désormais charger un document à partir de votre système de fichiers, demander un document ou lier un fichier à partir d’une application tierce (telle que Google ou Dropbox), le tout à partir d’un simple menu déroulant. 

Auparavant, ces options étaient disponibles lors du lancement de la boîte de dialogue Ajouter des documents . 

Pour plus d’informations, voir les informations suivantes :

* [Ajout de documents à Adobe Workfront à partir de votre système de fichiers](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [Demande d’un document](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [Liaison de documents à partir d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>Avec cette modification, l’option de collage d’une image ou d’un document à partir du Presse-papiers n’est plus disponible.

## Améliorations de la vérification dans Workfront {#proofing-enhancements-within-workfront}

* [Expérience utilisateur améliorée et fonctionnalité supplémentaire](#improved-user-experience-and-additional-functionality)
* [Partager directement à partir de la visionneuse de vérification](#share-directly-from-the-proofing-viewer)
* [Configuration des rôles de BAT par défaut](#configure-default-proof-roles)

### Expérience utilisateur améliorée et fonctionnalité supplémentaire {#improved-user-experience-and-additional-functionality}

Outre une meilleure expérience utilisateur lors de la création de BAT dans Workfront, les fonctionnalités supplémentaires suivantes sont désormais disponibles :

* Fusionnez plusieurs images en un seul BAT.
* Les sites web de BAT de plusieurs résolutions (plusieurs résolutions peuvent être créées sous la forme de BAT individuels ou combinées en un seul BAT).
* Modifiez le nom du fichier pendant le processus de chargement.
* Incluez des champs personnalisés dans le formulaire de création de BAT.
* Ajoutez un message personnalisé pour les notifications électroniques de BAT.
* Paramètres de BAT supplémentaires 
* Validation des erreurs en temps réel lors de la vérification d’une URL (auparavant, vous deviez attendre plusieurs minutes avant qu’une erreur ne s’affiche)

Pour plus d’informations, voir .

>[!NOTE]
>
> Lors de la création d’un BAT avec un workflow automatisé, le glisser-déposer n’est pas pris en charge pour déplacer les utilisateurs d’une étape à une autre. Supprimez plutôt l’utilisateur d’une étape et ajoutez-le à une autre.

*L’option permettant de déplacer les utilisateurs d’une étape à l’autre à l’aide du glisser-déposer sera réintroduite avec la version 2018.1.*

### Partager directement à partir de la visionneuse de vérification {#share-directly-from-the-proofing-viewer}

Vous pouvez désormais partager des données avec des utilisateurs Workfront spécifiques directement à partir de la visionneuse de vérification.

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement pour les nouveaux BAT (BAT créés après la version 2017.3) et uniquement pour les instances Workfront intégrées à un compte Workfront BAT Premium.

Avant cette modification, vous ne pouviez partager qu’en créant un lien, puis en le partageant avec un utilisateur. 

Pour plus d’informations, voir [Partage d’un BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Partage d’un BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Configuration des rôles de BAT par défaut {#configure-default-proof-roles}

Vous pouvez désormais configurer les rôles de BAT par défaut dont disposent les nouveaux utilisateurs et les utilisateurs invités pour créer de nouveaux BAT dans le système Workfront. 

Il s’agit du rôle par défaut auquel les utilisateurs sont affectés sur un BAT lorsque le BAT est partagé avec eux. 

## Améliorations de la vérification dans Workfront Proof et Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Redémarrez et passez dans la visionneuse de vérification vidéo HTML5 (raccourcis clavier).](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [Mises à jour de la visionneuse HTML5](#html5-proofing-viewer-updates)

### Redémarrez et passez dans la visionneuse de vérification vidéo HTML5 (raccourcis clavier). {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Il existe désormais des raccourcis clavier dans la visionneuse de vérification de contenu HTML5 pour la vidéo qui vous permettent de redémarrer la vidéo du début à la fin de la vidéo.

Pour plus d’informations sur les raccourcis clavier disponibles, voir [Raccourcis clavier dans la visionneuse de vérification de performance Workfront](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### Mises à jour de la visionneuse HTML5 {#html5-proofing-viewer-updates}

La visionneuse HTML5 prend désormais en charge les bons à tirer statiques.

Avant cette modification, la visionneuse HTML5 ne prenait en charge que les bons à tirer pour la vidéo. 

La visionneuse de HTMLS comprend les nouvelles fonctionnalités suivantes lors de la vérification du contenu statique :

* Faire un seul commentaire avec des balises sur plusieurs pages en mode Une seule vue

  Auparavant, cela n’était possible que dans la vue continue ou Magazine.

* Parcourir les BAT à partir des miniatures de BAT

   * Identifiez facilement la partie du BAT qui est en cours de révision. Ceci est important, en particulier lorsque les utilisateurs utilisent des bons à tirer plus volumineux et de longues pages web, ou à tout moment le niveau de zoom le plus élevé est nécessaire pour afficher les détails.
   * Modification du niveau de zoom
   * Panoramique du contenu

* Spécification de valeurs personnalisées dans l’outil de mesure
* Lors de l’annotation de texte dans un BAT dans la visionneuse de vérification dans le BAT Workfront, vous pouvez inclure des options pour indiquer que le texte doit être en gras, en italique et souligné.

La visionneuse HTML5 ne prend pas encore en charge toutes les fonctionnalités actuellement disponibles dans la visionneuse de Flashs existante. Les fonctionnalités suivantes ne sont actuellement pas disponibles, mais seront incluses dans une version ultérieure :

* Prise en charge des fichiers multimédias riches
* Mode de comparaison (vidéo et statique)
* Filtrage des commentaires (vidéo et statiques)
* Vérifier les hyperliens dans les documents (statiques)
* Traductions (vidéo et statiques)
* Indicateur de présence qui affiche les utilisateurs qui travaillent actuellement sur le BAT
* Partage de bons à tirer

Pour plus d’informations sur la vérification des bons à tirer statiques dans la visionneuse HTML5, voir .

En tant qu’administrateur Workfront dans Workfront BAT, vous pouvez déterminer si les utilisateurs de votre entreprise ont accès à la nouvelle visionneuse de BAT pour HTML5 pour les BAT vidéo.

## Nouvelle reconception du diagramme de Gantt {#new-gantt-chart-redesign}

Le nouveau graphique Gantt comprend les améliorations suivantes :

* Nouvelles icônes et marqueurs
* Nouvelle option permettant d’effectuer un zoom avant ou arrière sur une période spécifique
* Cellules de tâche plus petites dans la partie liste du graphique
* Options repensées pour les paramètres, l’impression et le passage aux dates de projection.

Pour plus d’informations sur la configuration des options dans le diagramme de Gantt, voir [Configuration de l’affichage des informations sur le diagramme de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Les rapports natifs contiennent des descriptions mises à jour {#built-in-reports-contain-updated-descriptions}

Nous avons mis à jour les descriptions de nos rapports système dans Workfront afin d’inclure des informations sur le type de rapport et les champs inclus.  

Avant cette modification, la plupart de nos rapports intégrés n’avaient aucune description ou étaient très limités.

Pour plus d’informations sur les rapports natifs, voir [Utilisation des rapports intégrés d’Adobe Workfront](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Marque dans les rapports, listes et tableaux de bord exportés {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible sur toutes les grappes dans l’environnement Aperçu .

Si vous utilisez l’identité graphique dans Workfront, le logo que vous utilisez dans votre barre de navigation globale est désormais inclus dans les fichiers .pdf que vous exportez à partir de Workfront.

Les fichiers .pdf suivants incluront le logo de votre organisation dans le document exporté :

* Listes exportées
* Rapports exportés et distribués
* Tableaux de bord imprimés

Pour plus d’informations sur l’exportation de données à partir de Workfront, voir [Exporter des données](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Améliorations apportées à la copie de tâches et au déplacement de tâches ou de problèmes {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

Nous avons amélioré la façon dont vous copiez une tâche ou déplacez une tâche ou un problème, afin de faciliter la sélection d’un parent pour la tâche ou le problème copié ou déplacé. Lors de la sélection d’un parent lors de la copie d’une tâche, par exemple, vous pouvez désormais voir une hiérarchie de tâches, avec leur relation parent-enfant, ainsi que rechercher un parent dans les projets comportant de nombreuses tâches.

Avant cette modification, aucun champ Rechercher n’était présent dans la variable **Sélection d’un parent** et la hiérarchie des tâches n’était pas visible dans la liste des tâches.

Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur les problèmes de déplacement, voir [Problèmes de déplacement](../../../../manage-work/issues/manage-issues/move-issues.md).

## Nouvelle configuration pour les requêtes d’appel dans la zone Paramètres d’approbation {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Nous avons ajouté un nouveau paramètre à la zone Paramètres d’approbation au niveau du système pour permettre aux administrateurs de Workfront de décider s’ils doivent autoriser les utilisateurs à rappeler un problème ou une demande dont le premier état est en attente d’approbation. Si le rappel est autorisé, le problème est supprimé. Si le rappel n’est pas autorisé, les utilisateurs ne peuvent pas voir un bouton Rappel lorsque le premier état d’un problème est en attente d’approbation.

Avant cette modification, le rappel du problème était toujours autorisé. Lorsque la validation a été rappelée, la validation a été complètement ignorée, plaçant le problème dans son premier état, sans validation.

Pour plus d’informations sur les paramètres d’approbation, voir [Configuration des paramètres d’approbation globaux](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md). 

>[!NOTE]
>
>Cette option sera désactivée par défaut, lorsque cette fonctionnalité sera disponible. Actuellement, les problèmes de rappel sont activés par défaut pour toutes les organisations. Lorsque cette fonctionnalité est disponible, l’administrateur de Workfront doit activer manuellement ce paramètre pour conserver les fonctionnalités telles quelles dans Workfront.

## Nouveau groupement pour les rapports d’heure budgétés de ressources : Date d’affectation {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

Nous avons ajouté la possibilité de regrouper vos résultats par date d’attribution lors de la création d’un rapport Heure budgétaire de ressource.

Avant cette modification, vous pouviez afficher la Date d&#39;affectation dans la vue du rapport, et l&#39;utiliser dans un filtre, mais vous ne pouviez pas utiliser ce champ dans un regroupement.

Pour plus d’informations sur la date d’affectation, voir [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Améliorations du planificateur de ressources {#resource-planner-improvements}

* [planificateur de ressources : afficher les données par éditeur de texte enrichi](#resource-planner-show-data-by-fte)
* [Planification des ressources : afficher les données par semaine et par trimestre](#resource-planner-show-data-by-week-and-quarter)
* [planificateur de ressources : affichage par utilisateur](#resource-planner-view-by-user)
* [Planification des ressources : faites glisser et déposez les projets pour établir la priorité](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [Resource Planner : exportez les données du Resource Planner vers Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### planificateur de ressources : afficher les données par éditeur de texte enrichi {#resource-planner-show-data-by-fte}

Vous pouvez maintenant afficher l’allocation et la disponibilité de vos ressources par EPT dans le planificateur de ressources. Avant cette modification, vous ne pouviez afficher que les valeurs en heures.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planification des ressources : afficher les données par semaine et par trimestre {#resource-planner-show-data-by-week-and-quarter}

Vous pouvez désormais modifier l’intervalle de temps de votre planificateur de ressources afin de l’afficher par semaine ou par trimestre. Avant cette modification, vous ne pouviez afficher l’allocation et la disponibilité de vos ressources et les budgétiser que par mois.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### planificateur de ressources : affichage par utilisateur {#resource-planner-view-by-user}

Vous pouvez désormais afficher les informations dans le planificateur de ressources par utilisateur, d’abord, puis par projets, rôles et tâches. Vous pouvez également afficher une différence entre les heures prévues et les heures disponibles ou l’éditeur de texte enrichi pour les utilisateurs. Avant cette modification, vous pouvez afficher les informations dans le planificateur de ressources par projets et rôles.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planification des ressources : faites glisser et déposez les projets pour établir la priorité {#resource-planner-drag-and-drop-projects-to-establish-priority}

Vous pouvez désormais faire glisser et déposer des projets dans l’ordre de priorité souhaité. Avant cette modification, vous ne pouviez définir la priorité des projets qu’en leur attribuant manuellement un nombre.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Resource Planner : exportez les données du Resource Planner vers Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

Vous pouvez désormais exporter les informations du planificateur de ressources vers un fichier Excel.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Présentation de Resource Planner](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Améliorations des périphériques mobiles {#mobile-improvements}

Nous avons ajouté la possibilité d’accéder à vos projets et de les gérer à partir de l’application mobile Workfront. Vous pouvez désormais effectuer les opérations suivantes à l’aide de l’application mobile Workfront :

* Accès à la liste de vos projets
* Accéder à une liste de tâches et de sous-tâches sur un projet
* Accès à une liste de problèmes sur un projet
* Enregistrer un nouveau problème sur un projet

Vous pouvez installer cette fonctionnalité lorsque vous mettez à jour votre application mobile Workfront. La mise à jour sera disponible dans les boutiques Apple et Android en novembre 2017.

## Intégration de Workfront avec Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>L’intégration de Slack n’est actuellement pas disponible. Il sera disponible pour utilisation avec votre environnement de production en novembre 2017.

Nous lançons une nouvelle intégration entre Workfront et Slack. Si votre entreprise a déjà utilisé Slack pour votre communication, vous pouvez désormais l’intégrer à Workfront et effectuer des actions Workfront courantes sans quitter vos canaux de communication dans Slack. Vous pouvez désormais effectuer les actions suivantes à partir de votre compte de Slack :

* Recherche d’un élément dans Workfront
* Accéder à vos listes de tâches et de validations
* Création d’une tâche
* Créer un événement
* Abonnez-vous à tout élément à partir d’un lien partagé avec vous vers cet élément.
* Affectez à des tâches et des problèmes à partir d’un lien partagé avec vous.
* Approuver votre travail
* Accédez à vos Favoris et à vos listes d’éléments récents

Pour plus d’informations sur l’accès à Workfront à partir de Slack, voir [Utilisation de Workfront avec Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Améliorations d’Outlook 365 {#outlook-365-improvements}

Nous avons apporté les améliorations suivantes au module complémentaire Workfront pour Outlook 365 :

* Ajouter une tâche ou un problème à un projet dans Workfront : vous pouvez désormais convertir un email en tâche ou en problème dans Workfront, à l’aide du module complémentaire Outlook 365. Au cours de ce processus, vous pouvez spécifier un projet auquel vous souhaitez ajouter la tâche ou le problème, ainsi qu’une personne désignée et une date d’échéance. Avant cette amélioration, vous ne pouviez envoyer qu’une requête à une file d’attente de requêtes ou ajouter une tâche personnelle à votre liste Travailler sur à partir d’Outlook 365. 
* Conserver un lien vers les objets Workfront dans l’email d’origine converti en tâches, problèmes ou requêtes : lorsque vous convertissez un email d’Outlook 365 en tâche, problème ou requête, Outlook 365 conserve un lien vers la tâche ou le problème converti à partir de cet email dans l’email d’origine. Avant cette modification, Outlook n’indiquait pas si un courrier électronique avait été converti en tâche ou envoyé en tant que requête. 

  Pour plus d’informations sur la conversion d’un email en une tâche ou d’un problème à partir d’Outlook 365, voir [Ajout d’un courrier électronique Outlook à un projet en tant que tâche ou problème](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

## Modifications des API {#api-changes}

* [API 8 désormais disponible](#api-8-now-available)
* [Versions supprimées et obsolètes de l’API](#removed-and-deprecated-versions-of-the-api)
* [Activité Version finale de la version 2017.3 bêta](#updated-message-format-for-event-subscriptions)
* [Reprises d’abonnement à un événement pour les messages en échec](#event-subscription-retries-for-undeliverable-messages)

### API 8 désormais disponible {#api-8-now-available}

L’API Workfront version 8 est désormais disponible et vous offre des ressources nouvelles et mises à jour pour vos intégrations Workfront.

Pour obtenir la liste des modifications apportées à l’API Workfront, voir [Mises à jour de l’API version 8](../../../../wf-api/api/new-api-version-8-updates.md).

### Versions supprimées et obsolètes de l’API {#removed-and-deprecated-versions-of-the-api}

### Mise à jour du format de message pour les abonnements à un événement

Afin de fournir des informations plus utiles pour vos intégrations qui incluent l’API d’abonnements aux événements Workfront, nous avons modifié le format du message sortant pour les ressources prises en charge en incluant les anciennes et nouvelles valeurs associées à ces ressources. Pour éviter tout échec, toutes les intégrations que vous avez à l’aide de l’API des abonnements aux événements de Workfront doivent être mises à jour dans le nouveau format, comme décrit dans la section [API d’abonnement à un événement](../../../../wf-api/general/event-subs-api.md).

### Reprises d’abonnement à un événement pour les messages en échec {#event-subscription-retries-for-undeliverable-messages}

La structure d’abonnement aux événements Workfront fournit désormais un mécanisme de gestion des messages sortants déclenchés par un événement qui ne parviennent pas à diffuser vers les points de terminaison clients. Afin d’assurer une diffusion continue des messages, les clients doivent s’assurer que tous les points de terminaison utilisant des messages sortants des abonnements à des événements sont correctement configurés. Pour plus d’informations, voir [Reprises d’abonnement à un événement](../../../../wf-api/api/event-sub-retries.md).
