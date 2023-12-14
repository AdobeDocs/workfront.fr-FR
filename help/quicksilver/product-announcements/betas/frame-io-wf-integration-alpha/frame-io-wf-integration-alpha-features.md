---
content-type: reference
navigation-topic: betas
title: "Adobe Workfront et Frame.io native integration alpha: features"
description: Fonctionnalités prévues pour l’alpha d’intégration native d’Adobe Workfront et de Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 4ab78cff65141636e9e2c95526d68face1f278ba
workflow-type: tm+mt
source-wordcount: '1248'
ht-degree: 0%

---

# alpha de l’intégration native Adobe Workfront et Frame.io : fonctionnalités et test

Avec cette intégration, notre objectif est de permettre aux créatifs de rester dans leur outil de choix (CC ou Frame.io) pour créer leur contenu et réaliser des révisions par les pairs, tout en ayant des chefs de projet pour coordonner le travail et initialiser et suivre le processus de révision formel depuis Workfront. Pour ce faire, vous pouvez utiliser les deux meilleures solutions : Workfront de nouvelles validations de document pour la gestion des validations de contenu, ainsi que les fonctionnalités d’examen de contenu proposées par Frame.io. Collectivement, les nouveaux documents approuvés et Frame.io formeront notre nouvelle expérience de révision et d’approbation de contenu de bout en bout. 

Pour en savoir plus sur le fonctionnement de l’alpha et les façons de participer, voir [alpha de l’intégration Adobe Workfront et Frame.io : présentation](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)

>[!NOTE]
>
>Si vous êtes tombé sur ces pages sans que votre entreprise ne participe à ce programme alpha, veillez à traiter les informations ici avec soin et à contacter votre administrateur Workfront ou Frame.io pour plus d’informations.
>

## scénario de test de base

Pour vous permettre de tester facilement les nouvelles fonctionnalités du programme alpha, nous avons créé un nouveau compte de test Frame.io et nous l’avons connecté à un nouveau groupe appelé `Frame.io alpha testing` dans votre environnement Workfront Preview ou Sandbox existant.

Pour tester la fonctionnalité, connectez-vous à votre instance Workfront Preview ou Sandbox et procédez comme suit :

1. **Coordonnateurs :** Dans Workfront, créez un projet avec le `Frame.io alpha testing` groupe affecté en tant que groupe de projet.

1. **Coordonnateurs :** Dans Workfront, marquez les tâches qui nécessitent un travail créatif comme étant activées dans les détails de la tâche et affectez-lui vos créatifs (affectez-vous également si vous souhaitez tester l’ensemble du workflow).

>[!NOTE]
>
>Les sous-tâches ne peuvent pas être marquées comme Frame activées.
>

1. **Coordonnateurs :** Chargez votre résumé créatif et définissez l’état du projet sur &quot;Actuel&quot;.

1. **Créatifs :** Recherchez dans vos emails une invitation au projet Frame.io nouvellement créé.

1. **Créatifs :** Cliquez sur le bouton &quot;Rejoindre le projet&quot; dans l’e-mail d’invitation pour rejoindre le projet Frame.io, passez en revue le dossier créatif du projet et commencez la création de contenu dans votre outil de Creative Cloud de votre choix.

1. **Créatifs :** Chargez les ressources créées sur Frame.io et ajoutez-les au projet Workfront lié en sélectionnant l’une des tâches Frame-enabled qui vous sont affectées. Sélectionnez l’option pour marquer la tâche comme terminée.

1. **Coordonnateurs :** Dans Workfront, recherchez les ressources Frame.io liées dans la tâche avec fonction de cadre et vérifiez que l’état de la tâche a été modifié pour &quot;terminer&quot;.

1. **Coordonnateurs :** Affectez des réviseurs/approbateurs à la ressource Frame.io liée. Vous pouvez également vous attribuer le rôle d’approbateur si vous souhaitez tester l’ensemble du workflow. (Pour plus d’informations sur l’attribution des révisions/approbateurs, voir [Ajout d’approbateurs ou de réviseurs à un document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Parties prenantes :** Dans Workfront, consultez votre demande d’approbation dans Accueil, Détails du document ou dans la notification électronique reçue. Ouvrez la ressource dans la visionneuse Frame.io, laissez un commentaire contenant des commentaires et prenez une décision.

1. **Coordonnateurs :** Dans Workfront, affichez les commentaires créés par les parties prenantes dans la section Mises à jour du document connecté à Frame.io, ainsi que la décision dans la section Approbation ou le volet Résumé du document.

1. **Créatifs :** Dans Frame.io, notez la décision d’approbation globale prise pour vos ressources.

1. **Créatifs :** Dans Frame.io, appliquez les modifications demandées en ajoutant la version mise à jour à la pile de versions de la ressource connectée.

1. **Coordonnateurs :** Dans Workfront, affectez les approbateurs/réviseurs à la version que vous venez de télécharger et surveillez la progression jusqu’à ce qu’elle atteigne l’approbation.

## Scénario de test détaillé

Pour les participants qui souhaitent tester des fonctionnalités supplémentaires, nous avons créé un scénario de test plus impliqué. Un guide pour ce scénario de test détaillé peut être téléchargé ici : [Présentation détaillée du scénario de test détaillé WF + Frame.io](/help/quicksilver/product-announcements/betas/assets/WF-Frame-Detailed-Test-Scenario-Walkthrough.pdf).

## Plans de fonctionnalités

Vous trouverez ci-dessous des informations sur les principaux cas d’utilisation que nous recherchons et sur les fonctionnalités que nous prévoyons de mettre en place. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>Puces sous un **&quot;Améliorations potentielles dans les prochaines versions&quot;** Un en-tête peut être inclus ou non dans une version ultérieure, en fonction des commentaires alpha et de l’évolution de nos plans de développement.
>

### Les administrateurs Workfront peuvent configurer une connexion entre les groupes Workfront et les comptes Frame.io

* Dans Workfront, vous pouvez connecter un groupe Workfront à un compte Frame.io.

* Une nouvelle équipe de Frame.io sera créée dans Frame.io représentant le groupe Workfront connecté (Notez que cette fonctionnalité n’a été activée que pour les clients qui utilisent l’intégration en production. Les clients qui effectuent toujours le test sur Sandbox ou Preview auront la connexion configurée par l’équipe Adobe.)

**Améliorations potentielles dans les prochaines versions :**

* Déconnexion d’un groupe Workfront d’un compte Frame.io

* Connexion d’un groupe Workfront à une équipe Frame.io existante

### Les coordinateurs de projet peuvent configurer les projets Workfront envoyés à Frame.io et auxquels les créatifs affectés dans Workfront sont ajoutés dans le projet Frame.io.

* Possibilité de marquer les projets Workfront comme Frame.io activé en attribuant un groupe connecté à Frame

* Possibilité de basculer les tâches dans les projets Workfront en tâches Frame qui à leur tour créent des dossiers de tâches dans Frame.io

* Dans le cas d’un projet Workfront, un groupe lié à un cadre est affecté et au moins une tâche compatible avec le cadre est affectée. Lorsque l’état du projet Workfront est défini sur Actuel, un projet correspondant connecté est créé dans le cadre, les utilisateurs affectés à Workfront sont ajoutés au projet cadre et une notification électronique leur est envoyée à partir de Frame.io.

   * Les utilisateurs et les équipes affectés aux tâches Workfront compatibles avec les images seront ajoutés en tant que collaborateurs au projet Frame.io et informés (lors de la création du projet et ultérieurement).

* Les documents (Creative Briefs) ajoutés au projet et les tâches Frame activées seront transférées au projet Frame.io (dans le dossier de travail respectif) lors de la création du projet (déclencheur : l’état du projet défini sur Actuel).

   * Nous vous recommandons de limiter la quantité de documents ajoutés à votre projet avant de n’être actifs qu’à vos mémoires créatives, afin d’éviter d’envoyer plusieurs documents inutiles à Frame.io.

   * Les documents/tâches ajoutés après la synchronisation initiale du projet ne seront pas transmis à Frame.io, seuls les utilisateurs/équipes

**Améliorations potentielles dans les prochaines versions :**

* Les tâches compatibles avec les images peuvent être configurées sur des modèles de projet.

* Les nouvelles versions téléchargées vers les conseils de création sont transférées vers le cadre.

* Synchronisation optimisée des projets (déconnexion des projets, resynchronisation des projets et documents, etc.)

### Dans Frame.io, les créatifs peuvent envoyer des ressources créées au projet Workfront pour révision formelle.

* Possibilité de connecter une ressource Frame.io unique à un projet ou à une tâche WF. Une référence de ressource sera créée dans Workfront.

* Les nouveaux chargements de version dans Frame.io créent automatiquement une version de document dans Workfront sur les ressources connectées.

* Possibilité de marquer les tâches Workfront référencées comme terminées dans Frame.io

* Si le document Workfront connecté est supprimé, il reste dans Frame.io et peut être reconnecté à la même tâche de projet ou à une autre.

**Améliorations potentielles dans les prochaines versions :**

* Possibilité d’envoyer plusieurs ressources Frame.io à Workfront simultanément

* Journalisation temporelle du projet/de la tâche Workfront depuis Frame.io

### Les coordinateurs de projet peuvent affecter le processus d’approbation formel aux documents liés à Frame.io.

* Les utilisateurs et les équipes de Workfront peuvent être ajoutés aux nouveaux documents approuvés pour les documents connectés à Frame.io.

* Lorsqu’un utilisateur/une équipe n’est plus partagé à partir d’un document compatible avec Frame, il perd également son accès à la ressource dans la visionneuse Frame.io

**Améliorations potentielles dans les prochaines versions :**

* Envoi de plusieurs ressources en tant que révision unique

* Affectation en masse d’approbateurs/de réviseurs aux documents Workfront

### Les parties prenantes peuvent procéder à leur révision et approbation dans la visionneuse Frame.io

* Les parties prenantes seront informées et pourront afficher le document Frame connecté dans la visionneuse Frame.io

* La visionneuse Frame.io est accessible à différents emplacements dans Workfront, par exemple, liste de documents, détails du document, page d’accueil de Workfront.

* Possibilité d’exploiter les fonctionnalités de révision et de commentaire existantes fournies par la visionneuse Frame.io qui sera synchronisée avec le flux de mise à jour de Workfront

* Possibilité de prendre une nouvelle décision concernant l’approbation des documents depuis la visionneuse Frame.io
