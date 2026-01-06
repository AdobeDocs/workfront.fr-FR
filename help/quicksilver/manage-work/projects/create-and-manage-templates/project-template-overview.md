---
product-area: templates
navigation-topic: templates-navigation-topic
title: Vue d’ensemble des modèles de projet
description: Vous pouvez utiliser des modèles de projet pour capturer la plupart des processus, informations et paramètres reproductibles associés aux projets de votre organisation.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 96%

---

# Vue d’ensemble des modèles de projet

<!-- Audited: 12/2023 -->

Vous pouvez utiliser des modèles de projet pour capturer la plupart des processus, informations et paramètres reproductibles associés aux projets de votre organisation.

Vous pouvez définir des tâches, des rubriques de file d’attente, des formulaires personnalisés et joindre des documents à votre modèle.

Après avoir créé des modèles, vous pouvez les joindre à des projets existants ou les utiliser pour créer de nouveaux projets. Toutes les informations contenues dans le modèle sont transférées aux projets créés à l’aide de celui-ci.

## Avantages de l’utilisation de modèles dans Adobe Workfront

Voici quelques-uns des avantages de l’utilisation de modèles pour la création de vos projets :

* Cela vous permet d’économiser du temps et des efforts lors de la création de nouveaux projets répétitifs.
* Vous disposez d’informations cohérentes pour des projets de portée similaire.
* C’est utile pour créer des rapports sur des projets. Par exemple, vous pouvez créer des rapports sur des projets qui partagent le même modèle, afin de comparer leur progression et de trouver des améliorations dans la manière dont ils pourraient être menés à bien.
* En plus de définir les paramètres du futur projet, vous pouvez ajouter les informations suivantes pour le futur projet sur un modèle :

   * Tâches
   * Documents
   * Approbations
   * Détails de la file d&#39;attente
   * Rubriques de file d&#39;attente
   * Groupes de sujets
   * Règles de routage
   * Formulaires personnalisés
   * Informations sur l’entreprise et le groupe

## Bonnes pratiques pour la création de modèles

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Tenez compte des éléments suivants lors de la création de modèles :

* N’affectez pas d’utilisateurs aux tâches de modèles. Bien que vous puissiez laisser les tâches non affectées, nous vous recommandons d’affecter des fonctions aux tâches. Cela vous donnera une idée des personnes qui pourront être affectées aux tâches lorsque vous créerez le projet à l’aide du modèle.
* Attribuez toujours aux tâches de votre modèle une valeur de durée et de nombre d’heures prévues. Chaque tâche du projet doit être associée à une durée pour savoir combien de temps la tâche peut rester ouverte et à une valeur de nombre d’heures prévues pour savoir combien de temps il faudra pour que la tâche soit achevée. Le budget des ressources associées aux tâches qui ne disposent pas de ces informations ne peut pas être planifié correctement lors de l’utilisation des outils de gestion des ressources dans Workfront.

  Pour plus d’informations sur la durée, voir les articles suivants :

   * [Vue d’ensemble de la durée des tâches et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Vue d’ensemble de la durée du projet](../../../manage-work/projects/planning-a-project/project-duration.md)

  Pour plus d’informations sur le nombre d’heures prévues, voir [Vue d’ensemble des heures prévues](../../../manage-work/tasks/task-information/planned-hours.md).

* Ajoutez des relations d’antériorité entre les tâches complètement à la fin, lorsque vous avez une compréhension claire de l’ensemble du plan du futur projet. L’ajout de tâches antérieures aux tâches du modèle est similaire à l’ajout de tâches antérieures aux tâches d’un projet.

  Pour plus d’informations sur l’ajout de tâches antérieures aux tâches, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indiquez les personnes avec lesquelles le modèle doit être partagé pour une utilisation future et les personnes avec lesquelles les projets qui seront créés à partir du modèle doivent être partagés. Pour plus d’informations sur le partage de modèles, voir [Partager des modèles de projet](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Utilisez des processus d’approbation globaux et ajoutez-les à votre modèle et à vos tâches de modèle si possible. Cela permettra de gagner du temps lorsque les tâches ou le projet futur devront faire l’objet des mêmes approbations.

  Pour plus d’informations sur la création d’approbations, voir [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Pour plus d’informations sur l’association d’un processus d’approbation à un élément de travail, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Comment créer des modèles

Vous pouvez créer un modèle des manières suivantes :

* À partir de zéro.\
  Pour plus d’informations sur la création d’un nouveau modèle à partir de zéro, voir [Créer un modèle de projet](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* À partir de projets existants, en enregistrant un projet en tant que modèle.\
  Pour plus d’informations sur la création de modèles à partir de projets existants, voir [Créer un modèle à partir d’un projet](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* En le copiant à partir d’un autre modèle.\
  Pour plus d’informations sur la copie d’un modèle existant, voir [Copier un modèle de projet](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* En utilisant nos exemples de modèles.\
  Pour plus d’informations sur la création de vos modèles à partir de nos modèles d’exemple, voir [Créer des modèles de projet à partir d’exemples](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
