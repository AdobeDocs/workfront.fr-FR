---
title: 'Bridge : relier l’intention stratégique aux projets'
description: Découvrez comment créer un « thread stratégique » entre vos plans généraux dans Adobe Workfront Planning et votre exécution quotidienne de workflows dans Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---


# Le pont : relier l’intention stratégique aux projets


## Objectif

Découvrez comment créer un « thread stratégique » entre vos plans généraux dans Workfront Planning et votre exécution quotidienne dans le module Workflow .



## Vue d’ensemble

Relier votre stratégie à votre travail quotidien transforme votre vision en réalité. Lorsque les plans de haut niveau sont synchronisés avec l’exécution, vous créez un **thread stratégique** qui garantit que chaque projet et tâche fait avancer l’entreprise.



Cet alignement nécessite un ensemble de liens techniques et de mécanismes de sécurisation des processus qui relient les efforts du module **Workflow** aux enregistrements stratégiques dans **Workfront Planning (WFP)**. En comblant l&#39;écart entre la planification et l&#39;action, vous vous assurez que l&#39;énergie de votre équipe est toujours concentrée sur vos objectifs prioritaires.



## Les bases : établir la connexion

Avant de pouvoir relier la planification et l’exécution, un gestionnaire d’espace de travail doit définir les types d’enregistrements éligibles à une connexion.



### Le champ de connexion : l’établissement de liaison technique

Le pont commence par un **champ de connexion**. Ce type de champ est le moteur de toutes les relations dans WFP. Il s’agit d’une expression d’intention, dans la mesure où elle établit qu’un type d’enregistrement spécifique (comme une *tactique de canal*) peut être lié à d’autres objets, qu’ils se trouvent dans le module de workflow ou dans la planification elle-même.



### Choix de la connexion

L’établissement de cette tolérance est une décision au niveau de la configuration qui se produit généralement avant la création d’un travail. En ajoutant un champ de connexion, vous concevez votre environnement pour prendre en charge un « thread stratégique », quelle que soit la manière dont les enregistrements individuels sont finalement créés.



## Stratégie et exécution synchronisées

Pour que votre couche stratégique reste concentrée, nous vous recommandons de concentrer vos enregistrements de planification sur l’intention de haut niveau tout en utilisant le module Workflow pour l’exécution tactique. Cette approche utilise les points forts uniques des deux modules :



* **Planification de Workfront (couche stratégique) :** reste à un niveau élevé. Il effectue le suivi de la *Campagne*, de la *Tactique de canal* et du *Budget*. Il est silencieux et prêt pour l&#39;exécutif.

* **Module de workflow (couche d’exécution) :** gère les détails tactiques. Les « expériences » ou « activités » individuelles sont gérées ici sous la forme **projets, tâches et événements**.



## Activer le pont : de l&#39;intention à l&#39;action

Une fois la connexion configurée, vous devez décider comment activer le lien entre un enregistrement stratégique spécifique et un projet d&#39;exécution.



### Triage professionnel : le chemin guidé par une table

Les stratèges et les utilisateurs expérimentés utilisent souvent la **vue de tableau** comme leur « pupitre » pour affiner les plans au fil du temps.

* **Transfert délibéré :** par défaut, la création d’un enregistrement dans une table n’établit pas de lien vers le module Workflow. La connexion à un projet d&#39;exécution est établie lorsqu&#39;un utilisateur décide d&#39;activer le lien. Pour ce faire, créez manuellement un projet connecté en aval directement à partir du champ de connexion dans WFP ou une **page de vue de connexion** facultative dans la vue détaillée de l&#39;enregistrement. Notez que la création manuelle donne lieu à un projet vierge sans formulaires personnalisés spécifiques ; pour les besoins plus complexes, vous pouvez utiliser une **automatisation WFP native**. Ces automatisations sont disponibles lorsque vous sélectionnez une ligne dans un tableau, apparaissant sous la forme de boutons dans la barre d’actions bleue située en bas de votre écran. Cela permet une supervision humaine ou la création d’espaces réservés, ce qui garantit que les projets ne sont générés dans votre environnement de workflow que lorsqu’ils sont vraiment nécessaires.



### Activation automatisée

Pour les organisations ayant des demandes volumineuses ou des besoins d’automatisation avancés, le pont peut être activé automatiquement en fonction d’événements ou de valeurs de champ spécifiques.

* **Déclencheurs d’envoi :** comme les formulaires fournissent un « événement d’envoi » unique et propre, ils peuvent être utilisés comme déclencheurs pour les **automatisations de Fusion**. Un scénario peut détecter un envoi de formulaire et générer immédiatement un projet lié dans le module de workflow.

* **Déclencheurs de valeur de champ :** pour une automatisation plus approfondie, vous pouvez configurer **Fusion** pour surveiller des champs spécifiques. Par exemple, une simple case à cocher intitulée « prêt pour exécution » peut servir de catalyseur, établissant le pont automatiquement au moment où il est coché.



## Visibilité de l’affichage : champs de recherche

Une fois qu’un projet est lié, vous pouvez afficher des données en temps réel à partir du module Workflow directement dans l’enregistrement WFP.



Un gestionnaire d&#39;espace de travail peut configurer des **champs de recherche** pour extraire n&#39;importe quel champ natif ou personnalisé du projet lié (par exemple *date d&#39;achèvement effective* ou *prospect créatif*) dans le type d&#39;enregistrement WFP. Une fois capturées, ces données peuvent être cumulées à plusieurs niveaux de votre hiérarchie stratégique, jusqu’au niveau de la campagne. Cela permet aux parties prenantes de créer des rapports agrégés puissants tout au long du cycle de vie marketing, en les tenant informées sans avoir à quitter l’environnement de planification.



## Visibilité de la stratégie en action

La valeur ultime du pont est **visibilité en temps réel**. En établissant un lien entre l’intention et l’action, vous pouvez répondre rapidement aux questions stratégiques de l’entreprise :



* « Notre campagne de sensibilisation à la marque pour l’exercice 26 produit-elle des résultats concrets en ce moment ? »

* « Où nos tactiques stratégiques ont-elles besoin d’un soutien plus créatif pour respecter le calendrier ? »

* « Comment alignons-nous nos ressources sur nos piliers stratégiques prioritaires ? »



## Bonnes pratiques et conseils



### Faire :

* **Utilisez la métaphore du « fil stratégique ».** Rappelez aux équipes que chaque projet doit être une « perle » sur une chaîne stratégique.

* **Automatiser la remise.** Utilisez les automatisations pour déclencher la création de projets afin de gagner du temps et d’économiser des efforts tout en améliorant la connectivité et la gouvernance des données.

* **Link, ne dupliquez pas.** Utilisez des champs de recherche pour faire apparaître les données d’exécution en temps réel (comme le statut ou les dates d’achèvement) dans vos enregistrements stratégiques. Cela garantit que vos vues stratégiques sont toujours exactes sans nécessiter de mises à jour manuelles de la part de votre équipe.



### Ne pas :

* **Ne pas traiter les enregistrements de planification comme des listes de tâches.** Le pont est conçu pour relier l’intention stratégique aux projets d’exécution. Gardez vos enregistrements de planification concentrés sur le « quoi » et le « pourquoi » et laissez le module de workflow gérer le « comment » granulaire à travers les tâches et les problèmes.

* **Ne pas synchroniser de manière excessive.** Vous n’avez pas besoin de resynchroniser avec Planning tous les détails au niveau du projet. Gardez la couche stratégique de haut niveau et sans bruit.

* **Ne contourne pas le pont.** Si le travail commence dans le module Workflow sans lien vers Planning, vous avez créé un « plan fantôme » qui est invisible pour les dirigeants.




