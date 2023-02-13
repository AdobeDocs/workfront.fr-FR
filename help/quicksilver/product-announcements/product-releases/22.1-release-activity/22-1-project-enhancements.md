---
title: 22.1 Améliorations apportées au projet
description: 22.1 Améliorations apportées au projet
author: Luke
draft: Probably
feature: Product Announcements
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# 22.1 Améliorations apportées au projet

Cette page décrit toutes les améliorations apportées aux projets avec la version 22.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 17 janvier 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.1, voir [Présentation de la version 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Modification de l’option par défaut pour les prédécesseurs lors de la copie ou du déplacement de tâches

Afin de minimiser le nombre d’étapes manuelles lors de la copie ou du déplacement de tâches, nous avons mis à jour les informations copiées ou déplacées avec la tâche par défaut. Désormais, tous les prédécesseurs sont copiés ou déplacés avec la tâche par défaut, car l’option Tous les prédécesseurs est sélectionnée par défaut.

Avant cette amélioration, l’option Tous les prédécesseurs était désélectionnée par défaut lors de la copie ou du déplacement d’une tâche.

Pour plus d’informations, voir les articles suivants :

* [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## Mise à jour de la barre d’outils sur la liste des tableaux de bord et les rapports dans les tableaux de bord

La barre d’outils de quatre pages de tableau de bord a désormais une apparence moderne qui correspond à d’autres listes Workfront telles que les projets, les tâches et les problèmes. Cette barre d’outils intuitive facilite désormais l’ajout, la modification, le partage, la copie et la suppression des tableaux de bord.

Les pages avec la barre d’outils mise à jour sont les suivantes :

* Rapports de tâches (affichés dans les tableaux de bord)
* Toutes les listes de tableaux de bord
* Liste Mes tableaux de bord
* Liste des tableaux de bord partagés

Pour plus d’informations, voir [Création et gestion des tableaux de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md).

## Ajout et modification du panneau Résumé des formulaires personnalisés pour les documents

Vous pouvez désormais ajouter et modifier des formulaires personnalisés directement dans le panneau Résumé du document.

Avec cette modification, vous verrez également une nouvelle apparence dans le résumé du document. Une nouvelle section Aperçu contient la miniature de l’image ainsi que les détails du document. Vous pouvez également archiver et extraire des documents dans la section des détails du document.

Auparavant, vous deviez accéder à l’onglet Formulaires personnalisés dans Détails du document pour apporter des modifications ou ajouter des formulaires personnalisés.

Pour plus d’informations, voir [Présentation du résumé des documents](../../../documents/managing-documents/summary-for-documents.md).

## Nouvelle expérience lors de la copie d’une ou de plusieurs tâches

Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Adobe Workfront, nous avons repensé l’interface lors de la copie d’une tâche. Cette option est actuellement disponible lors de la copie d’une tâche au niveau de la tâche ou de la copie d’une ou de plusieurs tâches dans une liste.

Voici quelques améliorations :

* Toutes les informations que vous devez mettre à jour avant de copier la tâche s’affichent sur une page continue.
* Workfront vérifie que vous avez accès au projet de destination immédiatement après avoir choisi le projet. Avant cette amélioration, un message d’avertissement indiquant que vous ne disposez pas d’un accès correct s’affichait après avoir confirmé la copie, ce qui entraînait des étapes supplémentaires et empêchait la copie d’être autorisée.
* Possibilité de demander l’accès à un projet pour lequel vous souhaitez copier la tâche sans quitter la zone Copier la tâche .

Pour plus d’informations, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

## Nouvelle expérience lors du déplacement d’une ou de plusieurs tâches d’une liste

Pour offrir une expérience cohérente lors de la même tâche, nous avons maintenant mis à jour l’interface permettant de déplacer une ou plusieurs tâches d’une liste afin qu’elles correspondent à l’expérience lors du déplacement de la tâche au niveau de la tâche. (Nous avions mis à jour l’expérience de déplacement d’une tâche au niveau de la tâche dans une version précédente de l’aperçu.)

Pour plus d’informations, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nouvelle expérience lors du déplacement d’une tâche au niveau de la tâche

Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface pour le déplacement d’une tâche. Cette option est actuellement disponible lors du déplacement d’une tâche au niveau de la tâche. Dans une version suivante, nous allons étendre cette reconception au déplacement d’une tâche à partir d’une liste.

Voici quelques-unes des améliorations apportées à cette nouvelle interface :

* Toutes les informations que vous devez mettre à jour avant le déplacement s’affichent sur une page continue.
* Workfront vérifie que vous avez accès au projet de destination immédiatement après avoir choisi le projet. Avant cette amélioration, Workfront vous avertissait que vous ne disposez pas d’un accès correct après avoir confirmé le déplacement, ce qui entraînait des étapes supplémentaires et empêchait le déplacement d’être autorisé.
* Possibilité de demander l’accès à un projet pour lequel vous souhaitez déplacer la tâche sans quitter la zone Déplacer la tâche.

Pour plus d’informations, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Nouvelle expérience lors de la conversion d’un problème en projet à l’aide d’un modèle au niveau du problème

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Il a ensuite été lancé dans un déploiement progressif à partir du 28 avril 2022. Le déploiement a été achevé le 5 mai 2022. Cette option est désormais disponible dans Aperçu et Production pour tous les clients. (Pour obtenir les dernières mises à jour sur l’état de cette fonctionnalité qui est disponible dans Production, voir [Présentation de la version 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface permettant de convertir un problème en projet lors de l’utilisation d’un modèle lorsque vous le convertissez à partir de la page de problèmes.

Vous pouvez désormais accéder plus facilement à votre liste de favoris immédiatement après avoir sélectionné pour convertir le problème.

L’interface repensée correspond à l’expérience lors de la création d’un projet à partir d’un modèle que nous avons également mis à jour récemment.

Pour plus d’informations, voir [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Convertir des problèmes en projets à l’aide d’un modèle à partir de listes, de rapports et de tableaux de bord

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Il a ensuite été lancé dans un déploiement progressif à partir du 28 avril 2022. Le déploiement a été achevé le 5 mai 2022. Cette option est désormais disponible dans Aperçu et Production pour tous les clients. (Pour obtenir les dernières mises à jour sur l’état de cette fonctionnalité qui est disponible dans Production, voir [Présentation de la version 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).)

Pour accroître l’efficacité de votre travail et faciliter la conversion des problèmes dans un environnement à rythme rapide, nous avons ajouté la possibilité de convertir un problème en projet à l’aide d’un modèle à partir d’une liste, d’un rapport ou d’un tableau de bord.

Avant cette amélioration, cette fonctionnalité existait uniquement lorsque vous convertiez le problème à partir de la page de problèmes.

Pour plus d’informations, voir [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Le filtre par liste d’utilisateurs sur les panoramas agiles affiche d’abord les utilisateurs avec la plupart des affectations.

>[!NOTE]
>
>Cette fonctionnalité ne sera pas incluse dans la version 22.1. Il a été supprimé de l’environnement Aperçu.

Désormais, le filtre affiche d’abord les utilisateurs qui ont le plus d’affectations afin qu’ils soient plus faciles à localiser sans faire défiler la liste.

Auparavant, le filtre par liste d’utilisateurs sur les panoramas Kanban et Scrum s’affichait par ordre alphabétique.

Pour plus d’informations, voir les informations suivantes

* [Filtrage par utilisateur sur le panneau de défilement](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [Filtrage par utilisateur sur le panorama Kanban](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## Limitez la possibilité d’ajouter des documents à un modèle que vous partagez.

Parfois, les gens ajoutent des documents à un modèle de projet en pensant qu’ils les ajoutent à un projet. Désormais, vous pouvez aider à empêcher cela : lorsque vous partagez un modèle avec l’accès Affichage, vous pouvez désactiver le nouveau paramètre avancé Ajouter des documents. Cela désactive la capacité de vos destinataires à ajouter des documents au modèle.

Pour plus d’informations sur le partage d’un modèle, voir [Partage de modèles de projet](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).

Pour plus d’informations sur le nouveau paramètre avancé Ajouter des documents, reportez-vous à la section de l’article [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Partage d’un dossier de document

Vous pouvez maintenant partager un dossier de documents et son contenu à partir de la zone Documents. Auparavant, cela n’était pas possible. Vous deviez partager chaque document séparément dans un dossier.

Pour plus d’informations, voir [Partage d’un dossier de document](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

