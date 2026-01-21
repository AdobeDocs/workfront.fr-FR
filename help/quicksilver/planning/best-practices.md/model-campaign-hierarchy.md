---
title: 'Le framework de la réussite : modéliser la hiérarchie de votre campagne'
description: Découvrez comment traduire vos processus d’entreprise complexes en une hiérarchie de campagnes évolutive et régie à l’aide de « centres de gravité » et d’une architecture multi-espace de travail.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 1158a49fc0b39ef49f23326935d4635530501687
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---


# Le framework de la réussite : modélisez la hiérarchie de vos campagnes



## Objectif

Découvrez comment traduire vos processus d’entreprise complexes en une hiérarchie de campagnes évolutive et régie à l’aide de « centres de gravité » et d’une architecture multi-espace de travail.



## Vue d’ensemble

La complexité des données augmente à mesure que vos opérations marketing se développent. Sans plan directeur clair, votre système d’enregistrement marketing (MSOR) peut rapidement devenir un « tiroir à rebuts » composé d’enregistrements déconnectés, de terminologie en conflit et de silos de création de rapports.



Le « Plan directeur de la réussite » est un framework permettant de modéliser la hiérarchie de vos campagnes dans Workfront Planning. Il vous fait passer du « chaos des feuilles de calcul » à un modèle régi et orienté objet qui garantit que chaque équipe parle le même langage tout en conservant l’agilité dont elle a besoin pour s’exécuter.



## La hiérarchie : trouver vos niveaux d’intention

Pour maintenir la clarté et l’évolutivité, nous vous recommandons de commencer par un **chemin principal** éprouvé. Bien que les entreprises puissent étendre cette hiérarchie à mesure que leurs besoins opérationnels évoluent, la mise en œuvre de ces trois niveaux permet d’assurer un lien étroit entre la stratégie et l’exécution.



### La voie principale : stratégie vers l’action

La plupart des implémentations réussies s’appuient sur un modèle propre à trois niveaux qui couvre à la fois Planning et Workflow :



1. **Niveau 1 : Campagnes (Module De Planification)**

   * **Point de mire** piliers stratégiques à long terme et initiatives annuelles (p. ex. « sensibilisation à la marque mondiale pour l&#39;exercice 26 »).

   * **Persona :** directeur marketing, vice-président du marketing, responsables stratégiques.

2. **Niveau 2 : tactiques des canaux (module de planification)**

   * **Focus :** les notes d’information opérationnelles définissant le « quoi » pour des canaux spécifiques (par exemple, « Q1 Social Media Blitz »). Il s&#39;agit de la dernière couche d&#39;intention stratégique avant le début des travaux.

   * **Persona : Opérations Marketing**, Responsables De Canal, Responsables De Campagne.

3. **Niveau 3 : projets de workflow (module de workflow)**

   * **Focus :** exécution réelle d’« expériences » ou d’« activités » (par exemple, publications sociales spécifiques, e-mails, pages web).

   * **Implémentation :** les tactiques de la planification sont liées directement à **Projets** dans le module Workflow, où les diffusions individuelles sont gérées comme des tâches et des événements.

   * **Persona :** créatifs, contributeurs individuels.



### Expansion stratégique : ajout de niveaux supplémentaires

Une fois le chemin d’accès de base établi, les entreprises peuvent choisir d’ajouter des couches supplémentaires après avoir soigneusement examiné leur complexité commerciale spécifique :



* **Plans de canaux :** couche comprise entre *Campagnes* et *Tactiques* pour regrouper les stratégies interfonctionnelles (par exemple, « Stratégie numérique »).

* **Activités de planification Workfront :** dans les environnements à faible volume (généralement &lt; 5 000 livrables/an), certaines équipes préfèrent effectuer le suivi des « expériences » individuelles en tant qu’enregistrements de planification Workfront avant de devenir des projets.


>[!TIP]
>
>**Conseil Crucial : Le Seuil De 5 000 Livrables**
>
>Si votre organisation produit plus de 5 000 activités par an, vous devez **toujours** décharger le suivi des diffusions individuelles sur le **module de workflow**. La gestion des enregistrements « Expérience » volumineux dans Planning peut entraîner une accumulation de données qui obscurcit votre visibilité stratégique. Utilisez Planning pour les champs « Pourquoi » et « Quoi », et le module Workflow pour le champ « Comment » volumineux.



## Architecture : Centres de gravité

Un modèle MSOR de niveau entreprise n&#39;est pas construit dans un seul espace de travail. Il utilise une architecture « en étoile » où les types d’enregistrements sont gérés dans leurs **centres de gravité** naturels.



### &#x200B;1. Le Hub De Taxonomie (Classifications)

Créez un espace de travail centralisé pour vos « classifications globales » (par exemple, marques, régions, produits, personas).

* **Emplacement du Principal :** cet espace de travail est le « Source de vérité » pour ces objets.

* **L’avantage :** en synthétisant ces définitions avec le reste de l’entreprise, vous résolvez la « dérive sémantique », en vous assurant que « Région : EMEA » signifie la même chose pour chaque équipe.



### &#x200B;2. Le Workspace de la planification stratégique (Centre exécutif)

C’est là que se trouvent les **campagnes** de haut niveau (et les **plans de canal**).

* **Emplacement du Principal :** il s’agit du centre de gravité exécutif, offrant un environnement silencieux pour la prise de décision stratégique.

* **L’avantage :** leadership peut gérer le portefeuille sans voir le désordre tactique au jour le jour.



### &#x200B;3. Rayons fonctionnels (espaces de travail d’équipe)

Les entités fonctionnelles (réseaux sociaux, Creative, e-mail) disposent de leurs propres espaces de travail pour gérer leurs **tactiques**.

* **Emplacement du Principal :** ces espaces de travail sont le centre de gravité de l&#39;exécution de l&#39;équipe locale.

* **L’avantage :** les équipes « consomment » les campagnes et classifications globales à partir des hubs, tout en conservant leurs propres objets locaux (tels que *Media Outlets* ou *Usage Rights*).



## Gouvernance Fondée Sur Les Noms : Parler Une Langue

Pour vous assurer que votre plan tient la route, respectez le principe de la **gouvernance par substantif**.



* **Utiliser des noms, pas des verbes :** attribuez un nom à vos types d’enregistrements d’après les « choses » que vous suivez (`Campaign`, `Tactic`), et non d’après les « actions » (`Campaigning`, `Planning`).

* **Nomenclature normalisée :** utilisez les mêmes noms sur tous les espaces de travail. Vous pouvez ainsi agréger les données de l’ensemble du portefeuille pour les rapports exécutifs.



## Qu&#39;en est-il des portefeuilles et programmes existants ?

Une question courante pour les organisations matures est de savoir comment gérer les portefeuilles et programmes qu’elles ont déjà créés dans le module **Workflow**. Par le passé, ces objets étaient souvent utilisés pour imiter la planification stratégique.



### &#x200B;1. Portefeuilles et programmes → types d’enregistrements

Dans de nombreuses organisations, les **Portfolios** sont utilisés pour représenter des marques ou des unités opérationnelles (BU) de haut niveau, tandis que les **Programmes** représentent des thèmes stratégiques.

* **Maj :** il est préférable de les modéliser en tant que **types d’enregistrement** dans votre **centre de taxonomie**. En traitant les types d’enregistrements « Marque » ou « Unité opérationnelle » comme des types d’enregistrements, vous pouvez les lier à n’importe quelle campagne ou tactique dans l’ensemble de l’entreprise, fournissant ainsi des rapports beaucoup plus flexibles qu’une structure Portfolio/programme statique.



### &#x200B;2. La stratégie « Reporting Bridge »

Bien que la planification Workfront soit l’avenir de l’intention stratégique, ses rapports natifs via **Tableaux de bord de la zone de travail** sont toujours en cours de développement. De nombreuses entreprises s’appuient toujours sur les solides fonctionnalités de création de rapports liées à leurs anciennes structures de Portfolio et de programme dans le module Workflow .

* **Recommandation** ne supprimez pas encore vos portefeuilles et programmes. Utilisez plutôt **Fusion Automations** pour créer un pont.

* **Fonctionnement :** lors de la création d’une tactique ou d’une campagne dans Workfront Planning, Fusion peut automatiquement mettre en miroir cet enregistrement dans un Portfolio ou un programme correspondant dans le module Workflow. Cela vous permet d’effectuer les opérations suivantes :

   1. Profitez de la qualité supérieure de la **visualisation stratégique** de Workfront Planning (calendriers/chronologies).

   2. Conservez vos **rapports hérités** dans le module Workflow pour les parties prenantes qui ne sont pas encore prêtes à passer à la zone de travail.

## Bonnes pratiques et conseils

### Faire :

* **Collez d’abord au chemin principal.** Établissez votre flux de campagne à tactique à projet avant d’ajouter plus de complexité.

* **Désigner des espaces de travail de Principal.** Assurez-vous que chaque type d’enregistrement dispose d’un espace de travail « d’accueil » (son centre de gravité) qui agit comme agrégateur pour la création de rapports.

* **Définition de la priorité de Forms pour la réception.** Utilisez des formulaires d’enregistrement pour les groupes moins sophistiqués dans Workfront Planning afin d’assurer l’intégrité des métadonnées. Bien que les utilisateurs expérimentés puissent bénéficier de la saisie directe des données dans les vues Tableau , cette opération doit être abordée avec précaution. Les modifications en masse dans un tableau peuvent facilement créer des problèmes de données pour d’autres parties prenantes.


### Ne pas :

* **Ne dis pas « Core ».** Se référer spécifiquement au module **Workflow** et aux objets **Project** lorsque l&#39;on parle d&#39;exécution.

* **Ne complique pas trop.** Chaque niveau supplémentaire de hiérarchie ajoute une « taxe de gestion ». Ajoutez uniquement des niveaux qui répondent à une question professionnelle à laquelle vous ne pouvez pas répondre actuellement.

* **Ne créez pas de silos.** Assurez-vous que vos types d’enregistrements sont partagés dans tous les espaces de travail afin que les équipes ne saisissent pas à nouveau les mêmes données.




