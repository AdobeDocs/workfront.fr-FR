---
title: 'Playbook : mise à l’échelle gérée, après la première victoire'
description: Découvrez comment déployer Adobe Workfront Planning après votre première implémentation réussie.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 28913661935d5a030cb33dd204fcb3c08daf0b26
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---


# Playbook : mise à l&#39;échelle gérée, après la première victoire

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