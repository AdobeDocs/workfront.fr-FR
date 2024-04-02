---
product-area: documents
navigation-topic: approvals
title: Présentation de l’examen et de l’approbation des ressources
description: En savoir plus sur le processus de révision et d’approbation formelles dans Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 63160895fc77994fdecd7aca8769b7d236d285d6
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# Présentation de l’examen et de l’approbation des ressources

Le nouveau workflow d’approbation et de révision des ressources repose sur une intégration étroite entre Workfront et Frame.io. Cette intégration tire le meilleur parti de ce que chaque produit a à offrir et l’associe pour créer une expérience qui permet à toutes les personnes impliquées dans la création de contenu de fonctionner dans leurs outils de choix, tout en ayant accès aux commentaires, aux fichiers et aux mises à jour d’état synchronisés en temps réel sur les deux systèmes.

<!-- link to frame docs-->

## Lancement et planification du travail dans Workfront

Le coordinateur de projet commence dans Workfront. Le projet est créé, des tâches sont affectées, des instructions sont envoyées.

Le coordinateur de projet crée un projet WF, utilise le dossier du projet synchronisé pour envoyer des informations et du matériel de support aux créatifs dans Frame.io.

Configurer le workflow de validation à partir de zéro ou via des modèles

Affecter des tâches

Définit le projet sur Actuel ou égal à pour créer un projet cadre et alerter les créatifs

### Configuration d’un compte Frame.io par défaut

Les administrateurs Workfront déclenchent l’intégration de Workfront et de Frame.io en ajoutant un compte Frame.io par défaut dans la zone Configuration de Workfront. Une fois qu’un compte Frame.io par défaut est configuré, l’intégration permet de créer des projets connectés entre Workfront et Frame.io.

Pour plus d’informations, voir [].


<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->


### Activation de Frame.io

Les utilisateurs de Workfront qui utilisent régulièrement Frame.io doivent être marqués comme des utilisateurs de Frame.io. Les administrateurs de Workfront peuvent désigner des utilisateurs de Frame.io dans le profil utilisateur de Workfront.

Lorsqu’un utilisateur est marqué comme utilisateur Frame.io dans Workfront et est ajouté à un projet :

* Ils sont ajoutés en tant que collaborateur dans Frame.io
* Ils peuvent envoyer des ressources de Frame.io à Workfront pour révision et approbation formelles.

Pour plus d’informations, voir [].

![](assets/Frame-enabled-user.png)

>[!TIP]
>
>Nous recommandons d’activer les utilisateurs qui travaillent régulièrement dans des outils de création et de charger des ressources pour révision et approbation en tant qu’utilisateurs de Frame.io.

### Création d’un projet connecté à Frame.io

Les coordinateurs de projets peuvent créer des projets Workfront connectés à Frame.io. Lorsque vous créez un projet connecté, vous pouvez :

* **Affecter des utilisateurs de Frame.io à des tâches**: les utilisateurs activés pour Frame.io sont avertis par e-mail lorsqu’ils sont affectés à une tâche qui leur signale qu’il reste du travail à accomplir.
* **Partage du projet avec les utilisateurs de Frame.io**: les projets partagés avec les utilisateurs activés pour Frame.io leur donnent accès au projet dans Frame.io.
* **Partage de contenu créatif avec Frame.io**: vous pouvez envoyer des instructions et du matériel de Workfront directement à l’utilisateur créatif de Frame.io à l’aide d’un dossier de projet de synchronisation unidirectionnel.
* **Suivi de la progression de la tâche**: les créatifs peuvent envoyer des ressources terminées et marquer les tâches terminées sans quitter Frame.io.

Pour plus d’informations, voir [].

<!--Preassign approval templates to asks coming in the future-->


## Création et collaboration de contenu dans Frame.io

Les créatifs peuvent rester dans leurs outils de choix et avoir la liberté de créer, d&#39;itérer et d&#39;effectuer des critiques par les pairs dans Frame.io.

Lorsqu’un élément créatif est ajouté à un projet intégré, il peut effectuer toutes les opérations suivantes sans quitter Frame.io :

* Accès aux instructions du coordinateur de projet
* Réaliser des examens par les pairs informels
* Envoi de ressources terminées à Workfront pour révision et approbation formelles
* Modifier l’état d’une tâche ou la marquer comme terminée
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->


## Révision et approbation de ressources dans Workfront

Une fois qu’un créatif envoie une ressource terminée à Workfront à partir de Frame.io, le coordinateur de projet peut lancer le processus de révision et d’approbation formel dans Workfront. Toutes les activités de révision et d’approbation sont enregistrées dans Workfront.

Tous les commentaires effectués dans Frame.io sont également pris en compte dans l’onglet Mises à jour de Workfront. Les réponses effectuées dans Workfront ne sont pas reflétées dans Frame.io.

Les commentaires marqués Équipe n’apparaîtront pas que dans l’onglet Mises à jour Workfront .

### Lancer des révisions et des approbations officielles

Vous pouvez créer une révision et des validations uniques, ou créer des modèles d’approbation fiables dans la zone Configuration du front de travail :

Vous avez la possibilité d’affecter des réviseurs, des approbateurs ou un mélange des deux :

* **Réviseurs** peuvent ajouter des commentaires et des balises aux ressources. Une fois la révision terminée, ils peuvent la marquer comme terminée. <!--example of when to add reviewers-->
* **Approbateurs** Peut commenter, marquer les ressources et doit prendre une décision pour faire avancer le processus d’approbation.

Les validants et les approbateurs peuvent être ajoutés à des modèles à usage unique ou de validation :

<!--can also assign teams and set deadline-->

* **Validations à usage unique**: définissez les délais de validation

* **Modèles de validation**
Dans la zone Configuration de Workfront , les utilisateurs disposant d’une licence Standard peuvent créer des modèles d’approbation réutilisables. Dans un modèle, les utilisateurs peuvent spécifier une période et ajouter des réviseurs et des approbateurs. <!--do we want to mention any upcoming plans here? -->

  Une fois créé, un modèle peut être appliqué aux ressources envoyées à partir de Frame.io pour lancer le processus de révision et d’approbation formel dans Workfront.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

### Notifications de révision et d’approbation

Combiner avec d’autres sections ?

Accueil en attente de mon widget d’approbation Courrier électronique - délai 72, 24, et à l’échéance.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Révision et approbation des ressources

Les parties prenantes de ressources connectées à Frame.io peuvent examiner et approuver dans la visionneuse de cadres avec la synchronisation des commentaires dans le flux de mise à jour du front de travail, les décisions, etc.

<!-- include screenshot from frame.io-->

Les utilisateurs de flux de travail externe devront créer une connexion pour le cadre.

Si la ressource n’est pas connectée au cadre, ils peuvent afficher la miniature dans WF et utiliser le flux de commentaires. des décisions de révision et d’approbation peuvent être prises.

### Suivi des mesures de révision et d’approbation

Widget dans le rapport vitesse de validation à domicile

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


* Transférez une ressource à partir de Workfront et envoyez-la au cadre de révision et d’approbation - Bientôt disponible ?

## Exemple de workflow d’approbation de ressource de campagne

intro para ?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->