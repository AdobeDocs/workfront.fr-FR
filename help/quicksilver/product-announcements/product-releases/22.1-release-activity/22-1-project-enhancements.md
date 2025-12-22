---
title: 22.1 Améliorations apportées au projet
description: 22.1 Améliorations apportées au projet
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 98%

---

# 22.1 Améliorations apportées au projet

Cette page décrit toutes les améliorations apportées aux projets avec la version 22.1 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

Semaine du 17 janvier 2022.

Pour consulter la liste de tous les changements disponibles avec la version 22.1, voir [Vue d’ensemble de la version 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Modifier l’option par défaut pour les tâches antérieures lors de la copie ou du déplacement de tâches

Afin de minimiser le nombre d’étapes manuelles lors de la copie ou du déplacement de tâches, nous avons mis à jour les informations copiées ou déplacées avec la tâche par défaut. Désormais, tous les prédécesseurs sont copiés ou déplacés avec la tâche par défaut, car l’option Toutes les tâches antérieures est sélectionnée par défaut.

Avant cette amélioration, l’option Toutes les tâches antérieures était désélectionnée par défaut lors de la copie ou du déplacement d’une tâche.

Pour plus d’informations, consultez les articles :

* [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## Mise à jour de la barre d’outils sur la liste des tableaux de bord et les rapports dans les tableaux de bord

La barre d’outils de quatre pages de tableau de bord a désormais un aspect moderne qui correspond à d’autres listes Workfront telles que les projets, les tâches et les problèmes. Cette barre d’outils intuitive facilite désormais l’ajout, la modification, le partage, la copie et la suppression des tableaux de bord.

Les pages avec la barre d’outils mise à jour sont les suivantes :

* Rapports de tâches (affichés dans les tableaux de bord)
* Liste Tous les tableaux de bord
* Liste Mes tableaux de bord
* Liste Tableaux de bord partagés

Pour plus d’informations, voir [Créer et gérer des tableaux de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md).

## Ajouter et modifier le panneau Résumé des formulaires personnalisés pour les documents

Vous pouvez désormais ajouter et modifier des formulaires personnalisés directement dans le panneau Résumé du document.

Avec cette modification, vous verrez également un nouvel aspect dans le résumé du document. Une nouvelle section Vue d’ensemble contient la miniature de l’image ainsi que les détails du document. Vous pouvez également archiver et extraire des documents dans la section des détails du document.

Auparavant, vous deviez accéder à l’onglet Formulaires personnalisés dans Détails du document pour apporter des modifications ou ajouter des formulaires personnalisés.

Pour plus d’informations, voir [Vue d’ensemble du résumé des documents](../../../documents/managing-documents/summary-for-documents.md).

## Nouvelle expérience lors de la copie d’une ou de plusieurs tâches

Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Adobe Workfront, nous avons repensé l’interface lors de la copie d’une tâche. Cette option est actuellement disponible lorsque vous copiez une tâche au niveau de la tâche ou une ou plusieurs tâches dans une liste.

Voici quelques améliorations :

* Toutes les informations que vous devez mettre à jour avant de copier la tâche s’affichent sur une page continue.
* Workfront vérifie que vous avez accès au projet de destination immédiatement après avoir choisi le projet. Avant cette amélioration, un message d’avertissement indiquant que vous ne disposiez pas d’un accès correct s’affichait après avoir confirmé la copie, ce qui entraînait des étapes supplémentaires et empêchait la copie d’être autorisée.
* Possibilité de demander l’accès à un projet pour lequel vous souhaitez copier la tâche sans quitter la zone Copier la tâche.

Pour plus d’informations, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Nouvelle expérience lors du déplacement d’une ou de plusieurs tâches d’une liste

Pour offrir une expérience cohérente lors de la répétition de la même tâche, nous avons maintenant mis à jour l’interface permettant de déplacer une ou plusieurs tâches d’une liste afin qu’elles correspondent à l’expérience du déplacement de la tâche au niveau de la tâche. (Nous avions mis à jour l’expérience de déplacement d’une tâche au niveau de la tâche dans une version précédente de l’environnement de prévisualisation.)

Pour plus d’informations, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nouvelle expérience lors du déplacement d’une tâche au niveau de la tâche

Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface pour le déplacement d’une tâche. Cette option est actuellement disponible lors du déplacement d’une tâche au niveau de la tâche. Dans une version suivante, nous allons étendre cette reconception au déplacement d’une tâche à partir d’une liste.

Voici quelques-unes des améliorations apportées à cette nouvelle interface :

* Toutes les informations que vous devez mettre à jour avant le déplacement s’affichent sur une page continue.
* Workfront vérifie que vous avez accès au projet de destination immédiatement après avoir choisi le projet. Avant cette amélioration, Workfront vous avertissait que vous ne disposiez pas d’un accès correct après avoir confirmé le déplacement, ce qui entraînait des étapes supplémentaires et empêchait le déplacement d’être autorisé.
* Possibilité de demander l’accès à un projet pour lequel vous souhaitez déplacer la tâche sans quitter la zone Déplacer la tâche.

Pour plus d’informations, voir [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nouvelle expérience lors de la conversion d’un problème en projet à l’aide d’un modèle au niveau du problème

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Elle a ensuite été déployée de manière progressive à partir du 28 avril 2022. Le déploiement s’est achevé le 5 mai 2022. Cette option est désormais disponible dans les environnements de prévisualisation et de production pour tous les clientes et clients. (Pour obtenir les dernières mises à jour sur le statut de cette fonctionnalité qui est disponible dans l’environnement de production, voir [Vue d’ensemble de la version 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Afin d’harmoniser votre utilisation de Workfront avec la nouvelle expérience Workfront, nous avons repensé l’interface de conversion d’un problème en projet lorsque vous utilisez un modèle et que vous le convertissez à partir de la page du problème.

Vous pouvez désormais accéder plus facilement à votre liste de favoris immédiatement après avoir choisi de convertir le problème.

L’interface reconçue correspond à l’expérience de création d’un projet à partir d’un modèle que nous avons mis à jour récemment.

Pour plus d’informations, voir [Convertir un événement en projet](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Convertir des problèmes en projets à l’aide d’un modèle à partir de listes, de rapports et de tableaux de bord

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Elle a ensuite été déployée de manière progressive à partir du 28 avril 2022. Le déploiement s’est achevé le 5 mai 2022. Cette option est désormais disponible dans les environnements de prévisualisation et de production pour tous les clientes et clients. (Pour obtenir les dernières mises à jour sur le statut de cette fonctionnalité qui est disponible dans l’environnement de production, voir [Vue d’ensemble de la version 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Pour améliorer l’efficacité de votre travail et faciliter la conversion des problèmes dans un environnement en constante évolution, nous avons ajouté la possibilité de convertir un problème en projet à partir d’un modèle d’une liste, d’un rapport ou d’un tableau de bord.

Avant cette amélioration, cette fonctionnalité n’existait que lorsque vous convertissiez le problème à partir de la page des problèmes.

Pour plus d’informations, voir [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## La liste Filtrer par utilisateur sur les tableaux Agile affiche d’abord les utilisateurs avec le plus d’affectations

>[!NOTE]
>
>Cette fonctionnalité ne sera pas incluse dans la version 22.1. Elle a été supprimée de l’environnement de prévisualisation.

Désormais, le filtre affiche d’abord les personnes qui ont le plus d’affectations afin qu’elles soient plus faciles à localiser sans faire défiler la liste.

Auparavant, le filtre par liste de personnes sur les panoramas Kanban et Scrum s’affichait par ordre alphabétique.

Pour plus d’informations, consultez les documents suivants.

* [Filtrer par personne sur le panorama Scrum](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [Filtrer par personne sur le tableau Kanban](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## Limiter la possibilité d’ajouter des documents à un modèle que vous partagez.

Parfois, les personnes ajoutent des documents à un modèle de projet en pensant qu’elles les ajoutent à un projet. Désormais, vous pouvez empêcher cela. Lorsque vous partagez un modèle avec l’accès Affichage, vous pouvez désactiver le nouveau paramètre avancé Ajouter des documents. Cela désactive la capacité de vos personnes destinataires à ajouter des documents au modèle.

Pour plus d’informations sur le partage d’un modèle, voir [Partager des modèles de projet](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).

Pour plus d’informations sur le nouveau paramètre avancé Ajouter des documents, reportez-vous à la section de l’article [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Partager un dossier de documents

Vous pouvez maintenant partager un dossier de documents et son contenu à partir de la zone Documents. Auparavant, cela n’était pas possible. Vous deviez partager chaque document séparément dans un dossier.

Pour plus d’informations, voir [Partager un dossier de documents](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

