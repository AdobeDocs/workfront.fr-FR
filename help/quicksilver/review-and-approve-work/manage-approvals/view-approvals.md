---
product-area: projects
navigation-topic: approvals
title: Afficher les approbations
description: Les processus de validation permettent de créer des validations à plusieurs étapes pour des projets, des tâches et des problèmes. Les administrateurs d’Adobe Workfront définissent les processus d’approbation pour assurer la cohérence de l’ensemble du système.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Afficher les approbations

Les processus de validation permettent de créer des validations à plusieurs étapes pour des projets, des tâches et des problèmes. Les administrateurs d’Adobe Workfront définissent les processus d’approbation pour assurer la cohérence de l’ensemble du système.

Pour plus d’informations sur la création de processus de validation, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Pour plus d’informations sur l’association des approbations à un travail dans Workfront, voir [Associer un processus d’approbation nouveau ou existant au travail](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Consulter ou accéder à des objets associés à des validations</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Consulter ou obtenir des autorisations supérieures aux objets associés aux validations</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Localisation des approbations dans Adobe Workfront

Vous pouvez afficher ou gérer les validations à partir de plusieurs zones de Workfront. Pour plus d’informations sur la gestion des validations dans divers domaines, voir [Valider le travail](../../review-and-approve-work/manage-approvals/approving-work.md).

Vous pouvez afficher ou gérer les validations dans les domaines suivants :

* Dans la zone Accueil

   * Tous les projets, tâches, problèmes, feuilles de temps, documents et accès en attente de votre approbation s’affichent dans la zone Accueil lorsque vous sélectionnez l’option Tout afficher ou Validations.
   * Les validations que vous avez soumises vous-même s’affichent également dans la zone Accueil, dans la section Validations que j’ai envoyées de la liste de tâches. Pour plus d’informations, voir [Examinez les travaux que vous soumettez pour approbation dans la zone d’accueil.](#review-work-you-submit-for-approval-in-the-home-area) dans cet article.
   * Les approbations sont supprimées de la zone d’accueil lorsque le projet, la tâche ou le problème associé est marqué Résolu, En attente, Fermé ou Annulé.

  Pour plus d’informations sur l’utilisation de la page d’accueil, voir [Prise en main de la page d’accueil](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* Dans l’en-tête d’un projet, d’une tâche, d’un problème, d’un document ou d’un BAT
* Dans la section Approbations d’un projet, d’une tâche ou d’un problème
* Dans un rapport

  >[!NOTE]
  >
  >Vous ne pouvez pas prendre de décision sur une validation à partir d’un rapport.

  Vous pouvez créer un rapport d’approbation de projet, de tâche, d’émission ou de document contenant les informations d’approbation.

  Pour plus d’informations sur la création de rapports, voir [Création d’un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Examinez les travaux que vous soumettez pour approbation dans la zone d’accueil. {#review-work-you-submit-for-approval-in-the-home-area}

1. Cliquez sur le bouton **Accueil** icon ![](assets/home-icon-30x29.png) dans le coin supérieur gauche d’Adobe Workfront.

   >[!NOTE]
   >
   >Votre administrateur Workfront peut apporter les modifications suivantes à l’icône Accueil de votre environnement :
   >
   >* Remplacez-le par une image personnalisée pour illustrer votre entreprise. Dans ce cas, l’icône sera différente de celle présentée dans cet article.
   >* Remplacez la page qui lui est liée par une autre page. Dans ce cas, cliquez sur le bouton **Menu Principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de la page, puis cliquez sur **Accueil**.

1. Sélectionner **Liste de tâches**, puis cliquez sur le bouton **Filtrer** menu déroulant et sélectionnez **Approbations**.
1. Développez l’objet **Validations que j’ai envoyées** et recherchez les validations que vous avez soumises.

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## Affichage de l’état d’approbation d’un objet

Vous pouvez consulter l’état d’approbation d’un objet dans les sections suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Mises à jour </td> 
   <td> <p>Affiche tous les états d’approbation lorsqu’ils se produisent. Les états de validation s'affichent en ligne avec les autres états affichés sur le <strong>Mises à jour</strong> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Approbations</td> 
   <td> <p>Affiche des informations plus détaillées sur le processus de validation, telles que chaque étape du processus de validation et indique si les approbateurs ont accordé la validation.</p> </td> 
  </tr> 
 </tbody> 
</table>

* [Utilisez la zone Mises à jour pour afficher le statut de la validation.](#use-the-updates-area-to-view-an-approval-status)
* [Utiliser la zone Validations pour afficher l’état de validation](#use-the-approvals-area-to-view-an-approval-status)

### Utilisez la zone Mises à jour pour afficher le statut de la validation. {#use-the-updates-area-to-view-an-approval-status}

Lorsqu’une approbation est lancée sur un projet, une tâche ou un problème, un état s’affiche dans la variable **Mises à jour** de l’objet, indiquant le statut de la validation. Un nouvel état s’affiche chaque fois que l’objet passe par le processus d’approbation. Cela inclut les événements suivants :

* Un processus d’approbation est lancé sur un objet. Le processus d’approbation est lancé lorsque l’état est modifié.
* L’objet est rejeté.
* L’objet est approuvé. 

>[!TIP]
>
>Si une validation est appliquée à une tâche, les mises à jour de validation sont affichées dans l’onglet Mises à jour de la tâche, et non dans l’onglet Mises à jour du projet où réside la tâche.

### Utiliser la zone Validations pour afficher l’état de validation {#use-the-approvals-area-to-view-an-approval-status}

Vous pouvez déterminer où se trouve une tâche ou un problème sur lequel vous travaillez actuellement dans le processus d’approbation. Vous pouvez consulter les informations suivantes :

* La phase du processus de validation
* Quels approbateurs l’ont déjà approuvé ?
* Quels approbateurs ne l’ont pas encore approuvé ?

Pour voir l’état actuel d’une tâche ou d’un problème dans le processus d’approbation :

1. Accédez au projet, à la tâche ou à l’émission auquel la validation est associée.
1. Dans le panneau de gauche, cliquez sur **Approbations**. Vous devrez peut-être cliquer en premier **Afficher plus**.

   L’onglet Validations affiche des informations complètes sur tous les parcours et étapes de validation précédents. Vous pouvez déterminer qui a pris une décision lors de l’approbation ou si l’approbation est définie pour une équipe, un rôle de tâche ou un utilisateur.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Pour plus d’informations sur la création d’un processus d’approbation, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
