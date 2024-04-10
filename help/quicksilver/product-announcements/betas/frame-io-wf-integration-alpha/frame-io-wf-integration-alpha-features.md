---
content-type: reference
navigation-topic: betas
title: '« Intégration native d’Adobe Workfront et de Frame.io en version bêta : fonctionnalités »'
description: Fonctionnalités prévues pour la version bêta de l’intégration native d’Adobe Workfront et Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: b7a0fe333f0d8f17bc2d6c612d8cff6ee484c935
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Intégration native d’Adobe Workfront et de Frame.io en version bêta : fonctionnalités et tests

Avec cette intégration, notre objectif est de permettre aux créatifs de rester dans l&#39;outil de leur choix (CC ou Frame.io) pour mener leur création de contenu et les révisions par les pairs, tout en demandant aux chefs de projet de coordonner le travail et d&#39;initialiser et de surveiller le processus de révision officiel depuis Workfront. Vous pouvez y parvenir en utilisant le meilleur des deux solutions : Workfront pour les approbations de nouveaux documents pour la gestion des validations de contenu, conjointement avec les fonctionnalités de révision de contenu proposées par Frame.io. Collectivement, les nouvelles approbations de documents et Frame.io formeront notre nouvelle expérience de bout en bout de révision et d&#39;approbation de contenu. 

Pour en savoir plus sur le fonctionnement de la version bêta et sur les différentes manières de participer, voir [Intégration d’Adobe Workfront et de Frame.io en version bêta : présentation](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>Si vous avez consulté ces pages sans que votre société ne participe à ce programme bêta, veillez à traiter les informations ici avec soin et à contacter votre administrateur Workfront ou Frame.io pour plus d&#39;informations.
>

## Vidéo de démonstration

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## Scénario de test de base

Pour vous permettre de tester facilement les nouvelles fonctionnalités du programme bêta, nous avons créé un nouveau compte de test Frame.io et l&#39;avons connecté à un nouveau groupe appelé `Frame.io testing` dans votre environnement Workfront Preview ou Sandbox existant.

Pour tester la fonctionnalité, connectez-vous à votre instance Workfront Preview ou Sandbox et procédez comme suit :

1. **Coordinateurs :** Dans Workfront, créez un projet avec `Frame.io testing` groupe affecté comme groupe de projet.

1. **Coordinateurs :** Dans Workfront, marquez les tâches qui nécessitent du travail créatif comme étant activées pour les cadres (dans les détails de la tâche) et affectez-y vos éléments créatifs (affectez-vous également si vous souhaitez tester l’ensemble du workflow).

>[!NOTE]
>
>Les sous-tâches ne peuvent pas être marquées comme Frame activé.
>

1. **Coordinateurs :** Chargez votre briefing de création et modifiez le statut du projet en « Actuel ».

1. **Éléments créatifs :** Vérifiez vos e-mails pour une invitation au nouveau projet Frame.io

1. **Éléments créatifs :** Cliquez sur le bouton « Rejoindre le projet » dans l’e-mail d’invitation pour rejoindre le projet Frame.io, passez en revue le briefing de création au sein du projet et commencez la création de contenu dans l’outil de Creative Cloud de votre choix.

1. **Éléments créatifs :** Chargez les ressources que vous avez créées dans Frame.io et ajoutez-les au projet Workfront lié en sélectionnant l’une des tâches compatibles avec Frame qui vous ont été affectées. Sélectionnez l’option pour marquer la tâche comme terminée.

1. **Coordinateurs :** Dans Workfront, recherchez les ressources Frame.io liées dans la tâche activée pour les images et vérifiez que le statut de la tâche est passé à « terminé ».

1. **Coordinateurs :** Attribuez des réviseurs/approbateurs à la ressource Frame.io liée. Vous devez également vous affecter en tant qu’approbateur si vous souhaitez tester l’ensemble du workflow. (Pour plus d&#39;informations sur l&#39;affectation de validants/approbateurs, voir [Ajouter d&#39;autres approbateurs ou réviseurs à un document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Parties prenantes :** Dans Workfront, affichez la demande d’approbation sur l’Accueil, dans les Détails du document ou dans l’e-mail de notification reçu. Ouvrez la ressource dans la visionneuse Frame.io, laissez un commentaire contenant des commentaires et prenez une décision.

1. **Coordinateurs :** Dans Workfront, affichez les commentaires créés par les parties prenantes dans la section Mises à jour du document connecté Frame.io, ainsi que la décision dans la section Approbation ou le volet de résumé du document.

1. **Éléments créatifs :** Dans Frame.io, remarquez la décision d’approbation globale prise pour vos ressources.

1. **Éléments créatifs :** Dans Frame.io, appliquez les modifications demandées en ajoutant la version mise à jour à la pile de versions de la ressource connectée.

1. **Coordinateurs :** Dans Workfront, affectez des approbateurs/réviseurs à la version nouvellement chargée et surveillez la progression jusqu’à ce qu’elle atteigne l’approbation.

## Scénario de test détaillé

Pour les participants qui souhaitent tester des fonctionnalités supplémentaires, nous avons créé un scénario de test plus impliqué. Un guide pour ce scénario de test détaillé peut être téléchargé ici : [Présentation du scénario de test détaillé WF + Frame.io](/help/quicksilver/product-announcements/betas/assets/MVP-WF-Frame-Detailed-Walk-Through.pdf).



## Plans de fonctionnalités

Vous trouverez ci-dessous des informations sur les principaux cas d’utilisation que nous cherchons à résoudre et sur les fonctionnalités que nous avons actuellement prévu de créer. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>Puces sous un **« Améliorations potentielles dans les prochaines versions »** selon les commentaires sur la version beta et l’évolution de nos plans de développement, l’en-tête peut être inclus ou non dans une version ultérieure.
>

### Les administrateurs Workfront peuvent configurer une connexion entre les groupes Workfront et les comptes Frame.io

* Dans Workfront, vous pouvez connecter un groupe Workfront à un compte Frame.io

* Une nouvelle équipe Frame.io sera créée dans Frame.io, représentant le groupe Workfront connecté (notez que cette fonctionnalité n&#39;a été activée que pour les clients qui utilisent l&#39;intégration en production. La connexion sera configurée par l’équipe d’Adobe pour les clients qui effectuent toujours des tests sur Sandbox ou sur Aperçu.)

**Améliorations possibles dans les prochaines versions :**

* Déconnexion d’un groupe Workfront d’un compte Frame.io

* Connecter un groupe Workfront à une équipe Frame.io existante

### Les coordinateurs de projet peuvent configurer les projets Workfront envoyés à Frame.io et faire ajouter les éléments créatifs affectés dans Workfront au projet dans Frame.io

* Possibilité de marquer les projets Workfront comme Frame.io activé en attribuant un groupe connecté à Frame

* Possibilité d’activer/désactiver des tâches dans les projets Workfront sous la forme de tâches Frame, qui à leur tour créent des dossiers de tâches dans Frame.io

* Étant donné qu’un projet Workfront se voit attribuer un groupe connecté à Frame et au moins une tâche activée pour Frame, lorsque le statut du projet Workfront est défini sur Actuel, un projet connecté correspondant est créé dans Frame, les utilisateurs affectés à Workfront sont ajoutés au projet Frame et une notification leur est envoyée par e-mail depuis Frame.io

   * Les utilisateurs et les équipes affectés aux tâches Workfront activées pour Frame seront ajoutés en tant que collaborateurs au projet Frame.io et notifiés (à la création du projet et ultérieurement)

* Les documents (résumés créatifs) ajoutés au projet et aux tâches activées pour Frame seront envoyés au projet Frame.io (dans le dossier de travail correspondant) lors de la création du projet (déclencheur : statut du projet défini sur Actuel)

   * Nous vous recommandons de limiter la quantité de documents ajoutés à votre projet avant de devenir actif uniquement dans vos briefs créatifs, afin d’éviter d’envoyer plusieurs documents inutiles à Frame.io

   * Les documents/tâches ajoutés après la synchronisation initiale du projet ne seront pas envoyés à Frame.io, mais uniquement les utilisateurs/équipes

**Améliorations possibles dans les prochaines versions :**

* Les tâches avec prise en charge des cadres peuvent être configurées sur des modèles de projet

* Les chargements de la nouvelle version vers les briefs créatifs seront envoyés à Frame.

* Synchronisation de projet optimisée (déconnexion de projets, resynchronisation de projets et de documents, etc.)

### Dans Frame.io, les créatifs peuvent envoyer des ressources créées au projet Workfront pour révision formelle

* Possibilité de connecter une ressource Frame.io unique à un projet ou une tâche WF. Une référence de ressource sera créée dans Workfront.

* Les chargements de nouvelle version dans Frame.io créent automatiquement une nouvelle version du document dans Workfront sur les ressources connectées

* Possibilité de marquer les tâches Workfront référencées comme terminées dans Frame.io

* Si le document Workfront connecté est supprimé, il reste dans Frame.io et peut être reconnecté à la même tâche de projet ou à une autre

**Améliorations possibles dans les prochaines versions :**

* Possibilité d’envoyer plusieurs ressources Frame.io à Workfront en même temps

* Journalisation du temps par rapport au projet/à la tâche Workfront depuis Frame.io

### Les coordinateurs de projet peuvent affecter le processus d&#39;approbation officiel aux documents liés depuis Frame.io

* Les utilisateurs et les équipes Workfront peuvent être ajoutés aux nouvelles approbations de documents pour les documents connectés Frame.io

* Lorsque le partage d’un utilisateur/d’une équipe est annulé à partir d’un document activé pour Frame, ils perdent également leur accès à la ressource dans la visionneuse Frame.io

**Améliorations possibles dans les prochaines versions :**

* Envoi de plusieurs ressources en tant que révision unique

* Affectation en bloc d’approbateurs/réviseurs à des documents Workfront

### Les parties prenantes peuvent effectuer leur révision et leur approbation dans la visionneuse Frame.io

* Les parties prenantes seront averties et pourront afficher le document connecté Frame dans la visionneuse Frame.io

* La visionneuse Frame.io est accessible à partir de différents emplacements dans Workfront, par exemple la liste des documents, les détails des documents, la page d’accueil Workfront

* Possibilité d&#39;exploiter les fonctionnalités de révision et de commentaire existantes fournies par la visionneuse Frame.io qui sera synchronisée avec le flux de mise à jour de Workfront

* Possibilité de prendre une nouvelle décision d’approbation de document à partir de la visionneuse Frame.io
