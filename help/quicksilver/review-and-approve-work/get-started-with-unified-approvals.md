---
product-area: documents
navigation-topic: approvals
title: Prise en main de la révision et de l’approbation unifiées
description: En savoir plus sur la révision et l’approbation unifiées optimisées par Workfront et Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 10962d59-284e-4c41-8523-18ea4ed78362
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: c989b5d6a91a4b1f19b044916b4f68a1738f9b16
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 4%

---

# Prise en main de la révision et de l’approbation unifiées


La révision et l’approbation unifiées rassemblent Adobe Workfront et Adobe Frame.io dans une expérience unique et profondément connectée, réduisant ainsi les écarts entre la gestion marketing, la révision créative et la diffusion de contenu. Les coordinateurs de projet gèrent le travail dans Workfront pendant que les créatifs, les spécialistes marketing et les parties prenantes examinent et approuvent les ressources dans la visionneuse Frame.io de qualité professionnelle, le tout sans déplacer les fichiers entre des outils déconnectés.

Pour plus d&#39;informations sur Frame.io, voir [Prise en main de Frame.io](https://support.frame.io/en/collections/49298-getting-started).

L’intégration Workfront et Frame.io doit être configurée dans votre instance Workfront. Pour plus d’informations, voir [Aperçu de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md#integration-requirements).

## Vidéo de présentation

>[!VIDEO](https://video.tv.adobe.com/v/3471078)

## Exigences d’intégration

* Workfront et Frame.io doivent être déployés sur la même organisation Identity Management system (IMS).

* Les utilisateurs ne peuvent appartenir qu’à une seule instance Workfront au sein de l’organisation IMS.

* L’instance Workfront doit être activée sur l’expérience unifiée Adobe et le stockage d’entreprise Adobe.

## Initiation et planification du travail dans Workfront

Les coordinateurs de projet peuvent créer des projets et planifier le travail dans Workfront. Les projets créés dans une instance avec l’intégration Frame.io activée utilisent le stockage d’entreprise d’Adobe, qui permet de stocker et de gérer les ressources dans l’écosystème Adobe.

Si votre entreprise dispose d’une licence d’entreprise Frame.io, les projets créés dans Workfront sont également visibles dans Frame.io, ce qui permet aux utilisateurs d’interagir et de charger des ressources dans les deux produits.

Pour plus d’informations sur le stockage d’entreprise ou les projets Adobe dans Frame.io, voir

* [Présentation de Workspace : projets](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Vue d’ensemble du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)

## Révision et approbation des ressources

Une fois qu’une ressource est terminée, le coordinateur du projet peut lancer le processus formel de révision et d’approbation dans Workfront.

Une fois le processus d’approbation créé, les réviseurs et les approbateurs peuvent utiliser la visionneuse Frame.io pour ajouter des commentaires et marquer la ressource. Il peut également prendre la décision d’approbation dans la visionneuse Frame.io.

Pour plus d’informations sur la configuration des projets, voir

* [Créer un projet](/help/quicksilver/manage-work/projects/create-projects/create-project.md)

### Lancement des révisions et des approbations formelles dans Workfront

Les coordinateurs de projet peuvent créer des révisions et des approbations uniques ou des modèles d’approbation réutilisables. Il peut affecter des réviseurs et des approbateurs, ou une combinaison des deux :

* **Les réviseurs** peuvent ajouter des commentaires et marquer les ressources. Une fois l’opération terminée, ils peuvent marquer leur révision comme terminée. Il n’est pas nécessaire de marquer la révision comme terminée pour que la ressource progresse dans le processus d’approbation.
* Les **approbateurs** peuvent ajouter des commentaires et marquer des ressources. Ils doivent prendre la décision de faire avancer le processus d&#39;approbation.

#### Création d’un workflow de révision et d’approbation

Les réviseurs et approbateurs peuvent être ajoutés à un workflow d’approbation à usage unique ou à un modèle d’approbation réutilisable :

* **Validations à usage unique** : dans le projet ou la tâche où réside la ressource, le coordinateur du projet peut affecter des validants et des approbateurs et définir une date limite d’achèvement. Un rappel est envoyé aux réviseurs et aux approbateurs 72 heures avant l’échéance, 24 heures avant l’échéance, puis à l’échéance elle-même.

  Pour plus d’informations, voir [Créer un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-from-the-summary-panel-in-the-new-document-area).

* **Modèles d’approbation** : dans la zone Configuration de Workfront, les coordinateurs de projet peuvent créer des modèles d’approbation réutilisables. Dans un modèle, les utilisateurs peuvent ajouter des réviseurs et des approbateurs et définir un délai d’achèvement. Lorsque le modèle d’approbation est appliqué à une ressource, l’échéance est calculée à partir de la période spécifiée.

  Une fois un modèle créé, il peut être appliqué à une ressource pour lancer le processus de révision et d’approbation formel dans Workfront.

  Pour plus d’informations, voir [Création d’un modèle de workflow d’approbation pour les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

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
* **Approuvé avec modifications** : la ressource est presque complète, mais des modifications mineures lui sont nécessaires avant de pouvoir être utilisée. Une fois les modifications spécifiées effectuées, la ressource est prête et n’a pas besoin de passer par une autre série d’approbations.
* **À retravailler** : la ressource a besoin d’être modifiée et n’est pas prête à être utilisée. Une fois les modifications spécifiées effectuées, la ressource doit être chargée en tant que nouvelle version et passer par un autre cycle d’approbations. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Les réviseurs et réviseuses peuvent marquer leur révision comme terminée dans Workfront, mais cela n’est pas nécessaire pour que la ressource passe au processus d’approbation.

Pour plus d’informations sur les décisions dans Workfront, voir [Présentation du statut de la décision du document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Visionneuse et décision Frame](assets/decision-fio.png)


### Suivi des mesures de révision et d’approbation

Les coordinateurs de projet peuvent surveiller la progression de toutes les approbations en cours dans la zone d’accueil de Workfront ou avec des rapports personnalisés dans les tableaux de bord de la zone de travail :

* **Tableau de bord personnalisé** : créez un tableau de bord de rapport dans la zone Tableaux de bord de la zone de travail pour afficher des informations détaillées et de haut niveau sur les révisions et les approbations avec la fonctionnalité d’approbations unifiées. Pour plus d’informations sur la prise en main, voir [Création d’un tableau de bord de rapports à des fins de révision et d’approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).
* **Widget Accueil des mesures d’approbation des documents** : affiche 2 graphiques avec des informations sur le temps d’approbation moyen et les décisions, ainsi que des vues de liste des approbations en attente et en retard.
  ![Toutes les approbations](assets/all-approvals.png)

## Envoi des ressources terminées vers Adobe Experience Manager

Vous pouvez utiliser le &#x200B;&#x200B; pour gérer et stocker vos ressources numériques qui ont passé le cycle de révision et d’approbation. [!DNL Experience Manager Assets] Cette intégration permet d’exploiter les fonctionnalités d’Adobe Experience Manager, Frame.io et Workfront afin de rationaliser vos processus de gestion de contenu et de collaboration.

Pour plus d’informations, voir [Utilisation d’Adobe Experience Manager avec l’intégration Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

