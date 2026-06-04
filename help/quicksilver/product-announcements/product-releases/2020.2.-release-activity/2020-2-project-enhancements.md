---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Améliorations apportées aux projets 2020.2
description: Cette page décrit toutes les améliorations apportées aux projets avec la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
TQID: https://experienceleague.adobe.com/eHXlWWa5b-t-g1m0E896PAbRA13VRZo12XPlccEaGgM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 837
ht-degree: 100%

---

# Améliorations apportées aux projets 2020.2

Cette page décrit toutes les améliorations apportées aux projets avec la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.2, consultez l’article [Présentation de la version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Pour les équipes d’administration Workfront : nouveau mécanisme de sécurité lorsque le statut du projet pour les nouveaux projets est masqué ou déverrouillé.

Dans Configuration, vous configurez une préférence afin de vous assurer que chaque nouveau projet a un certain statut lors de sa création. C’est important, car un projet a toujours besoin d’un statut pour fonctionner correctement dans Workfront, même s’il vient d’être créé.

Pour s’assurer que les nouveaux projets ont toujours un statut, même si un administrateur ou une administratrice masque ou déverrouille le statut configuré pour les nouveaux projets, le système attribue désormais le premier statut de la liste Statut à tous les nouveaux projets jusqu’à ce que vous configuriez à nouveau le statut pour les nouveaux projets.

Pour plus d’informations sur la définition de la préférence pour le statut de tous les nouveaux projets, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (ou si vous utilisez Adobe Workfront Classic, voir [Définir les préférences du projet](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Pour les équipes d’administration Workfront : amélioration de la conception dans les préférences du projet

La définition des préférences d’un projet est désormais plus simple et intuitive :

* Les titres sont plus grands que les libellés d’option afin que vous puissiez trouver plus rapidement ce que vous recherchez.
* Les lignes de séparation et les espaces blancs supplémentaires séparent chaque section afin que vous puissiez vous concentrer plus facilement sur ce que vous faites.
* Si vous saisissez un nombre non valide pour une option telle que « Heures habituelles par journée de travail », un message d’avertissement s’affiche immédiatement au lieu d’apparaître après avoir cliqué sur Enregistrer.
* Les libellés d’option correspondent au texte de l’interface correspondant ailleurs dans Workfront, comme la zone Détails et les rapports.

Pour plus d’informations sur la zone Préférences du projet, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (ou si vous utilisez Adobe Workfront Classic, voir [Définir les préférences du projet](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Filtre, vue et regroupement sélectionnés conservés dans les listes de rapports

Désormais, le dernier filtre, la dernière vue ou le dernier regroupement appliqué à un rapport spécifique est sélectionné, même si l’utilisateur ou l’utilisatrice se déconnecte et se reconnecte à Workfront.

Auparavant, lorsqu’une personne appliquait un filtre, une vue ou un regroupement à une liste de rapports et quittait ensuite cette page, le filtre, la vue ou le regroupement par défaut apparaissait la fois suivante, lorsque la personne accédait à ce même rapport.

**Disponibles dans ces environnements :**

* La nouvelle expérience Adobe Workfront
* Adobe Workfront Classic

## Le déplacement et la copie de tâches vers un autre projet conserve la contrainte de tâche si elles peuvent être intégrées dans la chronologie du projet.

Nous avons amélioré la façon dont Workfront gère la contrainte de tâche spécifique à une date lorsque vous copiez la tâche ou la déplacez vers un autre projet. Des exemples de contraintes de tâche spécifiques à une date comprennent : Il Faut Commencer Le, Doit se terminer le, Dates fixes, Commencer Au Plus Tard, etc.

Par exemple, lorsque vous déplacez ou copiez une tâche avec une contrainte Il Faut Commencer Le vers un autre projet dont la date de début planifiée est antérieure à celle de la tâche, la tâche conserve la contrainte après sa copie ou son déplacement. Lorsque vous déplacez ou copiez une tâche avec une contrainte Il Faut Commencer Le vers un projet dont la date de début planifiée est postérieure à celle de la tâche, la contrainte de tâche passe à Aussi Tôt Que Possible.

Avant cette modification, la contrainte de tâche passait toujours à Aussi Tôt Que Possible.

Pour plus d’informations sur le déplacement des tâches, voir [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md) (ou si vous utilisez Adobe Workfront Classic, voir [Déplacer des tâches](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (ou si vous utilisez Adobe Workfront Classic, voir [Copier et dupliquer des tâches](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

Pour une vue d’ensemble de toutes les contraintes de tâche, voir [Vue d’ensemble de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (ou si vous utilisez Adobe Workfront Classic, voir [Vue d’ensemble de la contrainte de tâche](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Empêcher les pertes de données lors des modifications dans l’onglet Détails ou dans une liste de tâches

Pour éviter toute perte de données lors de la mise à jour d’informations sur la page Détails d’un objet ou des tâches d’une liste de tâches au niveau du projet dans le cas de l’enregistrement manuel des modifications, un message d’avertissement s’affiche désormais avant toute tentative de modification de l’en-tête pour vous informer que des modifications n’ont pas été enregistrées. Les seules actions autorisées avant d’enregistrer vos modifications sont l’abonnement ou l’ajout de l’objet à vos favoris.

Pour plus d’informations sur la modification des tâches dans une liste, voir [Modifier les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponible dans ces environnements :**

* La nouvelle expérience Adobe Workfront

