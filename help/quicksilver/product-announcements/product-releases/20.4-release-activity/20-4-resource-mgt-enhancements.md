---
title: Améliorations de la gestion des ressources (version 20.4)
description: Améliorations de la gestion des ressources (version 20.4)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 99%

---

# Améliorations de la gestion des ressources (version 20.4)

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 20.4 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 9 novembre 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 20.4, voir [Vue d’ensemble de la version 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Planifier le travail en utilisant l’effort de travail au lieu du nombre d’heures prévues

Pour vous donner de la flexibilité lorsque vous planifiez le travail sur vos projets, nous avons introduit le nouveau concept d’effort de travail pour les tâches. Vous pouvez estimer si l’effort de travail pour une tâche est faible, moyen ou important sans estimer manuellement le nombre d’heures prévues pour la tâche. Chaque niveau d’effort est calculé sur la base d’un pourcentage de temps par rapport aux heures typiques par jour telles qu’elles sont configurées dans votre instance.

Les améliorations suivantes sont désormais disponibles avec cette nouvelle fonctionnalité :

* Activez ce paramètre pour les projets et les modèles afin qu’il soit disponible pour les tâches et les modèles de tâches.
* Mettez à jour ce paramètre pour chaque tâche avec un type de durée simple qui met automatiquement à jour le nombre d’heures prévues de la tâche.
* Désactivez ce paramètre à l’aide d’un modèle de disposition pour les personnes qui préfèrent continuer à utiliser le nombre d’heures prévues.
* Affichez la valeur de ce nouveau champ dans une liste de tâches ou un rapport.

Pour plus d’informations sur l’effort de travail, voir [Vue d’ensemble de l’effort de travail](../../../manage-work/tasks/task-information/work-effort.md).

Cette fonctionnalité est désormais incluse dans le [parcours de formation Principes de planification, partie 2](https://experienceleague.adobe.com/en/docs/workfront/using/home) sur Workfront One.

## Couleurs basées sur le statut du projet pour les éléments de travail dans l’équilibreur de charge de travail

Pour une meilleure visibilité et une personnalisation accrue de votre expérience dans l’équilibreur de charge de travail, vous pouvez maintenant changer les couleurs des projets et de leurs éléments de travail pour qu’elles correspondent au statut des projets. Les couleurs correspondent aux statuts des projets au niveau du groupe ou du système. Les couleurs affichées peuvent correspondre au statut du système ainsi qu’au statut des projets personnalisés.

Pour plus d’informations sur la personnalisation de la vue dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajuster l’affectation des personnes à l’aide de valeurs en pourcentage dans l’équilibreur de charge de travail.

Vous pouvez désormais gérer les affectations des personnes dans l’équilibreur de charge de travail en utilisant des pourcentages au lieu d’heures.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gérer les affectations de personnes dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Afficher ou masquer les travaux terminés dans l’équilibreur de charge de travail

Un nouveau paramètre permet désormais d’afficher ou de masquer les éléments de travail terminés dans l’équilibreur de charge de travail. Le paramètre est activé par défaut et les éléments de travail terminés qui correspondent aux critères de filtrage et à la période sélectionnée s’affichent dans l’équilibreur de charge de travail.

Avant cette amélioration, les éléments de travail terminés s’affichaient toujours dans l’équilibreur de charge de travail.

Pour plus d’informations sur l’ajustement des paramètres dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Améliorations apportées à la convivialité dans l’équilibreur de charge de travail

Afin de garantir une expérience rationalisée et conviviale lorsque vous gérez vos ressources dans l’équilibreur de charge de travail, les améliorations suivantes sont désormais disponibles :

* Vous pouvez désormais ouvrir le résumé des problèmes et des tâches à partir de l’icône Résumé au lieu du menu Plus. Cette expérience est désormais conforme à celle des listes.

  >[!NOTE]
  >
  >Cette option n’est disponible que dans la nouvelle expérience Adobe Workfront.

* Vous pouvez accéder au menu Plus à gauche d’une barre d’objets plutôt qu’à la fin d’une barre d’objets. Cela facilite la recherche lorsque les objets couvrent une longue période de temps.
* Vous pouvez accéder aux fonctions d’affectation à l’aide d’un raccourci clavier. Auparavant, cette fonction n’était disponible que dans le menu Plus.
* Vous pouvez charger tous les éléments restants sous le nom d’une personne au lieu des 20 éléments suivants en cliquant sur Charger plus.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Graphique d’affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail

Pour vous permettre d’avoir une représentation visuelle générale des affectations des personnes dans un laps de temps donné, un nouveau paramètre active désormais une vue graphique pour l’affichage des affectations dans l’équilibreur de charge de travail. L’activation de ce paramètre permet d’afficher les affectations des personnes dans un graphique linéaire qui indique les suraffectations dans des blocs rouges et les sous-affectations dans des blocs bleus.

Pour plus d’informations sur la configuration des paramètres dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualiser le travail terminé dans l’équilibreur de charge de travail

Pour vous permettre d’identifier facilement le travail qui a déjà été effectué afin de gérer correctement les affectations des personnes, nous avons activé un indicateur visuel dans l’équilibreur de charge de travail qui montre quand les éléments d’une période sélectionnée ont été terminés. Vous pouvez maintenant voir une coche verte pour les tâches et les problèmes lorsqu’ils sont terminés. Le projet affiche également la coche verte lorsque des éléments de travail ont été effectués pendant la période affichée à l’écran.

Pour plus d’informations sur l’affichage d’informations dans l’équilibreur de charge de travail, voir [Parcourir l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Nouveau filtre par défaut pour la zone de travail affecté dans l’équilibreur de charge de travail

Le filtre par défaut de la zone de travail affecté dans l’équilibreur de charge de travail affiche désormais uniquement les utilisateurs et utilisatrices qui sont membres de toutes les équipes auxquelles vous êtes associée en tant que personne connectée. Le nouveau filtre affiche désormais par défaut les informations les plus pertinentes.

Avant cette amélioration, tous les utilisateurs et utilisatrices auxquels vous aviez accès s’affichaient dans cette zone.

Pour plus d’informations sur l’utilisation des filtres dans l’équilibreur de charge de travail, voir [Gérer les filtres dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nouvelle icône permettant de basculer entre les heures et les pourcentages, ou entre le temps alloué et le temps restant dans l’équilibreur de charge de travail.

Nous avons ajouté un nouveau paramètre qui vous permet de basculer entre les heures allouées et les pourcentages lorsque vous visualisez l’équilibreur de charge de travail. Avec cette nouvelle icône, nous avons également supprimé la section sur la charge de travail de l’utilisateur ou de l’utilisatrice dans le panneau Paramètres. L’équilibreur de charge de travail affiche par défaut le temps alloué, et le paramètre Heures restantes a été déplacé vers la nouvelle icône Pourcentage ou Heures.

Cette amélioration élimine les clics et rend la navigation dans l’équilibreur de charge de travail plus facile et plus efficace.

Pour plus d’informations sur la gestion des paramètres de l’équilibreur de charge de travail, consultez la section [Parcourir l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Nouveau filtre intégré pour l’équilibreur de charge de travail : Utilisateurs et utilisatrices travaillant sur les projets

Afin de rendre votre expérience de filtrage dans l’équilibreur de charge de travail plus efficace, un nouveau filtre intégré a été ajouté dans la zone Travail affecté. Vous pouvez maintenant appliquer le filtre Utilisateurs et utilisatrices travaillant sur les projets qui affiche les utilisateurs et les utilisatrices affectés aux tâches et aux problèmes dans les projets que vous spécifiez.

Pour plus d’informations sur l’utilisation des filtres dans l’équilibreur de charge de travail, consultez la section [Filtrer des informations dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

