---
content-type: release-notes
keywords: notes,trimestrielle,mise à jour
navigation-topic: product-releases
title: Améliorations apportées à la gestion des projets
description: Cette page décrit toutes les améliorations apportées à la gestion de projets avec la version 21.1 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 100%

---

# Améliorations apportées à la gestion des projets

Cette page décrit toutes les améliorations apportées à la gestion de projets avec la version 21.1 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.

Pour obtenir une liste de tous les changements disponibles avec la version 21.1, voir [Vue d’ensemble de la version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Export désormais disponible dans la section Mesures d’un projet

Pour partager plus facilement le statut et la progression d’un projet, vous pouvez désormais exporter l’ensemble du tableau de bord de la section Mesures d’un projet vers un fichier .png.

Pour plus d’informations, voir [Vue d’ensemble des mesures des projets](../../../manage-work/projects/manage-projects/project-metrics.md).

Cette fonctionnalité est désormais incluse dans le parcours de formation [Principes de planification de la nouvelle expérience Workfront, Partie 3 : gérer un projet](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) sur Workfront One.

## Mise à jour du pourcentage terminé d’un problème lorsque le projet ou la tâche a été converti à partir de la mise à jour du problème

Nous avons mis à jour la façon dont le pourcentage terminé des problèmes fonctionne pour les problèmes qui ont été convertis en projets ou en tâches. Avec cette nouvelle fonctionnalité, lorsqu’un problème est converti en tâche ou en projet, le pourcentage terminé du problème est mis à jour en synchronisation avec le pourcentage terminé de la tâche ou du projet de résolution lorsque le paramètre « Mettre à jour automatiquement le statut des problèmes pouvant être résolus lorsque le statut de l’objet de résolution change » est activé dans la configuration.

Pour plus d’informations sur la conversion de problèmes, voir [Vue d’ensemble des objets de résolution et des objets résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Nouvelle liste des demandes envoyées

Pour vous permettre de gérer vos demandes soumises de manière plus simple et plus cohérente, nous avons supprimé les sections Demandes que j’ai envoyées et Toutes les demandes dans la zone Demandes et les avons remplacées par une nouvelle liste Demandes soumises. La liste a un aspect familier qui correspond à toutes les autres listes du système, ce qui vous permet de filtrer les différentes catégories de demandes soumises et de rechercher rapidement une demande qui pourrait être difficile à trouver.

Pour plus d’informations sur l’emplacement des demandes envoyées, voir [Localiser les demandes envoyées](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Cette fonctionnalité est désormais incluse dans le parcours de formation [Principes de collaboration pour la nouvelle expérience Workfront](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) sur Workfront One.

Cette fonctionnalité est désormais incluse dans le parcours de formation [Demandes dans la nouvelle expérience Workfront](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) sur Workfront One.

## Champs supprimés de la page Nouvelle demande

>[!NOTE]
>
>Retiré de la version.

Dans le cadre de la refonte de la page Nouvelle demande, nous avons mis à jour les champs Nouveau problème qui sont configurés dans la section Configuration de la file d’attente d’un projet.

Les champs Nouveau problème suivants s’affichent uniquement lors de la création d’un problème à partir de la section Problèmes du projet. Elles ne s’affichent pas lors de l’envoi d’un problème à l’aide d’une file d’attente des demandes dans la zone Demandes :

* Gravité
* Heures prévues
* Date de début prévue
* URL
* Affecté à
* Fonction
* Equipe

Nous avons remplacé les champs Affecté à, Fonction et Équipe par le nouveau champ Affectations de la page Nouvelle demande afin de désigner efficacement un utilisateur ou une utilisatrice, une fonction ou une équipe dans un champ commun lorsque vous envoyez une nouvelle demande.

Pour plus d’informations sur la définition des champs Nouveau problème pour un projet, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Nouvelle expérience lors de l’envoi de demandes dans la zone Demandes

>[!NOTE]
>
>Retiré de la version ; restera dans l’environnement de prévisualisation et sera publié en production avec la version 21.2.

Afin d’assurer la cohérence avec la nouvelle expérience Workfront et d’améliorer l’efficacité de la soumission des demandes, nous avons repensé la zone Nouvelle demande dans la zone Demandes. Voici quelques-unes des améliorations apportées :

* Une interface utilisateur est fournie avec le reste de la nouvelle expérience Workfront.
* Suppression de la zone Nouvelles demandes pour une expérience plus simple et plus intuitive
* Une nouvelle méthode plus efficace pour joindre des documents à vos demandes

Possibilité de partager un lien vers la file d’attente des demandes, le groupe de sujets ou la rubrique de file d’attente lorsque vous saisissez la demande.

Pour plus d’informations sur l’envoi de demandes, voir [Créer et soumettre des demandes Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Partager un lien vers une file d’attente des demandes lors de l’envoi d’une demande

>[!NOTE]
>
>Retiré de la version ; restera dans l’environnement de prévisualisation et sera publié en production avec la version 21.2.

Il est désormais possible de partager un lien vers une file d’attente des demandes, un groupe de rubriques ou une rubrique de file d’attente lorsque vous créez une demande.

Avant de soumettre une nouvelle demande, vous pouvez copier un lien vers la file d’attente des demandes, le groupe de rubriques ou la rubrique la file d’attente de la demande et le partager avec d’autres utilisateurs et utilisatrices, ou l’intégrer dans un tableau de bord.

Pour plus d’informations sur le partage d’un lien vers une file d’attente des demandes lors de la soumission d’une demande, voir [Partager un lien vers une file d’attente des demandes](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Rechercher un groupe à affecter à un projet et afficher ses détails

Il est désormais plus facile de s’assurer que vous identifiez le bon groupe lorsque vous assignez un groupe à un projet. Pointez sur le nom d’un groupe que vous trouvez dans la case Groupe, puis cliquez sur l’icône d’information qui s’affiche en regard du nom pour afficher l’infobulle Détails du groupe.

Cette info-bulle comprend la hiérarchie des groupes au-dessus du groupe, le cas échéant, et les administrateurs et administratrices du groupe.

En fonction des détails configurés pour le groupe, vous pouvez également voir le ou la chef d’entreprise et la description du groupe.

Grâce à ces informations, vous savez que vous sélectionnez le groupe approprié à affecter au projet.

Pour plus d’informations, voir [Gérer des informations dans la zone Vue d’ensemble du projet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## Nouveau rapport Délégation d’utilisateurs et d’utilisatrices

Auparavant, les informations relatives aux délégations d’approbation de tâches, de problèmes et de projets ne pouvaient être consultées par la personne déléguée que dans sa zone d’accueil. Pour permettre à d’autres personnes de consulter ces informations, les utilisateurs et utilisatrices du Plan peuvent désormais créer le rapport de délégation d’utilisateurs et d’utilisatrices, qui vous donne les informations suivantes :

* La personne qui a délégué ces approbations à une autre personne.
* La personne qui s’est vue déléguer ces approbations.
* Les dates de début et de fin de ces délégations.

Pour en savoir plus, voir [Créer un rapport Délégation d’utilisateurs et d’utilisatrices](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
