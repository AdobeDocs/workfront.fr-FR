---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: '2020.2 Améliorations de la gestion des ressources : l’équilibreur de charge de travail'
description: Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 0%

---

# 2020.2 Améliorations de la gestion des ressources : l’équilibreur de charge de travail

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.2, voir [Présentation de la version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

Les personnes sont une ressource de niveau 1. Avec l’équilibreur de charge de travail, vous pouvez les protéger contre le épuisement et leur permettre de faire de leur mieux, tout en les alignant sur les stratégies d’entreprise clés. Présentation d’une expérience de planification repensée qui vous permet de visualiser et de gérer les charges de travail et la demande des personnes dans la même vue. L’interface utilisateur fournit une cartographie visuelle claire de la surutilisation et de la sous-utilisation et est transparente pour toutes les parties prenantes. Les gestionnaires de personnes peuvent utiliser ces informations comme entrée et, à partir du même écran, rééquilibrer l’effort par le biais de la chronologie, qui est ensuite répercutée dans le reste de la plateforme Workfront.

>[!NOTE]
>
>L’équilibreur de charge de travail a commencé à sortir en version bêta avec la version 2019.4. Toutes les améliorations de l’équilibreur de charge de travail sont disponibles dans la version 2020.2. Les améliorations décrites sur cette page ont été ajoutées à la version 2020.2. Pour une présentation de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Ajuster l’affectation quotidienne et hebdomadaire dans l’équilibreur de charge de travail

Pour éviter l’épuisement de vos ressources, vous pouvez maintenant ajuster l’allocation quotidienne et hebdomadaire de vos utilisateurs afin qu’elle fonctionne à l’aide de l’équilibreur de charge de travail.

Avant cette amélioration, cela n’était possible qu’à l’aide des outils de planification des ressources.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Filtres d’équilibreur de charge de travail

Pour que les informations de l’équilibreur de charge de travail vous soient utiles, vous pouvez maintenant créer des filtres pour les zones de travail non assigné et de travail assigné de l’équilibreur de charge de travail et les enregistrer pour une utilisation ultérieure. Vous pouvez ensuite modifier la version enregistrée pour y apporter de petites modifications au lieu de commencer de zéro avec un nouveau filtre.

Pour plus d’informations sur le filtrage dans l’équilibreur de charge de travail, voir [Gestion des filtres dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Afficher les heures restantes dans l’équilibreur de charge de travail

Pour vous aider à prendre des décisions d’affectation correctes, un nouveau paramètre vous permet désormais d’afficher la différence d’heures entre les heures qu’un utilisateur est disponible pour travailler selon son planning et les heures qu’il a déjà été affecté au travail (les heures restantes). Le nouveau paramètre est désormais disponible dans l’équilibreur de charge de travail.

Pour plus d’informations sur l’affichage des informations dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Navigation dans l’équilibreur de charge de travail](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).)

**Disponible dans ces environnements :**

* Nouvelle expérience Adobe Workfront

## Afficher les heures planifiées quotidiennes pour les tâches et les projets dans la zone de travail non assignée de l’équilibreur de charge de travail

Pour vous aider à comprendre l’impact des tâches sur la charge de travail de vos utilisateurs avant de les affecter, le paramètre &quot;Afficher les affectations&quot; gère désormais les informations affichées dans la zone Travail non assigné de l’équilibreur de charge de travail. Lorsque ce paramètre est activé, les heures planifiées pour les tâches et les projets s’affichent dans la zone Travail non attribué de l’équilibreur de charge de travail.

Avant cette modification, ce paramètre ne mettait à jour que les informations de la zone Travail affecté de l’équilibreur.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Navigation dans l’équilibreur de charge de travail](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront (auparavant disponible uniquement pour les tâches)

## Nouvelle zone Paramètres de l’équilibreur de charge de travail

Pour simplifier votre expérience, une boîte Paramètres affiche désormais des outils supplémentaires pour mettre à jour la vue dans l’équilibreur de charge de travail. Cette zone comprend les paramètres suivants :

* Regrouper par projet
* Affichez les heures affectées ou les heures restantes pour vos tâches et projets.

Pour plus d’informations sur l’affichage des informations dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Navigation dans l’équilibreur de charge de travail](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Partage de l’équilibreur de charge de travail avec un lien

Vous pouvez maintenant partager la charge de travail de vos employés avec les cadres afin qu&#39;ils puissent avoir un contexte sur vos besoins en personnel. Pour ce faire, vous pouvez maintenant partager l’équilibreur de charge de travail en partageant une URL unique avec l’équilibreur de charge de travail avec n’importe qui d’autre.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Navigation dans l’équilibreur de charge de travail](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Modification de la période dans l’équilibreur de charge de travail

Pour vous aider à personnaliser davantage la durée de la chronologie de l’équilibreur de charge de travail en fonction de vos besoins, vous pouvez maintenant sélectionner une période personnalisée de 2, 4 ou 6 semaines à afficher simultanément.

Avant cette amélioration, l’équilibreur de charge de travail affichait toujours les informations à partir de la semaine en cours.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Navigation dans l’équilibreur de charge de travail](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront (précédemment disponible)

## Le déplacement et la copie de tâches vers un autre projet conserve la contrainte de tâche lorsque les tâches peuvent tenir dans la chronologie du projet.

Nous avons amélioré la manière dont Workfront gère la contrainte de tâche spécifique à la date d’une tâche lorsque vous copiez la tâche ou la déplacez vers un autre projet. Vous trouverez des exemples de contraintes de tâche spécifiques à une date : Doit commencer le, Doit se terminer le, Dates fixes, Ne pas démarrer plus tard que, etc.

Par exemple, lorsque vous déplacez ou copiez une tâche avec une contrainte De démarrage obligatoire vers un autre projet dont la date de début planifiée est antérieure à la date de début planifiée de la tâche, la tâche conserve la contrainte après sa copie ou son déplacement. Lorsque vous déplacez ou copiez une tâche avec une contrainte De démarrage obligatoire vers un projet dont la date de début planifiée est postérieure à la date de début de la tâche, la contrainte de tâche passe à Dès que possible.

Avant cette modification, la contrainte de tâche passe toujours à Dès que possible.

Pour plus d’informations sur le déplacement des tâches, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md) (ou si vous utilisez Adobe Workfront Classic, voir [Déplacement de tâches](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

Pour plus d’informations sur la copie de tâches, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (ou si vous utilisez Adobe Workfront Classic, voir [Copier et dupliquer des tâches](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

Pour une présentation de toutes les contraintes de tâche, voir [Présentation de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (ou si vous utilisez Adobe Workfront Classic, voir [Présentation de la contrainte de tâche](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Prévention des pertes de données lors des modifications dans l’onglet Détails ou dans une liste de tâches

Pour éviter toute perte de données lorsque vous mettez à jour les informations de la page Détails sur un objet ou des tâches dans une liste de tâches au niveau du projet lors de l’enregistrement manuel des modifications, un message d’avertissement s’affiche maintenant pour vous informer que vous avez enregistré des modifications avant de tenter de modifier les informations dans l’en-tête. Les seules actions autorisées avant d’enregistrer vos modifications sont l’abonnement ou l’ajout de l’objet à vos favoris.

Pour plus d’informations sur la modification des tâches dans une liste, voir [Editer les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponible dans ces environnements :**

* Nouvelle expérience Adobe Workfront

## Créer des processus d’approbation pour les groupes utilisant des états personnalisés

Afin de faciliter la gestion de leurs propres workflows uniques par les groupes, vous pouvez désormais utiliser des états personnalisés spécifiques aux groupes dans les processus d’approbation.

Auparavant, un groupe ne pouvait pas utiliser ses propres états personnalisés avec ses processus d’approbation spécifiques au groupe. Seuls les états à l’échelle du système étaient disponibles et ceux-ci ne correspondaient pas toujours aux processus d’approbation de groupe.

Les états personnalisés peuvent désormais être utilisés dans les processus d’approbation à usage unique et à l’échelle du système :

* Créez un processus d’approbation à usage unique pour un objet (projet, tâche ou problème) et basez-le sur les états associés au groupe travaillant sur cet objet. Cela inclut tous les états personnalisés associés au groupe.
* Créez un processus d’approbation globale et rendez-le disponible uniquement pour le groupe ou pour toutes les personnes du système.

Pour les utilisateurs disposant d’un accès administratif aux processus de validation, des informations sur la configuration des processus de validation sont disponibles dans [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (ou si vous utilisez Adobe Workfront Classic, voir [Création de processus de validation](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

Pour les utilisateurs, des informations sur l’association des processus d’approbation aux tâches sont disponibles dans [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (ou si vous utilisez Adobe Workfront Classic, voir [Association d’un processus d’approbation nouveau ou existant à un travail](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront

## Une méthode plus pratique pour mettre à jour les allocations dans l’équilibreur de charge de travail

Pour faciliter la gestion des affectations d’un utilisateur à un élément de travail dans l’équilibreur de charge de travail, vous pouvez maintenant double-cliquer sur l’élément de travail. Vous pouvez également continuer à utiliser l’option de menu Modifier les affectations existante. En outre, vous n’avez plus besoin d’activer l’affichage des allocations pour pouvoir les mettre à jour.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Mise à jour des heures planifiées de la tâche dans l’équilibreur de charge

>[!NOTE]
>
>Cette amélioration sera disponible dans Production peu de temps après la version 2020.2.

Une nouvelle option de la zone Gestion des ressources du niveau d’accès permet désormais aux utilisateurs disposant de cet accès de modifier les heures planifiées à partir de l’équilibreur de charge de travail. Lorsque vous ajustez les affectations dans l’équilibreur de charge de travail, le total des affectations quotidiennes n’a pas besoin de correspondre au nombre d’heures planifiées des tâches. Une fois les affectations enregistrées, le total des heures d’affectation devient les Heures planifiées de la tâche. Cela n’est possible que pour les tâches ayant un type de durée simple.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Pour plus d’informations sur l’octroi de l’accès à la gestion des ressources, voir [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Suppression du libellé &quot;bêta&quot; de l’équilibreur de charge de travail

Avec la version 2020.2, l’équilibreur de charge de travail ne sera plus en version bêta et vous pourrez utiliser l’équilibreur de ressources pour examiner et gérer vos affectations et affectations de ressources. Le libellé &quot;bêta&quot; a été supprimé dans l’environnement Aperçu. Cette même modification sera apportée à la version de production 20.2. Pour plus d’informations sur l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
