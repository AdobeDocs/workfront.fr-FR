---
product-area: projects
navigation-topic: create-tasks
title: Présentation de la création de tâches
description: Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Présentation de la création de tâches

Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.

Par exemple, après avoir créé un projet, vous pouvez ajouter des tâches et les modifier pour organiser le plan du projet. Pour plus d’informations sur la création d’un projet, voir [Création d’un projet](../../../manage-work/projects/create-projects/create-project.md). Pour plus d’informations sur la création de tâches, voir [Création de tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Cet article décrit les considérations, limitations et valeurs par défaut qui s’appliquent lors de la création de tâches.

## Méthodes de création de tâches sur un projet

Vous pouvez créer des tâches sur un projet de la manière suivante :

* À partir de zéro, comme décrit dans la section [Création de tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* Copiez des tâches dans le même projet ou dans un nouveau projet ou dupliquez des tâches sur le même projet, comme décrit dans la section [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Déplacez des tâches d’un projet vers un autre, comme décrit dans la section [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Limites de la création de tâches

Lorsque vous disposez des droits d’accès et des autorisations appropriés, vous pouvez créer des tâches sur un projet. Cependant, voici quelques cas où vous ne pourrez peut-être pas créer de tâches :

* Votre administrateur Adobe Workfront ou un administrateur de groupe doit activer l’ajout de tâches à un projet dont l’état est Terminé ou Mort dans la zone Préférences du projet. Pour plus d’informations sur la définition des préférences de projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Vous ne pouvez pas ajouter de tâches à un projet qui est en attente d’approbation.

## Nombre maximal de tâches autorisées sur un projet

Un projet peut contenir jusqu’à 5 000 tâches. Un message d’avertissement s’affiche sur le projet lorsque vous approchez de la limite, lorsque vous avez atteint la limite et si vous tentez de la dépasser.

Selon le nombre de tâches de vos projets lorsque cette limitation a été imposée, votre instance Workfront peut contenir plus de 5 000 tâches dans un seul projet.

Si vous pouvez inclure plus de 5 000 tâches dans un seul projet, tenez compte des points suivants :

* La limite de tâches de votre environnement Workfront est définie sur le nombre actuel de tâches de votre projet le plus volumineux, plus 10 % de tâches supplémentaires.

   Par exemple, si un projet de votre instance Workfront contient 10 000 tâches, la limite pour chaque projet de votre instance Workfront est de 11 000 tâches.

* Les projets plus petits améliorent les performances et réduisent les défis de gestion liés aux grands projets.

## Tâche par défaut lors de l’ajout de tâches à un projet

Workfront met automatiquement à jour deux types d’informations par défaut pour les tâches lorsque vous les créez :

* Informations par défaut au niveau du système

   Votre administrateur Workfront ou un administrateur de groupe établit les valeurs par défaut au niveau du système pour les tâches dans la zone Tâches et problèmes des préférences du projet. Pour plus d’informations sur les préférences de tâche et de problème, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) ou [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Informations par défaut au niveau du projet

   Le reste de cette section décrit les paramètres par défaut au niveau du projet que vous, en tant que chef de projet, pouvez définir pour toutes les nouvelles tâches ajoutées à un projet.

Lorsque vous ajoutez une tâche à un projet, en fonction de la configuration du projet, Workfront peut lui associer automatiquement un processus d’approbation ou des formulaires personnalisés.

Pour plus d’informations sur la configuration d’un projet pour les ajouter par défaut, reportez-vous à la section &quot;Tâches&quot; du [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md) article.

Lors de la définition des informations par défaut à associer aux tâches ajoutées à un projet au niveau du projet, tenez compte des points suivants :

* Vous devez disposer des autorisations Manage (Gérer) sur le projet pour définir les paramètres par défaut du processus d’approbation des tâches et des formulaires personnalisés.
* Toutes les nouvelles tâches sont créées avec le processus d’approbation et les formulaires personnalisés définis lors de la modification du projet.
* Vous pouvez modifier ces paramètres par défaut lorsque vous ajoutez des tâches à l’aide de la zone Modifier la tâche, mais pas lorsque vous ajoutez des tâches dans la modification en ligne.
* Vous pouvez définir le processus d’approbation et les formulaires personnalisés pour les tâches d’un modèle.

   * Lorsqu’un projet est créé à partir de ce modèle, le processus d’approbation et les formulaires personnalisés sont automatiquement appliqués au projet.
   * Lorsqu’un modèle est joint à un projet existant, le projet conserve le processus d’approbation de tâche d’origine et les paramètres de formulaires personnalisés s’ils sont définis. S’ils ne sont pas définis, les paramètres du modèle deviennent les paramètres du projet.
   * Lorsqu’un modèle est joint à un projet existant, les tâches ajoutées au projet à partir du modèle conservent le processus d’approbation et les paramètres de formulaires personnalisés qu’ils avaient sur le modèle, quels que soient les paramètres de tâche du projet.

   Pour plus d’informations sur l’association d’un modèle à un projet, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Lorsque vous copiez le projet, les paramètres par défaut de la tâche sont transférés vers le nouveau projet.

   Pour plus d’informations sur la copie d’un projet, voir [Copier un projet](../../../manage-work/projects/manage-projects/copy-project.md).

* Lorsque vous copiez des tâches d’un projet vers un autre et que le projet de destination dispose de paramètres par défaut différents pour les tâches, les tâches copiées conservent les paramètres par défaut du projet d’origine, sauf si elles sont effacées lors du processus de copie.
* Lorsque vous dupliquez une tâche sur le même projet, les formulaires personnalisés et le processus d’approbation sont transférés à la tâche en double.

   Pour plus d’informations sur la copie et la duplication de tâches, voir [ [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Lorsque vous déplacez la tâche vers un autre projet, les paramètres de tâche par défaut sont enregistrés sur les tâches du projet d’origine, quels que soient les paramètres par défaut de la tâche sur le nouveau projet.

   Pour plus d’informations sur le déplacement des tâches, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).
