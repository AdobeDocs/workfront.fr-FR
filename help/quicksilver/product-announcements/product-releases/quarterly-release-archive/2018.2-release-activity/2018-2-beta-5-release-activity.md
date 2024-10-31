---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.2 bêta 5
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version 2018.2 bêta 5. La fonctionnalité sera disponible dans l’environnement de prévisualisation le 1er août 2018. Les améliorations de la relecture avec la version bêta 5 seront disponibles dans l’environnement de prévisulation le lundi 4 juin. Elles seront disponibles dans l’environnement de production en juillet 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: 099d42ea0a09d8190a79893c4cbd8d7d8b674acd
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 100%

---

# Activité Version 2018.2 bêta 5

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version 2018.2 bêta 5.La fonctionnalité sera disponible dans l’environnement de prévisualisation le 1er juin 2018.Les améliorations de relecture avec la version bêta 5 seront disponibles dans l’environnement de prévisualisation le lundi 4 juin. Elles seront disponibles dans l’environnement de production en juillet 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.2, voir [Vue d’ensemble de l’activité Version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La version 2018.2 bêta 5 contient les améliorations apportées aux administrateurs et administratrices de Workfront, ainsi qu’aux autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices**

* [Affichage des modifications déclenchées par l’utilisateur ou l’utilisatrice avec les journaux d’audit](#view-user-triggered-changes-with-audit-logs)
* [Affichage des informations de licence en tant qu’administrateur ou administratrice de groupes](#view-license-information-as-a-group-administrator)

**Pour tous les utilisateurs et utilisatrices**

* [Vue Calendrier dans la zone d’accueil](#calendar-view-in-the-home-area)
* [Mises à jour supplémentaires de la liste de travail (panneau de gauche) dans la page d’accueil](#additional-updates-to-the-work-list-left-panel-in-home)
* [Configuration des limites de fonction pour la planification automatisée des ressources](#configure-job-role-limits-for-automated-resource-scheduling)
* [Améliorations des vues Projet et Rôle dans le planificateur de ressources](#project-and-role-view-improvements-in-the-resource-planner)
* [Redimensionnement de la largeur des colonnes pour les listes de projets](#resize-column-widths-for-project-lists)
* [Prise en charge des icônes pour les nouvelles listes de projets](#icon-support-for-the-new-project-lists)
* [Ajout d’un champ « Grande miniature » dans les vues de document](#add-large-thumbnail-field-in-document-views)
* [Augmentation de la limite d’export Excel](#increase-excel-export-limit)
* [Filtres rapides pour les listes de projets](#quick-filters-for-project-lists)
* [Collections de problèmes de référence dans les rapports de projet et de tâche](#reference-issue-collections-in-project-and-task-reports)
* [Nouveau menu de version plus robuste lors de l’ajout de nouvelles versions de document dans Workfront](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Améliorations mobiles dans la version bêta de l’application mobile Android](#mobile-improvements-in-the-android-beta-mobile-app)
* [Améliorations apportées à la visionneuse de relecture (Workfront et Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Améliorations de la relecture dans Workfront](#proofing-enhancements-in-workfront)
* [Améliorations de la relecture dans Workfront Proof](#proofing-enhancements-in-workfront-proof)

## Vue Calendrier dans la zone d’accueil {#calendar-view-in-the-home-area}

Vous pouvez désormais gérer vos tâches et plannings personnels à l’aide de la vue Calendrier de l’accueil de Workfront. La vue Calendrier de l’accueil vous permet d’effectuer les opérations suivantes :

* Définir votre propre planning pour accomplir les tâches Workfront qui vous sont affectées.
* Afficher rapidement les tâches qui sont en retard ou qui le seront bientôt.
* Afficher le total des heures allouées pour une semaine.
* Effectuer des mises à jour des tâches qui vous sont affectées.

Si vous utilisez un calendrier dans Outlook, vous pouvez intégrer votre calendrier pour afficher vos événements Outlook dans la vue Calendrier de l’accueil.

## Mises à jour supplémentaires de la liste de travail (panneau de gauche) dans la page d’accueil {#additional-updates-to-the-work-list-left-panel-in-home}

Les améliorations suivantes ont été apportées à la liste de tâches dans la zone Accueil :

* Le nombre d’éléments terminés s’affiche désormais entre parenthèses en regard de l’option Terminé dans le menu déroulant Filtre.

  Auparavant, le nombre d’éléments terminés ne s’affichait pas dans le menu Filtre. 

* Les éléments terminés sont affichés pour les deux semaines précédentes.

  Auparavant, les éléments terminés étaient affichés pour les trois mois précédents.

  Pour plus d’informations sur l’affichage du travail terminé dans la zone Accueil, voir [Afficher des éléments dans la liste de travail de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) dans l’article [Afficher des éléments dans la liste de travail de la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Ajoutez les champs Durée et Affectations à afficher lorsque des éléments sont sélectionnés dans la zone Accueil.

  Auparavant, le champ Affectations était disponible par défaut. Cependant, s’il était supprimé, il ne pouvait pas être ajouté à nouveau. Le champ Durée n’était pas disponible auparavant pour l’ajout.

  Pour plus d’informations sur l’ajout de champs à la zone Accueil, voir « Créer et gérer des modèles de disposition ».

Pour plus d’informations sur l’utilisation de la zone Accueil, voir [Utiliser la zone Accueil](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Afficher les modifications déclenchées par un utilisateur ou une utilisatrice avec les journaux d’audit {#view-user-triggered-changes-with-audit-logs}

Nous avons créé les journaux d’audit suivants pour les administrateurs et administratrices Workfront afin de suivre les modifications déclenchées par un utilisateur ou une utilisatrice :

* Journal d’audit de l’utilisateur ou utilisatrice
* Journal d’audit du niveau d’accès
* Journaux d’audit de groupe
* Journaux d’audit des tentatives de connexion

Auparavant, il n’était pas possible de suivre les modifications dans le système.

Pour plus d’informations, voir [Afficher et exporter des journaux d’audit](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Affichage des informations de licence en tant qu’administrateur ou administratrice de groupes {#view-license-information-as-a-group-administrator}

Nous avons créé une page Licences en lecture seule pour permettre aux administrateurs et administratrices de groupes d’afficher le nombre de licences pour les groupes qu’ils ou elles gèrent.

Avant cette modification, les administrateurs et administratrices de groupes ne pouvaient pas afficher les informations de licence.

Pour plus d’informations, voir [Administrateurs et administratrices de groupes](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## Configurer les limites des fonctions pour la planification automatisée des ressources {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Dans les paramètres de planification des ressources automatisée, vous pouvez désormais affecter une limite à une fonction. Cela vous permet de contrôler le nombre de ressources, avec le même rôle, auxquelles un travail est affecté.

Auparavant, vous ne pouviez pas spécifier le nombre de personnes pouvant se voir affecter une tâche au sein d’une fonction donnée.

Pour plus d’informations, voir « Attribuer manuellement des tâches et des problèmes non assignés dans les zones de planification ».

## Améliorations de la vue Projet et Rôle dans le planificateur de ressources {#project-and-role-view-improvements-in-the-resource-planner}

Les vues Projet et Rôle du planificateur de ressources contiennent désormais les améliorations suivantes :

* Amélioration des filtres qui extraient les informations de l’ensemble de la base de données, plutôt que les informations à l’écran seulement.
* Mode Plein écran.
* Les performances sont désormais plus rapides et plus efficaces.

   * Nouvelles limites pour le nombre de projets, de rôles et de personnes que vous pouvez afficher.
   * Chargement différé, pour un chargement plus rapide des projets et des rôles.

* Accès rapide aux projets et aux personnes directement à partir du planificateur de ressources.
* Fonction de glisser-déposer plus rapide dans la vue Projet pour classer vos projets par priorité.

Avant ces améliorations, vous avez signalé que le planificateur de ressources était lent à charger et que les données affichées présentaient des incohérences. Ces problèmes sont à présent résolus grâce à ces améliorations.

Pour plus d’informations et pour comprendre les nouvelles limites du planificateur de ressources, voir [Limites d’affichage du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## Redimensionner la largeur des colonnes pour les listes de projets {#resize-column-widths-for-project-lists}

Comme nous avons travaillé à l’amélioration de la fonctionnalité de nos listes, nous avons temporairement désactivé la capacité de redimensionner les largeurs des colonnes dans les listes de projets suivantes :

* Projets dont je suis propriétaire
* Projets auxquels je participe
* Tous les projets

Avec cette version, nous pouvons à nouveau redimensionner les colonnes de toutes les listes de projets.

Nous avons ajouté d’autres améliorations à cette fonctionnalité.

Désormais, lorsque vous faites glisser la bordure droite d’une colonne pour la redimensionner, la colonne voisine à droite conserve sa taille, ce qui élargit la liste, plutôt que d’être également modifiée. Vous pouvez également faire glisser la bordure d’une colonne vers la droite au-delà des bordures des colonnes voisines.

Avant cette amélioration, la colonne voisine à droite de la colonne redimensionnée était également redimensionnée proportionnellement pour s’adapter à l’écran. Vous ne pouviez pas faire glisser la bordure d’une colonne le long de la bordure droite de la colonne voisine.  

Pour plus d’informations sur le redimensionnement des colonnes de réorganisation dans les listes, voir [Modifier la largeur et l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Pour participer à notre programme de test bêta pour connaître les améliorations apportées à la liste actuelle, voir [Étude sur les nouvelles listes.](http://community.workfront.com/discussions/community-home/digestviewer/viewthread?GroupId=457&amp;MessageKey=6b135c15-33dd-4fa2-8bc3-7cd7f7740c57&amp;CommunityKey=0425cafc-f0ec-47fc-be20-a21dc073d520&amp;tab=digestviewer&amp;ReturnUrl=%2fdiscussions%2fcommunity-home%2fdigestviewer%3fCommunityKey%3d0425cafc-f0ec-47fc-be20-a21dc073d520) (connexion obligatoire)

## Prise en charge des icônes pour les nouvelles listes de projets {#icon-support-for-the-new-project-lists}

Comme nous nous efforçons d’améliorer la fonctionnalité de nos listes, nous avions temporairement désactivé l’affichage des icônes de statut dans les listes de projets suivantes :

* Projets dont je suis propriétaire
* Projets auxquels je participe
* Tous les projets

Avec cette version, les icônes de statut peuvent s’afficher à nouveau dans vos listes de projets pour les projets ou d’autres objets dans une liste de projets.

Pour plus d’informations sur l’utilisation des listes, voir [Commencer avec les listes dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Ajout d’un champ « Grande miniature » dans les vues de document {#add-large-thumbnail-field-in-document-views}

Nous ajoutons un nouveau champ appelé Grande miniature à une vue de document dans une liste ou un rapport. Lorsqu’il est sélectionné dans une vue de document, ce champ affiche une miniature de 400 pixels de large pour le document dans une liste ou un rapport.

Avant cette modification, vous ne pouviez ajouter que le champ Miniature à une vue de document, qui affiche une miniature de 33 à 66 pixels pour le document.

Pour plus d’informations sur les champs des listes et des rapports, voir [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Augmentation de la limite d’export Excel {#increase-excel-export-limit}

Nous avons augmenté la limite du nombre de lignes pouvant être exportées dans un fichier Excel. Vous pouvez désormais exporter les éléments suivants :

* 65 000 lignes dans un fichier Excel .xls
* 100 000 lignes dans un fichier Excel .xlsx

Les nouvelles limites s’appliquent lorsque vous exportez les éléments suivants depuis Workfront :

* Liste ou rapport à partir de l’interface web
* Liste ou rapport à l’aide de l’API
* Rapport planifié et remis

Avant cette amélioration, vous ne pouviez exporter que 50 000 lignes dans n’importe quel fichier Excel.

Pour plus d’informations sur l’export de données à partir de Workfront, voir [Exporter des données](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Filtres rapides pour les listes de projets {#quick-filters-for-project-lists}

Vous pouvez maintenant appliquer un filtre rapide aux listes.

L’objectif d’un filtre rapide est de vous aider à accéder directement aux éléments de vos listes volumineuses qui vous intéressent, afin que vous puissiez rapidement les examiner, les mettre à jour ou les partager avec d’autres personnes.

Actuellement, les filtres rapides ne sont disponibles que pour les listes de projets dans les sous-onglets suivants :

* Projets auxquels je participe
* Projets dont je suis propriétaire
* Tous les projets

Pour plus d’informations sur les filtres rapides, voir la section « Application de filtres rapides aux listes » dans [Commencer avec les listes dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Référencer des collections de problèmes dans les rapports de projet et de tâche {#reference-issue-collections-in-project-and-task-reports}

Vous pouvez désormais référencer une collection de problèmes dans une vue de projet ou de tâche et les filtrer. Vous pouvez le faire uniquement à l’aide du mode Texte lors de la création d’un rapport.

Avant cette amélioration, vous ne pouviez référencer qu’une collection de tâches dans une vue de projet ou un filtre.

Pour plus d’informations sur la manière de référencer une collection dans un rapport, voir [Référencer des collections dans un rapport](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

Pour plus d’informations sur l’utilisation du mode texte, voir [Vue d’ensemble des utilisations courantes du mode Texte](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

>[!NOTE]
>
>Dans la vidéo suivante, l’exemple de mode texte pour les collections de problèmes était incorrect. L’exemple de mode texte correct est disponible dans [Référencer des collections dans un rapport](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

## Nouveau menu de version plus robuste lors de l’ajout de nouvelles versions de document dans Workfront {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Désormais, lors de l’ajout de nouvelles versions aux documents dans Workfront, le menu Nouvelle version contient des options supplémentaires et est désormais cohérent dans toutes les zones de Workfront où vous pouvez ajouter une nouvelle version.

Vous pouvez ajouter une nouvelle version de document à partir des zones suivantes de Workfront :

* Dans le menu déroulant Plus de l’onglet Documents.
* Dans le menu Actions du document de la page Détails du document.
* Dans l’onglet Toutes les versions de la page de détails du document.

Avant cette modification, seul le menu déroulant Plus de l’onglet Documents contenait toutes les options pour ajouter une nouvelle version.

Les options suivantes sont désormais disponibles dans le menu Nouvelle version pour toutes les zones où vous pouvez ajouter une nouvelle version :

* Épreuve
* Document uniquement
* Options liées (de Dropbox, de Google Drive, etc.)
* Coller à partir du presse-papiers (nouvelle option disponible lors de l’ajout de versions)

Pour plus d’informations, voir la section [Ajouter des documents à Adobe Workfront à partir de votre système de fichiers](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) dans l’article [Ajouter des documents à Adobe Workfront à partir de votre système de fichiers](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

## Améliorations mobiles apportées à la version bêta de l’application mobile Android {#mobile-improvements-in-the-android-beta-mobile-app}

Les améliorations suivantes seront disponibles dans la version bêta de l’application mobile Android peu après le jour de la sortie de cette version :

* Actions de glissement

  Vous pouvez exécuter des activités telles que vous porter volontaire pour travailler sur une tâche, terminer une tâche, marquer une notification comme vue ou nouvelle, envoyer un message texte ou appeler un contact en faisant glisser divers objets dans l’application mobile Workfront.

  Les zones suivantes ont été améliorées avec cette fonctionnalité :

   * Mon travail et Accueil
   * Notifications
   * Contacts
   * Approbations

* Nouvelle apparence lors de l’affichage de l’onglet Détails d’un élément

  L’interface a été modifiée lors de l’affichage d’un élément dans la version bêta de l’application mobile Android afin de faciliter sa modification, son remplissage ou l’adjonction d’une pièce jointe.

* Nouvelle expérience lors de la consignation du temps

  La consignation du temps est plus rapide et plus facile qu’auparavant. Le bouton Consigner le temps est plus facile d’accès et l’interface est rationalisée pour consigner les heures.

Avec cette version, ces améliorations ne sont disponibles que pour la version bêta de l’application mobile Android de Workfront. Elles ne sont actuellement pas disponibles pour iOS.

Pour plus d’informations sur l’inscription à la phase de test bêta et le téléchargement de la version bêta de l’application mobile Android de Workfront, voir la section correspondante.

## Améliorations de la visionneuse de relecture (Workfront et Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [Page Résumé de l’impression mise à jour](#updated-print-summary-page)
* [Ajouter des utilisateurs et utilisatrices à une épreuve, directement à partir de la visionneuse de relecture](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [Afficher tous les outils d’annotation dans la visionneuse de relecture](#display-all-markup-tools-in-the-proofing-viewer)
* [Configurer les options de tri par défaut dans la visionneuse de relecture](#configure-default-sorting-options-in-the-proofing-viewer)
* [Afficher les approbations de documents Workfront dans la visionneuse de relecture de bureau](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [Configurer des liens qui ouvrent de nouveaux onglets et fenêtres pour qu’ils s’ouvrent dans la visionneuse de relecture de l’application de bureau.](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [Indicateur de présence dans la visionneuse de relecture](#presence-indicator-in-the-proofing-viewer)
* [Filtrer les commentaires pour afficher une seule page pour les épreuves d’URL interactives dans la visionneuse de relecture de l’application de bureau](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [Visionneuse de relecture de l’application de bureau pour le contenu statique et vidéo](#desktop-proofing-viewer-for-static-and-video-content)
* [Ajouter des périphériques personnalisés à votre système](#add-custom-devices-to-your-system)

### Page Résumé de l’impression mise à jour {#updated-print-summary-page}

La page Résumé de l’impression a été mise à jour et présente un nouvel aspect et des fonctionnalités améliorées.

Pour plus d’informations, voir la section [Imprimer un résumé de l’épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Ajouter des utilisateurs et utilisatrices à une épreuve directement à partir de la visionneuse de relecture {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Vous pouvez désormais ajouter des utilisateurs et utilisatrices à une épreuve directement à partir de la visionneuse de relecture web et de la visionneuse de relecture de l’application de bureau. 

Auparavant, il n’était pas possible d’ajouter des personnes à une épreuve. Vous pouviez uniquement copier l’URL publique ou le code intégré.

Pour plus d’informations, voir la section [Partager une épreuve en y ajoutant des personnes](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) dans l’article [Partager une épreuve à partir de la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

### Afficher tous les outils d’annotation dans la visionneuse de relecture {#display-all-markup-tools-in-the-proofing-viewer}

Vous pouvez maintenant configurer l’outil d’annotation pour qu’il reste affiché en continu, plutôt que dans un menu que vous devez ouvrir. Cela permet de basculer plus rapidement entre les outils. Lorsqu’ils sont configurés de cette manière, les outils d’annotation s’affichent horizontalement en haut de la visionneuse de relecture web et de la visionneuse de relecture de l’application de bureau.

Auparavant, les outils d’annotation n’étaient disponibles que dans un menu déroulant.

Pour plus d’informations sur la configuration de ce paramètre d’annotation, voir la section [Configurer des paramètres de la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Pour plus d’informations sur l’utilisation des options d’annotation lors de la révision d’une épreuve, voir l’article .

### Configurer des options de tri par défaut dans la visionneuse de relecture {#configure-default-sorting-options-in-the-proofing-viewer}

Désormais, lorsque vous modifiez l’option de tri dans la liste de commentaires d’une épreuve, cette option devient l’option de tri par défaut lors de la prochaine ouverture d’une épreuve dans la visionneuse de relecture web ou la visionneuse de relecture de l’application de bureau. 

Pour plus d’informations, voir l’article .

### Afficher les approbations de documents Workfront dans la visionneuse de relecture de bureau {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Vous pouvez désormais prendre des décisions concernant l’approbation de documents Workfront dans la visionneuse de relecture de bureau.

Auparavant, seule la visionneuse de relecture web vous permettait de prendre des décisions sur l’approbation de documents Workfront. 

Pour plus d’informations, voir [Prendre une décision concernant une épreuve dans la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) dans l’article [Prendre une décision concernant une épreuve dans la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

### Configurer des liens qui ouvrent de nouveaux onglets et fenêtres pour qu’ils s’ouvrent dans la visionneuse de relecture de bureau. {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

Pour la relecture du contenu interactif dans la visionneuse de relecture de bureau, vous pouvez désormais configurer les liens qui s’ouvrent dans un nouvel onglet ou une nouvelle fenêtre pour qu’ils s’ouvrent dans la visionneuse de relecture de bureau afin de pouvoir continuer la relecture.

Dans l’ancienne visionneuse de relecture, les liens ouverts dans un nouvel onglet ou une nouvelle fenêtre ne pouvaient pas être révisés dans la visionneuse de relecture.

Pour plus d’informations, voir [Configurer les paramètres de la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

### Indicateur de présence dans la visionneuse de relecture {#presence-indicator-in-the-proofing-viewer}

Désormais, lorsque vous révisez une épreuve dans la visionneuse de relecture web ou la visionneuse de relecture de bureau, l’avatar des utilisateurs et utilisatrices qui consultent actuellement l’épreuve s’affiche dans le coin supérieur droit de la visionneuse de relecture.

Pour plus d’informations, voir [Réviser une épreuve simultanément avec plusieurs réviseurs et réviseuses](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md).

### Filtrer les commentaires pour afficher une seule page pour les épreuves d’URL interactives dans la visionneuse de relecture de bureau {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

Lors de la révision d’une URL dans une épreuve interactive dans la visionneuse de relecture de bureau, vous pouvez désormais filtrer les commentaires afin d’afficher uniquement ceux qui concernent la page active. 

Avant cette modification, cette option était disponible uniquement pour les épreuves statiques.

Pour plus d’informations, voir l’article .

### Visionneuse de relecture de bureau pour le contenu statique et vidéo {#desktop-proofing-viewer-for-static-and-video-content}

La visionneuse de relecture de bureau prend désormais en charge le contenu statique et vidéo.

Auparavant, elle ne prenait en charge que le contenu interactif.

Pour plus d’informations sur la configuration d’épreuves vidéos et statiques pour les ouvrir dans la visionneuse de relecture de bureau, voir [Configurer les paramètres de la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

Pour plus d’informations sur la visionneuse de relecture de bureau, voir [Réviser des épreuves dans la visionneuse de relecture de bureau.](https://support.workfront.com/hc/fr-fr/sections/360000686434)

### Ajouter des appareils personnalisés à votre système {#add-custom-devices-to-your-system}

Vous pouvez désormais ajouter des appareils personnalisés à votre système, ce qui permet aux utilisateurs et utilisatrices de réviser le contenu interactif et de simuler son rendu sur un appareil spécifique lors de la révision d’une épreuve dans la visionneuse de relecture de bureau.

Avant cette modification, les utilisateurs et utilisatrices pouvaient choisir uniquement parmi une liste d’appareils standard préconfigurés.

Pour plus d’informations sur l’ajout d’appareils personnalisés, voir

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent sélectionner des appareils lors de la révision de contenu interactif, voir [Modifier la résolution de l’épreuve interactive dans la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Améliorations de la relecture dans Workfront {#proofing-enhancements-in-workfront}

* [Partager le lien de l’épreuve directement à partir de Workfront](#share-the-proof-link-directly-from-workfront)
* [Générer des rapports sur les données de relecture supplémentaires dans Workfront](#report-on-additional-proofing-data-in-workfront)
* [Afficher les données historiques pour les approbations d’épreuves dans Workfront](#view-historical-data-for-proof-approvals-in-workfront)

### Partager le lien de l’épreuve directement à partir de Workfront {#share-the-proof-link-directly-from-workfront}

Vous pouvez désormais générer un lien pour une épreuve dans Workfront et le partager directement à partir de Workfront. Vous pouvez également copier l’URL et la distribuer à l’aide d’une autre méthode.

Avant cette modification, vous ne pouviez copier que le lien de l’épreuve dans Workfront et le distribuer à l’aide d’une autre méthode.

Pour plus d’informations, voir [Partager une épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) dans l’article [Partager une épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

>[!NOTE]
>
>Le lien intégré actuellement disponible sera supprimé dans une version ultérieure. Le lien intégré sera toujours accessible via l’API Workfront.

### Générer des rapports sur les données de relecture supplémentaires dans Workfront {#report-on-additional-proofing-data-in-workfront}

Dans les rapports qui contiennent l’objet Version du document (tel qu’un rapport Version du document et un rapport Approbation d’épreuve), plusieurs champs sont désormais disponibles et vous permettent d’afficher des informations de relecture supplémentaires.

* Échéance de l&#39;épreuve

  Affiche le jour de la semaine, la date, l’heure et l’année de la date d’échéance pour la relecture.

* Décision concernant l&#39;épreuve

  Affiche le statut de la décision concernant l’épreuve (En attente, Modifications requises ou Approuvée).

* Nom de l’épreuve

  Affiche le nom de l’épreuve.

* Pages de l&#39;épreuve

  Affiche le nombre de pages incluses dans l’épreuve.

* Avancement de l&#39;épreuve

  Affiche le statut de la progression de l’épreuve (Envoyé, Ouvert, Commenté, Décision prise).

Pour plus d’informations sur chacun de ces champs, voir [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Affichage des données historiques pour les approbations d’épreuves dans Workfront {#view-historical-data-for-proof-approvals-in-workfront}

Dans le rapport d’approbation d‘épreuves, vous pouvez ajouter un champ qui permet d’afficher les décisions d’approbation des épreuves pour les épreuves qui ne sont plus actives. Pour ce faire, ajoutez le champ Décision de l’approbateur ou de l’approbatrice à votre rapport.

Avant cette modification, une fois qu’une décision avait été prise sur une épreuve, la décision ne pouvait plus être affichée dans un rapport Workfront.

Pour plus d’informations, voir [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Améliorations de la relecture dans Workfront Proof {#proofing-enhancements-in-workfront-proof}

* [Créer une version d’une épreuve directement à partir de la visionneuse de relecture (Workfront Proof)](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [Nouveau lien Détails de l’épreuve dans la visionneuse de relecture et la visionneuse de relecture de bureau (Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### Créer une version d’une épreuve directement à partir de la visionneuse de relecture (Workfront Proof) {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

Vous pouvez désormais créer une version d’une épreuve directement à partir de la nouvelle visionneuse de relecture et de la visionneuse de relecture de bureau lors de la relecture dans Workfront Proof.

Auparavant, cette option était disponible uniquement dans la visionneuse Flash héritée.

Pour plus d’informations, voir [Copie d’épreuves dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) dans l’article [Copie d’épreuves dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md).

### Nouveau lien Détails de l’épreuve dans la visionneuse de relecture et la visionneuse de relecture de bureau (Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

Lors de l’affichage d’une épreuve dans la visionneuse de relecture, les utilisateurs et les utilisatrices de Workfront Proof peuvent désormais accéder rapidement à la page des détails de l’épreuve dans Workfront Proof.

Pour plus d’informations, voir « Affichage des détails des épreuves ».
