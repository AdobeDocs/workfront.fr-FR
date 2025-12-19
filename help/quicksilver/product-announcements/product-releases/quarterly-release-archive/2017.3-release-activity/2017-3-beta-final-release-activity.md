---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de la version Beta finale 2017.3
description: Cette page décrit toutes les modifications récentes disponibles dans l’environnement de prévisualisation avec la version Beta finale 2017.3. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement de prévisualisation le 12 septembre 2017. Elles ont été rendues disponibles dans l’environnement de production début novembre 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '3791'
ht-degree: 91%

---

# Activité de la version Beta finale 2017.3

Cette page décrit toutes les modifications récentes disponibles dans l’environnement de prévisualisation avec la version Beta finale 2017.3. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement de prévisualisation le 12 septembre 2017. Elle ont été rendues disponibles dans l’environnement de production début novembre 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2017.3, voir [Vue d’ensemble de l’activité Version 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La version Beta finale 2017.3 contient des améliorations pour les administrateurs et administratrices de Workfront et d’autres personnes :

**Pour les administrateurs et administratrices**

* [Nouvelle configuration pour les demandes d’appel dans la zone Paramètres d’approbation](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [Configurer des rôles d’épreuve par défaut](#configure-default-proof-roles)

**Pour tous les utilisateurs et utilisatrices**

* [Zone Accueil (mise à jour de la zone Mon travail)](#home-area-updated-my-work-area)

* [Mise à jour du modèle de mise en page pour prendre en charge la zone Accueil](#updated-layout-template-to-support-the-home-area)

* [Kanban pour Agile](#kanban-for-agile)
* [Inclure des problèmes dans la liste d’attente Scrum d’une équipe Agile](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [Inclure des problèmes dans le storyboard Scrum Agile](#include-issues-on-the-scrum-agile-story-board)
* [Appliquer des regroupements et des filtres à la liste d’attente d’une équipe Agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Amélioration des retours de la fonctionnalité @Tagging dans l’environnement de prévisualisation](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [L’option Filtrer les mises à jour du système dans le flux de mise à jour est désormais persistante d’un objet à l’autre.](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Visualiser les données dans le rapport d’utilisation](#visualize-data-in-the-utilization-report)
* [Amélioration des performances des rapports d’utilisation](#utilization-report-performance-improvement)
* [Améliorations des documents : interface rationalisée](#document-enhancements-streamlined-interface)
* [Améliorations de la relecture dans Workfront](#proofing-enhancements-within-workfront)
* [Améliorations de la relecture dans Workfront Proof et Workfront](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [Formatage de texte enrichi pour les mises à jour et les e-mails](#rich-text-formatting-for-updates-and-emails)
* [Nouvelle conception du graphique de Gantt](#new-gantt-chart-redesign)
* [Les rapports intégrés contiennent des descriptions mises à jour.](#built-in-reports-contain-updated-descriptions)
* [Branding dans les rapports, listes et tableaux de bord exportés](#branding-in-exported-reports-lists-and-dashboards)
* [Améliorations apportées à la copie de tâches et au déplacement de tâches ou de problèmes](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [Nouveau regroupement pour les rapports sur les heures budgétées des ressources : date d’attribution](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [Améliorations du planificateur de ressources](#resource-planner-improvements)
* [Améliorations pour les appareils mobiles](#mobile-improvements)
* [Intégration de Workfront avec Slack](#workfront-integration-with-slack)
* [Améliorations apportées à Outlook 365](#outlook-365-improvements)
* [Modifications des API](#api-changes)

## Zone Accueil (mise à jour de la zone Mon travail) {#home-area-updated-my-work-area}

>[!NOTE]
>
>Cette fonctionnalité ne sera pas publiée dans l’environnement de production avec la version 17.3 ; elle restera en prévisualisation jusqu’au début de l’année 2018.

La nouvelle zone Accueil offre une autre vue améliorée des mêmes données actuellement disponibles dans la zone Mon travail. La zone Accueil offre les avantages suivants par rapport à la zone Mon travail :

* Interface plus simple et intuitive
* Amélioration des performances

Les fonctionnalités suivantes sont disponibles dans la zone Mon travail, mais ne sont pas encore mises en œuvre dans la zone Accueil :

* Afficher votre calendrier personnel
* Mettre à jour les tâches et les problèmes liés au formatage de texte enrichi
* Approuver les épreuves
* Afficher la liste des tâches que vous avez soumises pour approbation
* Créer un problème ad hoc sur un projet
* Afficher uniquement les approbations qui vous ont été déléguées.

Pour plus d’informations sur l’utilisation de la nouvelle zone Accueil, consultez [Utiliser la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Modèle de mise en page mis à jour pour prendre en charge la zone d’accueil {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>Cette fonctionnalité ne sera pas publiée dans l’environnement de production avec la version 17.3 ; elle restera en prévisualisation jusqu’au début de l’année 2018.

En tant qu’administrateur ou administratrice Workfront, vous pouvez déterminer si les utilisateurs et utilisatrices de votre entreprise ont accès à la zone d’accueil en configurant le modèle de mise en page auquel ils sont affectés. Les utilisateurs et utilisatrices auxquels aucun modèle de mise en page n’a été affecté peuvent toujours accéder à la zone d’accueil.

Pour plus d’informations, consultez « Personnaliser l’accueil » dans « Créer et gérer des modèles de mise en page ».

## Kanban pour Agile {#kanban-for-agile}

Les équipes Agile peuvent désormais utiliser une méthodologie Kanban dans Workfront, en plus de la méthodologie Scrum Agile déjà prise en charge.

Les méthodologies Scrum et Kanban Agile dans Workfront diffèrent des manières suivantes :

**Avantages de l’utilisation de Kanban dans Workfront**

* Affichez la liste d’attente sur le storyboard Kanban Agile.

  Pour plus d’informations, voir :

* Configurez les éléments de la liste d’attente pour qu’ils soient automatiquement ajoutés au storyboard agile kanban lorsque d’autres éléments sont déplacés vers un statut équivalent à Terminé.

  Pour plus d’informations, consultez [Configurer des histoires à ajouter automatiquement à partir de la liste d’attente](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) dans [Configurer Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configurez une limite de travail en cours (WIP) à afficher sur le storyboard Kanban Agile.

  Pour plus d’informations, consultez [Configurer la limite de travail en cours](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) dans [Configurer Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

**Avantages de Scrum dans Workfront**

* Ajoutez un ensemble d’histoires à une itération Agile et créez un storyboard pour cette itération.
* Incluez des problèmes sur le storyboard Scrum.
* Inclure les événements dans la liste d&#39;attente d&#39;une équipe Agile

  Pour plus d’informations, consultez [Configurer l’application des dates lors de l’ajout d’éléments de travail à une itération](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) dans [Configurer Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* Les sous-tâches peuvent être affichées sur le storyboard de Scrum.
* Affichez un graphique d’avancement pour voir les progrès réalisés par rapport aux histoires lors de l’itération.

  Pour plus d’informations, consultez [Vue d’ensemble du graphique d’avancement agile](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

Pour plus d’informations sur l’activation et la configuration de Kanban pour une équipe Agile, voir [Choisir une méthodologie Agile](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding) dans [Créer une équipe Agile](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Inclure des problèmes dans la liste d’attente Scrum pour une équipe agile {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de l’environnement de production le 14 novembre 2017. Elle devrait être réintroduite dans l’environnement de prévisualisation début 2018 avec une conception améliorée et une stabilité accrue. Elle sera publiée dans l’environnement de production de la version 2018.1.

Vous pouvez désormais inclure des problèmes dans la liste d’attente de votre équipe Agile lors de l’utilisation de la méthodologie Scrum Agile (les problèmes ne s’affichent pas dans la liste d’attente d’une équipe Agile lors de l’utilisation de la méthodologie Kanban). Les équipes Scrum Agile existantes doivent activer cette fonctionnalité pour que les problèmes soient inclus. Les problèmes sont automatiquement inclus dans la liste d’attente pour les équipes Scrum Agile créées après la version 2017.3.

Avant cette modification, seules les tâches pouvaient être ajoutées à la liste d’attente. Si vous vouliez ajouter un problème, vous deviez d’abord le convertir en une tâche avant de pouvoir l’ajouter.

Comme vous avez désormais accès à plus que les tâches de la liste d’attente, toutes les vues de tâches personnalisées disponibles précédemment dans la liste d’attente sont copiées et ajoutées à la liste d’attente en tant que vues d’élément de travail de la liste d’attente personnalisées.

Pour plus d’informations sur l’utilisation des événements dans la liste d’attente, voir  [Gérer la liste d’attente Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

Pour plus d&#39;informations sur l&#39;activation de problèmes dans la liste d&#39;attente d&#39;une équipe Agile Scrum, voir  [Configurez comment les dates sont appliquées lors de l’ajout d’éléments de travail à une itération](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) dans [Configurer Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Inclure les problèmes dans le storyboard Agile Scrum {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de l’environnement de production le 14 novembre 2017. Elle devrait être réintroduite dans l’environnement de prévisualisation début 2018 avec une conception améliorée et une stabilité accrue. Elle sera publiée dans l’environnement de production de la version 2018.1.

Vous pouvez désormais inclure des problèmes sur le storyboard lors de l’utilisation de la méthodologie Scrum Agile.

Pour plus d’informations, voir [Configurer les colonnes de statut sur le storyboard agile](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2) dans [Configurer Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Appliquer des regroupements et des filtres à la liste d’attente d’une équipe Agile {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de l’environnement de production le 14 novembre 2017. Elle devrait être réintroduite dans l’environnement de prévisualisation début 2018 avec une conception améliorée et une stabilité accrue. Elle sera publiée dans l’environnement de production de la version 2018.1.

Les options Regroupement et Filtre sont désormais disponibles dans la liste d’attente Agile. Vous pouvez ainsi organiser votre liste d’attente par regroupements et filtrer des tâches et des événements spécifiques.

Avant cette modification, vous pouviez appliquer des vues à la liste d’attente Agile.

Pour plus d’informations, voir  [Gérer la liste d’attente Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) dans  [Gérer la liste d’attente Agile](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Formatage de texte enrichi pour les mises à jour et les e-mails {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>Les modifications apportées à la mise en forme dans l’environnement de prévisualisation peuvent revenir à l’état non formaté.

Vous pouvez maintenant mettre l’accent sur les informations importantes en formatant les commentaires et les mises à jour que vous apportez aux objets Workfront. 

Les outils Texte enrichi vous permettent d’appliquer des attributs de mise en forme au texte, de créer des listes à puces et numérotées et d’ajouter des liens hypertexte à des ressources supplémentaires.

La mise en forme appliquée aux commentaires dans le flux de mise à jour s’affiche également dans les notifications de mise à jour par e-mail. Pour en savoir plus sur la mise en forme de vos commentaires, voir [Mettre à jour le travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Amélioration des retours de la fonctionnalité @Tagging dans l’environnement de prévisualisation {#enhanced-tagging-functionality-returns-in-the-preview-environment}

Vous pouvez à nouveau utiliser le symbole @ pour taguer d’autres personnes dans le flux de mise à jour de tous les objets de l’environnement de prévisualisation.Dans le passé, @tagging plaçait le prénom et le nom de la personne taguée dans le flux de mise à jour. Désormais, la fonctionnalité améliorée @tagging affiche uniquement le prénom de la personne. Pour en savoir plus sur le balisage des personnes dans les mises à jour, voir [Taguer les autres sur les mises à jour](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## L’option Filtrer les mises à jour du système dans le flux de mise à jour est désormais persistante d’un objet à l’autre. {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

L’option Filtrer les mises à jour du système est désormais persistante pour tous les objets du site Workfront. Cela vous permet de masquer les mises à jour du système et de n’afficher que les commentaires des utilisateurs et utilisatrices dans le flux de mises à jour d’un objet, et de conserver ce paramètre lorsque vous naviguez vers d’autres objets.

Avant cette modification, vous deviez choisir de filtrer les mises à jour du système pour chaque objet lorsque vous naviguiez sur le site Workfront.

Pour plus d’informations, voir [Mettre à jour le travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Visualiser les données dans le rapport d’utilisation {#visualize-data-in-the-utilization-report}

 Vous pouvez désormais afficher les informations d’utilisation dans une vue graphique. 

Pour plus d’informations, voir [Vue d’ensemble du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans [Vue d’ensemble du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Amélioration des performances de rapports d’utilisation {#utilization-report-performance-improvement}

>[!NOTE]
>
>Cette fonctionnalité a été publiée dans un correctif après la version finale beta.

Désormais, lors de l’exécution d’un rapport d’utilisation, il vous est demandé d’appliquer un filtre avant l’exécution du rapport. Cette modification garantit que les informations les plus pertinentes sont générées dans le rapport d’utilisation aussi rapidement que possible.

Pour plus d’informations sur l’exécution d’un rapport d’utilisation, voir [Vue d’ensemble du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans [Vue d’ensemble du rapport Utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Améliorations des documents : interface rationalisée {#document-enhancements-streamlined-interface}

L’expérience client de l’ajout de documents à Workfront est désormais plus simple et intuitive. Vous pouvez désormais charger un document à partir de votre système de fichiers, demander un document ou lier un fichier à partir d’une application tierce (telle que Google ou Dropbox), le tout à partir d’un simple menu déroulant. 

Auparavant, ces options étaient disponibles lors du lancement de la boîte de dialogue Ajouter des documents. 

Pour plus d’informations, consultez ce qui suit :

* [Ajouter des documents à Adobe Workfront à partir de votre système de fichiers](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [Demander un document](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [Lier des documents provenant d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!NOTE]
>
>Avec cette modification, l’option de collage d’une image ou d’un document à partir du presse-papiers n’est plus disponible.

## Améliorations de la relecture dans Workfront {#proofing-enhancements-within-workfront}

* [Expérience client améliorée et fonctionnalité supplémentaire](#improved-user-experience-and-additional-functionality)
* [Partager directement à partir de la visionneuse de relecture](#share-directly-from-the-proofing-viewer)
* [Configurer des rôles d’épreuve par défaut](#configure-default-proof-roles)

### Expérience client améliorée et fonctionnalité supplémentaire {#improved-user-experience-and-additional-functionality}

Outre une expérience client améliorée lors de la création d’épreuves dans Workfront, les fonctionnalités supplémentaires suivantes sont désormais disponibles :

* Combiner plusieurs images en une seule épreuve.
* Relire des sites web en plusieurs résolutions (plusieurs résolutions peuvent être créées sous la forme d’épreuves individuelles ou combinées en une seule épreuve).
* Modifier le nom du fichier pendant le processus de chargement.
* Inclure des champs personnalisés dans le formulaire de création d’épreuve.
* Ajouter un message personnalisé pour les notifications d’épreuves par e-mail.
* Paramètres supplémentaires d’épreuves
* Validation des erreurs en temps réel lors de la relecture d’une URL (auparavant, vous deviez attendre plusieurs minutes avant qu’une erreur ne s’affiche)

Pour plus d’informations, voir :

>[!NOTE]
>
>Lors de la création d’une nouvelle épreuve avec un workflow automatisé, l’action de faire glisser et déposer n’est pas prise en charge pour déplacer les personnes d’une étape à une autre. Supprimez plutôt la personne d’une étape et ajoutez-la à une autre.

*L’option permettant de déplacer les personness d’une étape à une autre en les faisant glisser et en les déposant sera réintroduite avec la version 2018.1.*

### Partager directement à partir de la visionneuse de relecture {#share-directly-from-the-proofing-viewer}

Vous pouvez désormais partager des données avec des utilisateurs et utilisatrices spécifiques de Workfront directement à partir de la visionneuse de relecture.

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement pour les nouvelles épreuves (épreuves créées après la version 2017.3) et uniquement pour les instances Workfront intégrées à un compte Workfront Proof Premium.

Avant cette modification, vous ne pouviez partager qu’en créant un lien, puis en le partageant avec une personne. 

Pour plus d’informations, voir [Partager une épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) dans [Partager une épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

### Configurer des rôles d’épreuve par défaut {#configure-default-proof-roles}

Vous pouvez désormais configurer les rôles d épreuves par défaut dont disposent les nouveaux utilisateurs et utilisatrices, et les utilisateurs et utilisatrices invités pour créer des épreuves dans le système Workfront. 

Il s’agit du rôle par défaut auquel les personnes sont affectées sur une épreuve lorsque l’épreuve est partagée avec elles. 

## Améliorations de la relecture dans Workfront Proof et Workfront {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [Redémarrer et faire des sauts dans la visionneuse de relecture vidéo HTML5 (raccourcis clavier)](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [Mises à jour de la visionneuse de relecture HTML5](#html5-proofing-viewer-updates)

### Redémarrer et ignorer dans la visionneuse de relecture vidéo HTML5 (raccourcis clavier) {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

Il existe désormais des raccourcis clavier dans la visionneuse de relecture HTML5 pour la vidéo qui vous permettent de redémarrer la vidéo au début et de sauter jusqu’à la fin de la vidéo.

Pour plus d’informations sur les raccourcis clavier disponibles, voir [Raccourcis clavier dans la visionneuse de relecture Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md).

### Mises à jour de la visionneuse de relecture HTML5 {#html5-proofing-viewer-updates}

La visionneuse HTML5 prend désormais en charge les épreuves statiques.

Avant cette modification, la visionneuse HTML5 ne prenait en charge que les épreuves vidéo. 

La visionneuse HTML comprend les nouvelles fonctionnalités suivantes lors de la relecture du contenu statique :

* Faire un seul commentaire avec des balises sur plusieurs pages en mode vue unique

  Auparavant, cela n’était possible que dans la vue Continu ou Magazine.

* Parcourir les épreuves à partir des miniatures d’épreuves

   * Identifiez facilement la partie de l’épreuve qui est en cours de révision. Ceci est important, en particulier lorsque les personnes utilisent des épreuves plus volumineuses et de longues pages web, ou chaque fois qu’une échelle plus grande est nécessaire pour afficher les détails.
   * Modifier l’échelle
   * Effectuer un panoramique du contenu

* Spécifier les valeurs personnalisées dans l’outil de mesure
* Lors de l’annotation de texte d’une épreuve dans la visionneuse de relecture dans Workfront Proof, vous pouvez inclure des options pour indiquer que le texte doit être en gras, en italique et souligné.

La visionneuse HTML5 ne prend pas encore en charge toutes les fonctionnalités actuellement disponibles dans la visionneuse Flash existante. Les fonctionnalités suivantes ne sont actuellement pas disponibles, mais seront incluses dans une version ultérieure :

* Prise en charge des fichiers de médias riches
* Mode comparaison (vidéo et statique)
* Filtrage des commentaires (vidéo et statiques)
* Vérifier les hyperliens dans les documents (statiques)
* Traductions (vidéo et statiques)
* Indicateur de présence qui affiche les personnes qui travaillent actuellement sur l’épreuve.
* Partager les épreuves

Pour plus d’informations sur la relecture des épreuves statiques dans la visionneuse HTML5, voir .

En tant qu’administrateur ou administratrice Workfront dans Workfront Proof, vous pouvez déterminer si les personnes de votre entreprise ont accès à la nouvelle visionneuse de relecture HTML5 pour les épreuves vidéo.

## Nouvelle conception du graphique de Gantt {#new-gantt-chart-redesign}

Le nouveau graphique de Gantt comprend les améliorations suivantes :

* Nouvelles icônes et nouveaux marqueurs
* Nouvelle option permettant d’effectuer un zoom avant ou arrière sur une période spécifique
* Cellules de petites tâches dans la partie Liste du graphique
* Options repensées pour les paramètres, l’impression et le passage aux dates prévisionnelles.

Pour plus d’informations sur la configuration des options dans le graphique de Gantt, voir [Configurer l’affichage des informations sur le graphique de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Les rapports intégrés contiennent des descriptions mises à jour {#built-in-reports-contain-updated-descriptions}

Nous avons mis à jour les descriptions de nos rapports système dans Workfront afin d’inclure des informations sur le type de rapport et les champs inclus.  

Avant cette modification, la plupart de nos rapports intégrés n’avaient aucune description, sinon une très limitée.

Pour plus d’informations sur les rapports intégrés, voir [Utiliser les rapports intégrés d’Adobe Workfront](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Branding dans les rapports, listes et tableaux de bord exportés {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>Cette fonctionnalité est actuellement indisponible sur tous les clusters dans l’environnement de prévisualisation.

Si vous travaillez avec le branding dans Workfront, le logo que vous utilisez dans votre barre de navigation globale est désormais inclus dans les fichiers .pdf que vous exportez à partir de Workfront.

Les fichiers .pdf suivants incluront le logo de votre organisation dans le document exporté :

* Listes exportées
* Rapports exportés et distribués
* Tableaux de bord imprimés

Pour plus d’informations sur l’export de données à partir de Workfront, voir [Exporter des données](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Améliorations lors de la copie de tâches et du déplacement de tâches ou de problèmes {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

Nous avons apporté des modifications aux modes de copie d’une tâche et de déplacement d’une tâche ou d’un problème, de façon à faciliter la sélection d’un parent pour l’objet (tâche ou problème) copié ou déplacé. Lorsque vous sélectionnez un parent en copiant une tâche, par exemple, vous pouvez désormais consulter une hiérarchie des tâches, comprenant leur relation parent-enfant, ainsi que rechercher un parent dans les projets comportant de nombreuses tâches.

Avant cette modification, aucun champ de recherche n’était présent dans l’étape **Sélectionner un parent** et la hiérarchie des tâches n’était pas visible dans la liste des tâches.

Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Pour plus d’informations sur le déplacement des problèmes, voir [Déplacer des problèmes](../../../../manage-work/issues/manage-issues/move-issues.md).

## Nouvelle configuration pour le rappel des demandes dans la zone des paramètres d’approbation {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

Nous avons ajouté une nouvelle option dans la zone Paramètres d’approbation à l’échelle du système, afin de permettre aux administrateurs et administratrices de Workfront d’autoriser les utilisateurs et utilisatrices à rappeler un problème ou une demande dont le premier statut est en attente d’approbation. Si le rappel est autorisé, le problème est supprimé. Si le rappel n’est pas autorisé, un bouton Rappel ne s’affiche pas pour les utilisateurs et utilisatrices lorsque le premier statut d’un problème est en attente d’approbation.

Avant cette modification, le rappel du problème était toujours autorisé. Lorsque l’approbation était rappelée, celle-ci était complètement contournée, ce qui plaçait le problème dans son premier statut, sans approbation jointe.

Pour plus d’informations sur les paramètres d’approbation, voir [Configurer les paramètres globaux du processus d’approbation](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

>[!NOTE]
>
>Lorsque cette fonctionnalité sera disponible, cette option sera désactivée par défaut. Le rappel de problèmes est actuellement activé par défaut pour toutes les organisations. Lorsque cette fonctionnalité est disponible, l’administrateur ou l’administratrice de Workfront doit activer manuellement ce paramètre pour conserver les fonctionnalités telles quelles dans Workfront.

## Nouveau regroupement pour les rapports sur les heures budgétées des ressources : date d’attribution {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

Nous avons ajouté la possibilité de regrouper vos résultats par date d’attribution lors de la création d’un rapport des heures budgétées pour les ressources.

Avant cette modification, vous pouviez afficher la date d’attribution dans la vue du rapport, ainsi que l’utiliser dans un filtre, mais vous ne pouviez pas utiliser ce champ dans un regroupement.

Pour plus d’informations sur la date d’attribution, voir [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Améliorations du planificateur de ressources {#resource-planner-improvements}

* [Planificateur de ressources : afficher les données par équivalent temps complet](#resource-planner-show-data-by-fte)
* [Planificateur de ressources : afficher les données par semaine et par trimestre](#resource-planner-show-data-by-week-and-quarter)
* [Planificateur de ressources : vue par utilisateur ou utilisatrice](#resource-planner-view-by-user)
* [Planificateur de ressources : faire glisser et déposer des projets pour établir des priorités](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [Planificateur de ressources : exporter les données du planificateur de ressources vers Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### Planificateur de ressources : afficher les données par équivalent temps complet {#resource-planner-show-data-by-fte}

Vous pouvez désormais afficher l’attribution et la disponibilité de vos ressources par équivalent temps complet dans le planificateur de ressources. Avant cette modification, vous ne pouviez afficher les valeurs qu’en heures.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planificateur de ressources : afficher les données par semaine et par trimestre {#resource-planner-show-data-by-week-and-quarter}

Vous pouvez désormais modifier l’intervalle de période de votre planificateur de ressources afin de l’afficher de façon hebdomadaire ou trimestrielle. Avant cette modification, vous ne pouviez afficher l’attribution et la disponibilité de vos ressources et les budgétiser que de façon mensuelle.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planificateur de ressources : vue par utilisateur ou utilisatrice {#resource-planner-view-by-user}

Vous pouvez désormais afficher les informations dans le planificateur de ressources par utilisateur ou utilisatrice dans un premier temps, puis par projets, rôles et tâches. Vous pouvez également afficher une différence entre les heures prévues et les heures disponibles ou l’équivalent temps complet pour les utilisateurs et utilisatrices. Avant cette modification, vous pouviez afficher les informations dans le planificateur de ressources par projets et rôles.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planificateur de ressources : faire glisser et déposer les projets pour établir des priorités {#resource-planner-drag-and-drop-projects-to-establish-priority}

Vous pouvez désormais faire glisser et déposer des projets dans l’ordre de priorité souhaité. Avant cette modification, vous ne pouviez définir la priorité des projets qu’en leur attribuant manuellement un nombre.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Planificateur de ressources : exporter les données du planificateur de ressources vers Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

Vous pouvez désormais exporter les informations du planificateur de ressources vers un fichier Excel.

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Améliorations apportées à l’application mobile {#mobile-improvements}

Nous avons ajouté la possibilité d’accéder à vos projets et de les gérer à partir de l’application mobile Workfront. Vous pouvez désormais effectuer les opérations suivantes à l’aide de l’application mobile Workfront :

* Accéder à la liste de vos projets
* Accéder à la liste des tâches et sous-tâches d’un projet
* Accéder à la liste des problèmes d’un projet
* Enregistrer un nouveau problème sur un projet

Vous pouvez installer cette fonctionnalité lorsque vous mettez à jour votre application mobile Workfront. La mise à jour sera disponible dans les boutiques mobiles Apple et Android en novembre 2017.

## Intégration Workfront avec Slack {#workfront-integration-with-slack}

>[!NOTE]
>
>L’intégration pour Slack n’est actuellement pas disponible. Elle sera disponible pour utilisation avec votre environnement de production en novembre 2017.

Nous lançons une nouvelle intégration entre Workfront et Slack. Si votre entreprise a déjà utilisé Slack pour votre communication, vous pouvez désormais l’intégrer à Workfront et effectuer des actions Workfront courantes sans quitter vos canaux de communication dans Slack. Vous pouvez désormais effectuer les actions suivantes à partir de votre compte Slack :

* Rechercher un élément dans Workfront
* Accéder à vos listes de tâches et d’approbations
* Créer une tâche
* Créer un événement
* S’abonner à un élément à partir d’un lien partagé avec vous
* Affecter des tâches et des problèmes à partir d’un lien partagé avec vous
* Approuver votre travail
* Accéder à vos favoris et à vos listes d’éléments récents

Pour plus d’informations sur l’accès à Workfront à partir de Slack, voir [Utiliser Workfront avec Slack.](https://support.workfront.com/hc/en-us/sections/115000458033)

## Améliorations apportées à Outlook 365 {#outlook-365-improvements}

Nous avons apporté les améliorations suivantes au module complémentaire Workfront pour Outlook 365 :

* Ajouter une tâche ou un problème à un projet dans Workfront : vous pouvez désormais convertir un e-mail en tâche ou en problème dans Workfront à l’aide du module complémentaire Outlook 365. Au cours de ce processus, vous pouvez spécifier un projet auquel vous souhaitez ajouter la tâche ou le problème, ainsi qu’une personne cessionnaire et une date d’échéance. Avant cette amélioration, vous ne pouviez envoyer qu’une demande à une file d’attente de demandes ou ajouter une tâche personnelle à votre liste En train de travailler sur à partir d’Outlook 365. 
* Conserver un lien vers les objets Workfront dans l’e-mail d’origine converti en tâches, problèmes ou demandes : lorsque vous convertissez un e-mail d’Outlook 365 en tâche, problème ou demande, Outlook 365 conserve un lien vers la tâche convertie ou le problème converti à partir de cet e-mail dans l’e-mail d’origine. Avant cette modification, Outlook n’indiquait pas si un e-mail avait été converti en tâche ou envoyé en tant que demande. 

## Modifications des API {#api-changes}

* [API 8 désormais disponible](#api-8-now-available)
* [Versions supprimées et obsolètes de l’API](#removed-and-deprecated-versions-of-the-api)
* [Activité de la version Beta finale 2017.3](#updated-message-format-for-event-subscriptions)
* [Reprises pour les abonnements aux événements pour les messages non distribuables](#event-subscription-retries-for-undeliverable-messages)

### API 8 désormais disponible {#api-8-now-available}

L’API Workfront version 8 est désormais disponible et vous offre des ressources nouvelles et mises à jour pour vos intégrations Workfront.

Pour obtenir la liste des modifications apportées à l’API Workfront, voir [Mises à jour de l’API version 8](../../../../wf-api/api/new-api-version-8-updates.md).

### Versions supprimées et obsolètes de l’API {#removed-and-deprecated-versions-of-the-api}

### Mise à jour du format de message pour les abonnements aux événements

Afin de fournir des informations plus utiles pour vos intégrations qui incluent l’API d’abonnement aux événements Workfront, nous avons modifié le format des messages sortants pour les ressources prises en charge en incluant les anciennes et nouvelles valeurs associées à ces ressources. Pour éviter tout échec, toutes les intégrations que vous avez à l’aide de l’API d’abonnement aux événements Workfront doivent être mises à jour dans le nouveau format, comme décrit dans la section [API d’abonnement aux événements](../../../../wf-api/general/event-subs-api.md).

### Reprises pour les abonnements aux événements pour les messages non distribuables {#event-subscription-retries-for-undeliverable-messages}

La structure d’abonnement aux événements Workfront fournit désormais un mécanisme de gestion des messages sortants déclenchés par un événement qui ne sont pas remis aux points d’entrée clients. Afin d’assurer une remise continue des messages, les clients et clientes doivent s’assurer que tous les points d’entrée utilisant des messages sortants des abonnements à des événements sont correctement configurés. Pour plus d’informations, voir [Reprises pour les abonnements aux événements](../../../../wf-api/api/event-sub-retries.md).
