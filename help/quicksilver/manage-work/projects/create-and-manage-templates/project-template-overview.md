---
product-area: templates
navigation-topic: templates-navigation-topic
title: Présentation du modèle de projet
description: Vous pouvez utiliser des modèles de projet pour capturer la plupart des processus, informations et paramètres répétables associés aux projets de votre entreprise.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# Présentation du modèle de projet

Vous pouvez utiliser des modèles de projet pour capturer la plupart des processus, informations et paramètres répétables associés aux projets de votre entreprise.

Vous pouvez définir des tâches, des rubriques de file d’attente, des formulaires personnalisés, joindre des documents dans votre modèle.

Après avoir créé des modèles, vous pouvez les joindre à des projets existants ou les utiliser pour créer des projets. Toutes les informations du modèle sont transférées vers les projets créés à l’aide de celui-ci.

## Avantages de l’utilisation de modèles dans Adobe Workfront

Voici quelques avantages de l’utilisation de modèles pour créer vos projets :

* Cela vous permet de gagner du temps et vous évite de créer de nouveaux projets répétitifs.
* Vous disposez d’informations homogènes sur les projets de portée similaire.
* Cela s’avère utile lorsque vous créez des rapports sur des projets. Par exemple, vous pouvez créer des rapports sur les projets qui partagent le même modèle, comparer leur progression et trouver des améliorations dans la manière dont ils peuvent être terminés.
* En plus de définir les futurs paramètres du projet, vous pouvez ajouter les informations suivantes pour le futur projet sur un modèle :

   * Tâches
   * Documents
   * Approbations
   * Détails de la file d&#39;attente
   * Rubriques de file d&#39;attente
   * Groupes de rubriques
   * Règles de transmission
   * Forms personnalisée
   * Informations sur la société et le groupe

## Bonnes pratiques relatives à la création de modèles

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Tenez compte des points suivants lors de la création de modèles :

* N’affectez pas d’utilisateurs aux tâches de modèle. Bien que vous puissiez ne pas affecter les tâches, nous vous recommandons d’affecter des rôles de tâche aux tâches. Vous aurez ainsi une idée des utilisateurs qui pourront être affectés aux tâches lorsque vous créerez le projet à l’aide du modèle.
* Donnez toujours une valeur Durée et Heures planifiées à vos tâches de modèle. Chaque tâche du projet doit être associée à une durée pendant laquelle la tâche peut rester ouverte et à une valeur Heure planifiée pour le temps nécessaire à l’exécution de la tâche. Les tâches sans ces informations ne peuvent pas être planifiées correctement pour les ressources lors de l’utilisation des outils de gestion des ressources dans Workfront.

   Pour plus d’informations sur la durée, voir les articles suivants :

   * [Présentation de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Présentation de la durée du projet](../../../manage-work/projects/planning-a-project/project-duration.md)

   Pour plus d’informations sur les heures planifiées, voir [Présentation des heures planifiées](../../../manage-work/tasks/task-information/planned-hours.md).

* Ajoutez les relations précédentes entre les tâches à la fin, lorsque vous avez une compréhension claire de l’ensemble du futur plan de projet. L’ajout de prédécesseurs aux tâches de modèle est similaire à l’ajout de prédécesseurs aux tâches d’un projet.

   Pour plus d’informations sur l’ajout de prédécesseurs aux tâches, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indiquez avec qui le modèle doit être partagé pour une utilisation ultérieure et avec qui les projets qui seront créés à partir du modèle doivent être partagés. Pour plus d’informations sur le partage de modèles, voir [Partage de modèles de projet](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Utilisez des processus de validation globaux et ajoutez-les à vos tâches de modèle et de modèle si possible. Cela permet de gagner du temps lorsque les tâches ou le futur projet devront passer par les mêmes validations.

   Pour plus d’informations sur la création des validations, voir [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   Pour plus d’informations sur l’association d’un processus d’approbation à un élément de travail, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Méthodes de création de modèles

Vous pouvez créer un modèle de la manière suivante :

* À partir de zéro.\
   Pour plus d’informations sur la création d’un modèle à partir de zéro, voir [Création d’un modèle de projet](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* À partir de projets existants, en enregistrant un projet en tant que modèle.\
   Pour plus d’informations sur la création de modèles à partir de projets existants, voir [Créer un modèle à partir d’un projet](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* En la copiant à partir d’un autre modèle.\
   Pour plus d’informations sur la copie d’un modèle existant, voir [Copier un modèle de projet](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* En utilisant nos exemples de modèles.\
   Pour plus d’informations sur la création de vos modèles à l’aide de nos exemples de modèles, voir [Création de modèles de projet à partir d’exemples](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
