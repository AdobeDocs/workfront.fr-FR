---
product-area: projects
navigation-topic: approvals
title: Connexion à Workfront et Frame.io
description: Workfront utilise Frame.io dans le processus de révision et d’approbation pour rencontrer les personnes qui souhaitent travailler. Le processus de gestion et d’approbation de projet est géré dans Workfront et la révision est effectuée dans Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: f50d102eb9c44abb9780c378c41c108b124077c4
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---


# Connexion à Workfront et Frame.io

Workfront utilise Frame.io dans le processus de révision et d’approbation pour rencontrer les personnes qui souhaitent travailler. Le processus de gestion et d’approbation de projet est géré dans Workfront et la révision est effectuée dans Frame.io. Pour configurer l’intégration, vous devez suivre toutes les sections suivantes :

* [Connexion d’un groupe Workfront à une équipe Frame.io](#connect-a-workfront-group-to-a-frameio-team)
* [Création d’un projet Workfront et ajout d’un groupe connecté](#create-a-workfront-project-and-add-a-connected-group)

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus de validation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Exigences d’accès

* Votre entreprise doit être intégrée manuellement pour utiliser les fonctionnalités décrites dans cet article. Pour plus d’informations, voir [alpha de l’intégration native Adobe Workfront et Frame.io : présentation](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


## Connexion d’un groupe Workfront à une équipe Frame.io

Nous améliorons activement cette fonctionnalité pour une disponibilité générale en mai.

### Conditions préalables

* Créez une équipe Frame.io à mapper à un groupe Workfront.
* Recherchez le jeton de développement de l’API pour l’équipe. Pour plus d’informations, voir [Jetons de développement](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) sur le site de développement de Frame.io.

### Connexion d’un groupe Workfront à une équipe Frame.io

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Sélectionnez un groupe existant ou cliquez sur **Créer un groupe**.
1. Dans le panneau de gauche, cliquez sur **Connexion à Frame.io**.
   ![](assets/connect-frame-group.png)
1. Saisissez le jeton développeur de l’API.
1. Cliquez sur **Lancer la connexion**.
1. (Conditionnel) Sélectionnez un compte Frame.io.

## Création d’un projet Workfront et ajout d’un groupe connecté

Une fois que vous avez connecté un groupe Workfront à une équipe Frame.io, vous devez créer un projet avec ce groupe connecté.

### Conditions préalables

* Un groupe Workfront doit être connecté à une équipe Frame.io, comme expliqué dans la section précédente.

### Création d’un projet Workfront et ajout d’un groupe connecté

{{step1-to-projects}}

1. Créez un projet à partir de zéro ou un modèle. Pour plus d’informations sur la création d’un projet, voir [Création d’un projet](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. Dans le panneau de gauche, recherchez **Détails du projet**.

1. Recherchez le **Groupe** sur le côté droit de l’écran, puis supprimez le groupe Par défaut .

1. Dans le menu déroulant, recherchez le groupe souhaité. Les groupes connectés à Frame.io affichent l’icône Frame.io.
   ![](assets/add-frame-group.png)

1. Apportez toute autre modification de configuration de projet.

1. Cliquez sur **Enregistrer les modifications**.

1. Passez à la section suivante.

### Ajouter une tâche et définir l’état d’intégration sur Actif

>[!NOTE]
>
>Les sous-tâches ne sont actuellement pas prises en charge.


1. Créez les tâches à remplir dans Frame.io.

1. Sélectionnez les tâches nécessaires, puis cliquez sur **Modifier**.

1. Faites défiler l’écran jusqu’à **Forms personnalisée** et recherchez le formulaire d’intégration Frame.io.

   >[!IMPORTANT]
   >
   >Vous devez ajouter le groupe connecté à Frame.io pour afficher ce formulaire personnalisé sur les tâches.

1. Activez la case à cocher, puis sélectionnez **Actif**.
   ![](assets/frame-custom-form.png)

1. Cliquez sur **Enregistrer les modifications**. Une icône Frame.io s’affiche en regard du nom du projet.

1. Affectez des utilisateurs ou des équipes à des tâches.

   >[!NOTE]
   >
   >Les utilisateurs ou équipes ajoutés aux tâches sont également ajoutés au projet Frame.io.

1. Chargez des documents ou des avis créatifs dans la zone Documents du projet .

Le projet n’est toujours pas connecté. Vous devez passer à la section suivante pour terminer l’intégration.

### Activation du projet dans Frame.io

1. Modifiez l’état à partir de **Planification** to **Actuel** ou un état personnalisé égal à actuel. Cela termine l’intégration et génère le projet, les tâches et tous les documents dans Frame.io.

L’icône Frame.io en regard du nom du projet devient violette pour signaler que l’intégration a réussi. Les utilisateurs reçoivent un e-mail les invitant au projet Frame.io.