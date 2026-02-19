---
title: 'Créer le Bridge : connecter l’intention stratégique aux projets'
description: Découvrez comment créer un « thread stratégique » entre vos plans généraux dans Adobe Workfront Planning et votre exécution quotidienne de workflows dans Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 0%

---


# Construire le pont : relier l’intention stratégique aux projets

>[!IMPORTANT]
>
>Les informations de cet article font référence à Adobe Workfront Planning, une fonctionnalité supplémentaire d’Adobe Workfront.
>
>Votre organisation doit disposer d’un package Workfront Planning Prime ou d’un package supérieur pour pouvoir prendre en charge les fonctionnalités recommandées dans cet article.
>
>Pour obtenir la liste des conditions requises pour accéder à Workfront Planning, consultez [Présentation de l&#39;accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Pour obtenir des informations générales sur Workfront Planning, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Découvrez comment créer un thread stratégique entre vos plans généraux dans Adobe Workfront Planning et votre exécution quotidienne dans Workfront. Vous pouvez créer un pont entre la stratégie et l’exécution à l’aide de connexions.

Ce guide est destiné aux administrateurs Workfront et aux responsables d’espace de travail qui implémentent Workfront Planning.

## Présentation de l’alignement de la stratégie sur l’exécution

Relier votre stratégie à votre travail quotidien transforme votre vision en réalité. Lorsque les plans de haut niveau sont synchronisés avec l’exécution, vous créez un thread stratégique qui garantit que chaque projet et tâche fait avancer l’entreprise.

Cet alignement nécessite un ensemble de liens techniques et de mécanismes de sécurisation des processus qui relient les efforts dans Workfront aux enregistrements stratégiques dans Workfront Planning.

En comblant l&#39;écart entre la planification et l&#39;action, vous vous assurez que l&#39;énergie de votre équipe est toujours concentrée sur vos objectifs prioritaires.

## Établir la base en créant une connexion

Avant de pouvoir relier la planification et l’exécution, en tant que gestionnaire d’espace de travail, vous devez définir les types d’enregistrements éligibles à une connexion.

### Présentation du champ de connexion

Le pont commence par la création d’un champ de connexion.

Un champ de connexion sert de liaison technique entre les types d’enregistrements.

Ce type de champ est le moteur de toutes les relations dans Workfront Planning. Il s’agit d’une expression d’intention, dans la mesure où elle établit qu’un type d’enregistrement spécifique (tel qu’une tactique de canal) peut être lié à d’autres types d’objets, qu’ils résident dans Planning ou Workfront.

Pour plus d’informations, voir [Présentation des types d’enregistrements connectés](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

### Définir quand créer une connexion

Idéalement, vous devez décider si vous devez créer des connexions avant la création de tout travail.

En ajoutant un champ de connexion, vous architecturez votre environnement pour prendre en charge un thread stratégique, quelle que soit la manière dont les enregistrements individuels sont finalement créés.

## Définition de la stratégie et de l’exécution synchronisées

Pour que votre couche stratégique reste concentrée, nous vous recommandons de concentrer vos enregistrements de planification sur l’intention de haut niveau tout en utilisant Workfront pour l’exécution tactique.

Cette approche utilise les points forts uniques des deux modules de la manière suivante :

* **Planification Workfront (la couche stratégique) :** reste de haut niveau. Il effectue le suivi de la campagne, de la tactique de canal et du budget. Il est silencieux et prêt pour l&#39;exécutif.

* **Workfront (la couche d’exécution) :** gère les détails tactiques. Vous pouvez gérer des expériences ou des activités individuelles en tant que projets, tâches et événements. Vous pouvez les affecter pour appropriation et intégrer des validations pour exécution.

## Passer de l&#39;intention à l&#39;action en activant le pont

Une fois la connexion configurée, vous devez décider comment activer le lien entre un enregistrement stratégique spécifique et un projet d’exécution.

### Utiliser un chemin d’accès dirigé par un tableau

Les stratèges et les utilisateurs expérimentés utilisent souvent la vue Tableau comme pupitre pour affiner les plans au fil du temps.

Par défaut, la création d’un enregistrement dans une table n’établit pas de lien vers Workfront.

La connexion à un projet d&#39;exécution est établie lorsqu&#39;un utilisateur décide d&#39;activer le lien.

Pour ce faire, procédez comme suit :

* Créez manuellement un projet connecté en aval directement à partir du champ de connexion dans Workfront Planning ou d&#39;une page Connexions facultative dans la vue détaillée de l&#39;enregistrement.

  La création manuelle génère un projet vierge sans formulaires personnalisés spécifiques.

  Pour plus d’informations, consultez [Connecter des enregistrements](/help/quicksilver/planning/records/connect-records.md).

* Automatiquement, en utilisant les automatisations de Workfront Planning, pour des besoins plus complexes.

  Ces automatisations sont disponibles sous forme de boutons dans la barre d’actions lorsque vous sélectionnez une ligne dans un tableau.

  Cela permet une supervision humaine ou la création d’espaces réservés, ce qui garantit que les projets ne sont générés dans votre environnement de workflow que lorsqu’ils sont vraiment nécessaires.

  Pour plus d’informations, voir [Création d’objets à l’aide des automatisations d’enregistrements Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)


### Créer des activations automatisées

Pour les organisations ayant des demandes volumineuses ou des besoins d’automatisation avancés, le pont peut être activé automatiquement en fonction d’événements spécifiques ou des valeurs de champ configurées dans un formulaire de demande.

Pour cette approche, vous aurez besoin d’une licence pour Adobe Workfront Fusion .

Pour plus d’informations, voir [Configuration et gestion de Workfront Fusion : index des articles](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc).

* **Utiliser des déclencheurs d’envoi :** les formulaires fournissent un événement d’envoi unique et propre. Ils peuvent donc être utilisés comme déclencheurs pour les automatisations Fusion. Un scénario Fusion peut détecter un envoi de formulaire et générer immédiatement un projet lié dans Workfront.

* **Utiliser des déclencheurs de valeur de champ :** pour une automatisation plus approfondie, vous pouvez configurer Fusion pour surveiller des champs spécifiques. Par exemple, une simple case à cocher intitulée « Prêt pour l’exécution » peut servir de catalyseur, établissant le pont automatiquement au moment où il est coché.

## Ajouter des champs de recherche à la visibilité de surface

Une fois qu’un projet est lié, vous pouvez afficher des données en temps réel à partir de Workfront directement dans l’enregistrement Planning en ajoutant des champs de recherche à partir du projet.

En tant que gestionnaire d&#39;espace de travail, vous pouvez configurer des champs de recherche pour extraire n&#39;importe quel champ système ou personnalisé du projet lié (comme la date d&#39;achèvement effective ou le prospect Creative) dans le type d&#39;enregistrement Planification. Une fois capturées, ces données peuvent être cumulées à plusieurs niveaux de votre hiérarchie stratégique, jusqu’au niveau de la campagne. Cela permet aux parties prenantes de créer des rapports agrégés puissants tout au long du cycle de vie marketing, en les tenant informées sans avoir à quitter l’environnement de planification.

## Atteindre la visibilité en connectant la stratégie à l&#39;action

La valeur ultime du pont est la visibilité en temps réel.

En établissant un lien entre l’intention et l’action, vous pouvez répondre rapidement aux questions critiques de l’entreprise. Voici des exemples de ces questions :

* Notre campagne &#39;FY26 Brand Awareness&#39; donne-t-elle des résultats concrets en ce moment ?

* Où nos tactiques stratégiques ont-elles besoin d’un soutien plus créatif pour respecter le calendrier ?

* Comment alignons-nous nos ressources sur nos piliers stratégiques prioritaires?

## Bonnes pratiques et conseils

### Fait :

* **Utilisez la métaphore du « fil stratégique »** rappelez aux équipes que chaque projet doit être une « perle » sur une chaîne stratégique.

* **Automatiser la remise :** utilisez les automatisations pour déclencher la création de projets afin de gagner du temps et de réduire les efforts, tout en améliorant la connectivité et la gouvernance des données.

* **Lien, ne pas dupliquer :** utilisez des champs de recherche pour faire apparaître les données d’exécution en temps réel (comme le statut ou les dates d’achèvement) dans vos enregistrements stratégiques. Cela garantit que vos vues stratégiques sont toujours exactes sans nécessiter de mises à jour manuelles de la part de votre équipe.

### Ne pas :

* **Ne traitez pas les enregistrements de planification comme des listes de tâches :** le pont est conçu pour relier l’intention stratégique aux projets d’exécution. Gardez vos enregistrements de planification concentrés sur le « quoi » et le « pourquoi » et laissez le module de workflow gérer le « comment » granulaire à travers les tâches et les problèmes.

* **Ne pas sursynchroniser :** il n’est pas nécessaire de resynchroniser avec Planning tous les détails au niveau du projet. Gardez la couche stratégique de haut niveau et sans bruit.

* **Ne pas contourner le pont :** si le travail commence dans le module Workflow sans lien vers Planning, vous avez créé un « plan fantôme » qui est invisible pour les dirigeants.

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



