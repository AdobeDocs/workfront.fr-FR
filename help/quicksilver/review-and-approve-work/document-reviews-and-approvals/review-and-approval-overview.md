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
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 7e970f4f707937a62f68c191a7cbd5dfa26e471c
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Présentation de l’examen et de l’approbation des ressources

Le nouveau workflow d’approbation et de révision des ressources repose sur une intégration étroite entre Workfront et Frame.io. Cette intégration tire le meilleur parti de ce que chaque produit a à offrir et l’associe pour créer une expérience qui permet à toutes les personnes impliquées dans la création de contenu de fonctionner dans leurs outils de choix, tout en ayant accès aux commentaires, aux fichiers et aux mises à jour d’état synchronisés en temps réel sur les deux systèmes.

Pour plus d’informations sur Frame.io, voir [Prise en main de Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Lancement et planification du travail dans Workfront

L’administrateur de Workfront active l’intégration entre Workfront et Frame.io en configurant le compte Frame.io par défaut dans la zone Configuration, puis en désignant les utilisateurs de Frame.io dans Workfront. Cela permet au coordinateur de planifier et de lancer des travaux à l’aide de projets Workfront, ainsi que de procéder à une révision et à une approbation officielles.

### Configuration d’un compte Frame.io par défaut

Les administrateurs de Workfront lancent l’intégration de Workfront et de Frame.io en ajoutant un compte Frame.io par défaut dans la zone Configuration de Workfront. Une fois qu’un compte Frame.io par défaut est configuré, l’intégration crée des projets connectés entre Workfront et Frame.io.

Pour plus d’informations, voir [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Activation de Frame.io

Les utilisateurs de Workfront qui utilisent régulièrement Frame.io doivent être marqués comme des utilisateurs de Frame.io. Les administrateurs de Workfront peuvent désigner des utilisateurs de Frame.io dans le profil utilisateur de Workfront.

Lorsqu’un utilisateur est marqué comme utilisateur de Frame.io dans Workfront et est ajouté à un projet,

* Ils sont ajoutés en tant que collaborateur dans Frame.io
* Ils peuvent envoyer des ressources de Frame.io à Workfront pour révision et approbation formelles.

>[!TIP]
>
>Nous recommandons d’activer les utilisateurs qui travaillent régulièrement dans des outils de création et de charger des ressources pour révision et approbation en tant qu’utilisateurs de Frame.io.


Pour plus d’informations, voir [].

![](assets/Frame-enabled-user.png)


### Création d’un projet connecté à Frame.io

Une fois que le compte Frame.io par défaut est ajouté et que les utilisateurs de Frame.io sont désignés, les coordinateurs de projet peuvent créer des projets Workfront connectés à Frame.io. Lorsque vous créez un projet connecté, vous pouvez :

* **Affecter des utilisateurs de Frame.io à des tâches**: les utilisateurs activés pour Frame.io sont avertis par e-mail lorsqu’ils sont affectés à une tâche, ce qui indique qu’il reste du travail à accomplir.
* **Partage du projet avec les utilisateurs de Frame.io**: les projets partagés avec les utilisateurs activés pour Frame.io leur donnent accès au projet dans Frame.io.
* **Partage de contenu créatif avec Frame.io**: vous pouvez envoyer des instructions et du matériel de Workfront directement à l’utilisateur créatif de Frame.io à l’aide d’un dossier de projet de synchronisation unidirectionnel.
* **Suivi de la progression de la tâche**: les créatifs peuvent envoyer des ressources terminées et marquer les tâches terminées sans quitter Frame.io.

Pour plus d’informations, voir [].

<!--Preassign approval templates to tasks coming in the future-->


## Création et collaboration de contenu dans Frame.io

Les créatifs peuvent rester dans leurs outils de choix et avoir la liberté de créer, d&#39;itérer et d&#39;effectuer des critiques par les pairs sur Frame.io.

Lorsqu’un élément créatif est ajouté à un projet connecté, il peut effectuer les opérations suivantes sans quitter Frame.io :

* Accès aux instructions du coordinateur de projet
* Réaliser des examens par les pairs informels
* Envoi de ressources terminées à Workfront pour révision et approbation formelles
* Modifier l’état d’une tâche ou la marquer comme terminée
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Pour plus d’informations sur la révision des ressources dans Frame.io, voir

## Révision et approbation de ressources

Une fois qu’un créatif envoie une ressource terminée à Workfront à partir de Frame.io, le coordinateur de projet peut lancer le processus de révision et d’approbation formel dans Workfront.

Une fois l’approbation créée, les utilisateurs reviennent sur Frame.io pour commenter et marquer la ressource. Ils peuvent également prendre une décision concernant l’approbation dans la visionneuse Frame.io.

### Lancer des révisions et des approbations formelles dans Workfront

Les coordinateurs de projet peuvent créer une révision et des approbations uniques ou des modèles d’approbation réutilisables dans la zone Configuration de Workfront. Toutes les activités de révision et d’approbation effectuées dans Frame.io sont également enregistrées dans Workfront.

Les coordinateurs de projet ont la possibilité d’affecter des réviseurs, des approbateurs ou une combinaison des deux :

* **Réviseurs** Vous pouvez ajouter des commentaires aux ressources et les marquer. Une fois la révision terminée, ils peuvent la marquer comme terminée. <!--example of when to add reviewers-->
* **Approbateurs** peut ajouter des commentaires sur les ressources de balisage. Ils doivent prendre la décision de faire avancer le processus d’approbation.



Tous les commentaires effectués dans Frame.io sont pris en compte dans l’onglet Mises à jour de Workfront. Les réponses effectuées dans Workfront ne sont pas reflétées dans Frame.io.

Les commentaires marqués Équipe n’apparaîtront pas que dans l’onglet Mises à jour Workfront .

Les validants et les approbateurs peuvent être ajoutés à des modèles à usage unique ou de validation :

<!--can also assign teams and set deadline-->

* **Validations à usage unique**: définissez les délais de validation

* **Modèles de validation**
Dans la zone Configuration de Workfront , les utilisateurs disposant d’une licence Standard peuvent créer des modèles d’approbation réutilisables. Dans un modèle, les utilisateurs peuvent spécifier une période et ajouter des réviseurs et des approbateurs. <!--do we want to mention any upcoming plans here? -->

  Une fois créé, un modèle peut être appliqué aux ressources envoyées à partir de Frame.io pour lancer le processus de révision et d’approbation formel dans Workfront.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Transférez une ressource à partir de Workfront et envoyez-la au cadre de révision et d’approbation - Bientôt disponible ?

### Approbation des ressources dans Frame.io

Les parties prenantes connectées à Frame.io peuvent examiner et approuver dans la visionneuse Frame.io les commentaires synchronisés avec le flux de mise à jour Workfront, les décisions, etc.

<!-- include screenshot from frame.io-->

Si vous travaillez exclusivement dans Frame, vous pouvez être averti d’une demande par e-mail.

Si vous travaillez exclusivement dans Workfront, vous pouvez utiliser le widget d’approbation à la maison.

vous pouvez accéder à la visionneuse Frame.io dès que vous travaillez

**Approbation de ressources à partir de Frame.io**
comment ils sont avertis

prendre une décision : approuver, approuver avec des modifications, nécessite du travail

**Approbation de ressources à partir de Workfront**
comment ils sont avertis

Accueil en attente de mon widget d’approbation

Email : emails d’échéance 72, 24 et date limite.

Les utilisateurs de flux de travail externe devront créer une connexion pour le cadre.

Si la ressource n’est pas connectée au cadre, ils peuvent afficher la miniature dans WF et utiliser le flux de commentaires. Des décisions d’examen et d’approbation peuvent être prises.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Suivi des mesures de révision et d’approbation

Widgets du rapport Vitesse de validation à domicile ?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Exemple de workflow d’approbation de ressource de campagne

intro para ?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
