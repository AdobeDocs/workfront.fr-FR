---
title: Améliorations apportées aux projets (version 21.3)
description: Améliorations apportées aux projets (version 21.3)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 1%

---

# Améliorations apportées aux projets (version 21.3)

Cette page décrit toutes les améliorations apportées aux projets avec la version 21.3 de l’environnement Aperçu. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 21 juillet 2021.

Pour obtenir la liste de toutes les modifications disponibles avec la version 21.3, consultez la [présentation de la version 21.3](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Associer un modèle à un groupe

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Pour vous aider à rationaliser le processus de création de projet et à identifier plus facilement les groupes qui possèdent les modèles de projet, nous avons ajouté la possibilité d’affecter un groupe à un modèle de projet.

Lorsque vous affectez un groupe à un modèle de projet, tous les projets créés à partir du modèle sont automatiquement associés au groupe du modèle. Pour plus d’informations, voir [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Vous pouvez également associer un processus de validation de groupe à un modèle et à ses tâches de modèle si le modèle est associé à votre groupe. Pour plus d’informations, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modification plus facile des champs dans la section Détails

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Les améliorations suivantes permettent de modifier plus facilement les informations dans la section Détails de n’importe quel objet :

* Un contour gris autour d’un champ lorsque vous le survolez indique qu’il est modifiable.
* Vous pouvez modifier les champs en cliquant dessus une seule fois.

Avant cette amélioration, les champs modifiables n’étaient pas clairement définis et vous deviez double-cliquer pour modifier un champ.

## Tenir compte des prédécesseurs sur plusieurs projets lors du calcul des dates de remise

Avec une nouvelle amélioration de la façon dont Adobe Workfront calcule les dates de remise des tâches, les dépendances entre projets sont désormais prises en compte.

Auparavant, les dates de remise étaient calculées uniquement sur la base des prédécesseurs de la tâche du même projet.

Maintenant, pour vous assurer que vous disposez toujours d’une date de remise précise pour une tâche avec un prédécesseur multi-projet, vous devez recalculer la chronologie du projet de la tâche qui lui succède. Après avoir recalculé la chronologie, les dates de remise de la tâche calculent en prenant en compte les dépendances entre les projets des tâches.

Pour plus d’informations sur les dates de remise, consultez la [présentation de la date de remise des tâches](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Ajout d’articles et de problèmes existants à partir du panneau Scrum

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Vous pouvez désormais ajouter un article ou un problème existant directement à partir du panneau de résumé. Cela facilite l’ajout d’articles existants à votre itération actuelle sans avoir à accéder à la page de journal.

Pour plus d’informations, voir [Ajout d’articles et de problèmes à partir du Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Ajout de nouveaux articles et de nouveaux problèmes à partir du panneau Scrum

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Vous pouvez maintenant créer un article ou un problème directement à partir du panneau de défilement. Cela facilite l’ajout rapide d’une nouvelle histoire à votre itération actuelle.

Pour plus d’informations, voir [Ajout d’articles et de problèmes à partir du Scrum board](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Supprimer un article ou un problème du panorama Kanban

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Vous pouvez désormais supprimer un article ou un problème directement à partir de votre panorama Kanban en cliquant sur l’icône Plus d’un article ou d’une carte de problème et en sélectionnant Supprimer. Lorsque vous supprimez un article ou un problème, il est déplacé dans la Corbeille pendant 30 jours et ne peut être récupéré que par l’administrateur système.

Pour plus d’informations, voir [Suppression d’articles ou de problèmes sur le panorama Kanban](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Mises à jour de l’en-tête et du panorama des cartes agiles

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Sur les tableaux Kanban et Scrum, les améliorations suivantes sont désormais disponibles :

* Les cartes d’article et les colonnes du panorama ont une largeur fixe, de sorte que les formats de carte ne changent pas si vous ajustez la taille de la fenêtre du navigateur.
* La colonne Articles a été renommée Article parent.
* Chaque carte comporte un libellé dans la partie supérieure pour l’identifier en tant qu’article parent, sous-tâche (associée à un article parent), article (non associé à un parent) ou problème.
* L’ombrage de fond sépare visuellement les colonnes.

Pour plus d’informations, voir [Présentation des itérations](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Préférences de projet, de tâche et de problème de groupe

Comme nous l’avons indiqué précédemment, nous avons déployé des personnalisations au niveau du groupe pour les préférences de projet, de tâche et de problème dans les phases qui ont précédé le 24 juin 2021. Le déploiement est maintenant terminé et ils sont disponibles en production pour tous les clients.

Pour plus d’informations, consultez les articles suivants :

* [Configuration des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Autoriser les utilisateurs externes à approuver un document

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Vous pouvez désormais utiliser des adresses électroniques externes pour affecter des approbateurs à un document dans la nouvelle expérience Workfront.

Auparavant, vous pouviez ajouter des utilisateurs externes par adresse électronique uniquement dans Workfront Classic.

Pour plus d’informations, voir [Demande d’approbation de document](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Exporter des informations depuis la section Détails d’un portfolio ou d’un programme

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement Aperçu le 20 mai 2021. Il sera publié dans l’environnement de production le 3 juin 2021.

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Vous pouvez désormais exporter vers un fichier .pdf à partir de la section Détails des portefeuilles et des programmes. Avant cette amélioration, vous ne pouviez exporter des informations de la section Détails qu’à partir de projets, de tâches et de problèmes.

Pour plus d’informations sur l’exportation de formulaires personnalisés à partir d’un objet, voir [Exportation de formulaires personnalisés et de détails d’objet](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Ajout d’un horodatage de date d’achèvement prévu dans l’en-tête de l’objet.

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Pour faciliter l’accès, la commodité et la précision, nous avons ajouté la possibilité de sélectionner un horodatage dans la date d’achèvement planifiée de l’en-tête des projets, tâches ou problèmes.

Avant cette amélioration, lorsque vous avez mis à jour la date de fin planifiée d’un objet, Workfront a sélectionné minuit comme heure par défaut. Vous pouvez désormais personnaliser l’heure ainsi que la date de fin.

Pour plus d’informations sur les en-têtes d’objet de la nouvelle expérience Workfront, voir [Nouveaux en-têtes d’objet](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Ajouter un formulaire personnalisé à un objet sans le modifier

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Nous avons rendu plus facile l’ajout à un objet d’un formulaire personnalisé que quelqu’un d’autre remplira (ou que vous remplirez plus tard). Le formulaire ne passe plus automatiquement en mode d’édition lorsque vous l’ajoutez. Vous pouvez simplement enregistrer le formulaire vide dans l’objet .

Auparavant, lorsque vous ajoutiez un formulaire personnalisé à un objet, la page était en mode d’édition et vous deviez remplir tous les champs requis du formulaire avant de pouvoir l’enregistrer dans l’objet. Cela ne s’avérait pas pratique lorsque le formulaire était destiné à être rempli par un autre utilisateur, ou lorsque vous ne saviez pas encore quoi placer dans un champ obligatoire du formulaire.

Pour plus d’informations sur l’ajout d’un formulaire personnalisé à un objet, voir [Ajout d’un formulaire personnalisé à un objet](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

