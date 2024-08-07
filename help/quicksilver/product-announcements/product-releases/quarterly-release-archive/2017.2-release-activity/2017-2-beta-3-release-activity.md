---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.2, version bêta 3
description: Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version 2017.2 de Beta 2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 24 mai 2017. Il sera disponible dans l’environnement de production entre fin juillet et début août 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 1%

---

# Activité Version 2017.2, version bêta 3

Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version 2017.2 de Beta 2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 24 mai 2017. Il sera disponible dans l’environnement de production entre fin juillet et début août 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées en 2017.2, consultez la [présentation de l’activité de version 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La version 2017.2 de Beta 2 contient des améliorations tant pour les administrateurs de Workfront que pour d’autres utilisateurs :

**Pour les administrateurs :**

* [Restauration d’éléments en bloc à partir de la Corbeille](#restoring-items-in-bulk-from-the-recycle-bin)
* [Les informations utilisateur sont synchronisées de Workfront vers ProofHQ (ProofHQ et Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**Pour Tous Les Utilisateurs :** 

* [Afficher les utilisateurs abonnés](#view-subscribed-users)
* [Configuration de l’affichage des jalons sur le diagramme de Gantt](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Inclure la légende du graphique de Gantt lors de l’exportation vers PDF](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [Afficher les validations de BAT dans ma zone de travail (Workfront)](#view-proof-approvals-in-the-my-work-area-workfront)
* [ Afficher les noms d’utilisateur lors de la réponse aux demandes d’approbation de vérification à partir de ma zone de travail (Workfront)](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [Visionneuse de vérification améliorée pour les BAT vidéo (BATHQ et Workfront)](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [Affichage de BAT de médias riches dans d’autres résolutions (ProofHQ et Workfront)](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [Nouvel objet &#39;Proof Creator&#39; dans le rapport Version du document (Workfront)](#new-proof-creator-object-in-document-version-report-workfront)
* [Nouvelle fonctionnalité de pool de ressources temporairement supprimée de l’aperçu](#new-resource-pool-functionality-temporarily-removed-from-preview)

## Restauration d’éléments en bloc à partir de la Corbeille {#restoring-items-in-bulk-from-the-recycle-bin}

Vous pouvez désormais restaurer jusqu’à 10 projets, tâches, problèmes ou documents supprimés à la fois.

Avant cette modification, vous pouviez restaurer un seul élément supprimé à la fois.

Pour plus d’informations sur la restauration d’éléments, voir [Restaurer les éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Afficher les utilisateurs abonnés {#view-subscribed-users}

Vous pouvez maintenant voir qui s’abonne à un élément en augmentant le nombre d’abonnés qui s’affiche en regard du lien d’abonnement.

Avant cette amélioration, vous n’aviez aucune visibilité sur le nom des abonnés aux éléments.

Pour plus d’informations sur l’abonnement aux éléments, voir [Abonnement aux éléments dans Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md). 

## Configuration de l’affichage des jalons sur le diagramme de Gantt {#configure-how-milestones-are-displayed-on-the-gantt-chart}

Deux options sont désormais disponibles pour afficher les informations de jalon dans un graphique Gantt. Vous pouvez configurer l’un des indicateurs de jalon suivants, ou les deux :

* Diamants de jalon (icône)

  Cette icône s’affiche dans le diagramme de Gantt après toute tâche associée à un jalon.

* Lignes de jalons

  Une ligne s’affiche après toute tâche associée au jalon, couvrant toutes les tâches du diagramme de Gantt.

Avant cette modification, il n’existait qu’une seule option permettant aux jalons de s’afficher sur un graphique de Gantt, appelé &quot;Jalons&quot;. Cette option a activé l’icône représentant un jalon et la ligne de jalon. Ces indicateurs n’ont pas pu être séparés.

Pour plus d’informations sur la configuration de l’affichage des informations dans le diagramme de Gantt, voir [Configuration de l’affichage des informations dans le diagramme de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Inclure la légende du diagramme de Gantt lors de l’exportation vers PDF {#include-the-gantt-chart-legend-when-exporting-to-pdf}

Lorsque vous exportez le diagramme de Gantt vers un PDF, vous pouvez maintenant choisir d’exporter également la légende du graphique avec le graphique lui-même. Les éléments inclus dans la légende ne sont que les options que vous avez activées pour être affichées dans le diagramme de Gantt de l’interface utilisateur. Ces options sont incluses dans la légende si elles existent sur les tâches du projet. Par exemple, si vous activez l’affichage des jalons dans le diagramme de Gantt, la légende les affiche également, mais uniquement si au moins une tâche est associée à un jalon.

Avant cette modification, vous ne pouviez pas exclure la légende du PDF exporté. La légende incluait toutes les options et marqueurs possibles du Gantt, qu’ils aient été activés ou qu’ils existent dans l’interface utilisateur.

Pour plus d’informations sur l’exportation du diagramme de Gantt, voir [Export du graphique de Gantt vers PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Les informations utilisateur sont synchronisées de Workfront vers ProofHQ (ProofHQ et Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

Les informations sur les utilisateurs (nom et adresse électronique) sont désormais synchronisées de Workfront vers BATHQ lorsque les utilisateurs sont créés ou mis à jour dans Workfront. 

Pour plus d’informations sur la synchronisation des utilisateurs de Workfront vers ProofHQ , voir .

## Nouvel objet &quot;Créateur de BAT&quot; dans le rapport Version du document (Workfront)

{#new-proof-creator-object-in-document-version-report-workfront}

Désormais, lors de la création d’un rapport Version du document, un nouvel objet Créateur de BAT est disponible. Cet objet permet de créer un rapport sur les informations concernant l&#39;utilisateur qui a créé le BAT. 

Le nouvel objet Créateur de BAT du rapport Version du document contient tous les champs disponibles avec l’objet Utilisateur existant dans d’autres types de rapports d’objet.

>[!NOTE]
>
> Ces informations ne sont disponibles dans le rapport qu’à partir du moment où cette fonctionnalité a été introduite pour la première fois dans les environnements de prévisualisation ou de production respectifs ; les informations contenues dans les rapports concernant l’objet Requester avant l’introduction de cette fonctionnalité ne sont pas disponibles.

Vous accédez à l’objet Créateur de BAT lors de la création d’un rapport Version du document, comme décrit dans la section [Création d’un rapport personnalisé](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur le rapport d’objet Version du document, reportez-vous à la section [Comprendre les objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) de la section [Comprendre les objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Affichage des validations de BAT dans la zone de travail Mes (Workfront) {#view-proof-approvals-in-the-my-work-area-workfront}

Toutes les validations de BAT que vous avez soumises pour approbation sont désormais affichées dans la zone Mon travail, dans l’onglet **Travail que j’ai envoyé pour approbation** .

Avant cette modification, l’onglet **Travail que j’ai envoyé pour approbation** n’incluait pas les validations de BAT.

Les validations de BAT ne s&#39;affichent que lorsque les critères suivants sont remplis :

* La validation est actuellement en attente d’approbation
* Le processus d’approbation est attribué à un utilisateur qui est un utilisateur Workfront sous licence (les processus d’approbation attribués à des utilisateurs qui ne sont pas des utilisateurs Workfront sous licence ne s’affichent pas).
* Les processus d’approbation ont été lancés après la publication de cette fonctionnalité (les processus d’approbation initiés avant la publication de cette fonctionnalité ne s’affichent pas).

Pour plus d’informations, voir [Afficher les approbations](../../../../review-and-approve-work/manage-approvals/view-approvals.md) dans [Afficher les approbations](../../../../review-and-approve-work/manage-approvals/view-approvals.md).

## Affichage des noms d’utilisateur lors de la réponse aux demandes d’approbation de vérification à partir de ma zone de travail (Workfront) {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

Désormais, lorsque vous approuvez les validations de vérification dans la zone Mon travail, le nom de l’utilisateur qui a demandé la validation s’affiche.

Pour plus d’informations, voir [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md) dans [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Amélioration de la visionneuse de vérification pour les bons à tirer vidéo (BAT et Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

La visionneuse de vérification de performance dans Workfront et dans ProofHQ est mise à jour avec une nouvelle apparence, une architecture HTML5 pour de meilleures performances et une prise en charge des nouvelles fonctionnalités.

La nouvelle visionneuse de correctifs contient les améliorations suivantes :

* Validation image par image
* Mise en mémoire tampon de la vidéo
* Fonctionnalité de recherche dans la liste des commentaires
* Toutes les actions définies sur le commentaire sont affichées sur chaque commentaire dans la liste des commentaires.
* Mode Plein écran
* Vérifier le contenu plus rapidement ou plus lentement
* Vérificateur orthographique lors de l’ajout de commentaires et de réponses

### Prévisualiser

La nouvelle visionneuse de vérification est disponible pour les tests dans les environnements d’aperçu suivants :

* Environnement d’aperçu de BATHQ

  Pour plus d’informations sur l’environnement d’aperçu de BATHQ, voir [Aperçu de l’environnement de test Sandbox - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

* Environnement de prévisualisation de Workfront, lorsque votre compte est activé avec la vérification

  Pour plus d’informations sur l’environnement Workfront Preview, voir  [Environnement Adobe Workfront Preview Sandbox](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

Dans cette version, la nouvelle visionneuse de vérification prend uniquement en charge la vérification vidéo. Cela signifie que tous les bons à tirer de la nouvelle visionneuse de correctifs vidéo, tandis que tous les bons à tirer statiques et multimédias enrichis continuent d’exploiter la visionneuse de correctifs existante.

### Production

Lorsqu’elles sont publiées dans l’environnement de production avec la version 17.2, les administrateurs peuvent choisir si la visionneuse de vérification de la version nouvelle ou héritée convient aux utilisateurs de leur entreprise. Par défaut, la visionneuse de vérification héritée sera utilisée.

Pour plus d’informations sur l’utilisation de la nouvelle visionneuse de vérification vidéo, voir  

## Affichage des bons à tirer pour les médias riches dans d’autres résolutions (BATHQ et Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

Vous pouvez désormais ajuster la résolution des BAT de médias riches en spécifiant une résolution personnalisée ou en faisant glisser l’image vers la résolution souhaitée.

Avant cette modification, vous pouviez passer en revue les BAT à l’aide de la résolution inhérente à l’écran ou l’appareil sur lequel vous visionniez le contenu.

Vous pouvez utiliser le mode Comparer pour comparer différentes résolutions de BAT.

Pour plus d’informations, voir [Ouvrir les bons à tirer dans la visionneuse de vérification de l’appli de bureau](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md). 

## Nouvelle fonctionnalité de pool de ressources temporairement supprimée de l’aperçu {#new-resource-pool-functionality-temporarily-removed-from-preview}

En raison de problèmes de développement, nous avons décidé de supprimer le nouvel onglet Planification des ressources et de renommer l’onglet Planification des ressources héritée en son nom d’origine &quot;Planification des ressources&quot;.

La nouvelle fonctionnalité des groupes de ressources a également été supprimée avec cette modification. Le nouvel onglet de la Planification des ressources et les fonctionnalités des pools de ressources retourneront à l’environnement Aperçu des environnements Sandbox à la fin du mois de juin 2017.
