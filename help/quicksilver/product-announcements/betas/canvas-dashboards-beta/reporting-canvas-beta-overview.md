---
content-type: reference
navigation-topic: betas
title: '« Version bêta de la zone de travail de reporting : vue d’ensemble »'
description: Informations sur le programme bêta de l’outil de zone de travail de reporting à venir pour Adobe Workfront
author: Nolan
feature: Product Announcements
hidefromtoc: true
hide: true
exl-id: 5767ef7d-1bc3-40d8-abeb-02b15166a0a3
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 100%

---

# Version bêta de la zone de travail de reporting : vue d’ensemble

## Zone de travail de reporting

Fonctionnalité de création de rapports complètement repensée dans Workfront, le nouvel outil de zone de travail de reporting est actuellement en cours de développement. Dans la conception de la zone de travail de reporting, nous avons travaillé dur pour offrir une flexibilité maximale associée à une conception modulaire intuitive, afin que les utilisateurs et utilisatrices comme vous puissent exploiter au mieux leurs propres données dans la création et le partage de rapports. Grâce à un nouveau type de rapport unifié qui vous permet de faire glisser pratiquement tous les éléments sur une zone de travail illimitée, la création d’un chef-d’oeuvre de données visuel sera plus facile que jamais.

Cet article contient des informations sur la version bêta privée actuelle, qui est limitée à des clientes et clients spécifiques. De nouvelles fonctionnalités de la zone de travail de reporting sont désormais déployées via les tableaux de bord Zone de travail. Voir **Plan de développement** ci-dessous pour plus d’informations.

### Plan de développement

Nous en sommes aux dernières étapes pour résoudre un problème de qualité des données que nous avons observé au début de la version bêta de la zone de travail de reporting. Nous allons bientôt reprendre le travail pour fournir de nouvelles visualisations, développer la sélection des objets Workfront pouvant être rapportés et améliorer la création de rapports et les expériences de distribution, qui font toutes partie intégrante de la réalisation de nos objectifs pour la zone de travail de reporting.

Ces nouvelles expériences seront mises à disposition progressivement, à compter de la version 23.2, via la nouvelle page Tableaux de bord Zone de travail désormais disponible dans votre environnement de prévisualisation. Les tableaux de bord Zone de travail vous permettent d’afficher les rapports existants avec les nouvelles fonctionnalités de création de rapports que nous sommes en train de créer. Ils serviront d’environnement principal pour le déploiement et le test de nouvelles fonctionnalités pour la zone de travail de reporting. Pour plus d’informations sur l’activation et l’utilisation des tableaux de bord Zone de travail, voir [Vue d’ensemble des tableaux de bord Zone de Travail](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Participer à la version bêta

>[!IMPORTANT]
>
>Les informations bêta ci-dessous sont destinées aux administrateurs et administratrices qui ont déjà été inclus dans la version bêta de la zone de travail de reporting, qui n’accepte plus les nouveaux participants et nouvelles participantes. Si vous souhaitez tester les nouvelles fonctionnalités de la zone de travail de reporting telles qu’elles sont ajoutées, reportez-vous à la section **Plan de développement** ci-dessus pour plus d’informations sur l’activation des tableaux de bord Zone de travail.

### Disponibilité

La version bêta de la zone de travail de reporting est disponible pour toutes les organisations sur AWS, quelle que soit leur région.

### Rejoindre la version bêta

La version bêta de la zone de travail de reporting est entièrement facultative, mais seul un administrateur ou une administratrice Workfront peut y adhérer. Pour vous inscrire en tant qu’administrateur ou administratrice système :

1. Sélectionnez l’icône **Reporting (version bêta)** dans le menu principal de votre instance Workfront.
1. Cliquez sur **Accepter** pour accepter les conditions générales.
1. Autorisez l’ajout des données de votre entreprise à la zone de travail de reporting (cela peut prendre jusqu’à quelques heures).
1. Commencez à utiliser la zone de travail de reporting.

Une fois que les données de votre entreprise ont été ajoutées à la zone de travail de reporting, d’autres administrateurs et administratrices système peuvent choisir d’y inscrire individuellement de la même manière (sans attendre que les données soient à nouveau ajoutées).

Pour inscrire d’autres personnes ne disposant pas de droits d’administration Workfront :

1. Sélectionnez l’icône **Reporting (version bêta)** dans le menu principal de votre instance Workfront.
1. Cliquez sur **Autorisations de la zone de travail de reporting**.
1. Recherchez et sélectionnez les personnes que vous souhaitez voir participer.

   >[!IMPORTANT]
   >
   >Les personnes auxquelles vous accordez l’accès à la zone de travail de reporting auront accès à **toutes** les données du système en lecture seule, quelles que soient leurs autorisations standard d’affichage de ces données.

1. Cliquer sur **Enregistrer**.
1. Ajoutez l’icône **Reporting (version bêta)** dans le modèle de mise en page principal de chaque personne sélectionnée. Pour plus d’informations, voir [Personnaliser le menu principal à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Chaque personne doit ensuite accéder individuellement à l’icône **Reporting (version bêta)** dans le menu principal et accepter les conditions générales.

### Envoyer des commentaires

Pour envoyer des commentaires sur la version bêta :

1. Dans la zone de travail de reporting de Workfront, cliquez sur le bouton **Envoyer un commentaire**.
1. Remplissez le formulaire, puis cliquez sur **Envoyer**.

## Questions fréquentes à propos de la version bêta

+++Puis-je migrer mes rapports hérités vers la zone de travail de reporting ?

En résumé, la migration des rapports hérités ne sera pas disponible avec la version bêta. Cependant, c’est une fonctionnalité qui est prévue (avec quelques avertissements décrits ci-dessous) pour le lancement officiel.

Bien que l’obstacle à la création de nouveaux rapports ait été considérablement réduit avec la zone de travail de reporting, nous comprenons que le transfert de certains de vos rapports et tableaux de bord existants contribuera à accélérer le processus d’adoption. À ce titre, nous voulons fournir les outils et les ressources nécessaires pour vous permettre d’importer tous les éléments hérités appropriés afin de vous assurer de bien démarrer dans la zone de travail de reporting. Cependant, comme la zone de travail de reporting représente un changement radical dans le fonctionnement des rapports actuels, il serait impossible de migrer chaque rapport ou tableau de bord exactement comme aujourd’hui.

Notre stratégie actuelle de migration dans la version officielle est de vous permettre d’effectuer les opérations suivantes :

1. Identifier les rapports et les tableaux de bord pertinents

   1. Vous permet d’exporter un fichier CSV de tous les rapports et tableaux de bord du système, ainsi que toutes les informations de suivi pertinentes (nombre de vues, quand et par qui).
   1. Fournissez un export des rapports configurés avec les diffusions planifiées et les personnes destinataires.

1. Sélectionnez les rapports et les tableaux de bord à migrer, puis cliquez sur **Migrer**.

   Il s’agit d’une migration à sens unique. Une copie des rapports et des tableaux de bord sélectionnés est alors créée dans la zone de travail de reporting, en conservant le rapport ou le tableau de bord hérité dans l’outil de reporting actuel.

   Vous pouvez migrer le même rapport ou tableau de bord autant de fois que vous le souhaitez.

1. Dans la zone de travail de reporting, assurez-vous que tous les rapports et tableaux de bord que vous avez sélectionnés ont été migrés.
+++

+++Pourquoi ne puis-je pas voir tous les objets que je vois normalement ?

Afin de fournir la version bêta à nos clients le plus tôt possible, nous l’avons publiée avec uniquement un sous-ensemble des nombreux types d’objets disponibles dans Workfront aujourd’hui. Vous trouverez ci-dessous les types d’objets actuellement pris en charge dans la version bêta :

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

+++Si un problème se produit dans le zone de travail de reporting au cours de la version bêta, les données de mon entreprise seront-elles affectées ?

Non. La version bêta utilise une copie des données de votre entreprise renseignée dans la zone de travail de reporting. Cela signifie que vous pouvez expérimenter en toute sécurité pendant la version bêta sans risque d’affecter les données importantes, mais cela signifie également que la modification en ligne des données dans la zone de travail de reporting sera indisponible jusqu’au lancement officiel.
+++

+++Puis-je me désinscrire de la version bêta une fois après mon inscription ?

Un administrateur ou une administratrice Workfront ne peut pas se désinscrire de la version bêta. Toutefois, les administrateurs et administratrices hors système peuvent être supprimés en procédant comme suit :

1. Connectez-vous en tant qu’administrateur ou adminsitratrice système.
1. Accédez à la zone de travail de reporting.
1. Cliquez sur les **autorisations** de la zone de travail de reporting.
1. Supprimez les personnes que vous souhaitez exclure de la version bêta de la liste des personnes inscrites.
1. Cliquer sur **Enregistrer**.
+++
