---
product-area: documents
navigation-topic: approvals
title: Prise en main de la révision et de l’approbation des ressources avec Frame.io
description: En savoir plus sur le processus de révision et d’approbation formel dans Utilisation de Workfront et Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 1%

---

# Prise en main de la révision et de l’approbation des ressources avec Frame.io

Le nouveau workflow de révision et d’approbation des ressources repose sur une intégration étroite entre Workfront et Frame.io. Cette intégration tire le meilleur parti de ce que chaque produit a à offrir et les combine pour créer une expérience qui permet à toutes les personnes impliquées dans la création de contenu de travailler dans les outils de leur choix, tout en ayant accès aux commentaires, fichiers et mises à jour de statut, le tout synchronisé sur les deux systèmes en temps réel.

Pour plus d&#39;informations sur Frame.io, voir [Prise en main de Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Initiation et planification du travail dans Workfront

L’administrateur Workfront permet l’intégration entre Workfront et Frame.io en configurant le compte Frame.io par défaut dans la zone Configuration , puis en désignant les utilisateurs Frame.io dans Workfront. Cela permet au coordinateur de planifier et de lancer le travail à l’aide des projets Workfront et des workflows de révision et d’approbation officiels.

### Configuration du compte Frame.io par défaut [!BADGE bientôt disponible]{type=Informative}

Les administrateurs de Workfront lancent l’intégration de Workfront et de Frame.io en ajoutant un compte Frame.io par défaut dans la zone Configuration de Workfront. Une fois le compte Frame.io par défaut configuré, un projet miroir est créé dans Frame.io pour tous les projets créés dans Workfront.

>[!IMPORTANT]
>
>Cette fonctionnalité sera bientôt disponible. Pour l’instant, les comptes Frame.io sont ajoutés manuellement par l’équipe Workfront. Contactez votre représentant de compte Adobe pour obtenir de l’aide.

<!--For more information, see [Configure the [!DNL Workfront] and [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

 in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Activer les utilisateurs Frame.io disponibles maintenant

Les utilisateurs de Workfront qui utilisent régulièrement Frame.io doivent être marqués comme des utilisateurs Frame.io. Les administrateurs Workfront peuvent désigner des utilisateurs Frame.io dans le profil utilisateur de Workfront.

>[!TIP]
>
>Nous vous recommandons d’activer les utilisateurs qui travaillent régulièrement dans des outils de création et qui chargent des ressources pour révision et approbation en tant qu’utilisateurs Frame.io.

Lorsqu’un utilisateur est marqué comme utilisateur Frame.io dans Workfront et est ajouté à un projet :

* Ils sont ajoutés en tant que collaborateur dans Frame.io.
* Ils peuvent envoyer des ressources de Frame.io vers Workfront pour révision et approbation officielles.
* Ils peuvent afficher des informations dans le dossier de synchronisation unidirectionnelle à partir de Workfront. [!BADGE Bientôt disponible]{type=Informative}

Pour plus d’informations, voir [Configuration de l’intégration  [!DNL Workfront]  et  [!DNL Frame.io] ](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

![Utilisateur avec trame activée](assets/Frame-enabled-user.png)


### Créer un projet connecté à Frame.io

Une fois le compte Frame.io par défaut ajouté et les utilisateurs Frame.io désignés, les coordinateurs de projet peuvent créer des projets Workfront connectés à Frame.io. Lorsque vous créez un projet connecté, vous pouvez :

* **Affecter des utilisateurs Frame.io à des tâches** : les utilisateurs ayant accès à Frame.io sont avertis par e-mail lorsqu’ils sont affectés à une tâche Workfront, ce qui signale qu’il reste du travail à accomplir.
* **Partager le projet avec des utilisateurs Frame.io** : lorsqu’un projet est partagé avec des utilisateurs dotés de Frame.io, ils ont accès au projet dans Workfront et Frame.io.
* **Partage de contenu créatif avec Frame.io** : les coordinateurs de projet peuvent envoyer des instructions et du contenu de Workfront directement à l’utilisateur créatif dans Frame.io à l’aide d’un dossier de projet de synchronisation unidirectionnelle. [!BADGE Bientôt disponible]{type=Informative}
* **Suivre la progression de la tâche** : les créatifs peuvent envoyer des ressources terminées et marquer les tâches comme terminées, le tout sans quitter Frame.io.

Pour plus d&#39;informations, voir [Créer un projet connecté à Frame.io](/help/quicksilver/manage-work/projects/create-projects/create-frame-connected-project.md).


## Création de contenu et collaboration dans Frame.io

Les créatifs peuvent rester dans les outils de leur choix et avoir la liberté de créer, d&#39;itérer et de mener des évaluations par les pairs à l&#39;intérieur de Frame.io.

Lorsqu’un élément créatif est ajouté à un projet connecté, il peut effectuer les opérations suivantes dans Frame.io :

<!--* Access instructions from the project coordinator -->
* Mener des examens informels par les pairs
* Envoyer les ressources terminées à Workfront pour révision et approbation officielles
* Modifier le statut d’une tâche ou la marquer comme terminée
* Chargez de nouvelles versions, puis soumettez-les à nouveau pour approbation <!--do they have to send to frame.io again?-->

Pour plus d&#39;informations sur Frame.io, voir [J&#39;ai été invité à collaborer sur un projet](https://support.frame.io/fr/articles/11125-j-ai-ete-invite-a-collaborer-sur-un-projet).

## Révision et approbation des ressources

Une fois qu’un élément créatif envoie une ressource terminée à Workfront à partir de Frame.io, le coordinateur du projet peut lancer le processus de révision et d’approbation formel dans Workfront.

Une fois le workflow d’approbation créé, les réviseurs et les approbateurs reviennent sur Frame.io pour ajouter des commentaires et marquer la ressource. Il peut également prendre la décision d’approbation dans la visionneuse Frame.io.

### Lancement des révisions et des approbations formelles dans Workfront

Les coordinateurs de projet peuvent créer des révisions et des approbations uniques ou des modèles d’approbation réutilisables. Toutes les activités de révision et d’approbation de Frame.io sont également enregistrées dans Workfront.

Les coordinateurs de projet ont la possibilité d’affecter des réviseurs et/ou des approbateurs :

* **Les réviseurs** peuvent ajouter des commentaires et marquer les ressources. Une fois l’opération terminée, ils peuvent marquer leur révision comme terminée. Il n’est pas nécessaire de marquer la révision comme terminée pour que la ressource progresse dans le processus d’approbation.
* Les **approbateurs** peuvent ajouter des commentaires et marquer des ressources. Ils doivent prendre la décision de faire avancer le processus d&#39;approbation.


#### Création d’un workflow de révision et d’approbation

Les réviseurs et approbateurs peuvent être ajoutés à un workflow d’approbation à usage unique ou à un modèle d’approbation réutilisable :

* **Validations à usage unique** : dans le projet ou la tâche où réside la ressource, le coordinateur du projet peut affecter des validants et des approbateurs et définir une date limite d’achèvement. Les réviseurs et les approbateurs reçoivent un rappel par e-mail 72 et 24 heures avant l’échéance, ainsi que sur l’échéance elle-même.

  Pour plus d’informations, voir * [Création d’une demande de révision ou d’approbation pour une ressource Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-request-for-frame-asset.md).

* **Modèles d’approbation** : dans la zone Configuration de Workfront, les coordinateurs de projet peuvent créer des modèles d’approbation réutilisables. Dans un modèle, les utilisateurs peuvent ajouter des réviseurs et des approbateurs et définir un délai d’achèvement. Lorsque le modèle d’approbation est appliqué à une ressource, l’échéance est calculée à partir de la période spécifiée.

  Une fois un modèle créé, il peut être appliqué aux ressources envoyées à partir de Frame.io pour lancer le processus de révision et d’approbation formel dans Workfront.

  Pour plus d&#39;informations, voir [Créer un modèle d&#39;approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)


![Attribuer un modèle](assets/assign-template.png)


#### Accès à la visionneuse Frame.io

Les utilisateurs peuvent accéder à la visionneuse Frame.io des manières suivantes :

* Notifications par e-mail de Workfront
* Le widget Mon approbation dans la nouvelle zone d’accueil de Workfront
  ![En attente de mon approbation](assets/awaiting-my-approval.png)

>[!NOTE]
>
>Les utilisateurs Workfront externes sont avertis par e-mail et sont invités à créer une connexion Frame.io pour examiner et approuver les ressources.

#### Ajout de commentaires et balisage de ressources

Tous les commentaires ajoutés dans la visionneuse Frame.io sont également enregistrés dans l’onglet Mises à jour de Workfront . Les réponses effectuées dans Workfront n&#39;apparaissent pas dans Frame.io. Si les commentaires sont marqués « Équipe uniquement » dans la visionneuse Frame.io, ils n’apparaîtront pas dans l’onglet Mises à jour de Workfront.

#### Prendre une décision

Une fois toutes les activités de révision terminées, les approbateurs doivent prendre l’une des décisions suivantes :

* **Approuver** : la ressource n’a pas besoin d’être modifiée et est prête à être utilisée.
* **Approuver avec modifications** : la ressource a besoin d’être modifiée et est prête à être utilisée une fois qu’elle a été effectuée. Aucune approbation supplémentaire n’est requise.
* **À retravailler** : la ressource a besoin d’être modifiée et n’est pas prête à être utilisée. Une fois les modifications spécifiées effectuées, la ressource doit être chargée en tant que nouvelle version et passer par un autre cycle d’approbations. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Les réviseurs peuvent marquer leur révision comme terminée dans la visionneuse Frame.io, mais cela n’est pas nécessaire pour que la ressource progresse dans le processus d’approbation.

Pour plus d’informations sur les décisions dans Workfront, voir [Présentation du statut de la décision du document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Visionneuse et décision Frame](assets/frame-viewer-and-decision.png)


<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Suivi des mesures de révision et d’approbation

Les coordinateurs de projet peuvent surveiller la progression de toutes les approbations en cours dans la zone d’accueil de Workfront à l’aide du widget suivant :

* **Toutes les approbations** : affiche 2 graphiques avec des informations sur le temps d’approbation moyen et les décisions, ainsi que des vues de liste des approbations en attente et en retard.
  ![Toutes les approbations](assets/all-approvals.png)
