---
title: Bonnes pratiques de planification d’Adobe Workfront
description: En tant que personne responsable des opérations marketing, vous pouvez utiliser Adobe Workfront Planning pour organiser le travail de toutes vos équipes au cours du cycle de vie marketing. Voici quelques bonnes pratiques que nous vous recommandons lorsque vous commencez à planifier Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ae10d35c61bf40c9e6f0422bd670b9733ad62aae
workflow-type: tm+mt
source-wordcount: '3225'
ht-degree: 2%

---


<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Bonnes pratiques relatives à la planification Adobe Workfront

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

En tant que personne responsable des opérations marketing, vous pouvez utiliser Adobe Workfront Planning pour organiser le travail de toutes vos équipes au cours du cycle de vie marketing.

Cet article présente les questions fréquentes et les bonnes pratiques que nous vous recommandons lorsque vous commencez à planifier Workfront.

## Bonnes pratiques de configuration

### Espaces de travail

Les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail. Un espace de travail est un ensemble de types d’enregistrement utilisés par une équipe et représente le cycle de vie du travail de l’équipe.

Vous trouverez ci-dessous quelques questions fréquentes sur la configuration de la planification Workfront.

#### Comment dois-je commencer ?

* ✅ Lorsque vous vous connectez à Planification pour la première fois, suivez notre processus d’intégration in-app qui communique clairement la valeur de Planning et vous guide sur la manière de naviguer et d’utiliser efficacement le produit. Cela vous permet de comprendre ses capacités et de commencer facilement votre travail.
* ✅ Commencez par explorer nos modèles d’espace de travail prédéfinis pour obtenir des idées de cas d’utilisation similaires existants. Vous pouvez utiliser les types d’enregistrements et les champs prédéfinis qui se trouvent dans un modèle, ou bien ajouter les vôtres.
* ✅ Identifiez les principaux cas d’utilisation que vous souhaitez résoudre avec la planification Workfront. Par exemple, la plupart des organisations veulent améliorer la visibilité des activités stratégiques, ce qui peut inclure la création d’un meilleur &quot;calendrier de campagne&quot;. Pour ce cas pratique, vous devez commencer par répondre à quelques questions :

   * Qui le demande ?
   * Comment appellent-ils les choses qu&#39;ils veulent mettre dans le calendrier ?
Campagnes ? Tactiques ? Des initiatives ? Activités ? Événements ?
   * Quels types de questions veulent-ils répondre avec ce calendrier ?
   * Y a-t-il des campagnes qui se chevauchent pour la même audience ?
   * Quel est notre budget pour cette campagne, cette tactique, cette activité ou cet événement ?

  Les réponses à ces questions dicteraient ce que vous devez intégrer à la planification Workfront.

  En outre, considérez qu’il peut y avoir d’autres planificateurs qui ne sont actuellement pas des utilisateurs de Workfront. Ces planificateurs peuvent utiliser des feuilles de calcul Excel, des documents Word, PowerPoint, etc. Tenez compte de la manière dont ils peuvent accéder à vos informations dans la planification Workfront.

* ✅ Pour tirer pleinement parti de la planification Workfront, envisagez de remplacer l’utilisation de Portfolios et de programmes dans le processus Workfront par une autre structure de niveau supérieur dans la planification Workfront.

  Aujourd’hui, les clients Workfront représentent leur travail stratégique au travers de portefeuilles et de programmes, parfois sous la forme de projets de différents types. Avec l’introduction de la planification, tous ces travaux stratégiques doivent être gérés par le biais de types d’enregistrements personnalisés dans la planification Workfront, tandis que Workfront sera centré sur la phase d’exécution des travaux représentée sous la forme de projets et de tâches.


#### Quand dois-je créer un nouvel espace de travail plutôt que d’en modifier un existant ?

* ✅ Conception pour le plus petit volume d’espaces de travail au niveau de l’organisation. Vous pouvez créer des espaces de travail pour des entités d’organisation opérationnelle spécifiques, en fonction de la manière dont chaque unité fonctionne.

  Disposer des informations dans un seul Workspace, afin de garantir que les relations entre toutes les données peuvent être facilement gérées.

  Par exemple, essayez de créer un espace de travail unique pour l’ensemble du marketing.

  Il est possible de créer un nouvel espace de travail pour une équipe dont la structure opérationnelle est complètement différente :

  Par exemple, un espace de travail **Développement de produit** doit être distinct d’un espace de travail **Marketing**.

* ⛔ Ne créez pas d’espaces de travail uniques pour chaque équipe ou processus au sein d’une organisation.

  L’organisation marketing doit s’efforcer de ne conserver qu’un seul espace de travail pour maintenir la visibilité et permettre aux données de se cumuler au niveau de la planification globale.

  Évitez de créer des espaces de travail similaires ou en double pour les équipes qui suivent des processus similaires (par exemple, Marketing EMEA par rapport à Marketing APAC), en particulier lorsque ces équipes peuvent travailler en fonction de campagnes stratégiques courantes.

#### Comment utiliser les sections Workspace ?

* ✅ Créez et étiquetez des sections pour aider vos utilisateurs à comprendre comment organiser votre cycle de vie opérationnel.

  Par exemple, vous pouvez créer une section intitulée **Enregistrements principaux** où placer vos campagnes, tactiles et éléments livrables dans votre espace de travail.
* ✅ Regroupez les types d’enregistrement &quot;j’aime&quot;.

  Par exemple, vous pouvez créer une section appelée **Geographies** qui contient des types d’enregistrement tels que : Région, Pays et Ville.

### Types d’enregistrements.

Les types d’enregistrement sont les blocs de création d’un Workspace de planification Workfront. Vous pouvez définir comment les types d’enregistrement sont interconnectés.


#### Comment définir les types d’enregistrement dans mon espace de travail ?

* ✅ Prenez le temps d’identifier les informations dont vous avez besoin pour effectuer le suivi (les types d’enregistrement dont j’ai besoin) et la manière dont ces informations doivent être connectées. Contactez les parties prenantes qui utiliseront l’espace de travail pour prendre en compte tous leurs besoins. Vous pouvez également créer des sections personnalisées avec différents types d’enregistrement afin de présenter les informations de manière très conviviale.


* ⛔ Ne dupliquez pas les types d’enregistrement pour une autre période (par exemple, ne créez pas de types d’enregistrement distincts pour **Campagnes 2024** et **Campagnes 2025**).

  La création de différents types d’enregistrement interrompt le flux de données lorsque vous souhaitez comparer des données sur plusieurs années. Les vues actuelles sont par type d’enregistrement. Dès la fin de l’année, l’affichage de ce type d’enregistrement n’affichera plus les éléments futurs. La bonne pratique consiste à disposer d’un type d’enregistrement pour le type de travail et à segmenter les données à l’aide de filtres ou à les archiver, si nécessaire.

#### Quand dois-je utiliser un champ à sélection simple ou multiple plutôt qu’un type d’enregistrement lié ?

* ✅ Ajoutez un nouveau type d’enregistrement si l’objet est utilisé en rapport avec plusieurs autres types d’enregistrement.

  Par exemple, une campagne peut avoir une connexion à plusieurs audiences Target et une tactique peut avoir une connexion à une seule audience Target. Par conséquent, Campaign, Tactique et Audience doivent être des types d’enregistrement plutôt que des champs à sélection multiple.

* ✅ Ajoutez un nouveau type d’enregistrement si l’objet doit stocker des valeurs de métadonnées supplémentaires qui pourraient s’avérer utiles dans les recherches.

  Par exemple, un type d’enregistrement de canal tel que **Email** peut stocker une liste de livrables pris en charge, soit comme métadonnées natives, soit comme connexion à un type d’enregistrement **Deliverables** autonome.
* ⛔ N’ajoutez pas de nouveau type d’enregistrement si les données que vous stockez ne sont pertinentes que pour un seul type d’enregistrement.

  Par exemple, un type d’enregistrement **Campaign** peut comporter un champ à sélection unique appelé **Taille de campagne** qui n’est pertinent que lorsqu’il est directement associé à une campagne spécifique.

#### Comment dois-je étiqueter mes types d’enregistrements ?

* ✅ Créez et étiquetez des types d’enregistrement qui représentent un seul concept ou nom, comme **Campagnes**.
* ⛔ Ne créez pas un type d’enregistrement mieux représenté sous la forme d’une vue.

  Par exemple, **Calendar** est un mauvais choix pour un type d’enregistrement, car il ne s’agit pas du type d’enregistrement lui-même, mais d’une vue d’enregistrements.

### Gestion de terrain

Les champs sont des attributs des types d’enregistrement et s’affichent sous forme de colonnes dans la vue de tableau. Vous pouvez créer des champs personnalisés pour les types d’enregistrement, puis associer les champs aux enregistrements de la planification Workfront afin d’améliorer les informations d’enregistrement.


#### Quel champ est recommandé de définir comme champ Principal ?


* ✅ Utilisez des valeurs de champ principal uniques pour faciliter la recherche et le &quot;choix&quot; de ces enregistrements lors de connexions. 

  Lors d’une connexion, les utilisateurs effectuent une recherche selon les valeurs du champ Principal et, s’ils ne sont pas uniques, les utilisateurs ne sauront pas lequel choisir. 
* ⛔ Évitez d’utiliser des valeurs non uniques comme champ principal, car cela peut créer une confusion pour les utilisateurs qui doivent effectuer des recherches sur le champ principal lors de l’utilisation du menu de sélecteur de connexions. 

#### Comment dois-je utiliser des formules ?

* ✅ Utilisez les types de champs Formule pour réduire les entrées manuelles. Lorsque vous saisissez des informations basées sur des données qui se trouvent déjà dans la vue de tableau, vous pouvez économiser de l’effort en calculant ces informations automatiquement à l’aide de formules.

#### Comment dois-je commencer à connecter les données dans mon espace de travail ?

* ✅ La création de connexions est l’une des fonctionnalités les plus puissantes de la planification Workfront. Vous pouvez connecter des types d’enregistrement les uns aux autres ou des types d’enregistrement avec des types d’objets provenant d’autres applications telles qu’Adobe Workfront (connexion à des projets, des Portfolios, des programmes, des entreprises et des groupes) et avec Adobe Experience Manager Assets (connexion à des ressources et des dossiers).

  La connexion des types d’objet et d’enregistrement vous donne une vue d’ensemble complète de la manière dont tout le contenu de votre entreprise est connecté.

  Par exemple, vous disposez d’un type d’enregistrement **Campaign** et d’un type d’enregistrement **Tactics**, et vous pouvez créer une connexion entre ces deux types d’enregistrement pour voir quels **Tactics** sont associés à une **Campaign** spécifique.

  Après avoir défini la connexion, toutes les personnes de l’espace de travail peuvent commencer à ajouter des valeurs pour **Campagnes** en double-cliquant dans le champ de connexion où une liste de toutes les **Tactiques** disponibles s’affiche. Vous pouvez ainsi trouver rapidement les tactiques à associer à vos campagnes.

#### Comment dois-je utiliser les champs de recherche ?

* ✅ Après avoir établi la connexion entre les enregistrements ou les types d’objets, vous pouvez connecter des enregistrements individuels les uns aux autres et afficher les champs de l’enregistrement ou des types d’objets liés sur un enregistrement Workfront Planning. Vous réduirez le nombre d’emplacements où vous devez mettre à jour la même information et vous assurez qu’ils correspondent parfaitement.

  Par exemple, une fois que vous disposez d’une connexion entre un type d’enregistrement **Campaign** et un type d’enregistrement **Tactics**, vous verrez les informations de champ principal, mais lorsque vous ajoutez des champs de recherche, vous pourrez apporter des informations supplémentaires à partir de ce type d’enregistrement, comme la **date de lancement** pour cette **Tactic**. Les données de ces champs de recherche sont automatiquement renseignées après l’ajout des enregistrements.

#### Quel type de champ est recommandé pour les URL ? 

* ✅ Utilisez un champ de texte Une seule ligne pour ajouter des données d’URL à un enregistrement.

### Vues

#### Comment puis-je choisir ce qui doit être un type d’affichage ou d’enregistrement ?

* ✅Pour les éléments qui représentent un seul concept ou un nom (comme **Campagnes**), créez un type d’enregistrement. 

* ⛔ Ne créez pas un type d’enregistrement mieux représenté sous la forme d’une vue.

  Par exemple, **Calendar** est un mauvais choix pour un type d’enregistrement, car il ne s’agit pas du type d’enregistrement lui-même, mais d’une vue d’enregistrements. 

#### Dois-je masquer ou supprimer les champs qui ne me concernent pas ?

* ✅ Masquez la colonne au lieu de la supprimer lorsque ces informations peuvent être pertinentes pour une autre personne utilisant le même type d&#39;enregistrement. Si vous supprimez le champ dans une vue de table spécifique, ce champ sera également supprimé dans le reste des vues de cet enregistrement, ainsi que partout où ce type d&#39;enregistrement est lié.

#### Comment utiliser les filtres et les regroupements dans les vues de tableau et de chronologie ?

* ✅ Utilisez des vues avec des filtres et des regroupements pour afficher un instantané de ce que vous devez voir. Vous pouvez filtrer et regrouper les données afin de disposer d’un moyen plus convivial de comprendre ce qui est prévu. Vous pouvez regrouper les enregistrements par champs de métadonnées.

  Par exemple, vous pouvez avoir une vue chronologique de votre type d’enregistrement **Campaign** que vous pouvez regrouper par **audiences cibles** et filtrer par **Date** pour n’afficher que l’année en cours.

#### Pourquoi tous les enregistrements ne s’affichent-ils pas dans la vue de la chronologie ?

* ✅ N&#39;oubliez pas de définir 2 champs de date pour vos enregistrements. Vous ne pouvez créer une vue de chronologie que si au moins deux champs de date sont associés à un type d’enregistrement. Certains enregistrements peuvent ne pas s’afficher dans la vue chronologique lorsque les dates de début ou de fin, ou les deux, n’ont aucune valeur et lorsque la date de début est postérieure à la date de fin.

#### Comment utiliser les paramètres de la vue de la chronologie

* ✅ Définissez les paramètres de votre vue de chronologie, comme le **style de barre** et la **couleur** pour obtenir une vue plus enrichissante visuellement. Vous pouvez personnaliser le **style de barre** en définissant si vous souhaitez afficher une miniature avec une image significative et ajouter d’autres champs à afficher sur la barre (par exemple, **Propriétaire** ou **Statut**).

  Par défaut, seul le champ principal s’affiche. Vous pouvez également définir la couleur de votre barre par valeurs de champ (par exemple, vous pouvez personnaliser les couleurs de vos barres en les faisant correspondre au champ Statut ) ou par le regroupement que vous avez appliqué. Par défaut, la couleur correspond à la couleur du type d’enregistrement.

  Seules les couleurs de type enregistrement ou les champs avec des options associées aux couleurs peuvent affecter les couleurs des barres d’enregistrement de la chronologie.

### Autorisations et partage

Utilisez la fonction de partage pour accorder aux employés les autorisations appropriées d’affichage et d’espace de travail.

#### Comment gérer les autorisations des espaces de travail ?

* ✅ Lorsque vous créez un **espace de travail**, il n&#39;est disponible que pour vous. Les autres utilisateurs, à l’exception des administrateurs système, ne pourront pas le trouver. Une fois l’espace de travail défini et que vous êtes prêt à amener votre équipe à démarrer la collaboration, vous devez le partager avec eux et définir leur niveau d’autorisation.

  Vous pouvez choisir parmi les niveaux d’autorisation suivants :

   * **Gérer** : les utilisateurs peuvent modifier, supprimer et partager l’espace de travail.
   * **Contribute** : les utilisateurs peuvent créer, modifier et supprimer des enregistrements.
   * **View** : les utilisateurs peuvent afficher des enregistrements.

* ✅ Bien que de nombreux clients aient l’impression d’accorder des autorisations **Gérer** aux espaces de travail à la plupart des personnes, limitez les autorisations **Gérer** à un groupe sélectionné de personnes de confiance qui ne supprimeront pas accidentellement un type d’enregistrement ou ne créeront pas de champs et de types d’enregistrement inutiles. Ils peuvent modifier, partager et même supprimer l’espace de travail. Ce niveau d’autorisation leur accorde un accès administratif complet à Workspace.

  Une licence d’utilisateur standard est requise pour qu’une personne dispose des autorisations de gestion pour un espace de travail.

* ✅ Donnez aux utilisateurs des autorisations **Contribute** si vous souhaitez qu’ils puissent simplement créer, modifier et supprimer des enregistrements, mais que vous ne souhaitez pas qu’ils modifient la structure et le schéma de l’espace de travail. Avec les autorisations **Contribute**, ils ne peuvent pas créer de types d’enregistrement ni modifier les champs sur les types d’enregistrement existants.

  Une licence d’utilisateur standard est requise pour qu’une personne dispose des autorisations **Contribute** sur un espace de travail.

* ✅ Donnez aux utilisateurs des autorisations **Afficher** si vous souhaitez qu’ils visualisent uniquement des enregistrements.

  >[!NOTE]
  >
  >Actuellement, nous n’avons pas d’autorisations spécifiques pour les types d’enregistrements ou les enregistrements. Cela signifie que tous les enregistrements de n’importe quel type d’enregistrement sont visibles si vous accordez à une personne l’accès **Affichage** à l’espace de travail.

#### Comment dois-je gérer les autorisations d’affichage ?

* ✅ Limitez les autorisations **Gérer** aux personnes que vous souhaitez pouvoir modifier, supprimer et partager la vue. Cela signifie qu&#39;ils peuvent modifier les filtres, les champs de groupement ou une partie de la configuration de la vue. Ces modifications affectent la configuration principale de la vue pour toutes les autres personnes qui utilisent également la vue.

  Une licence d’utilisateur standard est requise pour qu’une personne dispose des autorisations de gestion d’une vue.

* ✅ Donnez aux utilisateurs l’accès **Affichage** pour qu’ils puissent appliquer la vue. Ils pourront modifier certains des filtres ou regroupements et trier, mais ces modifications ne seront que temporaires ; les modifications ne seront pas enregistrées pour tous les autres utilisateurs accédant à la vue. Ces modifications n’auront aucune incidence sur la configuration principale de la vue pour toutes les autres personnes qui utilisent également la vue.  Leurs modifications ne sont visibles que par l’utilisateur qui applique les paramètres modifiés. Après avoir actualisé l’écran, les modifications sont réinitialisées à la valeur par défaut.

* ✅ Donnez à **tous les utilisateurs de l’espace de travail les autorisations nécessaires pour afficher** lorsque vous souhaitez que tous ceux qui peuvent afficher l’espace de travail voient les enregistrements et leurs champs dans cette vue spécifique. Ainsi, vous n’avez pas besoin d’ajouter manuellement personne à la zone d’autorisation de partage pour la vue.

  >[!NOTE]
  >
  >Si une vue n’a pas été partagée et que vous partagez un lien avec elle avec d’autres personnes, les enregistrements pourront être affichés dans la **vue de table par défaut**. S’ils disposent d’une licence Workfront standard, ils peuvent créer leur propre vue.


#### En quoi **Partage Workspace** diffère-t-il du **partage de vues** ?

* **Partage Workspace** définit l’accès des personnes à l’espace de travail, à ses types d’enregistrements, à ses enregistrements et à leurs champs.

* **Affichage du partage** définit si l’utilisateur peut voir la vue que vous avez créée et s’il peut modifier le filtre, les champs de regroupement ou toute autre configuration de la vue. La visibilité des enregistrements affichés dans la vue est contrôlée par le partage Workspace et non par le partage des vues.

#### En quoi les types de licence Workfront affectent-ils les autorisations de Workfront Planning ?

* Pour le **partage Workspace** : les utilisateurs de licences Light et Contribute ne peuvent accéder qu&#39;à l&#39;accès Affichage à un espace de travail. Pour accorder à un utilisateur Contribute ou Gérer l’autorisation d’accès à un espace de travail, il doit disposer d’une licence Standard.

* **Partage des vues** : les utilisateurs de licences standard disposant des autorisations de gestion d’un espace de travail pourront créer une vue. Les utilisateurs de licences Light et Contribute ne peuvent utiliser que les vues que les utilisateurs Standard ont créées et partagées avec eux. Dans le cas contraire, si rien n’a été partagé, les utilisateurs pourront voir la **vue de table par défaut**.


#### Que dois-je faire lorsqu’un propriétaire Workspace change ?

* Workfront définit le créateur de l’espace de travail en tant que propriétaire, mais au niveau des fonctionnalités, le propriétaire dispose des mêmes autorisations que tout utilisateur disposant des autorisations Gérer .
* Si le propriétaire est désactivé, les autres membres peuvent continuer leur travail dans l’espace de travail sans interruption.
* Les administrateurs système ont accès à n’importe quel espace de travail. Par conséquent, si le propriétaire était la seule personne disposant des autorisations Manage, les administrateurs peuvent ajouter une autre personne et lui accorder des autorisations Manage pour gérer l’espace de travail.

### Envoi de requêtes dans la planification Workfront

Vous pouvez créer un formulaire de demande pour chaque type d’enregistrement lorsque vous souhaitez que les utilisateurs ajoutent des enregistrements en dehors d’une page de type d’enregistrement. L’envoi du formulaire ajoute un nouvel enregistrement au type d’enregistrement.

#### Quand dois-je commencer à créer un formulaire de demande pour un type d’enregistrement ?

* ✅ Assurez-vous que la structure de type enregistrement est configurée en ajoutant les champs nécessaires au tableau. Ces champs décrivent vos enregistrements et seront accessibles dans le créateur de formulaires.

  Idéalement, créez le formulaire de demande ou de prise de vue une fois votre structure de type d’enregistrement finalisée afin d’éviter l’absence de champs clés.

#### Qui peut créer des formulaires de demande ?

* ✅ Tout utilisateur disposant de l’accès Gérer à l’espace de travail peut créer ou modifier un formulaire de demande. Assurez-vous que les autorisations de l’utilisateur sont correctement attribuées pour autoriser cette fonctionnalité.

#### Comment créer ou modifier un formulaire de demande pour un type d’enregistrement ?

* ✅ Tout utilisateur disposant de l’accès Gérer à l’espace de travail peut suivre les étapes décrites dans l’article [Créer et gérer un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


#### Qui pourra envoyer de nouveaux enregistrements à l’aide du formulaire de demande ?

* ✅ Les autorisations d’envoi dépendent des paramètres que vous configurez pour chaque formulaire.

  Dans le créateur de formulaires, une fois le formulaire publié, vous pouvez gérer les autorisations de contrôle de l’expéditeur des requêtes.

  Vous pouvez choisir parmi les trois options de partage suivantes :

   * **Toute personne disposant d’un accès en vue ou supérieur à l’espace de travail :** Permet à tous les utilisateurs disposant d’un accès en vue ou supérieur à l’espace de travail d’envoyer une requête qui crée un enregistrement.
   * **Toute personne disposant d’un accès à l’espace de travail ou d’un accès supérieur à** : limite les envois aux utilisateurs disposant d’autorisations Contribute ou d’autorisations supérieures à l’espace de travail.
   * **Toute personne disposant du lien :** Permet à toute personne disposant du lien de formulaire d’envoyer une requête.
   * **Date d’expiration :** veillez à définir une date d’expiration pour le lien public afin d’améliorer la sécurité.

### Bonnes pratiques pour la gestion des formulaires de demande

Voici quelques recommandations pour gérer les formulaires de demande :

* Planifiez : définissez clairement les informations nécessaires ou requises des demandeurs avant de créer le formulaire afin d’éviter les révisions excessives ultérieurement.
* Utiliser des libellés clairs : assurez-vous que les libellés et descriptions de champ sont clairs et compréhensibles pour tous les utilisateurs.
* Tester les formulaires : avant de déployer de nouveaux formulaires auprès d’un public plus large, testez-les à l’aide de l’option de prévisualisation de formulaire et de lien de formulaire afin de vous assurer que tous les champs et la logique fonctionnent comme prévu.
* Conserver les formulaires à jour : consultez régulièrement les formulaires et mettez-les à jour pour correspondre à toute modification de la structure de type d’enregistrement ou aux processus opérationnels.

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

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->