---
product-area: projects
navigation-topic: plan-a-project
title: Détermination de la structure de ventilation du travail dans un projet
description: La définition d’une structure de ventilation des tâches (WBS) pour un projet est un ensemble d’activités qui, en fin de compte, décrivent le plan du projet. Le WBS divise le résultat du projet en éléments de travail gérables, qui peuvent être utilisés pour définir des jalons et organiser des affectations de travail.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '1745'
ht-degree: 1%

---

# Détermination de la structure de ventilation du travail dans un projet

La définition d’une structure de ventilation des tâches (WBS) pour un projet est un ensemble d’activités qui, en fin de compte, décrivent le plan du projet. Le WBS divise le résultat du projet en éléments de travail gérables, qui peuvent être utilisés pour définir des jalons et organiser des affectations de travail.

Pour créer la structure de ventilation de travail d’un projet, vous devez disposer d’une licence Plan avec l’accès Modifier aux projets . Un accès supplémentaire à d’autres zones d’Adobe Workfront peut être nécessaire, en fonction du nombre d’activités que vous effectuez lors de la création du WBS.

Nous vous recommandons de conserver l’état Planification pendant que vous modifiez la structure de ventilation des tâches, afin d’éviter que les notifications ne se déclenchent aux utilisateurs de l’équipe de projet.

## Définition des livrables du projet

L’objectif d’un projet est de fournir des livrables tangibles aux parties prenantes internes et externes. Les éléments livrables d’un projet sont les résultats que vous souhaitez obtenir en exécutant le projet. Les résultats sont presque toujours associés à au moins un livrable et tous les livrables doivent être associés à un projet.

Les éléments livrables du projet peuvent être des biens de consommation, des produits intellectuels (comme les rapports) ou des services. Par exemple, si la portée de votre projet est de construire une maison, certains éléments livrables peuvent inclure :

* créer des plans architecturaux
* terminer la plomberie
* travail électrique
* verser la fondation
* travail de structure
* la fermeture de la vente de la maison.

En fonction de sa taille et de sa portée, un projet peut être constitué de plusieurs livrables.

Une fois que vous avez identifié vos livrables, vous pouvez commencer à les ventiler en tâches. Les tâches sont la sortie que vous obtenez pour obtenir le résultat global du projet. Lors de la définition de vos tâches, vous prenez en compte les paramètres suivants :

* Laps de temps requis pour l’achèvement.
* Budget nécessaire pour terminer le travail.
* Ressources requises pour terminer le travail.
* Planification des ressources en fonction de la chronologie logique des tâches.

Lorsque vous définissez des tâches, veillez à ne pas planifier trop de travail pour une seule tâche. Si le travail requis sur une tâche est supérieur à 40 heures (une semaine de travail type), vous devrez peut-être ventiler cette quantité de travail dans les sous-tâches. L’achèvement de toutes les sous-tâches terminera alors la tâche principale.

Pour définir les résultats WBS et les éléments livrables dans Workfront, nous vous recommandons d’exécuter les activités suivantes afin de créer une vue hiérarchique des tâches de projet :

* Si vous ne l’avez pas déjà fait, créez un projet.\
  Pour plus d’informations sur la création d’un projet, voir l’article [Création d’un projet](../../../manage-work/projects/create-projects/create-project.md).

* Créez des tâches pour tous les éléments d’action requis pour terminer chaque résultat et chaque livrable.\
  Pour plus d’informations sur la création de tâches, voir l’article [Création de tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* À partir des tâches que vous venez de créer, identifiez celles qui sont des résultats majeurs et associez-les aux jalons.\
  Pour plus d’informations sur la création de tâches de jalon, voir les articles [Création d’un chemin de jalon](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) et [Associer des jalons à des tâches](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Ventilez les tâches avec une portée trop grande en sous-tâches. Associez-les au parent qui définit votre livrable .\
  Pour plus d’informations sur la création de sous-tâches, voir l’article [Création de sous-tâches](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identifiez les relations de dépendance entre les sous-tâches et entre les jalons.\
  Dans une relation de dépendance, le début d’une tâche dépend de l’achèvement d’une autre tâche ou d’un groupe de tâches.\
  Pour plus d’informations sur les dépendances des tâches, voir les articles [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) et [Créer une relation de prédécesseur sur la liste des tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Déterminez si, à un moment quelconque de la durée de vie du projet, des approbations et des révisions sont nécessaires. Créez des processus de validation pour répondre à ce besoin.\
  Pour plus d’informations sur les validations, voir l’article [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Estimation du planning de travail et des contraintes de planification

Une fois que vous avez créé le jalon de base et la structure de tâche du projet, vous pouvez estimer le temps nécessaire pour terminer le projet global en définissant les contraintes et les durées de tâche.

Tenez compte des points suivants :

* Les contraintes de tâche définissent le moment où le travail sur une tâche doit commencer ou se terminer.

  Pour plus d’informations sur la définition des contraintes de tâche, voir l’article [Présentation de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* La Durée d’une tâche est la période disponible pour terminer une tâche. Lors de l’estimation de la durée, vous pouvez saisir une valeur qui prend en compte la possibilité d’un délai. Si des projets similaires ont été réalisés dans le passé, vous pouvez avoir une bonne idée de l’endroit où définir cette valeur.

  Comme la durée est une estimation, veillez à définir des valeurs temporelles optimistes afin de tenir compte des facteurs pouvant affecter la tâche, tels que les conditions météorologiques, les pannes de courant, les difficultés du fournisseur ou d’autres événements imprévus. En outre, veillez à examiner s’il existe des tâches associées de prédécesseur ou de dépendance, et comment elles peuvent imposer des contraintes au travail et affecter l’achèvement de la tâche.

  Selon le type de durée de la tâche, vous pouvez modifier la durée d’une tâche pendant la durée de vie d’un projet, mais cela aura également une incidence sur la chronologie du projet. Pour plus d’informations sur la durée d’une tâche, voir l’article [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Affecter des tâches

Une fois que vous avez défini la durée et les contraintes de chaque tâche, vous pouvez déterminer qui dispose du temps et des compétences pour accomplir le travail. Vous pouvez affecter des tâches aux entités suivantes dans Workfront :

* Utilisateurs et utilisatrices\
  Seuls les utilisateurs disposant d’un niveau d’accès de planificateur ou de traitement peuvent être affectés à des tâches. Bien que vous puissiez affecter des tâches aux Demandeurs et aux Réviseurs, ils ne peuvent pas les exécuter. Pour cette raison, il est déconseillé de leur assigner des tâches.

  Pour plus d’informations sur les niveaux d’accès et la manière dont ils définissent ce que les utilisateurs peuvent faire avec les objets Workfront, voir [Présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Fonctions
* Équipes

Pour plus d’informations sur l’affectation de tâches, reportez-vous aux articles de la section [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) .

## Gestion des ressources

La gestion des ressources dans Workfront vous permet de déterminer s’il y a suffisamment de personnel pour terminer le projet. Lorsque des utilisateurs sont ajoutés à un projet, Workfront indique l’utilisation de chaque utilisateur. Les gestionnaires de ressources peuvent voir le nombre total d’heures pendant lesquelles la personne est affectée à d’autres projets pendant la période du projet.

>[!NOTE]
>
>Tant que l’état du projet est Planning, les tâches assignées aux utilisateurs n’apparaissent pas dans leurs listes de tâches.

Au début d’un exercice ou d’un trimestre, vous souhaiterez peut-être gérer vos ressources à un niveau supérieur, dans plusieurs projets, sans avoir connaissance d’une structure de ventilation des tâches spécifique.\
Pour plus d’informations sur la planification de l’utilisation de vos ressources à un niveau supérieur, consultez l’article [Prise en main de la planification des ressources](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Lorsque vous gérez vos ressources dans le cadre de la création de la structure de ventilation des tâches d’un projet et en vous assurant que chaque tâche est affectée à la ressource appropriée, vous êtes prêt à planifier vos ressources pour le travail qui doit être effectué.\
Pour plus d’informations sur la planification de vos ressources, reportez-vous aux articles de la section [L’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/workload-balancer.md) .

## Estimation des finances du projet

Workfront calculera les coûts prévus pour chaque tâche et les coûts globaux d&#39;un projet. Les coûts prévus pour une tâche incluent toutes les dépenses de la tâche, plus le coût de l’employé ou du rôle affecté à la tâche. Les taux horaires de la tâche, du rôle et de l’employé sont attribués lors de la création de la tâche, du rôle et de l’utilisateur.

Pour plus d’informations sur les finances de projet, voir la section [Finances du projet](../../../manage-work/projects/project-finances/project-finances-overview.md) .

## Déterminer les points d’approbation du projet

En créant des processus d’approbation dans Workfront, vous pouvez établir des points de révision pour le projet afin de surveiller la progression et les zones à problème potentielles. Grâce au processus d’approbation, les propriétaires de projet peuvent identifier les tâches qui sont en retard et en avance, afficher les journaux d’audit qui répertorient les personnes ayant modifié l’état d’une tâche et consulter l’historique des problèmes, y compris la manière dont les problèmes ont été résolus et quand ils ont été fermés. Lors de la révision d’un projet, les propriétaires de projet peuvent déterminer les étapes à suivre et mettre à jour le plan du projet, si nécessaire.

Pour plus d’informations sur les validations, voir l’article [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## Afficher votre WBS

Pour comprendre le WBS d’un projet, vous souhaitez afficher les éléments de tâche suivants :

* Séquence et chronologie des tâches (dates de début et de fin planifiées et durée de la tâche)
* Dépendances du prédécesseur
* Relation enfant-parent
* Affectations

Une fois que vous avez terminé votre WBS, vous pouvez l’afficher dans une liste de tâches au niveau du projet ou dans un rapport.

* [Afficher le WBS dans une liste de tâches](#view-the-wbs-in-a-task-list)
* [Afficher le WBS dans un rapport de tâche](#view-the-wbs-in-a-task-report)

### Afficher le WBS dans une liste de tâches {#view-the-wbs-in-a-task-list}

Vous pouvez afficher la liste des tâches au niveau du projet.

1. Accédez au projet pour lequel vous souhaitez afficher la structure de ventilation de travail.
1. Sélectionnez la **Tâches** .
1. (Facultatif) Sélectionnez **Rien** dans le **Regroupement** menu déroulant.

   La structure de ventilation des tâches n’affiche pas la mise en retrait des tâches dans le WBS.

1. Dans la **Affichage** , puis sélectionnez l’option **Ventilation du travail** vue.

   La structure Répartition du travail s’affiche dans la seconde colonne de la vue sélectionnée.

   ![Structure de ventilation de travail dans une liste de tâches](assets/work-breakdown-structure.png)

### Afficher le WBS dans un rapport de tâche {#view-the-wbs-in-a-task-report}

Vous pouvez créer un rapport de tâches et afficher le WBS des tâches en effectuant l’une des opérations suivantes :

* Appliquez la vue Structure de ventilation de travail existante au rapport.
* Ajoutez la colonne Structure de ventilation de travail à n’importe quel rapport personnalisé.

>[!TIP]
>
>Nous vous recommandons d’ajouter un groupement Projet afin de clarifier les projets auxquels appartiennent les tâches. La mise en retrait des tâches ne s’affiche pas dans un rapport de tâches.

Pour plus d’informations sur la création de rapports, voir l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Enregistrement du WBS d’un projet en tant que modèle

Si vous travaillez sur d’autres projets qui suivent des horaires de travail similaires au WBS que vous venez de créer, vous pouvez enregistrer le projet en tant que modèle. Un modèle permet de gagner du temps et des efforts lors de la création de projets connexes futurs.

Si votre entreprise a peu de chiffre d’affaires, pensez à attendre jusqu’à ce que des affectations utilisateur soient effectuées pour enregistrer le modèle. Quel que soit le moment où un projet est enregistré en tant que modèle, les affectations d’utilisateurs ou des tâches spécifiques peuvent être supprimées lors de l’association du modèle à un nouveau projet.

Les éléments suivants d’une structure de ventilation de travail peuvent être enregistrés dans un modèle pour une utilisation ultérieure avec un autre projet :

* Dépendances du prédécesseur
* Affectations (notamment Propriétaire du projet, Parrain et Gestionnaire de ressources)
* Processus d’approbation
* Contraintes de tâche
* Documents
* Dépenses et autres informations financières
* Objectifs
* Types d&#39;heures
* Structure de la file d’attente des requêtes
* Notifications de rappel
* Risques
* Taux de facturation
* Partage d&#39;informations
* Formulaires personnalisés

Pour plus d’informations sur l’enregistrement de projets en tant que modèles, reportez-vous à l’article [Créer un modèle à partir d’un projet](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
