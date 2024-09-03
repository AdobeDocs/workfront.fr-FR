---
product-area: projects
navigation-topic: plan-a-project
title: Déterminer la structure de répartition du travail dans un projet
description: La définition d’une structure de répartition du travail (WBS) pour un projet est un ensemble d’activités qui, en fin de compte, décrivent le plan du projet. La structure WBS divise le résultat du projet en éléments de travail gérables, qui peuvent être utilisés pour définir des jalons et organiser des affectations de travail.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '1750'
ht-degree: 100%

---

# Déterminer la structure de répartition du travail dans un projet

La définition d’une structure de répartition du travail (WBS) pour un projet est un ensemble d’activités qui, en fin de compte, décrivent le plan du projet. La structure WBS divise le résultat du projet en éléments de travail gérables, qui peuvent être utilisés pour définir des jalons et organiser des affectations de travail.

Pour créer la structure de répartition du travail d’un projet, vous devez disposer d’une licence Plan avec l’accès Modifier aux projets. Un accès supplémentaire à d’autres zones d’Adobe Workfront peut être nécessaire, en fonction du nombre d’activités que vous effectuez lors de la création de la structure WBS.

Nous vous recommandons de conserver le statut Planification pendant que vous modifiez la structure de répartition du travail, afin d’éviter que des notifications ne se déclenchent pour les personnes membres de l’équipe de projet.

## Définir les éléments livrables du projet

L’objectif d’un projet est de fournir des éléments livrables tangibles aux parties prenantes internes et externes. Les éléments livrables d’un projet sont les résultats que vous souhaitez obtenir en exécutant le projet. Les résultats sont presque toujours associés à au moins un élément livrable et tous les éléments livrables doivent être associés à un projet.

Les éléments livrables du projet peuvent être des biens de consommation, des produits intellectuels (comme les rapports) ou des services. Par exemple, si la portée de votre projet est de construire une maison, certains éléments livrables peuvent inclure ce qui suit :

* Créer des plans architecturaux
* Terminer la plomberie
* Travail électrique
* Couler les fondations
* Travail de charpente
* Vente de la maison.

En fonction de sa taille et de sa portée, un projet peut être constitué de plusieurs éléments livrables.

Une fois que vous avez identifié vos éléments livrables, vous pouvez commencer à les répartir en tâches. Les tâches sont ce que vous accomplissez afin de fournir votre résultat global pour le projet. Lors de la définition de vos tâches, vous prenez en compte les paramètres suivants :

* Temps requis pour l’accomplissement.
* Budget nécessaire pour effectuer le travail.
* Ressources requises pour effectuer le travail.
* Planification des ressources en fonction de la chronologie logique des tâches.

Lorsque vous définissez des tâches, veillez à ne pas planifier trop de travail pour une seule tâche. Si le travail requis sur une tâche est supérieur à 40 heures (une semaine de travail type), vous devrez peut-être ventiler cette quantité de travail dans des sous-tâches. L’achèvement de toutes les sous-tâches terminera alors la tâche principale.

Pour définir les résultats de la structure WBS et les éléments livrables dans Workfront, nous vous recommandons d’exécuter les activités suivantes afin de créer une vue hiérarchique des tâches de projet :

* Si vous ne l’avez pas déjà fait, créez un projet.\
  Pour plus d’informations sur la création d’un projet, voir l’article [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

* Créez des tâches pour tous les éléments d’action requis pour obtenir chaque résultat et chaque élément livrable.\
  Pour plus d’informations sur la création de tâches, voir l’article [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

* À partir des tâches que vous venez de créer, identifiez celles qui sont des résultats majeurs et associez-les aux jalons.\
  Pour plus d’informations sur la création de tâches jalonnées, voir les articles [Créer un chemin jalonné](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) et [Associer des jalons à des tâches](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Ventilez les tâches avec une portée trop grande en sous-tâches. Associez-les à la tâche parent qui définit votre élément livrable.\
  Pour plus d’informations sur la création de sous-tâches, voir l’article [Créer des sous-tâches](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identifiez les relations de dépendance entre les sous-tâches et entre les jalons.\
  Dans une relation de dépendance, le début d’une tâche dépend de l’achèvement d’une autre tâche ou d’un groupe de tâches.\
  Pour plus d’informations sur les dépendances des tâches, voir les articles [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) et [Créer une relation d’antériorité dans la liste des tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Déterminez si, à un moment quelconque de la durée de vie du projet, des approbations et des révisions sont nécessaires. Créez des processus d’approbation pour répondre à ce besoin.\
  Pour plus d’informations sur les approbations, voir l’article [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Estimer le planning de travail et les contraintes de planification

Une fois que vous avez créé le jalon de base et la structure de tâche du projet, vous pouvez estimer le temps nécessaire pour terminer le projet global en définissant les contraintes et les durées de tâche.

Tenez compte des points suivants :

* Les contraintes de tâche définissent le moment où le travail sur une tâche doit commencer ou se terminer.

  Pour plus d’informations sur la définition des contraintes de tâche, voir l’article [Vue d’ensemble de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* La durée d’une tâche correspond au délai pour terminer une tâche. Lors de l’estimation de la durée, vous pouvez saisir une valeur qui prend en compte la possibilité d’un retard. Si des projets similaires ont été réalisés dans le passé, vous pouvez avoir une idée de comment définir cette valeur.

  Comme la durée est une estimation, veillez à définir des valeurs temporelles optimistes afin de tenir compte des facteurs pouvant affecter la tâche, tels que les conditions météorologiques, les pannes de courant, les difficultés avec les fournisseurs ou d’autres événements imprévus. En outre, veillez à examiner s’il existe des tâches antérieures ou de dépendance associées, et comment elles peuvent imposer des contraintes de travail et affecter l’achèvement de la tâche.

  Selon le type de durée de la tâche, vous pouvez modifier la durée d’une tâche pendant la durée de vie d’un projet, mais cela aura également une incidence sur la chronologie du projet. Pour plus d’informations sur la durée d’une tâche, voir l’article [Vue d’ensemble de la durée et du type de durée des tâches](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Attribuer des tâches

Une fois que vous avez défini la durée et les contraintes de chaque tâche, vous pouvez déterminer qui dispose du temps et des compétences pour réaliser le travail. Vous pouvez attribuer des tâches aux entités suivantes dans Workfront :

* Utilisateurs\
  Seuls les utilisateurs et utilisatrices disposant d’un niveau d’accès Planificateur ou planificatrice ou Travailleur ou travailleuse peuvent être affectés à des tâches. Bien que vous puissiez attribuer des tâches aux personnes en charge des demandes et des révisions, elles ne peuvent pas les réaliser. Il est donc déconseillé de leur attribuer des tâches.

  Pour plus d’informations sur les niveaux d’accès et la façon dont ils définissent les actions des utilisateurs et utilisatrices sur les objets Workfront, voir [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Fonctions
* Équipes

Pour plus d’informations sur l’attribution de tâches, voir les articles de la section [Attribuer des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md).

## Gérer les ressources

La gestion des ressources dans Workfront vous permet de déterminer s’il y a suffisamment de personnel pour réaliser le projet. Lorsque vous ajoutez des utilisateurs et utilisatrices à un projet, Workfront indique leur utilisation. Les gestionnaires de ressources peuvent voir le nombre total d’heures que la personne doit consacrer à d’autres projets pendant la durée du projet.

>[!NOTE]
>
>Tant que le statut du projet est Planification, les tâches attribuées aux utilisateurs et utilisatrices n’apparaissent pas dans leurs listes de tâches.

Au début d’un exercice ou d’un trimestre, vous souhaiterez peut-être gérer vos ressources à un niveau supérieur, dans plusieurs projets, sans vous appuyer sur une structure de répartition du travail concrète.\
Pour plus d’informations sur la planification de l’utilisation de vos ressources à un niveau supérieur, voir l’article [Commencer avec la planification des ressources](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Lorsque vous gérez vos ressources dans le cadre de la création de la structure de répartition du travail d’un projet et que vous vous assurez que chaque tâche est attribuée aux ressources appropriées, vous êtes prêt à planifier vos ressources pour le travail qui doit être effectué.\
Pour plus d’informations sur la planification de vos ressources, voir les articles de la section [Équilibreur de charge de travail : index des articles](../../../resource-mgmt/workload-balancer/workload-balancer.md).

## Estimer les finances du projet

Workfront calcule les coûts prévus pour chaque tâche ainsi que les coûts globaux d’un projet. Les coûts prévus d’une tâche incluent toutes les dépenses associées à la tâche, plus le coût de la personne salariée ou du rôle affecté à la tâche. Les taux horaires de la tâche, du rôle et de la personne salariée sont attribués lors de la création de la tâche, du rôle et de l’utilisateur ou l’utilisatrice.

Pour plus d’informations sur les finances de projet, voir la section [Finance d’un projet : index des articles](../../../manage-work/projects/project-finances/project-finances-overview.md).

## Déterminer les points d’approbation du projet

En créant des processus d’approbation dans Workfront, vous pouvez établir des points de révision pour le projet afin de surveiller la progression et les problème potentiels. Grâce au processus d’approbation, les propriétaires de projet peuvent identifier les tâches qui sont en retard et en avance, afficher les journaux d’audit qui répertorient les personnes ayant modifié le statut d’une tâche et consulter l’historique des problèmes, y compris la manière dont les problèmes ont été résolus et quand ils ont été clôturés. Lors de la révision d’un projet, les propriétaires du projet peuvent déterminer les étapes à suivre et mettre à jour le plan du projet, si nécessaire.

Pour plus d’informations sur les approbations, voir l’article [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Afficher votre SRT

Pour comprendre la SRT d’un projet, vous souhaitez afficher les éléments de tâche suivants :

* Séquence et chronologie de la tâche (dates de début et d’achèvement prévues et durée de la tâche)
* Dépendances de la tâche antérieure
* Relation enfant-parent
* Affectations

Une fois que vous avez terminé la SRT, vous pouvez l’afficher dans une liste de tâches au niveau du projet ou dans un rapport.

* [Afficher la SRT dans une liste de tâches](#view-the-wbs-in-a-task-list)
* [Afficher la SRT dans un rapport de tâches](#view-the-wbs-in-a-task-report)

### Afficher la SRT dans une liste de tâches {#view-the-wbs-in-a-task-list}

Vous pouvez afficher la liste des tâches au niveau du projet.

1. Accédez au projet dont vous souhaitez afficher la structure de répartition du travail.
1. Sélectionnez l’onglet **Tâches**.
1. (Facultatif) Sélectionnez **Rien** dans le menu déroulant **Regroupement**.

   La structure de répartition du travail n’affiche pas la mise en retrait des tâches dans la SRT.

1. Dans le menu déroulant **Vue**, sélectionnez la vue **Répartition du travail**.

   La structure de répartition du travail s’affiche dans la seconde colonne de la vue sélectionnée.

   ![Structure de répartition du travail dans une liste de tâches](assets/work-breakdown-structure.png)

### Afficher la SRT dans un rapport de tâches {#view-the-wbs-in-a-task-report}

Vous pouvez créer un rapport de tâches et afficher la SRT des tâches en effectuant l’une des opérations suivantes :

* Appliquez la vue Structure de répartition du travail existante au rapport.
* Ajoutez la colonne Structure de répartition du travail à n’importe quel rapport personnalisé.

>[!TIP]
>
>Nous vous recommandons d’ajouter un regroupement Projet afin d’identifier plus clairement les projets auxquels appartiennent les tâches. La mise en retrait des tâches ne s’affiche pas dans un rapport de tâches.

Pour plus d’informations sur la création de rapports, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Enregistrer la structure WBS d’un projet en tant que modèle

Si vous travaillez sur d’autres projets qui suivent des planings de travail similaires à la structure WBS que vous venez de créer, vous pouvez enregistrer le projet en tant que modèle. Un modèle permet d’économiser du temps et du travail lors de la création de futurs projets associés.

Si votre entreprise a peu de rotation, pensez à attendre jusqu’à ce que des affectations des personnes soient effectuées pour enregistrer le modèle. Quel que soit le moment où vous enregistrez un projet en tant que modèle, vous pouvez supprimer les affectations d’utilisateurs et utilisatrices ou des tâches spécifiques lorsque vous associez le modèle à un nouveau projet.

Les éléments suivants d’une structure de répartition du travail peuvent être enregistrés dans un modèle en vue d’une utilisation ultérieure avec un autre projet :

* Dépendances de la tâche antérieure
* Affectations (notamment Personne propriétaire du projet, Personne sponsor et Personne gestionnaire des ressources)
* Processus d’approbation
* Contraintes de tâche
* Documents
* Dépenses et autres informations financières
* Objectifs
* Types d&#39;heures
* Structure de la file d’attente des demandes
* Notifications de rappel
* Risques
* Taux de facturation
* Partager des informations
* Formulaires personnalisés

Pour plus d’informations sur l’enregistrement de projets en tant que modèles, voir l’article [Créer un modèle à partir d’un projet](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).
