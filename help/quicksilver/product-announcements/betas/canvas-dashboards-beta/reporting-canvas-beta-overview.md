---
content-type: reference
navigation-topic: betas
title: "Version bêta du canevas de rapports : aperçu"
description: Informations sur le programme bêta de l’outil de création de rapports à venir pour Adobe Workfront
author: Nolan
feature: Product Announcements
hidefromtoc: true
hide: true
exl-id: 5767ef7d-1bc3-40d8-abeb-02b15166a0a3
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 2%

---

# Version bêta du canevas de création de rapports : présentation

## Zone de travail de reporting

Le nouvel outil Canevas de création de rapports est actuellement en cours de développement, car il s’agit d’un outil totalement nouveau dans Workfront. Dans la conception du canevas de création de rapports, nous avons travaillé dur pour offrir une flexibilité maximale associée à une conception modulaire intuitive, afin que les utilisateurs comme vous puissent exploiter au mieux vos propres données dans la création et le partage de rapports. Grâce à un nouveau type de rapport unifié qui vous permet de faire glisser pratiquement tous les éléments sur un canevas illimité, la création d’un chef-d’oeuvre de données visuel sera plus facile que jamais.

Cet article contient des informations sur la version bêta privée actuelle, qui est limitée à des clients spécifiques. De nouvelles fonctionnalités du canevas de création de rapports sont désormais déployées via les tableaux de bord de la zone de travail. Voir **Plan de développement** ci-dessous pour plus d’informations.

### Plan de développement

Nous en sommes aux dernières étapes pour résoudre un problème de qualité des données que nous avons observé au début de la version bêta du canevas de création de rapports. Nous allons bientôt reprendre le travail pour fournir de nouvelles visualisations, développer la sélection des objets Workfront à rapporter et améliorer la création de rapports et les expériences de distribution, qui font toutes partie intégrante de la réalisation de nos objectifs pour le Canevas de création de rapports.

Ces nouvelles expériences seront diffusées progressivement, à compter de la version 23.2, via la nouvelle page Tableaux de bord du canevas désormais disponible dans votre environnement de prévisualisation. Les tableaux de bord de canevas vous permettent d’afficher les rapports existants avec les nouvelles fonctionnalités de création de rapports que nous sommes en train de créer. Ils serviront d’environnement principal pour le déploiement et le test de nouvelles fonctionnalités pour le canevas de rapports. Pour plus d’informations sur l’activation et l’utilisation des tableaux de bord de zone de travail, voir [Tableaux de bord de canevas - Aperçu](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Participer à la version bêta

>[!IMPORTANT]
>
>Les informations bêta ci-dessous sont destinées aux administrateurs qui ont déjà été inclus dans la version bêta du canevas de rapports, qui n’accepte plus les nouveaux participants. Si vous souhaitez tester les nouvelles fonctionnalités du Canevas de création de rapports telles qu’elles sont ajoutées, reportez-vous à la section **Plan de développement** ci-dessus pour plus d’informations sur l’activation des tableaux de bord de zone de travail.

### Disponibilité

La version bêta du canevas de création de rapports est disponible pour toutes les organisations qui se trouvent sur AWS, quelle que soit leur région.

### Rejoindre la version bêta

La version bêta du canevas de création de rapports est entièrement facultative, mais elle ne peut être activée que par un administrateur Workfront. Pour vous inscrire en tant qu’administrateur système :

1. Sélectionnez la variable **Reporting (version bêta)** dans le menu Principal de votre instance Workfront.
1. Cliquez sur **Accepter** pour accepter les conditions générales.
1. Permet d’ajouter les données de votre entreprise au canevas de création de rapports (cela peut prendre jusqu’à quelques heures).
1. Commencez à utiliser le canevas de création de rapports.

Une fois que les données de votre entreprise ont été ajoutées au canevas de création de rapports, d’autres administrateurs système peuvent choisir de les rejoindre individuellement de la même manière (sans attendre que les données soient à nouveau ajoutées).

Pour activer d’autres utilisateurs qui ne sont pas administrateurs Workfront :

1. Sélectionnez la variable **Reporting (version bêta)** dans le menu Principal de votre instance Workfront.
1. Cliquez sur **Autorisations du canevas de création de rapports**.
1. Recherchez et sélectionnez les utilisateurs spécifiques auxquels vous souhaitez participer.

   >[!IMPORTANT]
   >
   >Les utilisateurs auxquels vous accordez l’accès au Canevas de création de rapports auront accès à **all** données du système en lecture seule, quelles que soient leurs autorisations standard d’affichage de ces données.

1. Cliquer sur **Enregistrer**.
1. Ajoutez la variable **Reporting (version bêta)** dans le modèle de mise en page principal de chaque utilisateur sélectionné. Pour plus d’informations, voir [Personnalisation du menu principal à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Chaque utilisateur doit ensuite accéder individuellement à la fonction **Reporting (version bêta)** dans le menu principal et acceptez les conditions générales.

### Envoyer les commentaires

Pour envoyer des commentaires sur la version bêta :

1. Dans le canevas de création de rapports de Workfront, cliquez sur le bouton **Envoyer un commentaire** bouton .
1. Remplissez le formulaire, puis cliquez sur **Envoyer**.

## FAQ bêta

+++Puis-je migrer mes rapports hérités vers le canevas de rapports ?

En résumé, la migration des rapports hérités ne sera pas disponible pendant la version bêta. Cependant, il s’agit d’une fonctionnalité planifiée (avec quelques avertissements décrits ci-dessous) pour le lancement officiel.

Bien que l’obstacle à la création de nouveaux rapports ait été considérablement réduit avec le canevas de création de rapports, nous comprenons que la réintroduction de certains de vos rapports et tableaux de bord existants contribuera à accélérer le processus d’adoption. À ce titre, nous voulons fournir les outils et les ressources nécessaires pour vous assurer que vous pouvez importer tous les éléments hérités pertinents pour vous assurer que vous démarrez sur le bon pied dans le canevas de rapports. Cependant, comme le Canevas de création de rapports représente un changement radical dans le fonctionnement des rapports actuels, il serait impossible de migrer chaque rapport ou tableau de bord exactement comme aujourd’hui.

Notre stratégie actuelle de migration dans la version officielle est de vous permettre d’effectuer les opérations suivantes :

1. Identifier les rapports et les tableaux de bord pertinents

   1. Permet d’exporter un fichier CSV de tous les rapports et tableaux de bord du système, ainsi que toutes les informations de suivi pertinentes (nombre de vues, quand et par qui).
   1. Fournissez une exportation des rapports configurés avec les diffusions planifiées et les destinataires.

1. Sélectionnez les rapports et les tableaux de bord à migrer, puis cliquez sur **Migrer**

   Il s’agit d’une migration à sens unique. Une copie des rapports et des tableaux de bord sélectionnés est alors créée dans la zone de travail des rapports, en conservant le rapport ou le tableau de bord hérité dans l’outil de création de rapports actuel.

   Vous pouvez migrer le même rapport ou tableau de bord autant de fois que vous le souhaitez.

1. Dans la zone de travail des rapports, assurez-vous que tous les rapports et tableaux de bord que vous avez sélectionnés ont été migrés.
+++

+++Pourquoi ne puis-je pas voir tous les objets que je fais normalement ?

Afin de fournir la version bêta à nos clients le plus tôt possible, nous l’avons publiée avec uniquement un sous-ensemble des nombreux types d’objets disponibles dans Workfront aujourd’hui. Vous trouverez ci-dessous les types d’objets actuellement pris en charge dans la version bêta :

* Affectation
* Document
* Approbation du document
* Frais
* Heure
* Problème
* Note
* Portfolio
* Projet
* Programme
* Tâche
* Feuille de temps
* Élément de travail
+++

+++Si un problème se produit dans le Canevas de création de rapports au cours de la version bêta, les données de mon entreprise seront-elles affectées ?

Non. La version bêta utilise une copie des données de votre entreprise renseignée dans le canevas de création de rapports. Cela signifie que vous pouvez tester en toute sécurité pendant la version bêta sans risque d’affecter les données importantes, mais cela signifie également que la modification en ligne des données dans le Canevas de création de rapports sera indisponible jusqu’au lancement officiel.
+++

+++Puis-je me désinscrire de la version bêta une fois que j’ai rejoint ?

Un administrateur Workfront ne peut pas se désinscrire de la version bêta. Toutefois, les administrateurs non-système peuvent être supprimés en procédant comme suit :

1. Connectez-vous en tant qu’administrateur système.
1. Accédez au Canevas de création de rapports.
1. Cliquez sur Canevas de création de rapports **permissions**.
1. Supprimez les utilisateurs que vous souhaitez exclure de la version bêta de la liste qui ont été inscrits.
1. Cliquer sur **Enregistrer**.
+++
