---
title: Recommandations d’Adobe Workfront Planning pour la mise en œuvre
description: En tant que personne responsable des opérations marketing, vous pouvez utiliser Adobe Workfront Planning pour organiser le travail de toutes vos équipes au cours du cycle de vie marketing. Voici quelques bonnes pratiques que nous vous recommandons de suivre lors de la prise en main de Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '3362'
ht-degree: 2%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Recommandations d’Adobe Workfront Planning pour la mise en œuvre

<!-- this used to be called Adobe WFP best practices, but the best practice piece was replaced by this folder of articles: [Adobe Workfront Planning best practices: article index](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md) -->

{{planning-important-intro}}

En tant que personne responsable des opérations marketing, vous pouvez utiliser Adobe Workfront Planning pour organiser le travail de toutes vos équipes au cours du cycle de vie marketing.

Cet article présente quelques questions fréquentes et bonnes pratiques que nous vous recommandons de suivre lorsque vous commencez à utiliser Workfront Planning.

Pour plus d’informations, nous vous recommandons également de consulter les articles de la section [Bonnes pratiques relatives à Adobe Workfront Planning : index des articles](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md).


## Bonnes pratiques de configuration

### Espaces de travail

Les espaces de travail sont des emplacements centralisés pour que les équipes puissent planifier le travail. Un espace de travail est un ensemble de types d’enregistrements utilisés par une équipe et représente le cycle de vie de travail de l’équipe.

Vous trouverez ci-dessous quelques questions fréquentes sur la configuration de Workfront Planning.

#### Comment dois-je commencer ?

* ✅ Lorsque vous vous connectez pour la première fois à Planning, suivez notre processus d’intégration in-app qui communique clairement la valeur de Planning et vous guide sur la navigation et l’utilisation efficace du produit. Cela vous permet de comprendre ses fonctionnalités et de commencer votre travail en toute facilité.
* ✅ Commencez par explorer nos modèles d’espace de travail prédéfinis pour obtenir des idées de cas d’utilisation similaires existants. Vous pouvez utiliser les types d’enregistrements et les champs prédéfinis qui se trouvent dans un modèle, ou bien ajouter les vôtres.
* ✅ Identifiez les principaux cas d’utilisation que vous souhaitez résoudre avec Workfront Planning. Par exemple, la plupart des organisations souhaitent améliorer la visibilité des activités stratégiques, ce qui peut inclure la création d’un meilleur « calendrier de campagne ». Pour ce cas d’utilisation, vous souhaiterez donc commencer par répondre à quelques questions :

   * Qui le demande?
   * Comment appellent-ils les choses qu&#39;ils veulent mettre dans le calendrier ?
Campagnes ? Tactiques ? Initiatives ? Activités ? Événements ?
   * À quels types de questions veulent-ils répondre avec ce calendrier ?
   * Y a-t-il des campagnes qui se chevauchent pour la même audience ?
   * Quel est le budget de cette campagne, tactique, activité ou événement ?

  Les réponses à ces questions dictent ce que vous devez créer dans Workfront Planning.

  N’oubliez pas non plus que d’autres planificateurs ne sont pas des utilisateurs de Workfront pour le moment. Ces planificateurs peuvent utiliser des feuilles de calcul Excel, des documents Word, des présentations PowerPoint, etc. Réfléchissez à la manière dont ils peuvent accéder à vos informations dans Workfront Planning.

* ✅ Pour tirer pleinement parti de Workfront Planning, envisagez de remplacer l’utilisation des Portfolios et Programmes dans Workfront par une autre structure de niveau supérieur dans Workfront Planning.

  Aujourd’hui, les clients de Workfront représentent leur travail stratégique par le biais de portefeuilles et de programmes, dans certains cas sous la forme de projets de différents types. Avec l’introduction de Planning, tous ces travaux stratégiques doivent être gérés par le biais de types d’enregistrements personnalisés dans Workfront Planning, tandis que Workfront sera centré sur la phase d’exécution des travaux, représentée sous la forme de projets et de tâches.

#### Quand dois-je créer un nouvel espace de travail ou en modifier un existant ?

* ✅ Concevez pour le volume le plus faible d’espaces de travail au niveau de l’organisation. Vous pouvez créer des espaces de travail pour des unités d’organisation opérationnelle spécifiques, afin de correspondre à la manière unique dont chaque unité fonctionne.

  disposer des informations dans un seul Workspace, afin de garantir que les relations entre toutes les données peuvent être facilement gérées ;

  Par exemple, essayez de créer un espace de travail unique pour l’ensemble du marketing.

  Vous pouvez créer un nouvel espace de travail pour une équipe dont la structure opérationnelle est complètement différente :

  Par exemple, un espace de travail **Développement de produit** doit être distinct d’un espace de travail **Marketing**.

* ⛔ Ne créez pas d’espaces de travail uniques pour chaque équipe ou processus au sein d’une organisation.

  L’organisation marketing doit s’efforcer de ne conserver qu’un seul espace de travail pour maintenir la visibilité et permettre aux données de se cumuler au niveau de la planification globale.

  Évitez de créer des espaces de travail similaires ou en double pour les équipes qui suivent des processus similaires (par exemple, la comparaison de EMEA Marketing et APAC Marketing), en particulier lorsque ces équipes peuvent travailler sur des campagnes stratégiques courantes.

#### Comment utiliser les sections Workspace ?

* ✅ Créer et libeller des sections pour aider vos utilisateurs à comprendre comment vous organisez votre cycle de vie opérationnel.

  Par exemple, vous pouvez créer une section appelée **Enregistrements principaux** dans laquelle vous placez vos campagnes, tactiques et éléments livrables dans votre espace de travail.
* ✅ les types d’enregistrements « J’aime » du groupe ensemble.

  Par exemple, vous pouvez créer une section appelée **Zones géographiques** qui contient des types d’enregistrements tels que : Région, Pays et Ville.

### Types d’enregistrement

Les types d’enregistrements sont les blocs de construction d’un Workspace Workfront Planning. Vous pouvez définir la manière dont les types d’enregistrements sont interconnectés.

#### Comment dois-je définir les types d’enregistrements dans mon espace de travail ?

* ✅ Prenez le temps d’identifier les informations que vous devez suivre (quels types d’enregistrements sont nécessaires) et comment ces informations doivent être connectées. Discutez avec les parties prenantes qui utiliseront l’espace de travail pour prendre en compte tous leurs besoins. Vous pouvez également créer des sections personnalisées avec différents types d’enregistrements pour présenter les informations de manière très comestible.

* ⛔ Ne dupliquez pas les types d&#39;enregistrement pour une période différente (par exemple, ne créez pas de types d&#39;enregistrement distincts pour **Campagnes 2024** et **Campagnes 2025**).

  La création de différents types d’enregistrements interrompt le flux de données chaque fois que vous souhaitez comparer des données sur plusieurs années. Les vues aujourd&#39;hui sont par type d&#39;enregistrement, de sorte que dès la fin de l&#39;année, la vue de ce type d&#39;enregistrement n&#39;affichera plus les éléments futurs. La bonne pratique consiste à disposer d’un type d’enregistrement pour le type de travail et à segmenter les données à l’aide de filtres basés sur différents champs ou à les archiver, si nécessaire.

#### Quand dois-je utiliser un champ à sélection unique ou multiple par rapport à un type d’enregistrement lié ?

* ✅ Ajoutez un nouveau type d’enregistrement si l’objet sera utilisé conjointement avec plusieurs autres types d’enregistrement

  Par exemple, une campagne peut avoir une connexion à plusieurs audiences cibles et une tactique peut avoir une connexion à une seule audience cible. Par conséquent, Campaign, Tactique et Audience doivent être des types d’enregistrements plutôt que des champs à sélection multiple.

* ✅ Ajoutez un nouveau type d’enregistrement si l’objet doit stocker des valeurs de métadonnées supplémentaires qui peuvent s’avérer utiles dans les recherches

  Par exemple, un type d’enregistrement de canal tel que **E-mail** peut stocker une liste de livrables pris en charge, sous la forme de métadonnées natives ou d’une connexion à un type d’enregistrement autonome **Livrables**.
* ⛔ N’ajoutez pas de nouveau type d’enregistrement si les données que vous stockez ne sont pertinentes que pour un seul type d’enregistrement.

  Par exemple, un type d’enregistrement **Campagne** peut comporter un champ à sélection unique appelé **Taille de la campagne** qui n’est pertinent que lorsqu’il est directement associé à une campagne spécifique. Créez plutôt un champ pour capturer ces informations.

#### Comment dois-je libeller mes types d’enregistrements ?

* ✅ Créez et libellez des types d’enregistrements qui représentent un seul nom ou concept, comme **Campagnes**.
* ⛔ Ne créez pas de type d’enregistrement mieux représenté en tant que vue.

  Par exemple, **Calendrier** est un mauvais choix pour un type d’enregistrement, car il ne s’agit pas du type d’enregistrement lui-même, mais d’une vue d’enregistrements.

### Gestion de champ

Les champs sont des attributs de types d’enregistrement et sont affichés sous forme de colonnes dans la vue Tableau. Vous pouvez créer des champs personnalisés pour les types d’enregistrements, puis associer les champs aux enregistrements Workfront Planning afin d’améliorer les informations d’enregistrement.

#### Quel champ est recommandé de définir comme champ de Principal ?

* ✅ Utilisez des valeurs de champ principal uniques pour faciliter la recherche et le « choix » de ces enregistrements lors de l’établissement de connexions. 

  Lors de l’établissement d’une connexion, les utilisateurs recherchent les valeurs dans le champ de Principal et, si elles ne sont pas uniques, ils ne sauront pas laquelle sélectionner. 
* ⛔ Évitez d’utiliser des valeurs non uniques comme champ principal, car cela peut prêter à confusion pour les utilisateurs qui doivent effectuer une recherche dans le champ principal lors de l’utilisation du menu du sélecteur de connexions. 

#### Comment utiliser les formules ?

* ✅ N’utilisez pas de types de champ de formule pour réduire la saisie manuelle. Lorsque vous saisissez des informations en fonction de données qui se trouvent déjà dans votre vue Tableau, vous pouvez économiser un certain effort en calculant automatiquement ces informations à l’aide de formules.

#### Comment dois-je commencer à connecter les données de mon espace de travail ?

* ✅ La création de connexions est l&#39;une des fonctionnalités les plus puissantes de Workfront Planning. Vous pouvez connecter des types d’enregistrements les uns aux autres ou des types d’enregistrements à des types d’objets provenant d’autres applications telles qu’Adobe Workfront (connexion à des projets, des portfolios, des programmes, des entreprises et des groupes), Adobe Experience Manager Assets (connexion à des ressources et des dossiers) et Adobe GenStudio for Performance Marketing.

  La connexion des types d’objet et d’enregistrement vous donne un aperçu complet de la manière dont tout est connecté dans votre entreprise.

  Par exemple, vous disposez d’un type d’enregistrement **Campaign** et d’un type d’enregistrement **Tactics** et vous pouvez créer une connexion entre ces deux types d’enregistrements pour voir quels **Tactics** sont associés à une **Campaign** spécifique.

  Après avoir défini la connexion, toutes les personnes de l’espace de travail peuvent commencer à ajouter des valeurs pour **Campagnes** en double-cliquant dans le champ de connexion où elles verront une liste de toutes les **Tactiques** disponibles. Vous pouvez ainsi identifier rapidement les tactiques à associer à vos campagnes.

#### Comment utiliser les champs de recherche ?

* ✅ Après avoir établi la connexion entre les enregistrements ou les types d&#39;objet, vous pouvez connecter des enregistrements individuels entre eux et afficher les champs de l&#39;enregistrement ou des types d&#39;objet liés sur un enregistrement Workfront Planning. Vous réduirez le nombre d’emplacements où vous devez mettre à jour la même information et vous vous assurerez qu’ils correspondent parfaitement.

  Par exemple, une fois que vous disposez d’une connexion entre un type d’enregistrement **Campaign** et un type d’enregistrement **Tactique**, les informations du champ principal s’affichent, mais lorsque vous ajoutez des champs de recherche, vous pouvez apporter des informations supplémentaires à partir de ce type d’enregistrement, comme la **Date de lancement** pour un **Tactique**. Les données de ces champs de recherche sont automatiquement renseignées une fois les enregistrements ajoutés.

#### Quel type de champ est recommandé pour les URL ? 

* ✅ Utilisez un champ de texte d’une seule ligne pour ajouter des données d’URL à un enregistrement.

### Vues

#### Comment choisir ce qui doit être une vue ou un type d’enregistrement ?

* ✅Pour les éléments qui représentent un seul concept ou substantif (comme **Campagnes**), créez un type d’enregistrement. 

* ⛔ Ne créez pas de type d’enregistrement mieux représenté en tant que vue.

  Par exemple, **Calendrier** est un mauvais choix pour un type d’enregistrement, car il ne s’agit pas du type d’enregistrement lui-même, mais d’une vue d’enregistrements. 

#### Dois-je masquer ou supprimer les champs qui ne sont pas pertinents pour moi ?

* ✅ Masquez la colonne au lieu de la supprimer lorsque ces informations peuvent être pertinentes pour une autre personne utilisant le même type d’enregistrement. Si vous supprimez le champ dans une vue de table spécifique, ce champ sera également supprimé dans le reste des vues de cet enregistrement, ainsi que partout où ce type d&#39;enregistrement est lié.

#### Comment utiliser les filtres et les regroupements dans les vues Tableau et Chronologie ?

* ✅ Utilisez des vues avec des filtres et des regroupements pour afficher un instantané de ce que vous souhaitez voir. Vous pouvez filtrer et regrouper les données afin de disposer d’un moyen plus convivial de comprendre ce qui est prévu. Vous pouvez regrouper les enregistrements par champs de métadonnées.

  Par exemple, vous pouvez avoir une vue chronologique pour votre type d’enregistrement **Campagne** que vous pouvez regrouper par **Audiences cibles** et filtrer par **Date** pour n’afficher que l’année en cours.

#### Pourquoi tous les enregistrements ne s’affichent-ils pas dans ma vue chronologique ?

* ✅ N’oubliez pas de définir 2 champs de date pour vos enregistrements. Vous ne pouvez créer une vue chronologique que lorsque vous disposez d’au moins deux champs de date associés à un type d’enregistrement. Certains enregistrements peuvent ne pas s&#39;afficher dans la vue chronologique lorsque les dates de début ou de fin ou les deux n&#39;ont aucune valeur ou lorsque la date de début est postérieure à la date de fin.

#### Comment dois-je utiliser les paramètres de la vue Chronologie ?

* ✅ Définissez les paramètres de votre vue chronologique, tels que le style **Barre** et la **Couleur** pour obtenir une vue plus enrichissante visuellement. Vous pouvez personnaliser le style **Barre** en définissant si vous souhaitez afficher une miniature avec une image significative et ajouter d’autres champs à afficher sur la barre (par exemple, **Propriétaire** ou **Statut**).

  Par défaut, seul le champ principal s’affiche. Vous pouvez également définir la couleur de votre barre en fonction des valeurs de champ (par exemple, vous pouvez personnaliser les couleurs de vos barres en les faisant correspondre au champ État ) ou du regroupement que vous avez appliqué. Par défaut, la couleur correspond à celle du type d’enregistrement.

  Seules les couleurs de type enregistrement ou les champs avec des options associées aux couleurs peuvent affecter les couleurs des barres d’enregistrement dans le montage.

### Autorisations et partage

Utilisez la fonction de partage pour accorder aux autres utilisateurs les autorisations appropriées pour les vues et les espaces de travail.

#### Comment dois-je gérer les autorisations relatives aux espaces de travail ?

* ✅ Lorsque vous créez un **espace de travail**, il n’est disponible que pour vous. Toute autre personne qui n’est pas un administrateur système ne pourra pas le trouver. Une fois l’espace de travail défini et que vous êtes prêt(e) à inviter votre équipe à démarrer la collaboration, vous devez le partager avec elle et définir son niveau d’autorisation.

  Vous pouvez choisir parmi les niveaux d’autorisation suivants :

   * **Gérer** : les personnes peuvent modifier, supprimer et partager l’espace de travail, les types d’enregistrements, ainsi que modifier, supprimer et créer des enregistrements.
   * **Contribuer** : les utilisateurs peuvent créer, modifier et supprimer des enregistrements.
   * **Afficher** : les utilisateurs peuvent afficher les enregistrements.

* ✅ Bien que de nombreux clients aient l’impression d’accorder des autorisations **Gérer** aux espaces de travail à la plupart des personnes, limitez les autorisations **Gérer** à un groupe restreint de personnes de confiance qui ne supprimeront pas accidentellement un type d’enregistrement ou ne créeront pas de types d’enregistrement et de champs inutiles. Ils peuvent modifier, partager et même supprimer l’espace de travail. Ce niveau d’autorisations leur accorde un accès administratif complet au Workspace.

  Une licence utilisateur standard est requise pour qu&#39;une personne dispose des autorisations de niveau Gérer sur un espace de travail.

* ✅ Autorisez les utilisateurs **Contribuer** à créer, modifier et supprimer des enregistrements uniquement si vous ne souhaitez pas qu&#39;ils modifient la structure de l&#39;espace de travail. Avec les autorisations **Contribute**, ils ne peuvent pas créer de types d’enregistrements ni modifier les champs sur les types d’enregistrements existants.

  Une licence utilisateur standard est requise pour qu&#39;une personne dispose des autorisations **Contribute** pour accéder à un espace de travail.

* ✅ Donnez aux utilisateurs des autorisations **Affichage** s’ils souhaitent uniquement afficher les enregistrements.

#### Comment dois-je gérer les autorisations pour les types d’enregistrements ?

* ✅ N’oubliez pas que les utilisateurs disposant d’autorisations de niveau Gérer sur les espaces de travail ne peuvent pas voir leurs autorisations réduites pour le type d’enregistrement . Ils hériteront également des autorisations de gestion pour le type d’enregistrement. Vous ne pouvez pas accorder à un utilisateur des autorisations de niveau Gérer sur l&#39;espace de travail, mais des autorisations de niveau Contribuer ou Afficher sur le type d&#39;enregistrement.
* ✅ Si vous souhaitez que les utilisateurs disposent d&#39;un niveau d&#39;autorisation inférieur (par exemple, Autorisations d&#39;affichage) pour le type d&#39;enregistrement par rapport à l&#39;espace de travail, nous vous recommandons de leur accorder des autorisations de type Contributeur pour l&#39;espace de travail. Vous pouvez ensuite leur donner des autorisations d’affichage sur le type d’enregistrement.
* La suppression d’un utilisateur des autorisations du type d’enregistrement lui donne toujours au moins les autorisations d’affichage de l’espace de travail.

#### Comment dois-je gérer les autorisations pour les vues ?

* ✅ Réservez les autorisations **Gérer** aux personnes que vous souhaitez pouvoir modifier, supprimer et partager la vue. Cela signifie qu’ils peuvent modifier les filtres, les champs de regroupement ou une configuration de la vue. Ces modifications auront un impact sur la configuration principale de la vue pour toutes les autres personnes qui utilisent également la vue.

  Une licence utilisateur standard est requise pour qu&#39;une personne dispose des autorisations de niveau Gérer pour une vue.

* ✅ Donnez aux utilisateurs les autorisations **Affichage** pour pouvoir appliquer l’affichage. Ils pourront modifier certains filtres ou regroupements et tris, mais ces modifications ne seront que temporaires ; les modifications ne sont pas enregistrées pour tous les autres utilisateurs accédant à la vue. Ces modifications n’affecteront pas la configuration principale de la vue pour toutes les autres personnes qui utilisent également la vue.  Leurs modifications ne sont visibles que par l’utilisateur ou l’utilisatrice qui applique les paramètres modifiés. Après actualisation de l’écran, les modifications sont réinitialisées à la valeur par défaut.

* ✅ Accorder des autorisations **Tout le monde peut afficher dans l’espace de travail** lorsque vous souhaitez que toute personne pouvant afficher l’espace de travail puisse afficher les enregistrements et leurs champs dans cette vue spécifique. Ainsi, vous n’avez pas besoin d’ajouter manuellement qui que ce soit à la zone d’autorisation de partage pour la vue.

  >[!NOTE]
  >
  >Si une vue n&#39;a pas été partagée et que vous partagez un lien vers cette vue avec d&#39;autres personnes, ces dernières pourront voir les enregistrements dans la **Vue Tableau par défaut**. S’ils disposent d’une licence Workfront standard, ils peuvent créer leur propre vue.

#### En quoi le partage de **Workspace** est-il différent du partage de **Afficher** ?

* Le partage de **Workspace** définit l&#39;accès des personnes à l&#39;espace de travail, ses types d&#39;enregistrements, enregistrements et leurs champs.

* **Partage d’affichage** définit si l’utilisateur peut voir l’affichage que vous avez créé et s’il peut modifier le filtre, les champs de regroupement ou une autre configuration de l’affichage. La visibilité des enregistrements affichés dans la Vue est contrôlée par le partage de Workspace, et non par le partage de la Vue.

#### Comment les types de licence Workfront affectent-ils les autorisations Workfront Planning ?

* Pour le partage de **Workspace** : les utilisateurs disposant d&#39;une licence Light et Contribute peuvent uniquement obtenir un accès en affichage à un espace de travail. Pour accorder à une personne l’autorisation Contribuer ou Gérer d’un espace de travail, elle doit disposer d’une licence Standard.

* **Partage de vues** : les utilisateurs sous licence standard disposant d’autorisations de niveau Gérer sur un espace de travail peuvent créer une vue. Les utilisateurs de licences Light et Contribute ne peuvent utiliser que les vues créées et partagées par les utilisateurs standard. Sinon, si rien n’a été partagé, les utilisateurs pourront voir la **Vue du tableau par défaut**.

#### Que dois-je faire lorsqu’un propriétaire Workspace change ?

* Workfront définit le créateur de l’espace de travail comme propriétaire, mais au niveau des fonctionnalités, le propriétaire dispose des mêmes autorisations que tout utilisateur disposant des autorisations de niveau Gérer.
* Si le propriétaire est désactivé, les autres membres peuvent continuer leur travail dans l’espace de travail sans aucune interruption.
* Les administrateurs système ont accès à n’importe quel espace de travail. Par conséquent, si le propriétaire était la seule personne disposant d’autorisations de niveau Gérer, les administrateurs peuvent ajouter une autre personne et lui accorder des autorisations de niveau Gérer pour gérer l’espace de travail.

### Envoi de requêtes dans Workfront Planning

Vous pouvez créer un formulaire de demande pour chaque type d’enregistrement lorsque vous souhaitez que les utilisateurs ajoutent des enregistrements en dehors de la page d’un type d’enregistrement. L’envoi du formulaire ajoute un nouvel enregistrement au type d’enregistrement.

#### Quand dois-je commencer à créer un formulaire de demande pour un type d’enregistrement ?

* ✅ Vous devez vous assurer que la structure du type d’enregistrement est configurée en premier lieu en ajoutant les champs nécessaires à la table. Ces champs décrivent vos enregistrements et peuvent être accessibles dans le créateur de formulaires.

  Idéalement, créez le formulaire de demande ou de réception une fois la structure de type d’enregistrement finalisée afin d’éviter de manquer des champs clés.

#### Qui peut créer des formulaires de demande ?

* ✅ Tout utilisateur disposant d’un accès de niveau Gérer à l’espace de travail peut créer ou modifier un formulaire de demande pour un type d’enregistrement. Assurez-vous que les autorisations de l’utilisateur sont correctement attribuées pour autoriser cette fonctionnalité.

#### Comment créer ou modifier un formulaire de demande pour un type d’enregistrement ?

* ✅ Tout utilisateur disposant d’un accès de niveau Gérer à l’espace de travail peut suivre les étapes décrites dans l’article [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


#### Qui pourra soumettre de nouveaux enregistrements à l&#39;aide du formulaire de demande ?

* ✅ autorisations d’envoi dépendent des paramètres que vous configurez pour chaque formulaire.

  Dans le créateur de formulaires, une fois le formulaire publié, vous pouvez gérer les autorisations pour contrôler qui peut envoyer des requêtes.

  Vous pouvez choisir parmi les options de partage suivantes :

   * Pour le partage interne avec des personnes dans Workfront :

      * **Toute personne disposant d’un accès en affichage ou d’un niveau supérieur à l’espace de travail :** autorise tous les utilisateurs disposant d’autorisations en affichage ou d’un niveau supérieur à l’espace de travail à soumettre une requête qui crée un enregistrement.
      * **Toute personne disposant d’un accès de niveau Contributeur ou supérieur à l’espace de travail** : limite les envois aux utilisateurs disposant d’autorisations de niveau Contributeur ou supérieur à l’espace de travail.
      * **Seules les personnes invitées peuvent y accéder** : ajoutez des personnes, des équipes, des rôles, des groupes ou des entreprises qui peuvent envoyer des demandes au formulaire.
   * Pour le partage externe avec des personnes qui ne disposent pas d’un compte Workfront :
      * **Création d’un lien public**, puis copie et partage avec tout le monde, même les personnes sans compte Workfront : permet à toute personne disposant du lien de formulaire de soumettre une demande.
      * **Date d’expiration du lien :** assurez-vous de définir une date d’expiration pour le lien public afin de renforcer la sécurité.

### Bonnes pratiques relatives à la gestion des formulaires de demande

Voici des recommandations pour la gestion des formulaires de demande :

* Planifier à l’avance : définissez clairement les informations nécessaires ou requises des demandeurs avant de créer le formulaire afin d’éviter des révisions excessives par la suite.
* Utiliser des libellés clairs : assurez-vous que les libellés et les descriptions des champs sont clairs et compréhensibles pour tous les utilisateurs et utilisatrices.
* Tester les formulaires : avant de déployer les nouveaux formulaires auprès d’une audience plus large, testez-les à l’aide du lien du formulaire et de l’option de prévisualisation de formulaire pour vous assurer que tous les champs et toute la logique fonctionnent comme prévu.
* Conserver les formulaires à jour : révisez régulièrement les formulaires et mettez-les à jour pour tenir compte des modifications apportées à la structure du type d’enregistrement ou aux processus opérationnels.

<!--do we need to add anything for the Configuration tab of a request form?? -->

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/fr/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/fr/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/fr/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->