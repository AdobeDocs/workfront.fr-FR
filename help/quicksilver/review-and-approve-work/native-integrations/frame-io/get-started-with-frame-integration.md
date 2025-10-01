---
product-area: documents
navigation-topic: approvals
title: Prise en main de l’intégration Frame.io
description: Commencez avec l’intégration Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b9a83bc2-4dd8-4c77-a2e7-385baa809b3b
source-git-commit: 9825f095a7be7debb5150ca4bd50f7cf6fd12295
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 3%

---

# Prise en main de l’intégration Frame.io

L’intégration de Workfront et Frame.io aligne les créatifs, les spécialistes du marketing et les parties prenantes sur un workflow transparent. Accédez aux mises à jour en temps réel, évitez les doublons et assurez-vous que les ressources sont approuvées avant le lancement.

Pour plus d&#39;informations sur Frame.io, voir [Prise en main de Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Initiation et planification du travail dans Workfront

Les coordinateurs de projet peuvent créer des projets et planifier le travail dans Workfront. Les projets créés dans une instance avec l’intégration Frame.io activée utilisent le stockage d’entreprise d’Adobe, qui permet de stocker et de gérer les ressources dans l’écosystème Adobe.

Si votre entreprise dispose d’une licence d’entreprise Frame.io, les projets créés dans Workfront sont également visibles dans Frame.io, ce qui permet aux utilisateurs d’interagir et de charger des ressources dans les deux produits.

Pour plus d’informations sur le stockage d’entreprise Adobe ou les projets dans Frame.io, voir

* [Présentation de Workspace : projets](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Présentation du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)

## Révision et approbation des ressources

Une fois qu’une ressource est terminée, le coordinateur du projet peut lancer le processus formel de révision et d’approbation dans Workfront.

Une fois le processus d’approbation créé, les réviseurs et les approbateurs peuvent utiliser la visionneuse Frame.io pour ajouter des commentaires et marquer la ressource. Il peut également prendre la décision d’approbation dans la visionneuse Frame.io.

Pour plus d’informations sur la configuration des projets, voir

* [Créer un projet](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
* [Présentation de l’intégration Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)

### Lancement des révisions et des approbations formelles dans Workfront

Les coordinateurs de projet peuvent créer des révisions et des approbations uniques ou des modèles d’approbation réutilisables. Il peut affecter des réviseurs et des approbateurs, ou une combinaison des deux :

* **Les réviseurs** peuvent ajouter des commentaires et marquer les ressources. Une fois l’opération terminée, ils peuvent marquer leur révision comme terminée. Il n’est pas nécessaire de marquer la révision comme terminée pour que la ressource progresse dans le processus d’approbation.
* Les **approbateurs** peuvent ajouter des commentaires et marquer des ressources. Ils doivent prendre la décision de faire avancer le processus d&#39;approbation.

#### Création d’un workflow de révision et d’approbation

Les réviseurs et approbateurs peuvent être ajoutés à un workflow d’approbation à usage unique ou à un modèle d’approbation réutilisable :

* **Validations à usage unique** : dans le projet ou la tâche où réside la ressource, le coordinateur du projet peut affecter des validants et des approbateurs et définir une date limite d’achèvement. Un rappel est envoyé aux réviseurs et aux approbateurs 72 heures avant l’échéance, 24 heures avant l’échéance, puis à l’échéance elle-même.

  Pour plus d’informations, voir [Créer une demande d’approbation ou de révision de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

* **Modèles d’approbation** : dans la zone Configuration de Workfront, les coordinateurs de projet peuvent créer des modèles d’approbation réutilisables. Dans un modèle, les utilisateurs peuvent ajouter des réviseurs et des approbateurs et définir un délai d’achèvement. Lorsque le modèle d’approbation est appliqué à une ressource, l’échéance est calculée à partir de la période spécifiée.

  Une fois un modèle créé, il peut être appliqué à une ressource pour lancer le processus de révision et d’approbation formel dans Workfront.

  Pour plus d’informations, consultez [Créer un modèle d’approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


  ![Attribuer un modèle](assets/assign-template.png)

### Examen et approbation des ressources dans la visionneuse Frame.io

Une fois que le workflow de révision et d’approbation a été lancé dans Workfront, les réviseurs et les approbateurs peuvent accéder à la visionneuse Frame.io pour ajouter des commentaires, baliser la ressource et prendre une décision.

Pour plus d&#39;informations, voir [Vérifier et approuver avec la visionneuse Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md).

#### Accès à la visionneuse Frame.io

Les utilisateurs peuvent accéder à la visionneuse Frame.io des manières suivantes :

* Notifications par e-mail de Workfront
* Le widget Mon approbation dans la zone d’accueil de Workfront

>[!NOTE]
>
>Les utilisateurs Workfront externes sont avertis par e-mail et sont invités à créer une connexion Frame.io pour examiner et approuver les ressources.

![ouvrez la visionneuse d’images depuis l’Accueil](assets/open-fio-viewwer.png)

#### Ajout de commentaires et balisage de ressources

Les commentaires et les balises de ressources sont visibles dans la visionneuse Frame.io. Pour plus d&#39;informations sur l&#39;utilisation de la visionneuse Frame.io, voir [Commentaire sur vos médias](https://help.frame.io/en/articles/9105251-commenting-on-your-media).

#### Prendre une décision

Une fois toutes les activités de révision terminées, les approbateurs doivent prendre l’une des décisions suivantes :

* **Approuver** : la ressource n’a pas besoin d’être modifiée et est prête à être utilisée.
* **À retravailler** : la ressource a besoin d’être modifiée et n’est pas prête à être utilisée. Une fois les modifications spécifiées effectuées, la ressource doit être chargée en tant que nouvelle version et passer par un autre cycle d’approbations. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Les réviseurs et réviseuses peuvent marquer leur révision comme terminée dans Workfront, mais cela n’est pas nécessaire pour que la ressource passe au processus d’approbation.

Pour plus d’informations sur les décisions dans Workfront, voir [Présentation du statut de la décision du document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Visionneuse et décision Frame](assets/decision-fio.png)


### Suivi des mesures de révision et d’approbation

Les coordinateurs de projet peuvent surveiller la progression de toutes les approbations en cours dans la zone d’accueil de Workfront ou avec des rapports personnalisés dans les tableaux de bord de la zone de travail :

* **Tableau de bord personnalisé** : créez un tableau de bord de rapport dans la zone Tableaux de bord de la zone de travail pour afficher des informations détaillées et de haut niveau sur les révisions et les approbations avec la fonctionnalité d’approbations unifiées. Pour plus d’informations sur la prise en main, voir [Création d’un tableau de bord de rapports à des fins de révision et d’approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).
* **Widget Accueil des mesures d’approbation des documents** : affiche 2 graphiques avec des informations sur le temps d’approbation moyen et les décisions, ainsi que des vues de liste des approbations en attente et en retard.
  ![Toutes les approbations](assets/all-approvals.png)