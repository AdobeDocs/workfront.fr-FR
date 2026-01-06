---
product-area: projects
navigation-topic: create-tasks
title: Présentation de la création de tâches
description: Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 97%

---

# Créer une vue d’ensemble des tâches

Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.

Vous pouvez par exemple, après avoir créé un projet, vouloir créer des tâches et les modifier pour organiser le plan du projet. Pour en savoir plus sur la création d’un projet, voir [Créer un projet](../../../manage-work/projects/create-projects/create-project.md). Pour plus d’informations sur la création de tâches, voir [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Cet article décrit les considérations, les limitations et les valeurs par défaut qui s’appliquent lors de la création de tâches.

## Création de tâches dans un projet

Vous pouvez créer des tâches dans un projet des manières suivantes :

* En partant de zéro, tel que décrit dans [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copiez des tâches dans le même projet ou dans un nouveau projet ou dupliquez des tâches dans le même projet, tel que décrit dans [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Déplacez des tâches d’un projet à l’autre, tel que décrit dans [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limites de la création de tâches

Lorsque vous disposez des accès et des autorisations nécessaires, vous pouvez créer des tâches dans un projet. Toutefois, dans les cas suivants, il se peut que vous ne puissiez pas créer de tâches :

* Votre administrateur ou administratrice Adobe Workfront ou un administrateur ou une administratrice de groupes doit activer l’ajout de tâches à un projet dont le statut est Terminé ou Immobilisé dans la zone Préférences du projet. Pour plus d’informations sur la définition des préférences du projet, voir [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Vous ne pouvez pas ajouter de tâches à un projet dont l’approbation est en cours.

## Nombre maximum de tâches autorisées pour un projet

Un projet peut contenir jusqu’à 5 000 tâches. Un message d’avertissement s’affiche sur le projet lorsque vous vous rapprochez de la limite, lorsque vous l’avez atteinte et si vous tentez de la dépasser.

En fonction du nombre de tâches dans vos projets lorsque cette limitation a été imposée, votre instance Workfront peut autoriser plus de 5 000 tâches dans un seul projet.

Si vous êtes en mesure d’inclure plus de 5 000 tâches dans un seul projet, tenez compte des points suivants :

* La limite de tâches pour votre environnement Workfront est fixée au nombre actuel de tâches de votre projet le plus important, plus 10 % supplémentaires.

  Par exemple, si un projet de votre instance Workfront contient 10 000 tâches, votre limite pour chaque projet dans l’ensemble de votre instance Workfront est de 11 000 tâches.

* Les petits projets améliorent les performances et minimisent les problèmes de gestion qui accompagnent les grands projets.

## Tâches par défaut lors de l’ajout de tâches à un projet

Il existe deux types d’informations par défaut que Workfront met automatiquement à jour pour les tâches lorsque vous les créez :

* Informations par défaut au niveau du système

  Votre administrateur Workfront ou un administrateur de groupe établit les valeurs par défaut au niveau du système pour les tâches dans la zone Tâches et Événements des Préférences du projet. Pour plus d’informations sur les préférences en matière de tâches et de problèmes, voir [Configurer les préférences en matière de tâches et de problèmes à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) ou [Configurer les préférences en matière de tâches et de problèmes pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Informations par défaut au niveau du projet

  Le reste de cette section décrit les valeurs par défaut au niveau du projet que vous pouvez définir, en tant que personne responsable de projet, pour toutes les nouvelles tâches ajoutées à un projet.

Lorsque vous ajoutez une tâche à un projet, selon la façon dont le projet est configuré, Workfront peut automatiquement attacher un processus d’approbation ou des formulaires personnalisés à la tâche.

Pour plus d’informations sur la configuration d’un projet afin d’ajouter ces éléments par défaut, voir la section « Tâches » de l’article [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Lorsque vous définissez les informations par défaut à associer aux tâches ajoutées à un projet au niveau du projet, tenez compte des éléments suivants :

* Vous devez disposer des droits de gestion sur le projet pour définir les paramètres par défaut du processus d’approbation des tâches et des formulaires personnalisés.
* Toutes les nouvelles tâches sont créées avec le processus d’approbation et les formulaires personnalisés définis lors de la modification du projet.
* Vous pouvez modifier ces paramètres par défaut lorsque vous ajoutez des tâches en utilisant la case Modifier la tâche, mais pas lorsque vous ajoutez des tâches dans la modification en ligne.
* Vous pouvez définir le processus d’approbation et les formulaires personnalisés pour les tâches à l’aide d’un modèle.

   * Lorsqu’un projet est créé à partir de ce modèle, le processus d’approbation et les formulaires personnalisés sont automatiquement appliqués au projet.
   * Lorsqu’un modèle est joint à un projet existant, le projet conserve le processus d’approbation des tâches original et les paramètres des formulaires personnalisés s’ils sont définis. S’ils ne sont pas définis, les paramètres du modèle deviennent les paramètres du projet.
   * Lorsqu’un modèle est joint à un projet existant, les tâches ajoutées au projet à partir du modèle conservent le processus d’approbation et les paramètres des formulaires personnalisés qu’ils avaient sur le modèle, quels que soient les paramètres des tâches sur le projet.

  Pour plus d’informations sur l’association d’un modèle à un projet, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Lorsque vous copiez le projet, les paramètres par défaut de la tâche sont transférés vers le nouveau projet.

  Pour plus d’informations sur la copie d’un projet, voir [Copier un projet](../../../manage-work/projects/manage-projects/copy-project.md).

* Lorsque vous copiez des tâches d’un projet à un autre et que le projet de destination a des paramètres par défaut différents pour les tâches, les tâches copiées conservent les paramètres par défaut du projet original, à moins que ceux-ci ne soient effacés au cours du processus de copie.
* Lorsque vous dupliquez une tâche sur le même projet, les formulaires personnalisés et le processus d’approbation sont transférés à la tâche dupliquée.

  Pour plus d’informations sur la copie et la duplication de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Lorsque vous déplacez la tâche vers un autre projet, les paramètres par défaut de la tâche sont enregistrés sur les tâches du projet d’origine, quels que soient les paramètres par défaut de la tâche sur le nouveau projet.

  Pour plus d’informations sur le déplacement des tâches, consultez la section [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).
