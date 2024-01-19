---
title: 20.4 Améliorations de la gestion des ressources
description: 20.4 Améliorations de la gestion des ressources
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# 20.4 Améliorations de la gestion des ressources

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 20.4 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production durant la semaine du 9 novembre 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 20.4, voir [Présentation de la version 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Planifier le travail à l’aide de l’effort de travail au lieu des heures planifiées

Pour vous donner de la flexibilité lorsque vous planifiez le travail sur vos projets, nous avons introduit le nouveau concept d’effort de travail pour les tâches. Vous pouvez estimer si l’effort de travail d’une tâche est petit, moyen ou volumineux sans estimer manuellement les heures planifiées de la tâche. Chaque niveau d’effort est calculé sur la base d’un pourcentage du temps provenant des heures typiques par jour configurées dans votre instance.

Les améliorations suivantes sont désormais disponibles avec cette nouvelle fonctionnalité :

* Activer ce paramètre pour les projets et les modèles afin de le rendre disponible pour les tâches et les tâches de modèle
* Mettez à jour ce paramètre pour chaque tâche avec un type de durée simple qui met automatiquement à jour les heures planifiées de la tâche.
* Désactivez ce paramètre à l’aide d’un modèle de mise en page pour les utilisateurs qui préfèrent continuer à utiliser les heures planifiées.
* Afficher la valeur de ce nouveau champ dans une liste de tâches ou un rapport.

Pour plus d’informations sur l’effort de travail, voir [Présentation de l’effort de travail](../../../manage-work/tasks/task-information/work-effort.md).

Cette fonctionnalité est désormais incluse dans la variable [Principes de planification, deuxième partie du parcours d&#39;apprentissage](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-20Y0z000000bm79EAA) sur Workfront One.

## Couleurs basées sur l’état du projet pour les tâches dans l’équilibreur de charge de travail

Pour une meilleure visibilité et une personnalisation accrue de votre expérience dans l’équilibreur de charge de travail, vous pouvez désormais modifier les couleurs des projets et de leurs tâches afin qu’elles correspondent à l’état des projets. Les couleurs correspondent aux états de projet au niveau du groupe ou du système. Les couleurs affichées peuvent correspondre aux états du système et des projets personnalisés.

Pour plus d’informations sur la personnalisation de la vue dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajuster l’affectation des utilisateurs à l’aide de valeurs de pourcentage dans l’équilibreur de charge de travail

Vous pouvez désormais gérer les affectations de vos utilisateurs dans l’équilibreur de charge de travail à l’aide de pourcentages plutôt que d’heures.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Afficher ou masquer les tâches terminées dans l’équilibreur de charge de travail

Un nouveau paramètre permet désormais d’afficher ou de masquer les tâches terminées dans l’équilibreur de charge de travail. Le paramètre est activé par défaut et les tâches terminées qui correspondent aux critères de filtrage et la période sélectionnée s’affichent dans l’équilibreur de charge de travail.

Avant cette amélioration, les tâches terminées s’affichaient toujours dans l’équilibreur de charge de travail.

Pour plus d’informations sur l’ajustement des paramètres dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Améliorations de l’utilisation de l’équilibreur de charge de travail

Pour garantir une expérience simplifiée et conviviale lors de la gestion de vos ressources dans l’équilibreur de charge de travail, les améliorations de convivialité suivantes sont désormais disponibles :

* Vous pouvez désormais ouvrir le résumé des problèmes et des tâches à partir de l’icône Résumé au lieu du menu Plus . Cette expérience est désormais cohérente avec celle des listes.

  >[!NOTE]
  >
  >Cette option est disponible uniquement dans la nouvelle expérience Adobe Workfront.

* Vous pouvez accéder au menu Plus à gauche d’une barre d’objets plutôt qu’à la fin d’une barre d’objets. Cela facilite la recherche lorsque les objets s’étendent sur une longue période.
* Vous pouvez accéder aux fonctions d’affectation à l’aide d’un raccourci clavier. Auparavant, cette option n’était disponible que dans le menu Plus .
* Vous pouvez charger tous les éléments restants sous le nom d’un utilisateur au lieu des 20 éléments suivants en cliquant sur Charger plus.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Graphique d’affectation des utilisateurs dans l’équilibreur de charge de travail

Pour vous permettre d’avoir une représentation visuelle de haut niveau de l’allocation des utilisateurs au cours d’une période donnée, un nouveau paramètre permet désormais un affichage sous forme de graphique de la façon dont les allocations sont affichées dans l’équilibreur de charge de travail. L’activation de ce paramètre affiche l’allocation des utilisateurs dans un graphique en courbes qui indique les suraffectations en blocs rouges et les sous-affectations en bleu.

Pour plus d’informations sur la configuration des paramètres dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualiser le travail terminé dans l’équilibreur de charge de travail

Pour vous permettre d’identifier facilement le travail déjà terminé afin que vous puissiez gérer correctement les affectations des utilisateurs, nous avons activé un indicateur visuel dans l’équilibreur de charge de travail qui indique le moment où les éléments d’une période sélectionnée ont été terminés. Vous pouvez désormais voir une coche verte pour les tâches, les problèmes une fois qu’elles sont terminées. Le projet affiche également la coche verte lorsque des tâches sont terminées pendant la période affichée à l’écran.

Pour plus d’informations sur l’affichage des informations dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Nouveau filtre par défaut pour la zone de travail affectée dans l’équilibreur de charge de travail

Le filtre par défaut de la zone de travail affectée dans l’équilibreur de charge de travail affiche désormais uniquement les utilisateurs qui sont membres de toutes les équipes auxquelles vous, en tant qu’utilisateur connecté, êtes associé. Le nouveau filtre affiche désormais par défaut les informations les plus pertinentes.

Avant cette amélioration, tous les utilisateurs auxquels vous avez accès s’affichaient dans cette zone.

Pour plus d’informations sur l’utilisation de filtres dans l’équilibreur de charge de travail, voir [Gestion des filtres dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nouvelle icône pour basculer entre les heures et les valeurs de pourcentage, ou entre le temps alloué et le temps restant dans l’équilibreur de charge de travail

Nous avons ajouté un nouveau paramètre qui vous permet de basculer entre les heures allouées et les pourcentages lorsque vous affichez l’équilibreur de charge de travail. Avec cette nouvelle icône, nous avons également supprimé la section Charge de travail de l’utilisateur du panneau Paramètres. L’équilibreur de charge de travail affiche le temps alloué par défaut et nous avons déplacé le paramètre Autres heures vers la nouvelle icône Pourcentage ou Heures .

Cette amélioration élimine les clics et rend la navigation dans l’équilibreur de charge de travail plus facile et plus efficace.

Pour plus d’informations sur la gestion des paramètres de l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Un nouveau filtre intégré pour l’équilibreur de charge de travail : utilisateurs sur les projets

Pour optimiser votre expérience de filtrage dans l’équilibreur de charge de travail, nous avons ajouté un nouveau filtre intégré dans la zone Travail affecté . Vous pouvez maintenant appliquer le filtre Utilisateurs sur les projets qui affiche les utilisateurs affectés aux tâches et problèmes dans les projets que vous spécifiez.

Pour plus d’informations sur l’utilisation de filtres dans l’équilibreur de charge de travail, voir [Filtrage des informations dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

