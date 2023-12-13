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
source-git-commit: 31adfeffeda9fc6aa4e76ceae7ef410d9c4c178c
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 0%

---

# alpha de l’intégration native Adobe Workfront et Frame.io : fonctionnalités et test

Avec cette intégration, notre objectif est de permettre aux créatifs de rester dans leur outil de choix (CC ou Frame.io) pour créer leur contenu et réaliser des révisions par les pairs, tout en ayant des chefs de projet pour coordonner le travail et initialiser et suivre le processus de révision formel depuis Workfront. Pour ce faire, vous pouvez utiliser les deux meilleures solutions : Workfront de nouvelles validations de document pour la gestion des validations de contenu, ainsi que les fonctionnalités d’examen de contenu proposées par Frame.io. Collectivement, les nouveaux documents approuvés et Frame.io formeront notre nouvelle expérience de révision et d’approbation de contenu de bout en bout. 

Pour en savoir plus sur le fonctionnement de l’alpha et les façons de participer, voir [alpha de l’intégration Adobe Workfront et Frame.io : présentation](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Si vous êtes tombé sur ces pages sans que votre entreprise ne participe à ce programme alpha, veillez à traiter les informations ici avec soin et à contacter votre administrateur Workfront ou Frame.io pour plus d’informations.

## scénario de test de base

Pour vous permettre de tester facilement les nouvelles fonctionnalités du programme alpha, nous avons créé un nouveau compte de test Frame.io et nous l’avons connecté à un nouveau groupe appelé `Frame.io alpha testing` dans votre environnement Workfront Preview ou Sandbox existant.

Pour tester la fonctionnalité, connectez-vous à votre instance Workfront Preview ou Sandbox et procédez comme suit :

>[!NOTE]
>
><span class="preview">Texte mis en surbrillance</span> ci-dessous fait référence à des fonctionnalités qui ne sont pas encore mises en oeuvre à des fins de test, mais qui seront incluses dans une version ultérieure.
>

1. **Coordonnateurs :** Dans Workfront, créez un projet avec le `Frame.io alpha testing` groupe affecté en tant que groupe de projet.

1. **Coordonnateurs :** Dans Workfront, affectez vos créatifs au projet. <span class="preview">ou les tâches Frame enabled (notez que les sous-tâches ne peuvent pas être marquées comme étant Frame enabled).</span> et définissez l’état du projet sur &quot;Actuel&quot;.

1. **Créatifs :** Recherchez dans vos emails une invitation au projet Frame.io nouvellement créé.

1. **Créatifs :** Cliquez sur le bouton &quot;Rejoindre le projet&quot; dans l’e-mail d’invitation pour rejoindre le projet Frame.io, passez en revue le dossier créatif du projet et commencez la création de contenu dans votre outil de Creative Cloud de votre choix.

1. **Créatifs :** Chargez les ressources créées sur Frame.io et ajoutez-les au projet Workfront lié. <span class="preview">(ou tâches activées dans le cadre affectées).</span>

1. **Coordonnateurs :** Dans Workfront, recherchez les ressources Frame.io liées dans votre projet et affectez les réviseurs/approbateurs (pour plus d’informations sur l’attribution des révisions/approbateurs, voir [Ajout d’approbateurs ou de réviseurs à un document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Parties prenantes :** Dans Workfront, consultez votre demande d’approbation dans Détails du document ou de l’accueil, consultez le document Frame connecté dans la visionneuse Frame.io, puis laissez un commentaire contenant des commentaires.

1. <span class="preview">**Coordonnateurs :** Dans Workfront, consultez les commentaires créés par les parties prenantes dans la section Mises à jour du document connecté à Frame.io.</span>

1. <span class="preview">**Parties prenantes :** Prenez une décision dans la visionneuse Frame.io.</span>

1. <span class="preview">**Créatifs :** Dans Frame.io, notez la décision d’approbation globale prise pour vos ressources.</span>

1. **Créatifs :** Dans Frame.io, appliquez les modifications demandées en ajoutant la version mise à jour à la pile de versions de la ressource connectée.

1. **Coordonnateurs :** Dans Workfront, affectez les approbateurs/réviseurs à la version que vous venez de télécharger et surveillez la progression jusqu’à ce qu’elle atteigne l’approbation.

## Scénario de test détaillé

Pour les participants qui souhaitent tester des fonctionnalités supplémentaires, nous avons créé un scénario de test plus impliqué. Un guide pour ce scénario de test détaillé peut être téléchargé ici : [Présentation détaillée du scénario de test détaillé WF + Frame.io](/help/quicksilver/product-announcements/betas/assets/WF-Frame-Detailed-Test-Scenario-Walkthrough.pdf).

## Plans de fonctionnalités

Vous trouverez ci-dessous des informations sur les principaux cas d’utilisation que nous recherchons et sur les fonctionnalités que nous prévoyons de mettre en place. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">Texte mis en surbrillance</span> ci-dessous fait référence à des fonctionnalités qui ne sont pas encore mises en oeuvre, mais qui seront incluses dans une version ultérieure.
>
>Puces sous un **&quot;Améliorations potentielles dans les prochaines versions&quot;** Un en-tête peut être inclus ou non dans une version ultérieure, en fonction des commentaires alpha et de l’évolution de nos plans de développement.
>


### Les administrateurs Workfront peuvent configurer une connexion entre les groupes Workfront et les comptes Frame.io

* <span class="preview">Dans Workfront, vous pouvez connecter un groupe Workfront à un compte Frame.io.</span>

* Une nouvelle équipe Frame.io sera créée dans Frame.io, qui représente le groupe Workfront connecté.

**Améliorations potentielles dans les prochaines versions :**

* Déconnexion d’un groupe Workfront d’un compte Frame.io

* Connexion d’un groupe Workfront à une équipe Frame.io existante

### Les coordinateurs de projet peuvent configurer les projets Workfront envoyés à Frame.io et auxquels les créatifs affectés dans Workfront sont ajoutés dans le projet Frame.io.

* Possibilité de marquer les projets Workfront comme Frame.io activé en attribuant un groupe connecté à Frame

* <span class="preview">Amélioration : possibilité de basculer les tâches dans les projets Workfront en tâches Frame qui, à leur tour, créent des dossiers de tâches dans Frame.io</span>

* Lorsqu’un état de projet Workfront est défini sur Actuel, un projet connecté correspondant est créé dans Cadre, les utilisateurs affectés par Workfront sont ajoutés au projet Cadre et une notification par courrier électronique leur est envoyée à partir de Frame.io.

   * Tous les membres du projet Workfront (utilisateurs et équipes) seront ajoutés en tant que collaborateurs au projet Frame.io (lors de la création du projet et ultérieurement).

   * <span class="preview">Modification : les utilisateurs et les équipes affectés aux tâches Workfront compatibles avec les images seront ajoutés en tant que collaborateurs au projet Frame.io et informés (lors de la création du projet et ultérieurement).</span>

* Les documents (Creative Briefs) ajoutés au projet et les tâches Frame activées seront transférées au projet Frame.io (dans le dossier de travail respectif) lors de la création du projet (déclencheur : l’état du projet défini sur Actuel).

   * Nous vous recommandons de limiter la quantité de documents ajoutés à votre projet avant de n’être actifs qu’à vos mémoires créatives, afin d’éviter d’envoyer plusieurs documents inutiles à Frame.io.

* <span class="preview">Amélioration : les utilisateurs/équipes explicitement non affectés à une tâche Workfront compatible avec les images seront supprimés du projet Frame.io.</span>

**Améliorations potentielles dans les prochaines versions :**

* Les tâches compatibles avec les images peuvent être configurées sur des modèles de projet.

* Les nouvelles versions téléchargées vers les conseils de création sont transférées vers le cadre.

* Synchronisation optimisée des projets (déconnexion des projets, resynchronisation des projets et documents, etc.)

### Dans Frame.io, les créatifs peuvent envoyer des ressources créées au projet Workfront pour révision formelle.

* Possibilité de connecter une ressource Frame.io unique à un projet ou à une tâche WF. Une référence de ressource sera créée dans Workfront.

* Les nouveaux chargements de version dans Frame.io créent automatiquement une version de document dans Workfront sur les ressources connectées.

* <span class="preview">Amélioration : possibilité de marquer les tâches Workfront référencées comme terminées à partir de Frame.io</span>

* <span class="preview">Amélioration : si le document Workfront connecté est supprimé, il reste dans Frame.io et peut être reconnecté à la même tâche de projet ou à une autre.</span>

**Améliorations potentielles dans les prochaines versions :**

* Possibilité d’envoyer plusieurs ressources Frame.io à Workfront simultanément

* Journalisation temporelle du projet/de la tâche Workfront depuis Frame.io

### Les coordinateurs de projet peuvent affecter le processus d’approbation formel aux documents liés à Frame.io.

* Les utilisateurs et les équipes de Workfront peuvent être ajoutés aux nouveaux documents approuvés pour les documents connectés à Frame.io.

* <span class="preview">Amélioration : lorsqu’un utilisateur/une équipe n’est plus partagé à partir d’un document compatible avec Frame, il perd également son accès à la ressource dans la visionneuse Frame.io</span>

**Améliorations potentielles dans les prochaines versions :**

* Envoi de plusieurs ressources en tant que révision unique

* Affectation en masse d’approbateurs/de réviseurs aux documents Workfront

### Les parties prenantes peuvent procéder à leur révision et approbation dans la visionneuse Frame.io

* Les parties prenantes seront informées et pourront afficher le document Frame connecté dans la visionneuse Frame.io

* La visionneuse Frame.io est accessible à différents emplacements dans Workfront, par exemple, liste de documents, détails du document, page d’accueil de Workfront.

* Possibilité d’exploiter les fonctionnalités de révision et de commentaire existantes fournies par la visionneuse Frame.io qui sera synchronisée avec le flux de mise à jour de Workfront

* <span class="preview">Possibilité de prendre une nouvelle décision concernant l’approbation des documents depuis la visionneuse Frame.io</span>

### Dans Frame.io, les créatifs seront informés de la décision globale prise sur la ressource Frame.io connectée.

* <span class="preview">Amélioration : l’état global de l’approbation des documents s’affiche sur la ressource dans Frame.io</span>

### Les coordinateurs de projet peuvent envoyer les ressources finales à AEM

* <span class="preview">Amélioration : les documents liés à l’image, y compris les métadonnées, peuvent être envoyés à AEM à l’aide du connecteur Workfront + AEM Asset CS existant.</span>
