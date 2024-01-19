---
content-type: release-notes
keywords: notes,trimestriel,mise à jour
navigation-topic: product-releases
title: 21.1 Améliorations de la gestion de projet
description: Cette page décrit toutes les améliorations apportées à la gestion de projet avec la version 21.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 1%

---

# 21.1 Améliorations de la gestion de projet

Cette page décrit toutes les améliorations apportées à la gestion de projet avec la version 21.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.

Pour obtenir la liste de toutes les modifications disponibles avec la version 21.1, voir [Présentation de la version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Exportation désormais disponible dans la section Mesures d’un projet

Pour partager plus facilement l’état et la progression d’un projet, vous pouvez désormais exporter l’intégralité du tableau de bord dans la section Mesures d’un projet vers un fichier .png .

Pour plus d’informations, voir [Présentation des mesures de projet](../../../manage-work/projects/manage-projects/project-metrics.md).

Cette fonctionnalité est désormais incluse dans la variable [Principes de planification de la nouvelle expérience Workfront, Partie 3 : Gestion d’un projet](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) parcours d’apprentissage sur Workfront One.

## Mettre à jour le pourcentage de problème terminé lorsque le projet ou la tâche a été converti à partir de la mise à jour du problème

Nous avons mis à jour la façon dont le pourcentage de problèmes terminés fonctionne pour les problèmes qui ont été convertis en projets ou en tâches. Avec la nouvelle fonctionnalité, lorsqu’un problème est converti en tâche ou projet, le pourcentage de fin du problème est mis à jour en synchronisation avec le pourcentage de fin de la tâche ou du projet de résolution lorsque l’état &quot;Mettre à jour automatiquement le problème résolvable lorsque l’état du paramètre Résoudre l’objet change&quot; est activé à partir de la configuration.

Pour plus d’informations sur la conversion de problèmes, voir [Présentation de la résolution et des objets résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Nouvelle liste des requêtes envoyées

Pour vous permettre de gérer vos requêtes envoyées de manière plus simple et cohérente, nous avons supprimé les sections Demandes que j’ai envoyées et Toutes les requêtes de la zone Demandes et les avons remplacées par une nouvelle liste Envoyées. L’aspect familier de la liste correspond à toutes les autres listes du système, ce qui vous permet de filtrer différentes catégories de demandes envoyées et de rechercher rapidement une demande qui peut être difficile à trouver.

Pour plus d’informations sur la localisation des requêtes envoyées, voir [Recherche des requêtes envoyées](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Cette fonctionnalité est désormais incluse dans la variable [Principes de base des collaborateurs pour la nouvelle expérience Workfront](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) parcours d’apprentissage sur Workfront One.

Cette fonctionnalité est désormais incluse dans la variable [Requêtes dans la nouvelle expérience Workfront](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) parcours d’apprentissage sur Workfront One.

## Champs supprimés de la page Nouvelle requête

>[!NOTE]
>
>Retiré de la version.

Dans le cadre de la reconception de la page Nouvelle requête, nous avons mis à jour les nouveaux champs de problème configurés dans la section Configuration de la file d’attente d’un projet.

Les nouveaux champs de problème suivants s’affichent uniquement lors de la création d’un problème à partir de la section Problèmes du projet. Elles ne s’affichent pas lors de l’envoi d’un problème à l’aide d’une file d’attente de demandes dans la zone Demandes :

* Gravité
* Heures prévues
* Date de début prévue
* URL
* Affecté à
* Fonction
* Équipe

Nous avons remplacé les champs Affecté à, Rôle de tâche et Équipe par le nouveau champ Affectations de la page Nouvelle requête afin de désigner efficacement un utilisateur, un rôle de tâche ou une équipe dans un champ commun lorsque vous envoyez une nouvelle requête.

Pour plus d’informations sur la définition des nouveaux champs de problème pour un projet, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Nouvelle expérience lors de l’envoi de requêtes dans la zone Demandes

>[!NOTE]
>
>Retiré de la version ; restera dans Aperçu et version en production avec la version 21.2.

Afin d’assurer la cohérence avec la nouvelle expérience Workfront et d’améliorer l’efficacité de votre action lors de l’envoi de requêtes, nous avons repensé la zone Nouvelle requête dans la zone Demandes . Voici quelques améliorations :

* Une interface utilisateur est fournie avec le reste de la nouvelle expérience Workfront.
* Suppression de la zone Nouvelles requêtes pour une expérience plus simple et plus intuitive
* Une nouvelle méthode plus efficace pour joindre des documents à vos requêtes

Possibilité de partager un lien vers la file d’attente des demandes, le groupe de rubriques ou la rubrique de la file d’attente lorsque vous saisissez la requête.

Pour plus d’informations sur l’envoi de requêtes, voir [Création et envoi de requêtes Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Partage d’un lien vers une file d’attente de demandes lors de l’envoi d’une demande

>[!NOTE]
>
>Retiré de la version ; restera dans Aperçu et version en production avec la version 21.2.

Nous avons maintenant rendu possible le partage d’un lien vers une file d’attente de requêtes, un groupe de rubriques ou une rubrique de file d’attente.

Avant d’envoyer une nouvelle requête, vous pouvez copier un lien vers la file d’attente des requêtes, le groupe de rubriques ou la rubrique de la file d’attente de la requête et le partager avec d’autres utilisateurs, ou l’incorporer dans un tableau de bord.

Pour plus d’informations sur le partage d’un lien vers une file d’attente de demandes lors de l’envoi d’une demande, voir [Partage d’un lien vers une file d’attente de requêtes](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Recherchez un groupe à affecter à un projet et affichez ses détails.

Il est désormais plus facile de vous assurer d’identifier le bon groupe lorsque vous affectez un groupe à un projet. Pointez sur le nom d’un groupe que vous trouvez dans la zone Groupe, puis cliquez sur l’icône d’information qui s’affiche en regard du nom pour afficher l’info-bulle Détails du groupe.

Cette info-bulle comprend la hiérarchie des groupes au-dessus du groupe, le cas échéant, et les administrateurs du groupe.

En fonction des détails configurés pour le groupe, le chef d’entreprise et la description du groupe peuvent également s’afficher.

Grâce à ces informations, vous pouvez être assuré que vous sélectionnez le groupe approprié à affecter au projet.

Pour plus d’informations, voir [Gestion des informations dans la zone Aperçu du projet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## Nouveau rapport Délégation d’utilisateurs

Auparavant, les informations relatives aux délégations de tâche, de problème et d’approbation de projet ne pouvaient être visualisées que par le délégué dans sa zone d’accueil. Pour permettre à d’autres utilisateurs de voir ces informations, Planifier les utilisateurs peut maintenant créer le rapport Délégation d’utilisateurs , qui vous indique :

* Qui a délégué ces approbations à un autre utilisateur
* Quel utilisateur a reçu ces validations ?
* Les dates de début et de fin de ces délégations

Pour en savoir plus, voir [Créer un rapport Délégation d’utilisateurs](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
