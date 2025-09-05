---
title: Acquisition et installation d’applications à partir d’Adobe Exchange
description: Les extensions d’interface d’utilisation de Workfront, optimisées par Adobe App Builder, permettent aux clientes et clients et aux partenaires de créer des expériences d’utilisation personnalisées.
author: Courtney
feature: Digital Content and Documents
source-git-commit: 0a90da6978fc9b380d237dab74af1f14eabb857a
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 1%

---


# Acquisition et installation d’applications à partir d’Adobe Exchange

Vous pouvez désormais installer des applications créées par des partenaires pour Workfront directement depuis Adobe Exchange. Cette fonctionnalité connecte les clients à un écosystème grandissant de partenaires Adobe qui fournissent des outils spécialement conçus pour améliorer la productivité, rationaliser les opérations et étendre les fonctionnalités de Workfront. Grâce à Adobe Exchange, les clients peuvent découvrir et installer des applications qui s’intègrent facilement dans Workfront à l’aide des extensions d’interface utilisateur.

Adobe Exchange est le marché central pour les applications tierces, les extensions et les intégrations dans Adobe Experience Cloud, y compris Adobe Workfront. Pour les clients Workfront, il s’agit de la destination de référence pour découvrir et installer des applications qui améliorent les fonctionnalités, rationalisent les workflows et s’intègrent aux systèmes externes.

## Applications partenaires Adobe

Workfront Partner Network est un écosystème croissant de partenaires technologiques, des éditeurs de logiciels indépendants (ISV) qui créent des applications évolutives, sécurisées et extensibles à l’aide des extensions d’interface utilisateur Adobe App Builder et Workfront.

Les partenaires de Workfront tirent parti des extensions de l’interface utilisateur de Workfront, un cadre puissant qui permet d’incorporer directement des applications dans l’interface de Workfront. Une fois installées à partir d&#39;Adobe Exchange, les administrateurs Workfront peuvent ajouter ces applications aux modèles de disposition, ce qui les rend visibles et accessibles aux utilisateurs dans leurs workflows quotidiens. Cette intégration transparente permet aux utilisateurs d’interagir avec des outils conçus par des partenaires (tels que des tableaux de bord, des flux de validation ou des dispositifs de suivi de campagne) sans quitter l’environnement Workfront.

### AtApp

#### Résultats en temps réel, directement dans Adobe Workfront

Nous nous associons à des clients Adobe Workfront pour transformer les goulets d’étranglement quotidiens en solutions reproductibles aux résultats prévisibles. Notre bibliothèque croissante de solutions vous aide à accroître la précision, la vitesse et la responsabilité en utilisant des données en direct là où les gens travaillent. Vous pouvez aider les dirigeants à voir ce qui se passe maintenant et à planifier ce qui devrait se passer ensuite. Explorez les applications Adobe Exchange AtAppStore actuellement disponibles et prêtes à être installées, choisissez celles qui correspondent à vos priorités actuelles, puis effectuez une mise à l’échelle à mesure que vos besoins augmentent.

* [Excel Updater](https://exchange.adobe.com/apps/ec/abtt1rq7o9/atapp-excel-updater) : la solution Excel Updater vous offre un chemin rentable pour intégrer des données dans Workfront sans avoir à apprendre l’API, à écrire du code ou à configurer un serveur. Elle est idéale pour les chargements de données ponctuels et récurrents.

* [Recalc Helper](https://exchange.adobe.com/apps/ec/abv755903t/atapp-recalc-helper) : la solution Recalc Helper vous permet de recalculer facilement les expressions calculées du formulaire personnalisé, les chronologies de projet ou les finances du projet pour tous les éléments correspondant à un filtre sélectionné, directement depuis Workfront.

* UberTimesheet : la solution d&#39;UberTimesheet peut améliorer et élargir l&#39;adoption de Workfront par vos utilisateurs en rendant simple et pratique pour tout le monde de suivre le temps de leur navigateur, tablette ou smartphone, après coup.

### Workfocus

Workfocus fournit des solutions avancées d’automatisation et d’intégration pour Workfront. Leurs applications se concentrent sur :

* Rationalisation des délais

* Automatisation des workflows Fusion

* Activation de la collaboration entre instances

Les applications Workfocus sont conçues pour fonctionner de manière native dans Workfront, en utilisant les extensions d’interface utilisateur pour fournir aux utilisateurs et utilisatrices des outils puissants qui améliorent la productivité et réduisent les efforts manuels.

## Conditions préalables et autorisations

**Approvisionnement d’App Builder**

* App Builder doit être configuré dans le Adobe Admin Console des clients. Il s’agit d’un prérequis pour installer des applications à partir d’Adobe Exchange.

**Administrateurs ou développeurs d’organisation d’entreprise**

* Peut rechercher des applications, cliquer sur **Obtenir** et poursuivre l’installation.

* Si l’application est déjà acquise par une personne de l’organisation, cette personne peut voir **Commencer l’installation** ou **Gérer** à la place.

**Utilisateurs non-administrateurs**

* Peut lancer l’acquisition, mais sera invité à se connecter et pourra rencontrer des restrictions si l’application nécessite le consentement de l’administrateur ou une licence spéciale.

## Acquisition et installation d’applications à partir d’Adobe Exchange

Les clients Adobe peuvent parcourir, rechercher et installer des applications directement depuis Adobe Exchange Marketplace pour les utiliser dans Workfront.

Les applications créées avec Adobe App Builder sont répertoriées comme _Applications App Builder_ sur Adobe Exchange. Chaque liste d’applications comprend de la documentation, des captures d’écran et des instructions d’utilisation pour aider les clients à comprendre la valeur de l’application.

Pour afficher des applications pour Workfront, accédez à Adobe Exchange et recherchez des applications compatibles avec Workfront. Vous pouvez également filtrer les listes pour les applications Workfront App Builder :

1. Cliquez sur **Experience Cloud** dans le panneau de gauche.
1. Dans le panneau de gauche, recherchez **Produit**, puis sélectionnez **Workfront**.
1. Développez **Type d’application**, puis choisissez **App Builder**.

### Acquisition d’applications

Les applications peuvent nécessiter un achat auprès d’Adobe Exchange ou permettre l’installation, mais nécessitent une licence du développeur de l’application.

Pour acquérir une application

1. Cliquez sur le nom de l’application.
1. Cliquez sur le bouton situé dans le coin supérieur droit de la liste des applications.
1. Cliquez sur **Oui, continuer** puis acceptez le contrat de licence de l’utilisateur final.
   ![confirmer le contrat de licence](assets/2-aquire-application.png)

### Actions pour les administrateurs système

Lorsqu’un utilisateur acquiert une application à partir d’Adobe Exchange, le message suivant peut s’afficher : _Votre administrateur système doit approuver votre acquisition avant que vous puissiez installer et utiliser votre application._

Cela signifie que l’application nécessite une approbation au niveau de l’administrateur avant de pouvoir continuer l’installation. Les administrateurs système peuvent trouver la requête dans les zones suivantes :

**Notifications**

Les administrateurs système sont généralement avertis par e-mail lorsqu’un utilisateur de leur entreprise acquiert une application.

**Admin Console**

Les administrateurs système peuvent se connecter à Admin Console à l’adresse [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/) et accéder à Produits > Intégrations d’applications pour afficher toutes les applications acquises ou demandées.

Une fois qu’un administrateur système a accès aux demandes, il peut examiner et approuver la demande. Certaines applications peuvent demander à l’administrateur de consentir à l’accès aux données et affecter l’application à des profils de produit ou à des utilisateurs spécifiques.

Une fois l’application approuvée, elle peut être installée.

![examiner et approuver les applications](assets/3-manage.png)

## Installation des applications

Une fois une application acquise, elle peut être installée directement dans Workfront. Les administrateurs peuvent gérer les applications installées via l’interface de Workfront, en s’assurant qu’elles sont correctement configurées et accessibles aux utilisateurs.

1. Recherchez l’application à installer et ouvrez le menu Actions sur le côté droit de l’écran.
1. Cliquez sur Afficher les détails de l’application.
1. Sélectionnez un environnement dans la partie gauche de l’écran ou ajoutez-en un nouveau.
1. Cliquez sur **Déployer**.
   ![déployer l’application](assets/10-env-details-2.png)
1. Attribuez des droits d’installation ou d’utilisation (si nécessaire).

   Si votre entreprise contrôle l’accès à l’application via des profils de produit ou des groupes d’utilisateurs, affectez l’application au profil ou au groupe approprié afin que les utilisateurs puissent procéder à l’installation et utiliser.

## Ajouter au modèle de mise en page

Une fois déployée, l’application partenaire est disponible dans le modèle de mise en page Workfront. Vous pouvez ajouter l’application à la navigation principale ou secondaire à utiliser dans Workfront.

Pour ajouter l&#39;application au modèle de mise en page, ouvrez le modèle de mise en page et accédez au menu principal ou à la zone du menu secondaire. Ajoutez l’application à l’aide de l’icône Ajouter .

![ajouter l’application au modèle de mise en page](assets/add-to-lt.png)

## Contacter l’assistance technique de l’application

Les extensions installées à partir d’Adobe Exchange sont prises en charge par les propriétaires de l’application. Dans la gestion des applications, vous pouvez cliquer sur **Obtenir de l’aide** pour obtenir de l’aide sur n’importe quel problème.