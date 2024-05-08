---
product-area: documents
navigation-topic: approvals
title: Programme bêta - Workfront + Frame.io
description: Nous sommes ravis d’annoncer le lancement de notre programme bêta pour Workfront + Frame.io. Vous trouverez ici des informations sur la dernière version bêta, ainsi qu’une brève présentation vidéo pour commencer.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 23d1e241-ea5b-43f5-b097-8d96e13cb267
source-git-commit: 2ea9316e8cbe4474f22028f85204f9351182ba06
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Programme bêta - Workfront + Frame.io

Bienvenue dans le programme bêta d’intégration de Workfront + Frame.io ! Dans le cadre de cette version bêta, vous accéderez rapidement à notre expérience d’intégration native de Workfront + Frame.io et serez en mesure de partager vos commentaires qui définiront en fin de compte l’expérience finale que nous publierons sur notre base de clients élargie. Avec cette intégration, nous visons à créer un processus de bout en bout sans heurts entre Workfront et Frame.io, en mettant l’accent sur une solution idéale, unifiée de révision et d’approbation.

Vous trouverez ici des informations sur la dernière version bêta, ainsi qu’une brève présentation vidéo pour commencer.

>[!NOTE]
>
>Pour participer à cette version bêta, vous devez être activé par l’équipe produit. Contactez votre gestionnaire de compte ou votre service client pour demander à être ajouté.


## Mises à jour de la version bêta de Frame.io - Mars 2024

Dans cette version bêta, nous avons :

### Ajout de plusieurs ressources de Frame.io à Workfront

Vous pouvez désormais ajouter jusqu’à 10 ressources de Frame.io à Workfront à la fois. Vous pouvez choisir d’ajouter des documents au projet Workfront ou à une tâche de projet spécifique.

### Expérience améliorée lors de l’ajout d’une ressource Frame.io à Workfront

Les éléments de menu permettant d’ajouter une ressource à Workfront ont été mis à jour afin de faciliter l’affichage des tâches qui vous sont affectées, de la hiérarchie des tâches et de l’état des tâches.

>[!VIDEO](https://video.tv.adobe.com/v/3428213/)

## Mises à jour de la version bêta dans Workfront - Mars 2024

Dans cette version bêta, nous avons :

### Ajout d’une date limite aux révisions et validations de documents

Vous pouvez maintenant spécifier une échéance pour les utilisateurs ou les équipes affectés à la révision ou à l’approbation d’un document. Les réviseurs et les approbateurs reçoivent des notifications par e-mail 72 heures, puis 24 heures avant la date limite spécifiée. L’échéance est également répercutée dans le widget Validations de la nouvelle zone d’accueil.

Pour plus d’informations, voir [Créer une demande d’approbation ou de révision de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

### Créer et utiliser des modèles d’approbation

Vous pouvez maintenant créer des modèles d’approbation dans la zone Configuration afin de rationaliser le processus de révision et d’approbation. Les modèles d’approbation vous permettent de rendre le processus de révision et d’approbation plus répétable en

* Ajouter des validants et des approbateurs
* Définition d’une période

Vous pouvez appliquer des modèles d’approbation à partir de la zone Documents lors de la création d’un processus d’approbation pour un document.

Pour plus d’informations, voir [Création d’un modèle d’approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

### Afficher les informations sur toutes vos validations en une seule fois

Pour vous aider à gérer et analyser vos demandes d’approbation en un coup d’oeil, nous avons ajouté les indicateurs de performances clés suivants au widget Toutes les approbations :

* Approbations par décision
* Temps moyen d’approbation
* Approbations en attente
* Approbations en retard

Vous pouvez accéder aux catégories répertoriées ci-dessus pour obtenir une vue plus détaillée. Le widget Toutes les approbations est disponible dans Tableaux de bord Accueil et Zone de travail .

Pour plus d’informations, voir [Prise en main du nouvel accueil](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

### Verrouillez vos révisions et approbations une fois qu’une décision globale est prise

Pour garantir la conformité et réduire l’attrition de vos processus d’approbation de contenu, nous verrouillons désormais toute approbation sur un fichier une fois qu’une décision globale a été prise. Cela inclut le travail Approuvé, Approuvé avec des modifications ou Nécessite un travail.

Une fois verrouillé, toute personne effectuant une révision ou une approbation ne pourra plus faire de commentaires, de réponses, de décisions ou ajouter des balises de dessin, ce qui garantit que votre processus de révision et l’audit associé restent inchangés.

Lorsqu’une nouvelle version de document est téléchargée, le cycle de révision suivant peut être déclenché tout en maintenant verrouillées les révisions précédentes.

>[!VIDEO](https://video.tv.adobe.com/v/3428179/)

## Test des fonctionnalités

Avec cette intégration, notre objectif est de permettre aux créatifs de rester dans leur outil de choix (CC ou Frame.io) pour créer leur contenu et réaliser des révisions par les pairs, tout en ayant des chefs de projet pour coordonner le travail et initialiser et suivre le processus de révision formel depuis Workfront. Pour ce faire, vous pouvez utiliser les deux meilleures solutions : Workfront de nouvelles validations de document pour la gestion des validations de contenu, ainsi que les fonctionnalités d’examen de contenu proposées par Frame.io. Collectivement, les nouveaux documents approuvés et Frame.io formeront notre nouvelle expérience de révision et d’approbation de contenu de bout en bout. 

Pour vous permettre de tester facilement les nouvelles fonctionnalités du programme bêta, nous avons créé un nouveau compte de test Frame.io et nous l’avons connecté à un nouveau groupe appelé `Frame.io testing` dans votre environnement Workfront Preview ou Sandbox existant.

+++Développer pour afficher les instructions de test vasculaire

Pour tester la fonctionnalité, connectez-vous à votre instance Workfront Preview ou Sandbox et procédez comme suit :

1. **Coordonnateurs :** Dans Workfront, créez un projet avec le `Frame.io testing` groupe affecté en tant que groupe de projet.

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

+++

+++ Développer pour afficher des instructions de test détaillées

Pour les participants qui souhaitent tester des fonctionnalités supplémentaires, nous avons créé un scénario de test plus impliqué. Un guide pour ce scénario de test détaillé peut être téléchargé ici : [Présentation détaillée du scénario de test détaillé WF + Frame.io](/help/quicksilver/review-and-approve-work/Documents/assets/wf-frame-detailed-walk-through-may-release.pdf).
+++

<!-- 
## Demo Video

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)
-->

## Envoyer un commentaire

Nous apprécions votre contribution et pensons que votre point de vue est essentiel pour nous aider à créer le meilleur produit possible.

Comme vous avez des commentaires spécifiques sur ce qui serait nécessaire pour que votre entreprise adopte cette solution en production, envoyez-la à [etienneb@adobe.com](mailto:etienneb@adobe.com).
