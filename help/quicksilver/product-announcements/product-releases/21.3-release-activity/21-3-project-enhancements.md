---
title: Améliorations apportées aux projets (version 21.3)
description: Améliorations apportées aux projets (version 21.3)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 100%

---

# Améliorations apportées aux projets (version 21.3)

Cette page décrit toutes les améliorations apportées aux projets avec la version 21.3 de l’environnement de prévisualisation. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 21 juillet 2021.

Pour obtenir la liste de toutes les modifications disponibles avec la version 21.3, voir [Vue d’ensemble de la version 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Associer un modèle à un groupe

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Pour vous aider à rationaliser le processus de création de projet et à identifier plus facilement les groupes qui possèdent les modèles de projet, nous avons ajouté la possibilité d’attribuer un groupe à un modèle de projet.

Lorsque vous affectez un groupe à un modèle de projet, tous les projets créés à partir du modèle sont automatiquement associés au groupe du modèle. Pour plus d’informations, consultez [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Vous pouvez également associer un processus d’approbation de groupe à un modèle et à ses tâches de modèle si le modèle est associé à votre groupe. Pour plus d’informations, consultez [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modification plus facile des champs dans la section Détails

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Les améliorations suivantes permettent de modifier plus facilement les informations dans la section Détails de n’importe quel objet :

* Un contour gris autour d’un champ lorsque vous le survolez indique qu’il est modifiable.
* Vous pouvez modifier les champs en cliquant dessus une seule fois.

Avant cette amélioration, les champs modifiables n’étaient pas clairement définis et vous deviez double-cliquer pour modifier un champ.

## Tenir compte des projets transversaux antérieurs lors du calcul des dates de remise

Avec une nouvelle amélioration de la façon dont Adobe Workfront calcule les dates de remise des tâches, les dépendances inter-projets sont désormais prises en compte.

Auparavant, les dates de remise étaient calculées uniquement sur la base des tâches antérieures du même projet.

Maintenant, pour vous assurer que vous disposez toujours d’une date de remise précise pour une tâche avec des projets transversaux antérieurs, vous devez recalculer la chronologie du projet de la tâche ultérieure. Après avoir recalculé la chronologie, les dates de remise de la tâche calculent en prenant en compte les dépendances inter-projets des tâches.

Pour plus d’informations sur les dates de remise, consultez [Vue d’ensemble de la date de remise de la tâche](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Ajouter des histoires et des problèmes existants à partir du panorama Scrum

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Vous pouvez désormais ajouter une histoire ou un problème existant directement à partir du panorama Scrum. Cela facilite l’ajout d’histoires existantes à votre itération actuelle sans que vous ayez besoin d’accéder à la page de liste d’attente.

Pour plus d’informations, consultez [Ajouter des histoires et des problèmes à partir du panorama Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Ajouter de nouvelles histoires et de nouveaux problèmes à partir du panorama Scrum

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Vous pouvez maintenant créer une nouvelle histoire ou un nouveau problème directement à partir du panorama Scrum. Cela facilite l’ajout rapide d’une nouvelle histoire à votre itération actuelle.

Pour plus d’informations, consultez [Ajouter des histoires et des problèmes à partir du panorama Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Supprimer une histoire ou un problème du tableau Kanban

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Vous pouvez désormais supprimer une histoire ou un problème directement à partir de votre tableau Kanban en cliquant sur l’icône Plus d’une carte d’histoire ou de problème et en sélectionnant Supprimer. Lorsque vous supprimez une histoire ou un problème, l’élément est placé dans la Corbeille pendant 30 jours et ne peut être récupéré que par l’administrateur ou l’administratrice système.

Pour plus d’informations, consultez [Supprimer des histoires ou des problèmes du tableau Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Mises à jour de l’en-tête des cartes et des storyboards Agile

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Sur les tableaux Kanban et les panoramas Scrum, les améliorations suivantes sont désormais disponibles :

* Les cartes des histoires et les colonnes des panoramas ont une largeur fixe, de sorte que les tailles de carte ne changent pas si vous ajustez la taille de la fenêtre du navigateur.
* La colonne Histoires a été renommée Histoire parent.
* Chaque carte comporte un libellé dans la partie supérieure pour l’identifier en tant qu’histoire parent, sous-tâche (associée à une histoire parent), histoire (non associée à un parent) ou problème.
* Un ombrage de l’arrière-plan sépare visuellement les colonnes.

Pour plus d’informations, consultez [Vue d’ensemble des itérations](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Préférences pour les projets, tâches et problèmes de groupe

Comme nous l’avons indiqué précédemment, nous avons déployé des personnalisations au niveau du groupe pour les préférences de projet, de tâche et de problème dans les phases qui ont précédé le 24 juin 2021. Le déploiement est maintenant terminé et ces fonctionnalités sont disponibles en production pour l’ensemble de la clientèle.

Pour plus d’informations, consultez les articles suivants :

* [Configurer des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Configurer les préférences de tâches et de problèmes pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Autoriser des utilisateurs et des utilisatrices externes à approuver un document

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Vous pouvez désormais utiliser des adresses e-mail externes pour affecter des personnes chargées de l’approbation à un document dans la nouvelle expérience Workfront.

Dans Workfront Classic, auparavant, vous pouviez uniquement ajouter des utilisateurs et des utilisatrices externes par adresse e-mail.

Pour plus d’informations, consultez la section [Demander l’approbation de documents](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exporter des informations à partir de la section des détails d’un portfolio ou d’un programme

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement Aperçu le 20 mai 2021. Elle sera publiée dans l’environnement de production le 3 juin 2021.

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Vous pouvez désormais exporter vers un fichier .pdf des informations provenant de la section « Détails » des portfolios et des programmes. Avant cette amélioration, vous ne pouviez exporter des informations de la section « Détails » qu’à partir de projets, tâches et problèmes.

Pour plus d’informations sur l’export de formulaires personnalisés à partir d’un objet, consultez la section [Exporter les détails de formulaires personnalisés et d’objets](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Ajout de l’horodatage de la date d’achèvement prévue dans l’en-tête de l’objet

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Pour faciliter l’accès, la commodité et la précision, nous avons ajouté la possibilité de sélectionner un horodatage dans la date d’achèvement prévue de l’en-tête des projets, tâches ou problèmes.

Avant cette amélioration, Workfront sélectionnait minuit comme heure par défaut lorsque vous mettiez à jour la date d’achèvement prévue d’un objet. Vous pouvez désormais personnaliser l’heure ainsi que la date d’achèvement.

Pour plus d’informations sur les en-têtes d’objet de la nouvelle expérience Workfront, consultez la section [Nouveaux en-têtes d’objet](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Ajouter un formulaire personnalisé à un objet sans le modifier

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Nous avons simplifié l’ajout à un objet d’un formulaire personnalisé que quelqu’un d’autre remplira (ou que vous remplirez plus tard). Lorsque vous l’ajoutez, le formulaire ne passe plus automatiquement en mode de modification. Vous pouvez simplement enregistrer le formulaire vide dans l’objet.

Avant, lors de l’ajout d’un formulaire personnalisé à un objet, la page était en mode de modification, et vous deviez remplir tous les champs requis du formulaire avant de pouvoir l’enregistrer dans l’objet. C’était peu pratique lorsque le formulaire devait être rempli par un autre utilisateur ou une autre utilisatrice ou lorsque vous ne saviez pas encore quoi mettre dans un champ obligatoire.

Pour plus d’informations sur l’ajout d’un formulaire personnalisé à un objet, consultez la section [Ajouter un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

