---
title: 'Playbook : mise à l’échelle gérée, après la première victoire'
description: Découvrez comment déployer Adobe Workfront Planning après votre première implémentation réussie.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 54df36b3-01a3-4fd3-b2d3-64ffb2fe5918
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# Playbook : mise à l&#39;échelle gérée, après la première victoire

{{planning-important-intro}}

**Version** : 1.0

**Contexte** : « Nous avons réussi notre premier cas d’utilisation, et maintenant tout le monde veut y participer. »



## &#x200B;1. Le « piège du succès »

Parfois, il peut sembler que la phase la plus dangereuse de l&#39;adoption du PAM se situe immédiatement après le premier cas d&#39;utilisation réussi ou POC. L&#39;enthousiasme est grand, mais la crainte d&#39;une « dette technique » et d&#39;un « étalement administratif » peut conduire à deux réactions tout aussi dommageables :

1. **Sur-gouvernance** : verrouiller le système si étroitement que les nouvelles équipes reviennent aux feuilles de calcul.

2. **Gouvernance zéro** : laissez chaque équipe créer ses propres champs et types d’enregistrements, en recréant l’étalement de métadonnées fragmentées présent dans les environnements hérités.



## &#x200B;2. La philosophie de base : le PAM comme « moteur de réconciliation »

Au lieu d&#39;essayer d&#39;empêcher les équipes d&#39;être différentes, nous positionnons le PAM comme l&#39;endroit où ces différences sont **rendues visibles afin qu&#39;elles puissent être réconciliées**.



* **Gestion de la vitesse d’adoption** : il est naturel de se montrer prudent avant de développer un nouvel outil avant de « nettoyer » les environnements existants. Si le choix de **Simplifier d’abord** offre une base très gouvernée, il peut retarder le délai de rentabilisation pour les équipes prêtes à s’aligner. Nous croyons que la façon la plus efficace de mener à bien ce changement est de reconnaître que **la visibilité est l&#39;étape 1**. L’élan vers un outil partagé et prêt pour l’entreprise (en s’éloignant de l’étalement des stratégies de partenariat et des feuilles de calcul) est ce qui finit par débloquer les objectifs à long terme.



  **Recommandation** : Au lieu d&#39;un mandat « Nettoyage d&#39;abord », nous recommandons d&#39;affecter une plus petite partie des ressources à la maintenance continue et une plus grande partie à la résolution des besoins opérationnels urgents. Par exemple, passer un an uniquement à « nettoyer » les taxonomies produit peu de valeur incrémentale. Cependant, offrir une **visibilité interéquipes** (par exemple, par le biais d’un calendrier d’entreprise unifié ou d’une feuille de route GTM consolidée) offre la valeur de transformation dont vos parties prenantes ont besoin, tout en fournissant la structure de données unifiée dont vous avez besoin pour gérer l’environnement au fil du temps.

* **Reconnaître la réalité** : Les équipes indépendantes développent naturellement leurs propres processus, qui restent souvent cachés dans des feuilles de calcul compartimentées. La transition vers le PAM ne crée pas de désordre, elle met en lumière celui qui existe déjà. En rendant ces processus visibles dans un environnement partagé, vous les mettez au même endroit où ils peuvent enfin être traités et améliorés.

* **Le signal de progression** : lorsqu’une équipe demande ses propres champs, ce n’est pas de l’« étalement », mais bien de l’**adoption**. Cela signifie qu&#39;ils considèrent le PAM comme leur espace de travail.

* **Gérer la dette, ne la cachez pas** : il est naturel de s&#39;inquiéter des efforts nécessaires pour nettoyer ultérieurement les taxonomies divergentes. Cependant, l’alternative (imposer des normes strictes trop tôt) pousse souvent les équipes à revenir à des feuilles de calcul où leurs processus (et leur dette) restent cachés. En permettant aux équipes de commencer au PAM avec leurs classifications actuelles, vous déplacez cette dette vers un environnement visible et régi. Cela fait de la réconciliation finale une tâche itérative plutôt qu&#39;un projet de migration unique et écrasant.



## &#x200B;3. Le modèle de gouvernance « Couloirs sur route »

Échelonner sans endettement en définissant les « voies globales » et les « terrains de jeu locaux ».



### A. Voies Globales

* **Objets contrôlés** : objets que chaque équipe doit utiliser pour le reporting d&#39;entreprise (par exemple, `Strategic Pillar`, `Region`, `Fiscal Quarter`).

* **Géré par** : l’administrateur central du code/des opérations marketing.

* **Règle** : ces champs sont « Partagés » et obligatoires.



### B. Les Terrains De Jeux Locaux (Rayons)

* **Objets expérimentaux** : champs ou types d’enregistrements spécifiques aux besoins tactiques d’une équipe (par exemple, `Influencer Handle` d’une équipe sociale ou `URL Slug` d’une équipe web).

* **Géré par** : le chef d’équipe (avec des conseils légers).

* **Règle** : les équipes peuvent innover ici. Si un champ « Local » est adopté par >3 équipes, il est « promu » en piste globale.



## &#x200B;4. Le Paradoxe De La Gouvernance : Les Équipes D’Abord, Les Normes Suivent

Un défi commun dans l&#39;expansion du PAM est de décider lequel vient en premier : **Gouvernance d&#39;entreprise** ou **Alignement opérationnel des équipes**.



Nous pensons que la manière la plus efficace de gérer cette situation est de reconnaître que la valeur de l’entreprise est construite dans les deux sens :

1. **Les équipes ont besoin de pertinence** : L’entreprise ne tire parti de la valeur que lorsque ses équipes sont activement en cours d’exécution. Par conséquent, la gouvernance doit **servir les équipes** en fournissant une structure qui répond à leurs besoins opérationnels connus.

2. **L’entreprise a besoin de visibilité** : la direction ne peut prendre des décisions informées que lorsque les données sont suffisamment claires pour être agrégées. Par conséquent, les équipes doivent **servir l’entreprise** en fournissant le minimum de métadonnées viables requises pour la visibilité du portefeuille.



Le but de la « mise à l’échelle gérée » est de trouver l’intersection de ces deux besoins, en assurant une normalisation suffisante pour fournir une visibilité, mais pas au point de bloquer l’exécution de l’équipe.



### A. Alignement des priorités : données par rapport à visualisation

Lors de la mise à l’échelle, reconnaissez que la définition de « Valeur » diffère entre les personnages :

* **Administrateur/Propriétaire de produit** : valeurs **taxonomies et classifications unifiées**. Leur objectif est une architecture de données propre qui prend en charge l’évolutivité à long terme.

* **Partie prenante/leader** : valeurs **visualisation et insight** (par exemple, un calendrier global ou un calendrier Portfolio). Leur objectif est le « moment d’éclair » qui rend les données exploitables.



**La stratégie** : utilisez le besoin de visualisation des parties prenantes comme *incitation* pour que l’équipe respecte les normes de données requises par l’administrateur. Vous obtenez la taxonomie unifiée en fournissant le « Super Calendrier » que le leadership exige.



### B. La Phase D&#39;Observation « Dirigée Par Les Services »

Lors de la mise à l’échelle précoce, le rôle de l’administrateur est de faciliter cet échange entre les équipes et l’entreprise.

* **Donner la priorité aux opérations sur la normalisation** : il est préférable que les équipes planifient activement les espaces de travail compartimentés plutôt que de les voir bloquées par un manque de définitions globales. Cette activité constitue les « données brutes » requises pour établir des normes saines et concrètes.

* **Identifier les « minimums de visibilité »** : travaillez avec les dirigeants pour identifier les 3 à 5 champs qui *doivent* être propres pour les rapports d’entreprise (par exemple, `Strategic Alignment`, `Start Date`, `Budget`). Concentrez votre énergie d&#39;application SEULEMENT ici.



### B. Harmonisation rétroactive (gouvernance en tant que service)

Une fois qu’un modèle de « besoins connus » apparaît au sein des équipes, l’entreprise peut procéder à la consolidation de ces modèles en un service global.

1. **Observer les modèles réussis** : identifiez les taxonomies « gagnantes » que les équipes ont déjà créées et adoptées.

2. **L’établissement d’une poignée de main collaborative** : rassemblez les champions de l’équipe pour affiner leurs réussites locales dans une norme d’entreprise partagée.

3. **Déployer en tant que service** : le déploiement des nouvelles pistes globales n’est pas une « restriction », mais un moyen de simplifier le reporting et l’alignement entre les équipes pour les personnes qui effectuent le travail.



**Principaux points à retenir** : la gouvernance devrait être une réponse au succès opérationnel et non une condition préalable à celui-ci.



## &#x200B;5. Mécanismes d’échelonnement : modèle de croissance fondé sur les modèles

L’application de cette philosophie nécessite une approche réfléchie de la structure des données. Pour éviter « l&#39;étalement de la gouvernance », résistez à l&#39;envie de construire des champs globaux pour chaque demande individuelle. Utilisez plutôt le **chemin de maturité du champ** pour permettre à l’utilisation réelle de guider les normes de votre entreprise :



1. **Niveau 1 : expérience locale** : l’équipe A crée un champ personnalisé dans son espace de travail.

2. **Niveau 2 : reconnaissance des motifs** : l’administrateur constate que les équipes B et C utilisent ou demandent un champ similaire.

3. **Niveau 3 : normalisation des entreprises** : l’administrateur crée une version unique et normalisée de ce champ en tant que type d’enregistrement dans le **Workspace de taxonomie globale** et l’associe aux équipes.



### Les mécanismes de la « retraite douce »

Comme le PAM ne dispose pas actuellement d&#39;une fonctionnalité native d&#39;« archivage » pour les champs, le retrait d&#39;un champ local nécessite un processus délibéré de « retrait progressif » pour conserver les données historiques sans encombrer l&#39;interface utilisateur :



1. **Migration des données** : utilisez une vue de tableau (ou Fusion) pour copier en masse les valeurs du champ local « Ombre » dans le nouveau champ de piste globale. Assurez-vous que les données sont validées et nettoyées pendant ce déplacement.

2. **Renommer en cas d’obsolescence** : renommez le champ local avec un préfixe tel que `[DEPRECATED]` ou `z_` (par exemple, `z_Language (Old)`). Cela pousse le champ au bas des sélecteurs de champ et signale aux utilisateurs qu&#39;il n&#39;est plus le « Source de la vérité ».

3. **Suppression de formulaire** : **Il s’agit de l’étape la plus critique.** Supprimer le champ obsolète de tous les **Record Forms**. Cela empêche la saisie de nouvelles données tout en conservant les anciennes données visibles dans les tableaux ou rapports existants, si nécessaire.

4. **Période de « fin de vie »** : conservez le champ obsolète (avec préfixe et hors formulaire) pendant 30 à 60 jours pour vous assurer qu’aucune donnée n’a été manquée lors de la migration. Passé ce délai, si les données sont entièrement réconciliées dans la piste globale, le champ local peut être supprimé de l’espace de travail.



## &#x200B;6. Éviter la « dérive du noyau » (la règle de l&#39;abstraction)

Pour éviter que Planning ne devienne aussi encombré que Core :

* **La couche d&#39;abstraction** : Chaque champ du PAM devrait répondre à une **question stratégique**. Si un champ est uniquement utilisé pour le suivi tactique (par exemple, « Cette épreuve a-t-elle été approuvée ? »), conservez-le dans Core.

* **Consolidation d’abord** : si une équipe souhaite un nouveau champ de métadonnées, invitez-la à vérifier d’abord la taxonomie globale. Cela nécessite d’accorder aux responsables d’équipe **accès en lecture seule** à l’espace de travail Taxonomie globale (voir la section 7). En associant leurs besoins tactiques à un champ stratégique existant, vous évitez les doublons inutiles et préservez l’intégrité des rapports.



## &#x200B;7. Le Modèle De Visibilité « Accès En Lecture Seule »

Résolvez le sentiment « Siloed » sans le bruit du travail « Siloed ».

* **Le problème** : les équipes dans les rayons se sentent isolées car elles ne voient que leurs propres enregistrements.

* **Correctif** : accordez aux équipes **accès en lecture seule aux espaces de travail désignés comme « Principal » pour ces types d’enregistrements partagés**.

* **Résultat** : ils peuvent s’inspirer du contexte plus large de l’entreprise et s’y aligner, mais leur espace de travail local reste propre et axé sur leurs tâches spécifiques.



## &#x200B;8. Gérer la croissance au moyen d’ateliers

L&#39;expansion du PAM est tout autant un défi culturel qu&#39;un défi technique. Utiliser des ateliers ciblés pour combler le « fossé de gouvernance ».



### A. L&#39;atelier de découverte du « Gâchis nécessaire »

* **Audience** : responsables marketing régionaux et champions des opérations.

* **Objectif** : documenter la « réalité compartimentée » actuelle (les données opérationnelles fragmentées).

* **Le message** : « Nous ne sommes pas ici pour supprimer vos champs. Nous sommes ici pour comprendre comment ils sont liés à la stratégie mondiale. »

* **Résultat** : Projet de cartographie des champs tactiques locaux aux voies stratégiques mondiales.



### B. Séance d&#39;alignement sur la « visibilité stratégique »

* **Audience** : parties prenantes du marketing de haut niveau (leadership).

* **Objectif** : Recadrer l’anxiété de « Simplifier d’abord ».

* **Le Message** : « Nous n’avons pas besoin d’une taxonomie parfaite pour commencer. Nous utilisons le PAM comme environnement pour *construire* la taxonomie parfaite ».

* **Résultat** : Approbation de l&#39;adoption du PAM en tant que moteur de réconciliation, alors que Core reste dans son état actuel.



### C. La vitrine « Spoke-to-Global »

* **Audience** : nouvelles équipes qui explorent le PAM.

* **Objectif** : Réduire le sentiment de « cloisonnement ».

* **Le message** : « Voyez comment le travail local de l’équipe A alimente automatiquement le Workspace de Principal désigné ? Vous pouvez avoir la même visibilité pour votre travail. »

* **Résultat** : Souscription des nouveaux départements qui voient l’avantage d’être « connectés » sans perdre leur indépendance locale.



### D. Heures d’ouverture du « support continu »

* **Public** : Tous les utilisateurs du PAM (actuels et futurs).

* **Objectif** : fournir un environnement récurrent et à faibles enjeux pour le dépannage et les conseils tactiques.

* **Le message** : « Il n’y a pas de mauvaises questions. Nous sommes là pour vous aider à résoudre vos problèmes de planification spécifiques en temps réel. »

* **Résultat** : confiance accrue des utilisateurs, résolution plus rapide des frictions techniques et identification de nouveaux schémas qui pourraient justifier une normalisation mondiale.



## &#x200B;9. Dotation en personnel en fonction de l&#39;échelle : rôles et responsabilités

La réussite d’un modèle de mise à l’échelle géré nécessite plus qu’une simple configuration d’outil ; elle nécessite une répartition claire des rôles entre les équipes globales et en étoile.



### A. L’architecte d’entreprise (central COE/opérations marketing)

* **Focus** : intégrité de l’entreprise, performances du système et **taxonomie des données unifiée**.

* **Responsabilités** :

   * Gère **Global Taxonomy Workspace**.

   * Facilite le **parcours de maturité du terrain** (promotion des réussites locales aux normes mondiales).

   * Conserve les vues **Principal Workspace** pour les rapports exécutifs.

   * Dirige l’**audit sémantique** mensuel sur tous les espaces de travail.



### B. Le champion parlé (propriétaire du processus d’équipe)

* **Focus** : pertinence de l’équipe et vitesse d’adoption.

* **Responsabilités** :

   * Il sert de point de contact unique pour l’équipe fonctionnelle.

   * possède la structure de l’espace de travail local et les expériences de champs personnalisés ;

   * S’assure que l’équipe utilise la **passerelle régie** (Forms) pour la saisie des données.

   * Participe à l’**poignée de main collaborative** lors de l’harmonisation.



### C. Partenaire exécutif (Marketing Leadership)

* **Focus** : alignement stratégique, visibilité OKR et **visualisation de portfolio (par exemple, calendrier global)**.

* **Responsabilités** :

   * Définit l’entreprise **OKR marketing** dans l’espace de travail Taxonomie globale.

   * Fait valoir la valeur de « l’étape 1 de visibilité » auprès des autres dirigeants.

   * Renforce l’allocation des ressources 80/20 (valeur par rapport au nettoyage).



### D. Responsable De L’Activation (Gestion Des Modifications)

* **Focus** : Changement culturel et développement des compétences.

* **Responsabilités** :

   * Héberge régulièrement des **Office Hours** et **Discovery Workshops**.

   * Conserve la vitrine interne « Success Story ».

   * Identifie les points de friction techniques que l’architecte d’entreprise doit résoudre.



## &#x200B;10. Liste de contrôle pour le développement de l’équipe suivante

* [ ] **Identifier le champion** : qui est le « propriétaire du processus » ou le « champion » de cette nouvelle équipe ?

* [ ] **Définir le « delta local »** : de quels 2 à 3 champs cette équipe a-t-elle besoin que la norme mondiale ne fournit pas actuellement ?

* [ ] **Mapper aux routes globales** : quels champs globaux existants peuvent répondre à 80 % de leurs besoins ?

* [ ] **Accorder une visibilité globale** : donnez-leur un accès en lecture seule aux espaces de travail de Principal appropriés et à l’espace de travail de taxonomie globale le jour 1.

* [ ] **Établir la remise** : comment leur travail « alimente »-t-il les espaces de travail de Principal pertinents ? (par exemple, via un type d’enregistrement global ou une recherche spécifique).

<!--original content: 

**Version**: 1.0 

**Context**: "We've landed our first use case, and now everyone wants in." 

 

## 1. The "Success Trap" 

Sometimes it can feel like the most dangerous phase of WFP adoption is immediately after the first successful use case or POC. Enthusiasm is high, but the fear of "technical debt" and "administrative sprawl" can lead to two equally damaging responses: 

1.  **Over-Governance**: Locking down the system so tightly that new teams revert to spreadsheets. 

2.  **Zero-Governance**: Letting every team create their own fields and record types, recreating the fragmented metadata sprawl found in legacy environments. 

 

## 2. The Core Philosophy: WFP as the "Reconciliation Engine" 

Instead of trying to stop teams from being different, we position WFP as the place where those differences are **made visible so they can be reconciled**. 

 

*   **Managing Adoption Velocity**: It is natural to feel cautious about expanding into a new tool before "cleaning up" existing environments. While choosing to **Simplify First** provides a highly governed foundation, it can delay time-to-value for teams ready to align. We believe the most effective way to lead through this change is to recognize that **visibility is Step 1**. Momentum toward a shared, enterprise-ready tool (moving away from the sprawl of PPTs and spreadsheets) is what ultimately unblocks long-term goals.  

 

    **Recommendation**: Instead of a "Clean Up First" mandate, we recommend allocating a smaller portion of resources to ongoing maintenance and a significantly larger portion to solving pressing business needs. For example, spending a year solely on "cleaning up" taxonomies yields little incremental value. However, delivering **cross-team visibility** (e.g., through a Unified Enterprise Calendar or a consolidated GTM roadmap) provides the transformative value your stakeholders need, while providing the unified data structure you need to govern the environment over time. 

*   **Acknowledge the Reality**: Independent teams naturally develop their own processes, which often stay hidden in siloed spreadsheets. Transitioning to WFP doesn't create a mess; it shines a light on the one that already exists. By making these processes visible in a shared environment, you put them in the one place where they can finally be addressed and improved. 

*   **The Progress Signal**: When a team asks for their own fields, it's not "sprawl"—it's **Adoption**. It means they see WFP as their workspace. 

*   **Manage Debt, Don't Hide It**: It is natural to be concerned about the effort required to clean up divergent taxonomies later. However, the alternative—forcing strict standards too early—often drives teams back to spreadsheets where their processes (and their debt) remain hidden. By allowing teams to begin in WFP with their current classifications, you are moving that debt into a visible, governed environment. This makes the eventual reconciliation an iterative task rather than a single, overwhelming migration project. 

 

## 3. The "Lanes on a Road" Governance Model 

Scale without debt by defining "Global Lanes" and "Local Playgrounds." 

 

### A. The Global Lanes 

*   **Controlled Objects**: Objects that every team must use for enterprise reporting (e.g., `Strategic Pillar`, `Region`, `Fiscal Quarter`). 

*   **Managed By**: The Central COE/Marketing Ops Admin. 

*   **Rule**: These fields are "Shared" and mandatory. 

 

### B. The Local Playgrounds (Spokes) 

*   **Experimental Objects**: Fields or record types specific to a team's tactical needs (e.g., a Social team's `Influencer Handle` or a Web team's `URL Slug`). 

*   **Managed By**: The Team Lead (with light guidance). 

*   **Rule**: Teams can innovate here. If a "Local" field is adopted by >3 teams, it is "Promoted" to a Global Lane. 

 

## 4. The Governance Paradox: Teams First, Standards Follow 

A common challenge in scaling WFP is deciding which comes first: **Enterprise Governance** or **Team Operational Alignment**.  

 

We believe the most effective way to navigate this is to recognize that enterprise value is built on a two-way street: 

1.  **Teams need relevance**: The enterprise only realizes value when its teams are actively executing. Therefore, governance must **serve the teams** by providing structure that supports their known operational needs. 

2.  **The Enterprise needs visibility**: Leadership can only make informed decisions when data is clean enough to aggregate. Therefore, the teams must **serve the enterprise** by providing the minimum viable metadata required for portfolio visibility. 

 

The goal of "Managed Scaling" is to find the intersection of these two needs—standardizing enough to provide visibility, but not so much that you stall team execution. 

 

### A. Aligning Priorities: Data vs. Visualization 

When scaling, recognize that the definition of "Value" differs between personas: 

*   **The Admin/Product Owner**: Values **unified taxonomies and classifications**. Their goal is a clean data architecture that supports long-term scalability. 

*   **The Stakeholder/Leader**: Values **visualization and insight** (e.g., a Global Calendar or a Portfolio Timeline). Their goal is the "Lightning Moment" that makes the data actionable. 

 

**The Strategy**: Use the stakeholder's need for visualization as the *incentive* for the team's compliance with the admin's need for data standards. You get the unified taxonomy by delivering the "Super Calendar" that leadership demands. 

 

### B. The "Service-Led" Observation Phase 

During early scale-up, the Admin's role is to facilitate this exchange between teams and the enterprise. 

*   **Prioritize Operation over Standardization**: It is better to have teams actively planning in siloed workspaces than to have them stalled by a lack of global definitions. This activity is the "raw data" required to build healthy, real-world standards. 

*   **Identify the "Visibility Minimums"**: Work with leadership to identify the 3-5 fields that *must* be clean for enterprise reporting (e.g., `Strategic Alignment`, `Start Date`, `Budget`). Focus your enforcement energy ONLY here. 

 

### B. Retroactive Harmonization (Governance as a Service) 

Once a pattern of "known needs" emerges across teams, the enterprise can move to consolidate those patterns into a global service. 

1.  **Observe Successful Patterns**: Identify the "winning" taxonomies that teams have already built and adopted. 

2.  **The Collaborative Handshake**: Bring team champions together to refine their local successes into a shared enterprise standard. 

3.  **Deploy as a Service**: Roll out the new global lanes not as a "restriction," but as a way to simplify reporting and cross-team alignment for the people doing the work. 

 

**Key Takeaway**: Governance should be a response to operational success, not a prerequisite for it.  

 

## 5. Scaling Mechanics: The Pattern-Based Growth Model 

Applying this philosophy requires a thoughtful approach to data structure. To avoid "Governance Sprawl," resist the urge to build global fields for every individual request. Instead, use the **Field Maturity Path** to let real-world usage guide your enterprise standards: 

 

1.  **Level 1: Local Experiment**: Team A creates a custom field in their workspace. 

2.  **Level 2: Pattern Recognition**: The Admin notices Teams B and C are using or asking for a similar field. 

3.  **Level 3: Enterprise Standardization**: The Admin creates a single, standardized version of that field as a record type in the **Global Taxonomy Workspace** and syndicates it to teams. 

 

### The Mechanics of "Soft Retirement" 

Because WFP does not currently have a native "Archive" feature for fields, retiring a local field requires a deliberate "Soft Retirement" process to preserve historical data without cluttering the UI: 

 

1.  **Data Migration**: Use a table view (or Fusion) to bulk-copy values from the local "Shadow" field into the new Global Lane field. Ensure the data is validated and cleaned during this move. 

2.  **Rename for Deprecation**: Rename the local field with a prefix like `[DEPRECATED]` or `z_` (e.g., `z_Language (Old)`). This pushes the field to the bottom of field pickers and signals to users that it is no longer the "Source of Truth." 

3.  **Form Removal**: **This is the most critical step.** Remove the deprecated field from all **Record Forms**. This prevents new data from being entered while keeping the old data visible in existing table views or reports if needed. 

4.  **The "Sunset" Period**: Keep the deprecated field (prefixed and off-form) for 30-60 days to ensure no data was missed during migration. After this period, if the data is fully reconciled in the Global Lane, the local field can be deleted from the workspace. 

 

## 6. Avoiding the "Core Drift" (The Abstraction Rule) 

To prevent Planning from becoming as cluttered as Core: 

*   **The Abstraction Layer**: Every field in WFP should answer a **Strategic Question**. If a field is only used for tactical tracking (e.g., "Was this proof approved?"), keep it in Core. 

*   **Consolidation First**: If a team wants a new metadata field, invite them to check the Global Taxonomy first. This requires granting team leads **Read-Only access** to the Global Taxonomy workspace (see Section 7). By mapping their tactical needs to an existing strategic field, you prevent unnecessary duplication and maintain reporting integrity. 

 

## 7. The "Read-Only Access" Visibility Model 

Solve the "Siloed" feeling without the noise of "Siloed" work. 

*   **The Problem**: Teams in spokes feel isolated because they only see their own records. 

*   **The Fix**: Grant teams **Read-Only access to the workspaces designated as 'Primary' for those shared record types**.  

*   **The Result**: They can see the broader enterprise context for inspiration and alignment, but their local workspace remains clean and focused on their specific tasks. 

 

## 8. Managing Growth through Workshops 

Scaling WFP is as much a cultural challenge as a technical one. Use targeted workshops to bridge the "Governance Gap." 

 

### A. The "Necessary Mess" Discovery Workshop 

*   **Audience**: Regional Marketing Leads and Ops Champions. 

*   **Goal**: Document the current "Siloed Reality" (the fragmented operational data). 

*   **The Message**: "We aren't here to delete your fields. We're here to understand how they link to the global strategy." 

*   **Outcome**: A draft mapping of local tactical fields to global strategic lanes. 

 

### B. The "Strategic Visibility" Alignment Session 

*   **Audience**: High-level Marketing Stakeholders (leadership). 

*   **Goal**: Reframe the "Simplify First" anxiety. 

*   **The Message**: "We don't need a perfect taxonomy to start. We are using WFP as the environment to *build* the perfect taxonomy." 

*   **Outcome**: Approval to move forward with WFP as the reconciliation engine while Core remains in its current state. 

 

### C. The "Spoke-to-Global" Showcase 

*   **Audience**: New teams exploring WFP. 

*   **Goal**: Reduce the "siloed" feeling. 

*   **The Message**: "See how Team A's local work automatically feeds the designated Primary Workspace? You can have that same visibility for your work too." 

*   **Outcome**: Opt-in from new departments who see the benefit of being "connected" without losing their local independence. 

 

### D. The "Ongoing Support" Office Hours 

*   **Audience**: All WFP users (current and prospective). 

*   **Goal**: Provide a recurring, low-stakes environment for troubleshooting and tactical guidance. 

*   **The Message**: "There are no wrong questions. We are here to help you solve your specific planning challenges in real-time." 

*   **Outcome**: Increased user confidence, faster resolution of technical friction, and the identification of new patterns that might warrant global standardization. 

 

## 9. Staffing for Scale: Roles and Responsibilities 

Success in a managed scaling model requires more than just tool configuration; it requires a clear distribution of roles across the Global and Spoke teams. 

 

### A. The Enterprise Architect (Central COE/Marketing Ops) 

*   **Focus**: Enterprise integrity, system performance, and **unified data taxonomy**. 

*   **Responsibilities**: 

    *   Manages the **Global Taxonomy Workspace**. 

    *   Facilitates the **Field Maturity Path** (promoting local successes to global standards). 

    *   Maintains the **Primary Workspace** views for executive reporting. 

    *   Leads the monthly **Semantic Audit** across workspaces. 

 

### B. The Spoke Champion (Team Process Owner) 

*   **Focus**: Team relevance and adoption velocity. 

*   **Responsibilities**: 

    *   Acts as the single point of contact for the functional team. 

    *   Owns the local workspace structure and custom field experiments. 

    *   Ensures the team uses the **Governed Gateway** (Forms) for data entry. 

    *   Participates in the **Collaborative Handshake** during harmonization. 

 

### C. The Executive Sponsor (Marketing Leadership) 

*   **Focus**: Strategic alignment, OKR visibility, and **portfolio visualization (e.g., Global Calendaring)**. 

*   **Responsibilities**: 

    *   Defines the enterprise **Marketing OKRs** in the Global Taxonomy workspace. 

    *   Champions the value of "Visibility Step 1" to other leaders. 

    *   Reinforces the 80/20 resource allocation (Value over Cleanup). 

 

### D. The Enablement Lead (Change Management) 

*   **Focus**: Cultural shift and skill development. 

*   **Responsibilities**: 

    *   Hosts recurring **Office Hours** and **Discovery Workshops**. 

    *   Maintains the internal "Success Story" showcase. 

    *   Identifies technical friction points for the Enterprise Architect to resolve. 

 

## 10. Checklist for Scaling the Next Team 

* [ ] **Identify the Champion**: Who is the "Process Owner" or "Champion" of this new team? 

* [ ] **Define the "Local Delta"**: What 2-3 fields does this team need that the Global standard doesn't currently provide? 

* [ ] **Map to Global Lanes**: Which existing Global fields can satisfy 80% of their needs? 

* [ ] **Grant Global Visibility**: Give them Read-Only access to the relevant Primary Workspaces and the Global Taxonomy workspace on Day 1. 

* [ ] **Establish the Handoff**: How does their work "feed" the relevant Primary Workspaces? (e.g., via a Global Record Type or a specific lookup).

-->