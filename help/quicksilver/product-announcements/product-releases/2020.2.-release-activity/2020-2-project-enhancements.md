---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Améliorations des projets (version 2020.2)
description: Cette page décrit toutes les améliorations apportées aux projets avec la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Améliorations des projets (version 2020.2)

Cette page décrit toutes les améliorations apportées aux projets avec la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.2, consultez la [présentation de la version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Pour les administrateurs Workfront : nouveau paramètre de sécurité intégrée lorsque l’état du projet pour les nouveaux projets est masqué ou déverrouillé

Dans Configuration, vous configurez une préférence afin de vous assurer que chaque nouveau projet a un certain état lors de sa création. C’est important, car un projet a toujours besoin d’un état pour fonctionner correctement dans Workfront, même s’il est tout nouveau.

Pour s’assurer que les nouveaux projets ont toujours un état, même si un administrateur masque ou déverrouille l’état configuré pour les nouveaux projets, le système attribue désormais le premier état de la liste État à tous les nouveaux projets jusqu’à ce que vous configuriez à nouveau l’état pour les nouveaux projets.

Pour plus d’informations sur la définition des préférences pour l’état de tous les nouveaux projets, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (ou si vous utilisez Adobe Workfront Classic, voir [Définition des préférences du projet](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Pour les administrateurs de Workfront : amélioration de la conception dans les préférences du projet

La définition des préférences d’un projet est désormais plus intuitive et facile à utiliser :

* Les titres sont plus volumineux que les libellés d’option afin que vous puissiez trouver plus rapidement ce que vous recherchez.
* Les lignes de séparation et les espaces blancs supplémentaires séparent chaque section afin que vous puissiez vous concentrer plus facilement sur ce que vous faites.
* Si vous saisissez un nombre non valide pour une option telle que &quot;Heures types par jour de travail&quot;, un message d’avertissement s’affiche immédiatement au lieu d’apparaître après avoir cliqué sur Enregistrer.
* Les libellés d’option correspondent au texte de l’interface correspondant ailleurs dans Workfront, tel que la zone Détails et les rapports.

Pour plus d’informations sur la zone Préférences du projet, voir [Configuration des préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (ou si vous utilisez Adobe Workfront Classic, voir [Définition des préférences du projet](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Filtre, affichage et regroupement sélectionnés conservés dans les listes de rapports

Désormais, le dernier filtre, affichage ou regroupement appliqué à un rapport spécifique est sélectionné, même si l’utilisateur se déconnecte puis se reconnecte à Workfront.

Auparavant, lorsqu’un utilisateur appliquait un filtre, une vue ou un regroupement à une liste de rapports, puis qu’il quittait cette page, le filtre, l’affichage ou le regroupement par défaut s’affichait la prochaine fois que l’utilisateur accédait à ce même rapport.

**Disponible dans ces environnements :**

* Nouvelle expérience Adobe Workfront
* Adobe Workfront Classic

## Le déplacement et la copie de tâches vers un autre projet conserve la contrainte de tâche lorsque les tâches peuvent tenir dans la chronologie du projet.

Nous avons amélioré la manière dont Workfront gère la contrainte de tâche spécifique à la date d’une tâche lorsque vous copiez la tâche ou la déplacez vers un autre projet. Vous trouverez des exemples de contraintes de tâche spécifiques à une date : Doit commencer le, Doit se terminer le, Dates fixes, Ne pas démarrer plus tard que, etc.

Par exemple, lorsque vous déplacez ou copiez une tâche avec une contrainte De démarrage obligatoire vers un autre projet dont la date de début planifiée est antérieure à la date de début planifiée de la tâche, la tâche conserve la contrainte après sa copie ou son déplacement. Lorsque vous déplacez ou copiez une tâche avec une contrainte De démarrage obligatoire vers un projet dont la date de début planifiée est postérieure à la date de début de la tâche, la contrainte de tâche passe à Dès que possible.

Avant cette modification, la contrainte de tâche passe toujours à Dès que possible.

Pour plus d’informations sur le déplacement des tâches, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md) (ou si vous utilisez Adobe Workfront Classic, voir [Déplacement de tâches](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (ou si vous utilisez Adobe Workfront Classic, voir [Copier et dupliquer des tâches](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

Pour obtenir un aperçu de toutes les contraintes de tâche, consultez la [présentation de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (ou si vous utilisez Adobe Workfront Classic, consultez la [présentation de la contrainte de tâche](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Prévention des pertes de données lors des modifications dans l’onglet Détails ou dans une liste de tâches

Pour éviter toute perte de données lorsque vous mettez à jour les informations de la page Détails sur un objet ou des tâches dans une liste de tâches au niveau du projet lors de l’enregistrement manuel des modifications, un message d’avertissement s’affiche maintenant pour vous informer que vous avez enregistré des modifications avant de tenter de modifier les informations dans l’en-tête. Les seules actions autorisées avant d’enregistrer vos modifications sont l’abonnement ou l’ajout de l’objet à vos favoris.

Pour plus d’informations sur l’édition de tâches dans une liste, voir [Modifier les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponible dans ces environnements :**

* Nouvelle expérience Adobe Workfront

