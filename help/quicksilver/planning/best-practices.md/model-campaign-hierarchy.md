---
title: 'Concevoir La Réussite : Modéliser La Hiérarchie De Votre Campagne'
description: Découvrez comment traduire vos processus d’entreprise complexes en une hiérarchie de campagnes évolutive et régie à l’aide de « centres de gravité » et d’une architecture multi-espace de travail.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 699add479d958b9f3fc01ae30513ddf6689620f1
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 1%

---

# Concevoir la réussite : modéliser la hiérarchie de vos campagnes

<!--see the file again for additional comments from Seth and others-->

{{planning-important-intro}}

Découvrez comment traduire vos processus d’entreprise complexes en une hiérarchie de campagnes évolutive et gouvernée à l’aide de centres de gravité et d’une architecture multi-espaces de travail dans Adobe Workfront Planning.

Ce guide est destiné aux administrateurs Workfront et aux utilisateurs expérimentés qui implémentent et conçoivent l’architecture de votre environnement dans Workfront Planning.

## Présentation de l’architecture de la réussite

La complexité de vos données augmente à mesure que vos opérations marketing évoluent. En l’absence d’un plan directeur clair, votre système d’enregistrement marketing peut rapidement se transformer en un tiroir-poubelle d’enregistrements déconnectés, de terminologie en conflit et de silos de création de rapports.

Lorsque vous créez une architecture de succès, vous établissez un framework pour modéliser la hiérarchie de vos campagnes dans Workfront Planning. Il vous fait passer du chaos des feuilles de calcul à un modèle régi et orienté objet qui garantit que chaque équipe parle le même langage tout en conservant l’agilité dont elle a besoin pour s’exécuter.

## Créer une hiérarchie pour définir vos niveaux d’intention

Pour maintenir la clarté et l’évolutivité, nous vous recommandons de commencer par un chemin principal éprouvé lors de la conception de votre workflow dans Workfront Planning.

De là, vous pouvez développer votre stratégie en ajoutant d’autres niveaux à votre architecture.

### La voie principale : comment passer de la stratégie à l’action

Bien que les entreprises puissent étendre cette hiérarchie à mesure que leurs besoins opérationnels évoluent, en commençant par les trois niveaux décrits dans les sections ci-dessous, vous garantirez un lien étroit entre la stratégie et l’exécution.

Nos résultats ont montré que la plupart des implémentations réussies de Workfront Planning reposent sur un modèle épuré à trois niveaux, couvrant à la fois Planning et Workfront.

Vous trouverez ci-dessous les niveaux d’une implémentation de Planning réussie et les artefacts que vous pouvez envisager de créer pour vous aider dans le processus :

* **Niveau 1 : campagnes (planification Workfront)**

   * **Objectif :** définir les piliers stratégiques à long terme et les initiatives annuelles. Par exemple, définissez une initiative pour votre organisation appelée « Notoriété mondiale de la marque FY26 ». Il s’agit de votre objectif pour une période donnée. Créez des campagnes pour prendre en charge cette initiative.

   * **Personnes :** les parties prenantes à ce niveau peuvent être un responsable marketing, un vice-président marketing ou d’autres prospects stratégiques.

  Pour plus d’informations, consultez [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

* **Niveau 2 : tactiques des canaux (planification Workfront)**

   * **Focus :** définit les résumés opérationnels qui décrivent le « quoi » pour des canaux spécifiques. Il s&#39;agit de la dernière couche d&#39;intention stratégique avant le début des travaux. Par exemple, créez une tactique « Blitz sur les médias sociaux du 1er trimestre ». Vous pouvez ensuite l’associer à vos campagnes .

   * **Personnes :** les principales parties prenantes sont un responsable des opérations marketing, des responsables de canaux ou des responsables de campagne.

* **Niveau 3 : projets (Planification et Workfront)**

   * **Se concentrer :** exécuter sur les expériences ou activités exactes qui accompliront finalement votre initiative. Certains des éléments livrables sont spécifiques, tels que les publications sur les réseaux sociaux, les e-mails, les pages web.

   * **Implémentation :** vous pouvez créer des tactiques dans Planning et les lier directement à des **projets** dans Workfront, où les diffusions individuelles sont gérées sous la forme de tâches et d&#39;événements.

   * **Persona :** principales parties prenantes ici sont les créatifs, les contributeurs individuels, toute personne responsable de faire le travail pour soutenir l&#39;initiative.

### Extension stratégique : comment ajouter d’autres niveaux

Une fois le chemin d’accès de base établi, vous pouvez choisir d’ajouter des couches supplémentaires après avoir soigneusement examiné leur complexité commerciale spécifique.

Il peut s’avérer utile de créer les éléments supplémentaires suivants :

* **Plans de canaux :** couche entre les campagnes et les tactiques pour regrouper les stratégies interfonctionnelles. Par exemple, un plan appelé « Stratégie numérique ».

* **Activités :** si vous travaillez dans un environnement à faible volume (vous pouvez avoir 5 000 livrables ou moins par an), certaines équipes peuvent préférer effectuer le suivi d’expériences individuelles sous la forme d’enregistrements Workfront Planning avant qu’elles ne deviennent des projets Workfront.

>[!IMPORTANT]
>
>Si votre organisation produit plus de 5 000 activités par an, vous devez déplacer le suivi des diffusions individuelles vers Workfront.
>
>La gestion des enregistrements d’expérience volumineux dans Planning peut entraîner une accumulation de données qui obscurcit votre visibilité stratégique.
>Nous recommandons cette règle générale pour une efficacité maximale :
>
>* Utiliser Planning pour les champs « pourquoi » et « quoi »
>* Utilisez Workfront pour le « comment » relatif aux volumes élevés.

## Comprendre les centres de gravité pour construire votre architecture

Un système d’enregistrement marketing de niveau entreprise n’est pas créé dans un seul espace de travail. Elle utilise une architecture en « étoile » où les types d&#39;enregistrements sont gérés dans leurs centres de gravité naturels.

Pour plus d’informations, voir [Déploiement de votre page d’accueil stratégique : une page de lancement de 30 jours](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md).

Pour créer votre architecture à l’aide de l’approche en étoile, vous devez créer les éléments suivants :

* Un hub de taxonomie
* Un espace de travail de planification stratégique
* Rayons fonctionnels

### Créer le hub de taxonomie en tant que classifications

Vous devez d’abord créer un espace de travail centralisé pour vos classifications globales afin de définir les principaux concepts que tous les membres de votre organisation doivent comprendre. Par exemple, créez les types d’enregistrements suivants dans un espace de travail central : Marques, Régions, Produits, Personnes.

Pour plus d’informations, consultez [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

Établissez les éléments suivants lorsque vous créez vos classifications :

* **Emplacement du Principal :** choisissez un espace de travail principal. Cet espace de travail doit être la source de vérité pour les types d’enregistrements que vous créez.

* **L’avantage :** en synthétisant ces définitions avec le reste de l’entreprise, vous clarifiez le fait que des concepts tels que « Région : EMEA » signifient la même chose pour chaque équipe.

### Créez l’espace de travail de planification stratégique en tant que centre exécutif

Le centre exécutif est l’endroit où se trouvent les campagnes de haut niveau (et les plans de canal).

* **Emplacement du Principal :** il s’agit du centre de gravité exécutif, offrant un environnement silencieux pour la prise de décision stratégique.

* **L’avantage :** leadership peut gérer le portefeuille de campagnes sans écouter le bruit tactique au jour le jour.

### Définir les rayons fonctionnels comme espaces de travail de vos équipes

Les entités fonctionnelles (réseaux sociaux, Creative, e-mail) disposent de leurs propres espaces de travail pour gérer leurs tactiques.

* **Emplacement du Principal :** ces espaces de travail sont les centres de gravité individuels pour l&#39;exécution de l&#39;équipe locale.

* **L’avantage :** les équipes utilisent les campagnes et classifications globales à partir des hubs, tout en conservant leurs propres objets locaux.

  Par exemple, l’équipe peut ajouter le type d’enregistrement Campagne de l’espace de travail central à l’espace de travail de son équipe, mais créer des campagnes pertinentes uniquement pour son espace de travail. Parmi les exemples de campagnes, citons les « Supports » ou les « Droits d’utilisation ».

## Utiliser une approche de gouvernance basée sur les substantifs

Pour vous assurer que votre architecture résiste à la pression, suivez le principe de gouvernance basée sur les substantifs.

Voici nos recommandations pour la création de vos entités dans Workfront Planning :

* **Utilisez des noms, pas des verbes :** nommez vos types d’enregistrements d’après les éléments que vous suivez (nommez-les « Campagne » ou « Tactique »), et non d’après les actions à effectuer (ne les nommez pas « Campagne » ou « Planification »).

* **Normaliser la nomenclature :** utilisez les mêmes noms dans tous les espaces de travail. Vous pouvez ainsi agréger les données de l’ensemble du portefeuille pour les rapports exécutifs.

## Qu’en est-il des portefeuilles et programmes existants ?

Une question courante pour les organisations matures est de savoir comment gérer les portefeuilles et programmes qu’elles ont déjà créés dans Workfront. Par le passé, ces objets étaient souvent utilisés pour imiter la planification stratégique.

Nous vous recommandons maintenant de passer à la planification Workfront, qui correspond naturellement à l’approche stratégique de la planification.

### Remplacer les portefeuilles et programmes par des types d&#39;enregistrements

Dans de nombreuses organisations, les portefeuilles sont utilisés pour représenter des marques ou des unités opérationnelles de haut niveau, tandis que les programmes représentent des thèmes stratégiques.

Dans Workfront Planning, il est préférable de les modéliser en tant que types d’enregistrements dans votre hub de taxonomie.

En traitant une marque ou une unité opérationnelle comme un type d’enregistrement, vous pouvez les lier à une campagne ou à une tactique dans l’ensemble de l’entreprise, offrant ainsi un reporting beaucoup plus flexible qu’une structure statique Portfolio - Programme.

### Utilisation d’une stratégie de reporting-bridge

Bien que la planification Workfront soit l’avenir de l’intention stratégique, ses rapports natifs via le tableau de bord de la zone de travail sont encore en cours de développement.

De nombreuses entreprises s’appuient toujours sur les solides fonctionnalités de création de rapports liées à leurs anciennes structures de Portfolio et de programme dans Workfront.

Nous recommandons ce qui suit :

* Ne supprimez pas vos portefeuilles et programmes.
* Utilisez les automatisations de Planning pour créer un pont entre vos types d&#39;enregistrements et vos portefeuilles et programmes.

  Lors de la création d’une tactique ou d’une campagne dans Workfront Planning, cet enregistrement peut générer un Portfolio ou un programme correspondant dans Workfront.

  Pour plus d’informations, voir [Création d’objets à l’aide des automatisations d’enregistrements Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Cela vous permet d’effectuer les opérations suivantes :

* Profitez de la visualisation stratégique de qualité supérieure de Workfront Planning à l’aide de calendriers et de chronologies.

* Conservez les rapports hérités dans Workfront pour les parties prenantes qui ne sont pas encore prêtes à passer à la zone de travail.

## Bonnes pratiques et conseils

### Dos

* **Respectez l’approche de base « chemin d’accès d’abord » :** établissez votre flux de Campagne à tactique à projet avant d’ajouter plus de complexité.

* **Désigner les espaces de travail principaux :** assurez-vous que chaque type d’enregistrement comporte un espace de travail principal (considérez que son centre de gravité) qui agit comme agrégateur pour le compte rendu des performances.

* **Hiérarchiser les formulaires de demande pour le processus de réception :** utilisez des formulaires d’enregistrement pour les groupes moins complexes dans Workfront Planning afin d’assurer l’intégrité des métadonnées.

  >[!CAUTION]
  >
  >Bien que les utilisateurs expérimentés puissent bénéficier de la saisie directe des données dans les vues de tableau, cette opération doit être abordée avec prudence.
  >Les modifications en bloc d’un tableau peuvent facilement créer des casse-têtes de données pour d’autres parties prenantes.

### Ne pas

* **N’utilisez pas de généralisations :** par exemple, au lieu de parler d’un environnement « principal », référez-vous spécifiquement à Workfront et à l’objet Projet lorsque vous parlez d’exécution.

* **Ne pas trop compliquer :** chaque niveau supplémentaire de hiérarchie ajoute une taxe de gestion. Ajoutez uniquement des niveaux qui répondent à une question professionnelle à laquelle vous ne pouvez pas répondre actuellement.

* **Ne pas créer de silos :** assurez-vous que vos types d’enregistrements sont partagés entre les espaces de travail afin que les équipes ne saisissent pas à nouveau les mêmes données.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->