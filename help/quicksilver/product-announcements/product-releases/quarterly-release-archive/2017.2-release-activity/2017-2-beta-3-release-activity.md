---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.2, version bêta 3
description: Cette page décrit tous les changements disponibles dans l’environnement de prévisualisation avec la version 2017.2 bêta 2. Les fonctionnalités de cette page ont été mises à disposition dans l’environnement de prévisualisation le 24 mai 2017. Elles seront disponibles dans l’environnement de production entre fin juillet et début août 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 100%

---

# Activité Version 2017.2, version bêta 3

Cette page décrit tous les changements disponibles dans l’environnement de prévisualisation avec la version 2017.2 bêta 2. Les fonctionnalités de cette page ont été mises à disposition dans l’environnement de prévisualisation le 24 mai 2017. Elles seront disponibles dans l’environnement de production entre fin juillet et début août 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour une liste de tous les changements apportés avec la version 2017.2, voir [Vue d’ensemble de l’activité de la version 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La version 2017.2 bêta 2 contient des améliorations pour les équipes d’administration de Workfront et les autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices :**

* [Restaurer des éléments en masse à partir de la corbeille](#restoring-items-in-bulk-from-the-recycle-bin)
* [Les informations sur les utilisateurs et utilisatrices sont synchronisées de Workfront vers ProofHQ (ProofHQ et Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**Pour tous les utilisateurs et utilisatrices :** 

* [Afficher les utilisateurs et utilisatrices abonnés](#view-subscribed-users)
* [Configurer l’affichage des jalons sur le graphique de Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Inclure la légende du graphique de Gantt lors de l’export au format PDF](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Afficher les approbations d’épreuve dans la zone Mon travail (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront)
* [Afficher les noms d’utilisateur ou d’utilisatrice lors de la réponse aux demandes d’approbation de relecture à partir de la zone Mon travail (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Amélioration de la visionneuse de relecture pour les épreuves vidéo (ProofHQ et Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Afficher les épreuves pour les médias riches dans d’autres résolutions (ProofHQ et Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Nouvel objet « Créateur ou créatrice de l’épreuve » dans le rapport Version du document (Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Nouvelle fonctionnalité Groupe de ressources temporairement supprimée de la prévisualisation](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Restauration d’éléments en bloc à partir de la corbeille {#restoring-items-in-bulk-from-the-recycle-bin}

Vous pouvez désormais restaurer jusqu’à 10 projets, tâches, problèmes ou documents supprimés à la fois.

Avant cette modification, vous pouviez restaurer un seul élément supprimé à la fois.

Pour plus d’informations sur la restauration d’éléments, voir [Restaurer des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Afficher les utilisateurs et utilisatrices abonnés {#view-subscribed-users}

Vous pouvez maintenant voir qui s’abonne à un élément en développant le nombre de personnes abonnées qui s’affiche en regard du lien d’abonnement.

Avant cette amélioration, vous n’aviez aucune visibilité sur l’identité des personnes abonnées aux éléments.

Pour plus d’informations sur l’abonnement aux éléments, voir [S’abonner aux éléments dans Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md).

## Configurer l’affichage des jalons sur le graphique de Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Il existe désormais deux options pour afficher les informations sur les jalons dans un graphique de Gantt. Vous pouvez configurer l’un des indicateurs de jalon suivants, ou les deux :

* Losanges de jalons (icône)

  Cette icône s’affiche dans le graphique de Gantt après toute tâche associée à un jalon.

* Lignes de jalons

  Une ligne s’affiche après toute tâche associée au jalon, couvrant toutes les tâches du graphique de Gantt.

Avant cette modification, il n’existait qu’une seule option pour permettre l’affichage des jalons dans un graphique de Gantt, appelée « Jalons ». Cette option permet d’activer à la fois l’icône de losange de jalon et la ligne de jalon. Ces indicateurs ne pouvaient pas être séparés.

Pour plus d’informations sur la configuration de l’affichage des informations dans le graphique de Gantt, voir [Configurer l’affichage des informations sur le graphique de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Inclure la légende du graphique de Gantt lors de l’export au format PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Lorsque vous exportez le graphique de Gantt au format PDF, vous pouvez maintenant choisir d’exporter également la légende du graphique avec le graphique lui-même. Les éléments inclus dans la légende ne sont que les options que vous avez activées pour qu’elles s’affichent dans le graphique de Gantt de l’IU. Ces options sont incluses dans la légende si elles existent sur les tâches du projet. Par exemple, si vous activez l’affichage des jalons dans le graphique de Gantt, la légende les affiche également, mais uniquement si au moins une tâche est associée à un jalon.

Avant cette modification, vous ne pouviez pas exclure la légende du PDF exporté. La légende incluait toutes les options et tous les marqueurs possibles du graphique de Gantt, qu’ils aient été activés ou qu’ils existent ou non dans l’IU.

Pour plus d’informations sur l’export du graphique de Gantt, voir [Exporter le graphique de Gantt au format PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Les informations sur les utilisateurs et utilisatrices sont synchronisées de Workfront vers ProofHQ (ProofHQ et Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

Les informations sur les utilisateurs et utilisatrices (nom et e-mail) sont désormais synchronisées de Workfront vers ProofHQ lors de la création ou de la mise à jour d’utilisateurs et utilisatrices dans Workfront. 

Les sections suivantes fournissent plus d’informations sur la synchronisation des utilisateurs et utilisatrices de Workfront vers ProofHQ.

## Nouvel objet « Créateur ou créatrice de l’épreuve » dans le rapport Version du document (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Désormais, lors de la création d’un rapport Version du document, un nouvel objet Créateur ou créatrice de l’épreuve est disponible. Cet objet permet de créer un rapport sur les informations concernant l’utilisateur ou l’utilisatrice ayant créé l’épreuve. 

Le nouvel objet Créateur ou créatrice de l’épreuve du rapport Version du document contient tous les champs disponibles avec l’objet Utilisateur existant ou utilisatrice existante dans d’autres types de rapports d’objet.

>[!NOTE]
>
>Ces informations ne sont disponibles dans le rapport qu’à partir du moment où cette fonctionnalité a été introduite pour la première fois dans les environnements de prévisualisation ou de production respectifs ; les informations contenues dans les rapports concernant l’objet Demande avant l’introduction de cette fonctionnalité ne sont pas disponibles.

Vous accédez à l’objet Créateur ou créatrice de l’épreuve lors de la création d’un rapport Version du document, comme décrit dans la section [Créer un rapport personnalisé](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur le rapport d’objet Version du document, consultez la section [Comprendre les objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) dans [Comprendre les objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Afficher les approbations d’épreuve dans la zone Mon travail (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Toutes les approbations d’épreuve que vous avez soumises pour approbation sont désormais affichées dans la zone Mon travail, dans l’onglet **Travail que j’ai envoyé pour approbation**.

Avant cette modification, l’onglet **Travail que j’ai envoyé pour approbation** n’incluait pas les approbations d’épreuve.

Les approbations d’épreuve ne s’affichent que lorsque les critères suivants sont remplis :

* L’approbation a actuellement le statut Approbation en attente.
* Le processus d’approbation est affecté à un utilisateur ou une utilisatrice qui est un utilisateur ou une utilisatrice Workfront sous licence (les processus d’approbation affectés à des utilisateurs et utilisatrices qui ne sont pas des utilisateurs et utilisatrices Workfront sous licence ne s’affichent pas).
* Les processus d’approbation ont été lancés après la publication de cette fonctionnalité (les processus d’approbation initiés avant ne s’affichent pas).

Pour plus d’informations, consultez la section [Afficher les approbations](../../../../review-and-approve-work/manage-approvals/view-approvals.md) dans [Afficher les approbations](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Afficher les noms d’utilisateur ou d’utilisatrice lors de la réponse aux demandes d’approbation de relecture à partir de la zone Mon travail (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Désormais, lorsque vous approuvez les approbations de relecture dans la zone Mon travail, le nom de l’utilisateur ou de l’utilisatrice qui a demandé l’approbation s’affiche.

Pour plus d’informations, consultez la section [Approuver du travail](../../../../review-and-approve-work/manage-approvals/approving-work.md) dans [Approuver du travail](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Amélioration de la visionneuse de relecture pour les épreuves vidéo (ProofHQ et Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

La visionneuse de relecture dans Workfront et dans ProofHQ a été mise à jour avec un nouvel aspect, une architecture HTML5 pour de meilleures performances et une prise en charge des nouvelles fonctionnalités.

La nouvelle visionneuse de relecture contient les améliorations suivantes :

* Relecture image par image
* Mise en mémoire tampon de la vidéo
* Fonctionnalité de recherche dans la liste des commentaires
* Toutes les actions définies dans le commentaire s’affichent dans chaque commentaire de la liste des commentaires.
* Mode Plein écran
* Réviser le contenu plus rapidement ou plus lentement
* Vérificateur orthographique lors de l’ajout de commentaires et de réponses

### Aperçu

La nouvelle visionneuse de relecture est disponible en phase de test dans les environnements de prévisualisation suivants :

* Environnement de prévisualisation de ProofHQ

  Pour plus d’informations sur l’environnement de prévisualisation de ProofHQ, consultez la section [Environnement de test de prévisualisation de sandbox - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Environnement de prévisualisation de Workfront, lorsque votre compte est activé avec la relecture.

  Pour plus d’informations sur l’environnement de prévisualisation de Workfront, consultez la section [Environnement de prévisualisation de sandbox - Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

Dans cette version, la nouvelle visionneuse de relecture prend uniquement en charge la relecture vidéo. Cela signifie que toutes les épreuves vidéo utilisent la nouvelle visionneuse de relecture, tandis que toutes les épreuves statiques et de médias riches continuent d’utiliser la visionneuse de relecture existante.

### Production

Une fois publiée dans l’environnement de production avec la version 17.2, l’administration peut choisir quelle visionneuse de relecture, nouvelle ou héritée, convient aux utilisateurs et utilisatrices de leur entreprise. Par défaut, la visionneuse de relecture héritée sera utilisée.

Pour plus d’informations sur l’utilisation de la nouvelle visionneuse de relecture vidéo, voir

## Afficher les épreuves pour les médias riches dans d’autres résolutions (ProofHQ et Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

Vous pouvez désormais ajuster la résolution des épreuves pour les médias riches en spécifiant une résolution personnalisée ou en faisant glisser l’image vers la résolution souhaitée.

Avant cette modification, vous pouviez passer en revue les épreuves à l’aide de la résolution inhérente à l’écran ou à l’appareil sur lequel vous visionniez le contenu.

Vous pouvez utiliser le mode Comparer pour comparer différentes résolutions d’épreuves.

Pour plus d’informations, consultez la section [Ouvrir des épreuves dans la visionneuse de relecture de bureau](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md).

## Nouvelle fonctionnalité Groupe de ressources temporairement supprimée de la prévisualisation {#new-resource-pool-functionality-temporarily-removed-from-preview}

En raison de problèmes de développement, nous avons décidé de supprimer le nouvel onglet Planification des ressources et de renommer l’onglet Planification des ressources héritée en son nom d’origine « Planification des ressources ».

La nouvelle fonctionnalité des groupes de ressources a également été supprimée avec cette modification. Le nouvel onglet Planification des ressources et les fonctionnalités des groupes de ressources retourneront à l’environnement sandbox de prévisualisation à la fin du mois de juin 2017.
