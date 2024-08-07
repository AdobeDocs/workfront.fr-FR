---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.2, version bêta 5
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.2 de Beta 5. Cette fonctionnalité sera disponible dans l’environnement Aperçu le 1er juin 2018. Les améliorations de la vérification avec Beta 5 seront disponibles dans l’environnement Aperçu le lundi 4 juin. Il sera disponible dans l’environnement de production en juillet 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3165'
ht-degree: 1%

---

# Activité Version 2018.2, version bêta 5

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.2 de Beta 5. Cette fonctionnalité sera disponible dans l’environnement Aperçu le 1er juin 2018. Les améliorations de la vérification avec Beta 5 seront disponibles dans l’environnement Aperçu le lundi 4 juin. Il sera disponible dans l’environnement de production en juillet 2018.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.2, voir  [Présentation de l’activité de version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La version 2018.2 de Beta 5 contient les améliorations apportées aux administrateurs de Workfront et aux autres utilisateurs :

**Pour les administrateurs**

* [ Afficher les modifications déclenchées par l’utilisateur avec les journaux d’audit ](#view-user-triggered-changes-with-audit-logs)
* [Affichage des informations de licence en tant qu’administrateur de groupe](#view-license-information-as-a-group-administrator)

**Pour Tous Les Utilisateurs**

* [Vue Calendrier dans la zone d’accueil](#calendar-view-in-the-home-area)
* [Mises à jour supplémentaires de la liste de travail (panneau de gauche) à l’accueil](#additional-updates-to-the-work-list-left-panel-in-home)
* [Configuration des limites de rôle de tâche pour la planification automatisée des ressources](#configure-job-role-limits-for-automated-resource-scheduling)
* [Améliorations de la vue Projet et Rôle dans le planificateur de ressources](#project-and-role-view-improvements-in-the-resource-planner)
* [Redimensionner la largeur des colonnes pour les listes de projets](#resize-column-widths-for-project-lists)
* [Prise en charge des icônes pour les nouvelles listes de projets](#icon-support-for-the-new-project-lists)
* [Ajouter un champ &quot;grande miniature&quot; dans les vues de document](#add-large-thumbnail-field-in-document-views)
* [Augmentation de la limite d’exportation Excel](#increase-excel-export-limit)
* [Filtres rapides pour les listes de projets](#quick-filters-for-project-lists)
* [Collections de problèmes de référence dans les rapports de projet et de tâche](#reference-issue-collections-in-project-and-task-reports)
* [Nouveau menu de version plus robuste lors de l’ajout de nouvelles versions de document dans Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Améliorations mobiles dans l’application mobile Android Beta](#mobile-improvements-in-the-android-beta-mobile-app)
* [ Améliorations apportées à la visionneuse de test (Workfront et Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Améliorations de la vérification dans Workfront](#proofing-enhancements-in-workfront)
* [Améliorations de la vérification dans Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Mode Calendrier dans la zone d’accueil {#calendar-view-in-the-home-area}

Vous pouvez désormais gérer vos tâches et plannings personnels à l’aide de la vue Calendrier d’accueil de Workfront. La vue Calendrier d’accueil vous permet d’effectuer les opérations suivantes :

* Définissez votre propre planning pour accomplir les tâches Workfront qui vous sont affectées.
* Afficher rapidement les tâches qui sont en retard ou en retard
* Afficher le total des heures allouées pour une semaine
* Effectuer des mises à jour des tâches qui vous sont affectées

Si vous utilisez un calendrier dans Outlook, vous pouvez intégrer votre calendrier pour afficher vos événements Outlook dans la vue Calendrier d’accueil.

Pour plus d’informations, voir la [vue Calendrier d’accueil](../../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## Mises à jour supplémentaires de la liste de travail (panneau de gauche) dans la page d’accueil {#additional-updates-to-the-work-list-left-panel-in-home}

Les améliorations suivantes ont été apportées à la liste de tâches dans la zone Accueil :

* Le nombre d’éléments terminés s’affiche désormais entre parenthèses en regard de l’option Terminé dans le menu déroulant Filtre .

  Auparavant, le nombre d’éléments terminés ne s’affichait pas dans le menu Filtre . 

* Les éléments terminés sont affichés pour les 2 semaines précédentes.

  Auparavant, les éléments terminés étaient affichés pour les 3 mois précédents.

  Pour plus d’informations sur l’affichage des tâches terminées dans la zone d’accueil, voir [Affichage des éléments dans la liste de travail de la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) dans l’article [Affichage des éléments dans la liste de travail de la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Ajoutez les champs Durée et Affectations à afficher lorsque des éléments sont sélectionnés dans la zone Accueil .

  Auparavant, le champ Affectations était disponible par défaut. Cependant, s’il était supprimé, il ne pouvait pas être ajouté à nouveau. Le champ Durée n’était pas disponible auparavant pour l’ajout.

  Pour plus d’informations sur l’ajout de champs à la zone Accueil, voir &quot;Création et gestion des modèles de mise en page&quot;.

Pour plus d’informations sur l’utilisation de la zone d’accueil, voir [Utilisation de la zone d’accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Affichage des modifications déclenchées par l’utilisateur avec les journaux d’audit {#view-user-triggered-changes-with-audit-logs}

Nous avons créé les journaux d’audit suivants pour les administrateurs Workfront afin de suivre les modifications déclenchées par l’utilisateur :

* Journal d’audit utilisateur
* Journal d’audit du niveau d’accès
* Journaux d’audit de groupe
* Journaux d’audit des tentatives de connexion

Auparavant, il n’était pas possible de suivre les modifications dans le système.

Pour plus d’informations, voir [Affichage et exportation des journaux d’audit](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Affichage des informations de licence en tant qu’administrateur de groupe {#view-license-information-as-a-group-administrator}

Nous avons créé une page Licences en lecture seule pour permettre aux administrateurs de groupe d’afficher le nombre de licences pour les groupes qu’ils gèrent.

Avant cette modification, les administrateurs de groupe ne pouvaient pas afficher les informations de licence.

Pour plus d’informations, voir [Administrateurs de groupe](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Configuration des limites de rôle de tâche pour la planification automatisée des ressources {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Dans les paramètres de planification des ressources automatisée, vous pouvez désormais attribuer une limite à un rôle de tâche. Cela vous permet de contrôler le nombre de ressources, avec le même rôle, auxquelles un travail est affecté.

Auparavant, vous ne pouviez pas spécifier le nombre d’utilisateurs pouvant se voir attribuer une tâche au sein d’un rôle de tâche donné.

Pour plus d’informations, voir &quot;Affectation manuelle de tâches et de problèmes non attribués dans les zones Planification&quot;.

## Améliorations de la vue Projet et Rôle dans le planificateur de ressources {#project-and-role-view-improvements-in-the-resource-planner}

Les vues Projet et Rôle du planificateur de ressources contiennent désormais les améliorations suivantes :

* Amélioration des filtres qui extraient les informations de l’ensemble de la base de données, plutôt que simplement des informations à l’écran.
* Mode Plein écran.
* Les performances sont désormais plus rapides et plus efficaces.

   * Nouvelles limites pour le nombre de projets, de rôles et d’utilisateurs que vous pouvez afficher.
   * Chargement différé, pour un chargement plus rapide des projets et des rôles.

* Accès rapide aux projets et aux utilisateurs directement à partir du planificateur de ressources.
* Fonction de glisser-déposer plus rapide dans la vue Projet pour classer vos projets par priorité.

Avant ces améliorations, vous avez signalé que le planificateur de ressources était lent à charger et que vous aviez remarqué des incohérences dans les données affichées. Ces améliorations devraient maintenant être éliminées.

Pour plus d’informations et pour comprendre les nouvelles limites du planificateur de ressources, voir [ Limites d’affichage du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Redimensionner la largeur des colonnes pour les listes de projets {#resize-column-widths-for-project-lists}

Comme nous avons travaillé à l&#39;amélioration de la fonctionnalité de nos listes, nous avons temporairement désactivé la capacité de redimensionner les largeurs des colonnes dans les listes de projets suivantes :

* Projets dont je suis propriétaire
* Projets auxquels je participe
* Tous les projets

Avec cette version, nous pouvons à nouveau redimensionner les colonnes de toutes les listes de projets.

Nous avons ajouté d’autres améliorations à cette fonctionnalité.

Désormais, lorsque vous faites glisser la bordure droite d’une colonne pour la redimensionner, la colonne voisine à droite conserve sa taille, ce qui élargit la liste, plutôt que d’être également modifiée. Vous pouvez également faire glisser la bordure d’une colonne vers la droite au-delà des bordures des colonnes voisines.

Avant cette amélioration, la colonne voisine à droite de la colonne redimensionnée était également redimensionnée proportionnellement pour s’adapter à l’écran. Vous ne pouviez pas faire glisser la bordure d’une colonne le long de la bordure droite de la colonne voisine.  

Pour plus d’informations sur le redimensionnement des colonnes de réorganisation dans les listes, voir [Modification de la largeur et de l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Pour participer à notre programme de test bêta pour connaître les améliorations actuelles de la liste, consultez l&#39; [étude sur les nouvelles listes.](http://community.workfront.com/discussions/community-home/digestviewer/viewthread?GroupId=457&amp;MessageKey=6b135c15-33dd-4fa2-8bc3-7cd7f7740c57&amp;CommunityKey=0425cafc-f0ec-47fc-be20-a21dc073d520&amp;tab=digestviewer&amp;ReturnUrl=%2fdiscussions%2fcommunity-home%2fdigestviewer%3fCommunityKey%3d0425cafc-f0ec-47fc-be20-a21dc073d520) (connexion requise)

## Prise en charge des icônes pour les nouvelles listes de projets {#icon-support-for-the-new-project-lists}

Comme nous nous sommes efforcés d’améliorer la fonctionnalité de nos listes, nous avions temporairement désactivé l’affichage des icônes d’état dans les listes de projets suivantes :

* Projets dont je suis propriétaire
* Projets auxquels je participe
* Tous les projets

Avec cette version, les icônes d’état peuvent s’afficher à nouveau dans les listes de projets pour les projets ou d’autres objets dans une liste de projets.

Pour plus d’informations sur l’utilisation des listes, voir [Prise en main des listes dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Ajout d’un champ &quot;Grande miniature&quot; dans les vues de document {#add-large-thumbnail-field-in-document-views}

Nous ajoutons un nouveau champ appelé Grande miniature à un affichage de document dans une liste ou un rapport. Lorsqu’il est sélectionné dans une vue de document, ce champ affiche une miniature de 400 pixels pour le document dans une liste ou un rapport.

Avant cette modification, vous ne pouviez ajouter que le champ Miniature à une vue de document, qui affiche une miniature de 33 à 66 pixels pour le document.

Pour plus d’informations sur les champs des listes et des rapports, voir le [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Augmentation de la limite d’exportation Excel {#increase-excel-export-limit}

Nous avons augmenté la limite du nombre de lignes pouvant être exportées dans un fichier Excel. Vous pouvez désormais exporter les éléments suivants :

* 65 000 lignes dans un fichier Excel .xls
* 100 000 lignes dans un fichier Excel .xlsx

Les nouvelles limites s’appliquent lorsque vous exportez les éléments suivants depuis Workfront :

* Liste ou rapport à partir de l’interface web
* Liste ou rapport à l’aide de l’API
* Rapport planifié et remis

Avant cette amélioration, vous ne pouviez exporter que 50 000 lignes dans n’importe quel fichier Excel.

Pour plus d&#39;informations sur l&#39;export de données depuis Workfront, voir [Export de données](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Filtres rapides pour les listes de projets {#quick-filters-for-project-lists}

Vous pouvez maintenant appliquer un filtre rapide aux listes.

L’objectif d’un filtre rapide est de vous aider à accéder directement aux éléments de vos listes volumineuses qui vous intéressent, afin que vous puissiez rapidement les examiner, les mettre à jour ou les partager avec d’autres personnes.

Actuellement, les filtres rapides ne sont disponibles que pour les listes de projets dans les sous-onglets suivants :

* Projets auxquels je participe
* Projets dont je suis propriétaire
* Tous les projets

Pour plus d’informations sur les filtres rapides, reportez-vous à la section &quot;Application de filtres rapides aux listes&quot; dans [Prise en main des listes dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Collections de problèmes de référence dans les rapports de projet et de tâche {#reference-issue-collections-in-project-and-task-reports}

Vous pouvez désormais référencer un ensemble de problèmes dans une vue de projet ou de tâche et les filtrer. Vous pouvez le faire uniquement à l’aide du mode Texte lors de la création d’un rapport.

Avant cette amélioration, vous ne pouviez référencer qu’une collection de tâches dans une vue de projet ou un filtre.

Pour plus d’informations sur la manière de référencer une collection dans un rapport, voir [Référencer des collections dans un rapport](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

Pour plus d’informations sur l’utilisation du mode texte, voir  [Présentation des utilisations courantes du mode Texte](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>Dans la vidéo suivante, l’exemple de mode de texte pour les collections de problèmes était incorrect. Le mode de texte d’exemple correct est disponible dans [Collections de référence dans un rapport](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

## Nouveau menu de version plus robuste lors de l’ajout de nouvelles versions de document dans Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Désormais, lors de l’ajout de nouvelles versions aux documents dans Workfront, le menu Nouvelle version contient des options supplémentaires et est désormais cohérent dans toutes les zones de Workfront où vous pouvez ajouter une nouvelle version.

Vous pouvez ajouter une nouvelle version de document à partir des zones suivantes de Workfront :

* Dans le menu déroulant Plus de l’onglet Documents .
* Dans le menu Actions de document de la page Détails du document.
* Dans l’onglet Toutes les versions de la page de détails du document.

Avant cette modification, seul le menu déroulant Plus de l’onglet Documents contenait toutes les options pour ajouter une nouvelle version.

Les options suivantes sont désormais disponibles dans le menu Nouvelle version pour toutes les zones où vous pouvez ajouter une nouvelle version :

* Épreuve
* Document uniquement
* Options liées (de Dropbox, de Google Drive, etc.)
* Coller à partir du Presse-papiers (cette nouvelle option est disponible lors de l’ajout de versions)

Pour plus d’informations, voir [Ajout de documents à Adobe Workfront à partir de votre système de fichiers](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) dans l’article [Ajout de documents à Adobe Workfront à partir de votre système de fichiers](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Améliorations apportées à l’application mobile Android Beta {#mobile-improvements-in-the-android-beta-mobile-app}

Les améliorations suivantes seront disponibles dans la version Beta d’Android de l’application mobile peu après le jour de cette version :

* Actions de glissement

  Vous pouvez exécuter des activités telles que le bénévolat pour travailler sur une tâche, terminer une tâche, marquer une notification comme vue ou une nouvelle, envoyer un texte ou appeler un contact en faisant glisser divers objets dans l’application mobile Workfront.

  Les zones suivantes ont été améliorées avec cette fonctionnalité :

   * Mon travail et mon foyer
   * Notifications
   * Contacts
   * Approbations

* Nouvelle apparence lors de l’affichage de l’onglet Détails d’un élément

  L’interface a changé lors de l’affichage d’un élément dans la version Beta d’Android de l’application mobile afin de faciliter sa modification, sa saisie ou la pièce jointe.

* Nouvelle expérience lors de la connexion

  Le temps de journalisation est plus rapide et plus facile qu’auparavant, avec un bouton Temps de journalisation plus facile d’accès et une interface plus rationalisée pour les heures de journalisation.

Avec cette version, ces améliorations ne sont disponibles que pour la version Beta Android de l’application mobile Workfront. Ils ne sont actuellement pas disponibles pour iOS.

Pour plus d’informations sur l’inscription à un testeur bêta et le téléchargement de la version Beta Android de l’application mobile Workfront, voir .

## amélioration de la visionneuse de correctifs (Workfront et Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Page de résumé d’impression mise à jour](#updated-print-summary-page)
* [Ajouter des utilisateurs à un bon à tirer directement à partir de la visionneuse de vérification](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [Afficher tous les outils de balisage dans la visionneuse de vérification](#display-all-markup-tools-in-the-proofing-viewer)
* [Configuration des options de tri par défaut dans la visionneuse de correctifs](#configure-default-sorting-options-in-the-proofing-viewer)
* [Afficher les approbations de documents Workfront dans la visionneuse de vérification de l’appli de bureau](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Configurer des liens qui ouvrent de nouveaux onglets et Windows à ouvrir dans la visionneuse de vérification de l’appli de bureau](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [Indicateur de présence dans la visionneuse de vérification](#presence-indicator-in-the-proofing-viewer)
* [Filtrer les commentaires pour afficher une seule page pour les bons à tirer d’URL interactifs dans la visionneuse de vérification de l’appli de bureau](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [Visionneuse de vérification de poste de travail pour le contenu statique et vidéo](#desktop-proofing-viewer-for-static-and-video-content)
* [Ajout de périphériques personnalisés à votre système](#add-custom-devices-to-your-system)

### Page Résumé de l’impression {#updated-print-summary-page}

La page Résumé de l’impression a été mise à jour avec une nouvelle apparence et une fonctionnalité améliorée.

Pour plus d’informations, voir [Imprimer un résumé de BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Ajout d’utilisateurs à un BAT directement à partir de la visionneuse de vérification {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Vous pouvez désormais ajouter des utilisateurs à un BAT directement à partir de la visionneuse de BAT et de la visionneuse de BAT. 

Auparavant, vous ne pouviez pas ajouter des utilisateurs individuels à un BAT. Vous pouvez uniquement copier l’URL publique ou le code intégré.

Pour plus d’informations, voir [Partager un BAT en y ajoutant des utilisateurs](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) dans l’article  [Partagez un BAT à partir de la visionneuse de vérification](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Afficher tous les outils de balisage dans la visionneuse de vérification {#display-all-markup-tools-in-the-proofing-viewer}

Vous pouvez maintenant configurer l’outil de balisage pour qu’il s’affiche tout le temps plutôt que dans un menu que vous devez ouvrir. Cela permet de basculer plus rapidement entre les outils. Lorsqu’ils sont configurés de cette manière, les outils de balisage s’affichent horizontalement en haut de la visionneuse de vérification et de l’écran de bureau.

Auparavant, les outils de balisage n’étaient disponibles que dans un menu déroulant.

Pour plus d’informations sur la configuration de ce paramètre de balisage, voir [Configuration des paramètres de la visionneuse de vérification de l’orthographe](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Pour plus d’informations sur l’utilisation des options de balisage lors de la révision d’un BAT, reportez-vous à l’ article .

### Configuration des options de tri par défaut dans la visionneuse de vérification {#configure-default-sorting-options-in-the-proofing-viewer}

Désormais, lorsque vous modifiez l’option de tri dans la liste de commentaires d’un BAT, cette option devient l’option de tri par défaut la prochaine fois que vous ouvrez un BAT dans la visionneuse de BAT ou de BAT de bureau. 

Pour plus d’informations, voir dans l’article .

### Affichage des approbations de documents Workfront dans la visionneuse de vérification de l’appli de bureau {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Vous pouvez désormais effectuer une décision d’approbation de document Workfront dans la visionneuse de vérification de l’appli de bureau.

Auparavant, seule la visionneuse de Web Proofing vous permettait de prendre une décision concernant l’approbation de documents Workfront. 

Pour plus d’informations, voir  [Prendre une décision sur un BAT dans la visionneuse de vérification](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) de l’article  [Prenez une décision sur un BAT dans la visionneuse de correctifs](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Configuration de liens qui ouvrent de nouveaux onglets et Windows à ouvrir dans la visionneuse de vérification de l’appli de bureau {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

Lors de la vérification du contenu interactif dans la visionneuse de vérification de l’appli de bureau, vous pouvez maintenant configurer les liens qui s’ouvrent dans un nouvel onglet ou une nouvelle fenêtre pour qu’ils s’ouvrent dans la visionneuse de vérification de l’appli de bureau afin de pouvoir continuer la vérification de l’orthographe.

Dans la visionneuse de vérification héritée, les liens ouverts dans un nouvel onglet ou une nouvelle fenêtre n’ont pas pu être vérifiés dans la visionneuse de vérification.

Pour plus d’informations, voir [Configuration des paramètres de la visionneuse de correctifs](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Indicateur de présence dans la visionneuse de vérification {#presence-indicator-in-the-proofing-viewer}

Désormais, lorsque vous passez en revue un BAT dans la visionneuse de BAT ou la visionneuse de BAT pour ordinateur, vous pouvez voir l’avatar de chaque utilisateur qui regarde actuellement le BAT s’affiche dans le coin supérieur droit de la visionneuse de BAT.

Pour plus d&#39;informations, voir [Vérifier un BAT simultanément avec plusieurs réviseurs](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filtrage des commentaires pour afficher une seule page pour les bons à tirer d’URL interactifs dans la visionneuse de vérification de l’appli de bureau {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

Lors de la révision d’une URL dans un BAT interactif dans la visionneuse de vérification de l’appli de bureau, vous pouvez désormais filtrer les commentaires afin d’afficher uniquement les commentaires effectués sur la page active. 

Avant cette modification, cette option était disponible uniquement pour les bons à tirer statiques.

Pour plus d’informations, voir dans l’article .

### Visionneuse de vérification de poste pour le contenu statique et vidéo {#desktop-proofing-viewer-for-static-and-video-content}

La visionneuse de vérification de l’appli de bureau prend désormais en charge le contenu statique et vidéo.

Auparavant, il ne prenait en charge que le contenu interactif.

Pour plus d’informations sur la configuration des BAT statiques et vidéo à ouvrir dans la visionneuse de vérification de l’appli de bureau, voir [ Configuration des paramètres de la visionneuse de vérification de l’orthographe ](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Pour plus d’informations sur la visionneuse de vérification de l’appli de bureau, voir [Vérification des bons à tirer dans la visionneuse de vérification de l’appli de bureau.](https://support.workfront.com/hc/en-us/sections/360000686434)

### Ajout de périphériques personnalisés à votre système {#add-custom-devices-to-your-system}

Vous pouvez désormais ajouter des appareils personnalisés à votre système, ce qui permet aux utilisateurs de passer en revue le contenu interactif et de simuler son apparence sur un appareil spécifique lors de la révision d’un BAT dans la visionneuse de vérification de l’application de bureau.

Avant cette modification, les utilisateurs pouvaient choisir uniquement parmi une liste de périphériques standard préconfigurés.

Pour plus d’informations sur l’ajout d’appareils personnalisés, voir

Pour plus d’informations sur la façon dont les utilisateurs peuvent sélectionner les appareils lors de la révision du contenu interactif, voir [Modification de la résolution du BAT interactif dans la visionneuse de vérification de performance](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Améliorations de la vérification dans Workfront {#proofing-enhancements-in-workfront}

* [Partager directement le lien du BAT à partir de Workfront](#share-the-proof-link-directly-from-workfront)
* [Rapport sur les données de vérification supplémentaires dans Workfront](#report-on-additional-proofing-data-in-workfront)
* [Affichage des données historiques pour les approbations de BAT dans Workfront](#view-historical-data-for-proof-approvals-in-workfront)

### Partage direct du lien du bon à tirer à partir de Workfront {#share-the-proof-link-directly-from-workfront}

Vous pouvez désormais générer un lien pour un BAT dans Workfront et le partager directement à partir de Workfront. Vous pouvez également copier l’URL et la distribuer à l’aide d’une autre méthode.

Avant cette modification, vous ne pouviez copier que le lien du BAT dans Workfront et le distribuer à l’aide d’une autre méthode.

Pour plus d’informations, voir [Partager un BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) dans l’article [ Partager un BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

>[!NOTE]
>
>Le lien d’intégration actuellement disponible sera supprimé dans une version ultérieure. Le lien d’intégration sera toujours accessible via l’API Workfront.

### Rapport sur les données de vérification supplémentaires dans Workfront {#report-on-additional-proofing-data-in-workfront}

Dans les rapports qui contiennent l’objet Version du document (tel qu’un rapport Version du document et un rapport Approbation de BAT), plusieurs champs sont désormais disponibles et vous permettent d’afficher des informations de vérification supplémentaires.

* Échéance de l&#39;épreuve

  Affiche le jour de la semaine, la date, l’heure et l’année de la date limite du BAT.

* Décision concernant l&#39;épreuve

  Affiche l’état de décision du BAT (en attente, modifications requises ou approuvées).

* Nom de l’épreuve

  Affiche le nom du BAT.

* Pages de l&#39;épreuve

  Affiche le nombre de pages incluses dans le BAT.

* Avancement de l&#39;épreuve

  Affiche l’état d’avancement du BAT (Envoyé, Ouvert, Commenté, Décision prise).

Pour plus d’informations sur chacun de ces champs, voir  [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Affichage des données historiques pour les approbations de BAT dans Workfront {#view-historical-data-for-proof-approvals-in-workfront}

Dans le rapport Validation du BAT, vous pouvez ajouter un champ qui permet de visualiser les décisions de validation des BAT pour les BAT qui ne sont plus actifs. Pour ce faire, ajoutez le champ Décision de l’approbateur à votre rapport.

Avant cette modification, une fois qu’une décision a été prise sur un BAT, la décision ne pouvait plus être affichée dans un rapport Workfront.

Pour plus d’informations, voir  [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Améliorations de la vérification dans Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Créer une version d’un bon à tirer directement à partir de la visionneuse de correctifs (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [Nouveau lien Détails du bon à tirer dans la visionneuse de vérification et la visionneuse de vérification de l’appli de bureau (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Création d’une version d’un bon à tirer directement à partir de la visionneuse de correctifs (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

Vous pouvez désormais créer une version d’un BAT directement à partir de la nouvelle visionneuse de vérification et de la visionneuse de vérification de l’appli de bureau lors de la vérification dans Workfront Proof.

Auparavant, cette option était disponible uniquement dans la visionneuse de Flashs héritée.

Pour plus d’informations, voir [Copie de BAT dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) dans l’article  [Copie de BAT dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### Nouveau lien Détails du bon à tirer dans la visionneuse de vérification et la visionneuse de vérification de l’appli de bureau (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

Lors de l’affichage d’un BAT dans la visionneuse de BAT, les utilisateurs de Workfront Proof peuvent désormais accéder rapidement à la page des détails du BAT dans Workfront Proof.

Pour plus d’informations, voir &quot;Affichage des détails du bon à tirer&quot;.
