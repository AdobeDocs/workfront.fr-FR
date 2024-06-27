---
title: "Bonnes pratiques relatives à la planification Adobe Workfront"
description: En tant que personne responsable des opérations marketing, vous pouvez utiliser Adobe Workfront Planning pour organiser le travail de toutes vos équipes au cours du cycle de vie marketing. Voici quelques bonnes pratiques que nous vous recommandons lorsque vous commencez à planifier Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 5%

---


# Bonnes pratiques relatives à la planification Adobe Workfront

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

En tant que personne responsable des opérations marketing, vous pouvez utiliser Adobe Workfront Planning pour organiser le travail de toutes vos équipes au cours du cycle de vie marketing.

Cet article présente quelques bonnes pratiques que nous vous recommandons lorsque vous commencez à planifier Workfront.

## Qu’est-ce que la planification Workfront ?

Le module de planification de Workfront est l’une des trois fonctionnalités Workfront distinctes mais connectées qui, ensemble, créent un système d’enregistrement marketing. Les trois fonctionnalités sont les suivantes :

* **Planification**: nouvelles fonctionnalités avancées incluses dans la planification Workfront.

* **Workflow**: les fonctionnalités de gestion de travail collaboratif que vous utilisez aujourd’hui dans Workfront (gestion de projet, gestion des ressources, etc.)

* **Automatisation et intégration**: fonctionnalités complètes d’intégration et d’automatisation optimisées par Workfront Fusion.

La planification Workfront est hautement personnalisable. Pour plus d’informations sur la terminologie et le concept de la planification Workfront, voir [Présentation de la planification Adobe Workfront](/help/quicksilver/planning/general/planning-overview.md).

## Questions à poser avant de configurer Workfront Planning

Après vous être familiarisé avec la terminologie et l’architecture de Workfront Planning, vous pouvez commencer à configurer votre nouvel environnement.

Voici quelques questions que vous pouvez vous poser lorsque vous configurez la planification :

* **Voulez-vous utiliser des espaces de travail pour des groupes organisationnels plus importants ? Ou devrais-je encourager les gens à en créer des personnels ?**

  Vous pourriez trouver qu&#39;il y a un bon usage pour les deux. Il est recommandé de ne pas avoir trop d’espaces de travail, car ils peuvent devenir difficiles à gérer et vos workflows peuvent être trop fragmentés.

  >[!TIP]
  >
  >    Vous pouvez avoir 1 000 espaces de travail dans une instance Workfront.

* **Quels types d’enregistrement personnalisés dois-je créer dans chaque espace de travail ?**

  Les types d’enregistrement sont semblables aux types d’objet Workfront. Pensez à vos workflows et décidez quels types d’enregistrement (objets de travail, objets de personnes, taxonomies, etc.) chaque workflow peut avoir besoin de.

  Pour plus d’informations, voir [Création de types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md)

* **Comment vais-je créer mes enregistrements ? Existe-t-il une liste ou une feuille de calcul externe qui contient déjà les enregistrements que je dois ajouter à la planification que je peux utiliser ? L&#39;ajout des enregistrements sera-t-il progressif en fonction des besoins ? Ou seront-ils importés à l’aide d’une intégration d’API Fusion ou personnalisée ?**

  Pour plus d’informations, voir :

   * [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md)
   * [Modules Adobe Workfront Planning](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **Quels champs dois-je créer pour mes enregistrements ?**

  Pour plus d’informations, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

* **Quels types d’objets Workfront ou AEM Assets ai-je besoin de me connecter aux types d’enregistrements Workfront Planning pour afficher les dépendances et créer un workflow transparent pour mon entreprise ?**

  Pour plus d’informations, consultez la section [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

* **Quels calendriers et vues marketing vais-je avoir besoin pour raconter l’histoire de mes campagnes ? Et à quelles parties prenantes puis-je mettre ces points de vue à disposition pour une collaboration harmonieuse ?**

  Pour plus d’informations, voir [Gérer des vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).


## Bonnes pratiques relatives à la planification Workfront

Cette section répertorie plusieurs tâches et recommandations relatives aux bonnes pratiques lors de la configuration de la planification Workfront.

Les instructions sont organisées en fonction de l’objet ou de la zone que vous configurez.

### Espaces de travail

#### À ne pas faire des espaces de travail

* Concevez les espaces de travail au niveau de l’organisation avec le plus faible volume

  Par exemple, essayez de créer une Workspace unique pour l’ensemble du marketing.

* Traitez vos espaces de travail régulièrement. Vous pouvez en modifier un existant plutôt que d’en créer un nouveau à partir de zéro.

* Créez un nouveau Workspace pour une équipe dont le mouvement opérationnel est complètement différent.

  Un espace de travail &quot;Développement de produit&quot; doit être distinct d’un espace de travail &quot;Marketing&quot;.

* Ne créez pas un espace de travail unique pour chaque petite chose. Considérez les espaces de travail davantage comme un système d’enregistrement qui peut bénéficier à l’ensemble de l’organisation et permettre à chacun de mapper des workflows et de collaborer plutôt qu’un espace privé pour effectuer le suivi des requêtes personnelles.

* Ne créez pas d’espaces de travail uniques pour chaque équipe ou processus au sein d’une organisation.

  L’organisation marketing doit s’efforcer de ne gérer qu’un seul espace de travail afin de maintenir la visibilité et de permettre aux données d’être cumulées au niveau de la planification globale.

  Évitez de créer des espaces de travail similaires ou en double pour les équipes qui suivent des processus similaires (par exemple, marketing EMEA ou marketing APAC), en particulier lorsque ces équipes peuvent travailler sur des déploiements de campagne stratégique commune.

#### Comment dois-je utiliser les sections de l’espace de travail ?

* Créez et étiquetez des sections pour aider vos utilisateurs à comprendre comment organiser votre cycle de vie opérationnel.

  Vous pouvez par exemple créer une section intitulée &quot;Enregistrements principaux&quot; dans laquelle placer vos campagnes, tactiques et éléments livrables.

* Regroupez les types d’enregistrement &quot;j’aime&quot;.

  Vous pouvez créer une section intitulée &quot;Géographies&quot; qui contient des types d’enregistrement tels que : Région, Pays et Ville.

#### Comment gérer les autorisations de l’espace de travail ?

* Limitez l’accès à &quot;Gérer&quot; à un groupe sélectionné de personnes de confiance, qui ne supprimeront pas accidentellement un type d’enregistrement ou ne créeront pas de types d’enregistrement et de champs inutiles.

  >[!TIP]
  >
  >Au cours de notre programme bêta, nous avons découvert que de nombreux clients avaient l’impression d’accorder l’accès &quot;Gérer&quot; aux administrateurs de groupe.

* Ajoutez la zone Planning au modèle de mise en page des utilisateurs disposant d&#39;une licence Standard.

* N’autorisez pas les utilisateurs disposant d’une licence Standard à créer des espaces de travail personnels. Cela leur donne un espace sûr pour apprendre l&#39;outil et s&#39;y mettre à l&#39;aise. Cela n’encombrera pas l’expérience des autres et peut améliorer la productivité personnelle de l’utilisateur.

  >[!TIP]
  >
  >    Conseillez-leur de ne pas partager leurs espaces de travail personnels en tant que bonne pratique.


### Types d’enregistrements.

#### Champ à sélection unique ou multiple et type d’enregistrement lié

* Créez un nouveau type d’enregistrement si l’objet est utilisé dans plusieurs autres types d’enregistrement.

  Par exemple, une campagne peut avoir une connexion à plusieurs audiences Target et une tactique peut avoir une connexion à une seule audience Target.

* Créez un nouveau type d’enregistrement si l’objet doit stocker des valeurs de métadonnées supplémentaires qui pourraient s’avérer utiles dans les recherches.

  Par exemple, un type d’enregistrement Canal tel que &quot;Email&quot; peut stocker une liste de éléments livrables pris en charge, soit comme métadonnées natives, soit comme connexion à un type d’enregistrement autonome &quot;éléments livrables&quot;.

* N’ajoutez pas de nouveau type d’enregistrement si les données que vous stockez doivent uniquement être incluses dans un type d’enregistrement unique. Utilisez plutôt un champ de sélection.

  Par exemple, un type d’enregistrement Campaign peut comporter un champ à sélection unique nommé Taille de campagne, qui n’est pertinent que lorsqu’il est directement associé à une campagne spécifique.

#### Comment dois-je étiqueter mes types d’enregistrements ?

Créez et étiquetez des types d’enregistrement qui représentent un seul concept ou nom, comme &quot;Campagnes&quot;.

:no_entry_sign: Ne créez pas de type d’enregistrement mieux représenté sous la forme d’une couche d’affichage ; par exemple, &quot;Calendrier&quot; est un mauvais choix pour un type d’enregistrement, car il ne s’agit pas du type d’enregistrement proprement dit, mais d’une vue d’enregistrements.

### Combien de couches de hiérarchie dois-je créer ?

Vues

..

Workflow

..

### Gestion des champs

Champ Principal

Utilisez des valeurs de champ principal uniques pour faciliter la recherche et le &quot;choix&quot; de ces enregistrements lors de connexions.

Lors d’une connexion, les utilisateurs effectuent une recherche selon les valeurs du champ Principal et, s’ils ne sont pas uniques, les utilisateurs ne sauront pas lequel choisir.

Évitez d’utiliser des valeurs non uniques comme champ principal, car cela peut créer de la confusion pour les utilisateurs qui doivent effectuer des recherches sur le champ principal lors de l’utilisation du menu de sélecteur de connexions.



De Chris O&#39;Neal :

Un autre domaine à ne pas négliger est celui des cas d’utilisation qui sont (ou ne sont pas) les meilleures utilisations de la planification. Par exemple, la discussion sur la gestion des ressources que nous avons eue aujourd&#39;hui.



Alina&#39;s note :

Exemple d&#39;article &quot;Bonnes pratiques&quot; de ExL : https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

Informations complémentaires de Field Readiness de Lauren S : https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346