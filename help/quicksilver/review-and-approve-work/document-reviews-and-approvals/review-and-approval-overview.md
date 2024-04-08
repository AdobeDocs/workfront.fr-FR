---
product-area: documents
navigation-topic: approvals
title: Aperçu de la révision et de l’approbation des ressources
description: En savoir plus sur le processus de révision et d’approbation formel dans Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 959bd3cab0de8b76c94fad1be5b6b2b8b7ae904b
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Aperçu de la révision et de l’approbation des ressources

Le nouveau workflow de révision et d’approbation des ressources s’articule autour d’une étroite intégration entre Workfront et Frame.io. Cette intégration tire le meilleur parti de ce que chaque produit a à offrir et les combine pour créer une expérience qui permet à toutes les personnes impliquées dans la création de contenu de travailler dans les outils de leur choix, tout en ayant accès aux commentaires, aux fichiers et aux mises à jour de statut synchronisés sur les deux systèmes en temps réel.

Pour plus d&#39;informations sur Frame.io, voir [Prise en main de Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Initiation et planification du travail dans Workfront

L’administrateur Workfront permet l’intégration entre Workfront et Frame.io en configurant le compte Frame.io par défaut dans la zone Configuration , puis en désignant les utilisateurs Frame.io dans Workfront. Cela permet au coordinateur de planifier et de lancer le travail à l’aide des projets Workfront et des workflows de révision et d’approbation officiels.

### Configuration d’un compte Frame.io par défaut

Les administrateurs Workfront lancent l’intégration de Workfront et Frame.io en ajoutant un compte Frame.io par défaut dans la zone Configuration de Workfront. Une fois qu’un compte Frame.io par défaut est configuré, un projet miroir est créé dans Frame.io pour tous les projets créés dans Workfront.

Pour plus d’informations, voir [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Activer les utilisateurs Frame.io

Les utilisateurs de Workfront qui utilisent régulièrement Frame.io doivent être marqués comme utilisateurs Frame.io. Les administrateurs Workfront peuvent désigner des utilisateurs Frame.io dans le profil utilisateur Workfront.

Lorsqu’un utilisateur est marqué comme utilisateur Frame.io dans Workfront et est ajouté à un projet,

* Ils sont ajoutés en tant que collaborateur dans Frame.io
* Ils peuvent envoyer des ressources de Frame.io vers Workfront pour révision et approbation officielles
* Ils peuvent afficher des informations dans le dossier de synchronisation unidirectionnelle à partir de Workfront

>[!TIP]
>
>Nous vous recommandons d’activer les utilisateurs qui travaillent régulièrement dans des outils de création et qui chargent des ressources pour révision et approbation en tant qu’utilisateurs Frame.io.

Pour plus d’informations, voir [].

![](assets/Frame-enabled-user.png)


### Créer un projet connecté avec Frame.io

Une fois le compte Frame.io par défaut ajouté et les utilisateurs Frame.io désignés, les coordinateurs de projet peuvent créer des projets Workfront connectés à Frame.io. Lorsque vous créez un projet connecté, vous pouvez :

* **Affectation d’utilisateurs Frame.io à des tâches**: les utilisateurs activés pour Frame.io sont avertis par e-mail lorsqu’ils sont affectés à une tâche, ce qui signale qu’il reste du travail à accomplir.
* **Partager le projet avec des utilisateurs Frame.io**: les projets partagés avec les utilisateurs compatibles avec Frame.io leur accordent l’accès au projet dans Frame.io.
* **Partage de contenu créatif avec Frame.io**: vous pouvez envoyer des instructions et des ressources de Workfront directement à l’utilisateur créatif dans Frame.io à l’aide d’un dossier de projet de synchronisation unidirectionnelle.
* **Suivre la progression de la tâche**: les créatifs peuvent envoyer des ressources terminées et marquer les tâches comme terminées sans quitter Frame.io.

Pour plus d’informations, voir [].

<!--Preassign approval templates to tasks coming in the future-->


## Création de contenu et collaboration dans Frame.io

Les créatifs peuvent rester dans les outils de leur choix et avoir la liberté de créer, d&#39;itérer et de mener des évaluations par les pairs dans Frame.io.

Lorsqu’un élément créatif est ajouté à un projet connecté, il peut effectuer les opérations suivantes sans quitter Frame.io :

* Accès aux instructions du coordinateur de projet
* Mener des examens informels par les pairs
* Envoi des ressources terminées à Workfront pour révision et approbation officielles
* Modifier le statut d’une tâche ou la marquer comme terminée
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Pour plus d’informations sur la révision des ressources dans Frame.io, voir

## Révision et approbation des ressources

Une fois qu’un élément créatif envoie une ressource terminée à Workfront à partir de Frame.io, le coordinateur du projet peut lancer le processus de révision et d’approbation formel dans Workfront.

Une fois l’approbation créée, les utilisateurs reviennent sur Frame.io pour ajouter des commentaires sur la ressource et la marquer. Il peut également prendre une décision d’approbation dans la visionneuse Frame.io.

### Lancement des révisions et des approbations formelles dans Workfront

Les coordinateurs de projet peuvent créer des révisions et des approbations ponctuelles ou des modèles d’approbation réutilisables dans la zone Configuration de Workfront. Toutes les activités de révision et d’approbation effectuées dans Frame.io sont également enregistrées dans Workfront.

#### Ajout de réviseurs et d’approbateurs

Les coordinateurs de projet ont la possibilité d’affecter des réviseurs et/ou des approbateurs :

* **Reviewers** peut ajouter des commentaires sur les ressources et les marquer. Une fois l’opération terminée, ils peuvent marquer leur révision comme terminée. <!--example of when to add reviewers-->
* **Approbateurs** peut ajouter des commentaires sur les ressources et les marquer. Ils doivent prendre la décision de faire avancer le processus d&#39;approbation.


#### Création d’un workflow de révision et d’approbation

Les réviseurs et approbateurs peuvent être ajoutés à un workflow d’approbation à usage unique ou à un modèle d’approbation :

<!--can also assign teams and set deadline-->
E-mail : les e-mails d’échéance 72, 24 et à l’échéance.

* **Validations à usage unique**: définition des dates limites de validation

* **Modèles de validation**
Dans la zone Configuration de Workfront , les utilisateurs disposant d’une licence Standard peuvent créer des modèles d’approbation réutilisables. Dans un modèle, les utilisateurs peuvent spécifier une période et ajouter des réviseurs et des approbateurs. <!--do we want to mention any upcoming plans here? -->

  Une fois qu’un modèle est créé, il peut être appliqué aux ressources envoyées à partir de Frame.io pour lancer le processus de révision et d’approbation formel dans Workfront.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Charger une ressource depuis Workfront et l’envoyer vers frame pour révision et approbation - Bientôt disponible ?

### Approbation de ressources dans Frame.io

Les parties prenantes peuvent examiner et approuver les ressources connectées avec la visionneuse Frame.io.

#### Accès à la visionneuse Frame.io

Les utilisateurs peuvent accéder à la visionneuse Frame.io des manières suivantes :

* Le widget En attente de mon approbation dans la nouvelle zone d’accueil de Workfront
* Notifications par e-mail Workfront.

Les utilisateurs Workfront externes seront invités à créer une connexion Frame.io pour examiner et approuver les ressources.

#### Commentaire et balisage des ressources

Tous les commentaires ajoutés dans la visionneuse Frame.io sont également enregistrés dans l’onglet Mise à jour de Workfront . Les réponses effectuées dans Workfront n&#39;apparaissent pas dans Frame.io. Les commentaires marqués Équipe uniquement n’apparaîtront pas dans l’onglet Mises à jour de Workfront .

#### Prendre une décision

Les approbateurs doivent prendre l&#39;une des décisions suivantes :

* Approuver : ce(tte)
* Approuver avec des modifications
* Travail nécessaire

Les réviseurs peuvent marquer leur révision comme terminée dans les visionneuses Frame.io.

<!-- include screenshot from frame.io-->



<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Suivi des mesures de révision et d’approbation

Widgets dans l’accueil Rapport sur la vitesse d’approbation ?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Exemple de workflow de validation de ressources de campagne

intro para ?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
