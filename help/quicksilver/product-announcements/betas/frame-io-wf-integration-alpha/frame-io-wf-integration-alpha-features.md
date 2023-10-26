---
content-type: reference
navigation-topic: betas
title: "Adobe Workfront et Frame.io native integration alpha: features"
description: Fonctionnalités prévues pour l’alpha d’intégration native d’Adobe Workfront et de Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# alpha de l’intégration native Adobe Workfront et Frame.io : fonctionnalités

## Cas d’utilisation et tests de fonctionnalités

Avec cette intégration, notre objectif est de permettre aux créatifs de rester dans leur outil de choix (CC ou Frame.io) pour créer leur contenu et réaliser des révisions par les pairs, tout en ayant des chefs de projet pour coordonner le travail et initialiser et suivre le processus de révision formel depuis Workfront. Pour ce faire, vous pouvez utiliser les deux meilleures solutions : Workfront de nouvelles validations de document pour la gestion des validations de contenu, ainsi que les fonctionnalités d’examen de contenu proposées par Frame.io. Collectivement, les nouveaux documents approuvés et Frame.io formeront notre nouvelle expérience de révision et d’approbation de contenu de bout en bout. 

Pour en savoir plus sur le fonctionnement de l’alpha et les façons de participer, voir [alpha de l’intégration Adobe Workfront et Frame.io : présentation](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Si vous êtes tombé sur ces pages sans que votre entreprise ne participe à ce programme alpha, veillez à traiter les informations ici avec soin et à contacter votre administrateur Workfront ou Frame.io pour plus d’informations.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## Plans de fonctionnalités

Vous trouverez ci-dessous des informations sur les principaux cas d’utilisation que nous recherchons et sur les fonctionnalités que nous prévoyons de mettre en place. <!--, along with documentation to get you started testing.-->


### Les administrateurs Workfront peuvent configurer une connexion entre les groupes Workfront et les comptes Frame.io

* _Dans Workfront, vous pouvez connecter un groupe Workfront à un compte Frame.io._

* Une nouvelle équipe Frame.io sera créée dans Frame.io, qui représente le groupe Workfront connecté.

**Améliorations potentielles dans les prochaines versions :**

* Déconnexion d’un groupe Workfront d’un compte Frame.io

* Connexion d’un groupe Workfront à une équipe Frame.io existante

### Les coordinateurs de projet peuvent configurer les projets Workfront envoyés à Frame.io et auxquels les créatifs affectés dans Workfront sont ajoutés dans le projet Frame.io.

* Possibilité de marquer les projets Workfront comme Frame.io activé en attribuant un groupe connecté à Frame

* _Amélioration : possibilité de basculer les tâches dans les projets Workfront en tâches Frame qui, à leur tour, créent des dossiers de tâches dans Frame.io_

* Lorsqu’un état de projet Workfront est défini sur Actuel, un projet connecté correspondant est créé dans Cadre, les utilisateurs affectés par Workfront sont ajoutés au projet Cadre et une notification par courrier électronique leur est envoyée à partir de Frame.io.

   * Tous les membres du projet Workfront (utilisateurs et équipes) seront ajoutés en tant que collaborateurs au projet Frame.io (lors de la création du projet et ultérieurement).

   * _Modification : les utilisateurs et les équipes affectés aux tâches Workfront compatibles avec les images seront ajoutés en tant que collaborateurs au projet Frame.io et informés (lors de la création du projet et ultérieurement)._

* Les documents (Creative Briefs) ajoutés au projet et les tâches Frame activées seront transférées au projet Frame.io (dans le dossier de travail respectif) lors de la création du projet (déclencheur : l’état du projet défini sur Actuel).

   * Nous vous recommandons de limiter la quantité de documents ajoutés à votre projet avant de n’être actifs qu’à vos mémoires créatives, afin d’éviter d’envoyer plusieurs documents inutiles à Frame.io.

* _Amélioration : les utilisateurs/équipes explicitement non affectés à une tâche Workfront compatible avec les images seront supprimés du projet Frame.io._

**Améliorations potentielles dans les prochaines versions :**

* Les tâches compatibles avec les images peuvent être configurées sur des modèles de projet.

* Les nouvelles versions téléchargées vers les conseils de création sont transférées vers le cadre.

* Synchronisation optimisée des projets (déconnexion des projets, resynchronisation des projets et documents, etc.)

### Dans Frame.io, les créatifs peuvent envoyer des ressources créées au projet Workfront pour révision formelle.

* Possibilité de connecter une ressource Frame.io unique à un projet ou à une tâche WF. Une référence de ressource sera créée dans Workfront.

* Les nouveaux chargements de version dans Frame.io créent automatiquement une version de document dans Workfront sur les ressources connectées.

* _Amélioration : possibilité de marquer les tâches Workfront référencées comme terminées à partir de Frame.io_

* _Amélioration : si le document Workfront connecté est supprimé, il reste dans Frame.io et peut être reconnecté à la même tâche de projet ou à une autre._

**Améliorations potentielles dans les prochaines versions :**

* Possibilité d’envoyer plusieurs ressources Frame.io à Workfront simultanément

* Journalisation temporelle du projet/de la tâche Workfront depuis Frame.io

### Les coordinateurs de projet peuvent affecter le processus d’approbation formel aux documents liés à Frame.io.

* Les utilisateurs et les équipes de Workfront peuvent être ajoutés aux nouveaux documents approuvés pour les documents connectés à Frame.io.

* _Amélioration : lorsqu’un utilisateur/une équipe n’est plus partagé à partir d’un document compatible avec Frame, il perd également son accès à la ressource dans la visionneuse Frame.io_

**Améliorations potentielles dans les prochaines versions :**

* Envoi de plusieurs ressources en tant que révision unique

* Affectation en masse d’approbateurs/de réviseurs aux documents Workfront

### Les parties prenantes peuvent procéder à leur révision et approbation dans la visionneuse Frame.io

* Les parties prenantes seront informées et pourront afficher le document Frame connecté dans la visionneuse Frame.io

* La visionneuse Frame.io est accessible à différents emplacements dans Workfront, par exemple, liste de documents, détails du document, page d’accueil de Workfront.

* Possibilité d’exploiter les fonctionnalités de révision et de commentaire existantes fournies par la visionneuse Frame.io qui sera synchronisée avec le flux de mise à jour de Workfront

* _Possibilité de prendre une nouvelle décision concernant l’approbation des documents depuis la visionneuse Frame.io_

### Dans Frame.io, les créatifs seront informés de la décision globale prise sur la ressource Frame.io connectée.

* _Amélioration : l’état global de l’approbation des documents s’affiche sur la ressource dans Frame.io_

### Les coordinateurs de projet peuvent envoyer les ressources finales à AEM

* _Amélioration : les documents liés à l’image, y compris les métadonnées, peuvent être envoyés à AEM à l’aide du connecteur Workfront + AEM Asset CS existant._