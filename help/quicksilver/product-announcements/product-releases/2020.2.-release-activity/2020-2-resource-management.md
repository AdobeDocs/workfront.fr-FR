---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 'Améliorations de la gestion des ressources (version 2020.2) : équilibreur de charge de travail'
description: Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 99%

---

# Améliorations de la gestion des ressources (version 2020.2) : équilibreur de charge de travail

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.2, consultez l’article [Présentation de la version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

Les personnes sont des ressources de premier ordre. Avec l’équilibreur de charge de travail, vous pouvez les protéger contre l’épuisement tout en leur permettant de donner leur maximum et en les alignant sur les stratégies clés de l’entreprise. Présentation d’une expérience de planification repensée qui vous permet de visualiser et de gérer les charges de travail et la demande des personnes au même endroit. L’interface utilisateur fournit un mappage visuel clair de la surutilisation et de la sous-utilisation et reste transparente pour toutes les parties prenantes. Dans le même écran, les personnes gestionnaires du personnel peuvent utiliser ces informations comme entrée et rééquilibrer les tâches dans le journal. Ceci est ensuite répercuté dans le reste de la plateforme Workfront.

>[!NOTE]
>
>La première version de l’équilibreur de charge de travail était la version bêta 2019.4. Toutes les améliorations de l’équilibreur de charge de travail sont disponibles dans la version 2020.2. Les améliorations décrites sur cette page ont été ajoutées à la version 2020.2. Pour une vue d’ensemble de l’équilibreur de charge de travail, consultez [Vue d’ensemble de l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Ajuster les affectations quotidiennes et hebdomadaires dans l’équilibreur de charge de travail

Pour éviter l’épuisement de vos ressources, vous pouvez maintenant ajuster l’affectation quotidienne et hebdomadaire de vos utilisateurs et utilisatrices à l’aide de l’équilibreur de charge de travail.

Avant cette amélioration, cela n’était possible qu’à l’aide des outils de planification des ressources.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**Disponibles dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Filtres de l’équilibreur de charge de travail

Pour que les informations de l’équilibreur de charge de travail vous soient utiles, vous pouvez maintenant créer des filtres pour les zones de travail non affecté et de travail affecté de l’équilibreur de charge de travail et les enregistrer pour une utilisation ultérieure. Vous pouvez ensuite modifier la version enregistrée pour y apporter de légères modifications au lieu de commencer de zéro avec un nouveau filtre.

Pour plus d’informations sur le filtrage dans l’équilibreur de charge de travail, consultez [Gérer les filtres dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**Disponibles dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Afficher les heures restantes dans l’équilibreur de charge de travail

Pour vous aider à prendre de bonnes décisions d’affectation, un nouveau paramètre vous permet désormais d’afficher la différence entre les heures de disponiblité du planning de travail d’un utilisateur ou d’une utilisatrice et ses heures déjà affectées (heures restantes). Le nouveau paramètre est désormais disponible dans l’équilibreur de charge de travail.

Pour plus d’informations sur l’affichage des informations dans l’équilibreur de charge de travail, consultez [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, [Naviguer dans l’équilibreur de charge de travail](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponibles dans ces environnements :**

* La nouvelle expérience Adobe Workfront

## Afficher le nombre d’heures prévues par jour pour les tâches et les projets dans la zone Travail non affecté de l’équilibreur de charge de travail

Pour vous aider à comprendre l’impact des tâches sur la charge de travail de vos utilisateurs et utilisatrices avant de les affecter, le paramètre « Afficher les allocations » gère désormais les informations affichées dans la zone Travail non affecté de l’équilibreur de charge de travail. Lorsque ce paramètre est activé, le nombre d’heures prévues pour les tâches et les projets s’affiche dans la zone Travail non attribué de l’équilibreur de charge de travail.

Avant cette modification, ce paramètre ne mettait à jour que les informations de la zone Travail affecté de l’équilibreur.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Naviguer dans l’équilibreur de charge de travail](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront (disponible précédemment pour les tâches uniquement)

## Nouvelle zone Paramètres dans l’équilibreur de charge de travail

Pour simplifier votre expérience, une zone Paramètres affiche désormais des outils supplémentaires pour mettre à jour la vue dans l’équilibreur de charge de travail. Cette zone comprend les paramètres suivants :

* Regrouper par projet
* Affichez les heures affectées ou les heures restantes pour vos tâches et projets.

Pour plus d’informations sur l’affichage des informations dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Naviguer dans l’équilibreur de charge de travail](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponibles dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Partager l’équilibreur de charge de travail avec un lien

Vous pouvez désormais partager la charge de travail de vos collaborateurs et collaboratrices avec les dirigeantes et dirigeants afin qu’ils puissent connaître vos besoins en personnel. Pour ce faire, vous pouvez désormais partager l’équilibreur de charge de travail en communiquant à d’autres personnes une URL unique vers l’équilibreur de charge de travail.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Naviguer dans l’équilibreur de charge de travail](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Modifier la période dans l’équilibreur de charge de travail

Pour vous aider à personnaliser la durée de la chronologie de l’équilibreur de charge de travail en fonction de vos besoins, vous pouvez désormais sélectionner une période personnalisée de 2, 4 ou 6 semaines à afficher en une seule fois.

Avant cette amélioration, l’équilibreur de charge de travail affichait toujours les informations à partir de la semaine en cours.

Pour plus d’informations sur la navigation dans l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou si vous utilisez Adobe Workfront Classic, voir [Naviguer dans l’équilibreur de charge de travail](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponible dans ces environnements :**

* Adobe Workfront Classic
* Nouvelle expérience Adobe Workfront (disponible précédemment)

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

Lors de l’enregistrement manuel des modifications effectuées sur la page Détails du projet ou des tâches dans une liste de tâches à l’échelle du projet., un message d’avertissement s’affiche pour vous informer que vous avez enregistré des modifications avant que vous ne tentiez de modifier les informations dans l’en-tête. Cela est fait afin d’éviter toute perte de données lorsque vous mettez à jour les informations de ces éléments. Les seules actions autorisées avant d’enregistrer vos modifications sont l’abonnement ou l’ajout de l’objet à vos favoris.

Pour plus d’informations sur la modification des tâches dans une liste, voir [Modifier les tâches dans une liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponible dans ces environnements :**

* La nouvelle expérience Adobe Workfront

## Créer des processus d’approbation pour les groupes utilisant des statuts personnalisés

Afin qu’il soit plus facile pour les groupes de gérer leurs propres workflows uniques, vous pouvez désormais utiliser des statuts personnalisés spécifiques aux groupes dans les processus d’approbation.

Auparavant, un groupe ne pouvait pas utiliser ses propres statuts personnalisés avec ses processus d’approbation spécifiques aux groupes. Seuls les statuts à l’échelle du système étaient disponibles et ceux-ci ne correspondaient pas toujours aux processus d’approbation des groupes.

Les statuts personnalisés peuvent désormais être utilisés dans les processus d’approbation à usage unique et à l’échelle du système :

* Créez un processus d’approbation à usage unique pour un objet (projet, tâche ou problème) et basez-le sur les statuts associés au groupe travaillant sur cet objet. Cela inclut tous les statuts personnalisés associés au groupe.
* Créez un processus d’approbation global et rendez-le disponible pour le groupe uniquement ou pour toutes les personnes du système.

Pour les utilisateurs et utilisatrices disposant d’un accès administratif aux processus d’approbation, des informations sur la configuration des processus d’approbation sont disponibles dans [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (ou, si vous utilisez Adobe Workfront Classic, consultez [Créer un processus d’approbation](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

Pour les utilisateurs et utilisatrices, des informations sur l’association des processus d’approbation aux éléments de travail sont disponibles dans [Associer un processus d’approbation nouveau ou existant à un travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (ou, si vous utilisez Adobe Workfront Classic, consultez [Associer un processus d’approbation nouveau ou existant à un travail](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

**Disponibles dans ces environnements :**

* Adobe Workfront Classic
* La nouvelle expérience Adobe Workfront

## Méthode plus pratique pour mettre à jour les affectations dans l’équilibreur de charge de travail

Pour faciliter la gestion des affectations d’un utilisateur ou d’une utilisatrice à un élément de travail dans l’équilibreur de charge de travail, vous pouvez maintenant double-cliquer sur l’élément de travail. Vous pouvez également continuer à utiliser l’option de menu Modifier les allocations existante. En outre, vous n’avez plus besoin d’activer l’affichage des affectations pour pouvoir les mettre à jour.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir [Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Mettre à jour le nombre d’heures prévues dans l’équilibreur de charge de travail

>[!NOTE]
>
>Cette amélioration sera disponible dans l’environnement de production peu de temps après la version 2020.2.

Une nouvelle option de la zone Gestion des ressources du niveau d’accès permet désormais aux personnes disposant de cet accès de modifier le nombre d’heures prévues à partir de l’équilibreur de charge de travail. Lorsque vous ajustez les affectations dans l’équilibreur de charge de travail, le total des affectations quotidiennes n’a pas besoin de correspondre au nombre d’heures prévues des tâches. Une fois les affectations enregistrées, le total des heures d’affectation devient le nombre d’heures prévues de la tâche. Cela n’est possible que pour les tâches ayant un type de durée simple.

Pour plus d’informations sur la gestion des affectations dans l’équilibreur de charge de travail, voir la section [Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Pour plus d’informations sur l’octroi de l’accès à la gestion des ressources, voir [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Suppression du libellé « bêta » de l’équilibreur de charge de travail

Avec la version 2020.2, l’équilibreur de charge de travail ne sera plus en version bêta et vous pourrez utiliser l’équilibreur de ressource pour passer en revue et gérer vos affectations et allocations de ressources. Le libellé « bêta » a été supprimé dans l’environnement de prévisualisation. Cette même modification sera apportée avec la version de production 20.2. Pour plus d’informations sur l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
