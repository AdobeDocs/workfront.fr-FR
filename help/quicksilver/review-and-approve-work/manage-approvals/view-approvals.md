---
product-area: projects
navigation-topic: approvals
title: Afficher les approbations
description: Les processus d’approbation offrent une flexibilité permettant de créer des approbations à plusieurs étapes pour des projets, des tâches et des problèmes. Les administrateurs et administratrices Adobe Workfront définissent les processus d’approbation pour assurer la cohérence de l’ensemble du système.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: c6e3e3d8d4fd6b6916c8fd49983bc3572949acaa
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 85%

---

# Afficher les approbations

Les processus d’approbation offrent une flexibilité permettant de créer des approbations à plusieurs étapes pour des projets, des tâches et des problèmes. Les administrateurs et administratrices Adobe Workfront définissent les processus d’approbation pour assurer la cohérence de l’ensemble du système.

Pour plus d’informations sur la création de processus d’approbation, voir [Créer un processus d’approbation pour des éléments de travail](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Pour plus d’informations sur l’association des approbations à du travail dans Workfront, voir [Associer un processus d’approbation nouveau ou existant à du travail](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès Afficher ou supérieur aux objets associés à des approbations</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Afficher ou supérieures pour les objets associés aux approbations</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Localiser des approbations dans Adobe Workfront

Vous pouvez afficher ou gérer des approbations à partir de plusieurs zones dans Workfront. Pour plus d’informations sur la gestion des approbations dans les différentes zones, voir [Approuver du travail](../../review-and-approve-work/manage-approvals/approving-work.md).

Vous pouvez afficher ou gérer des approbations dans les zones suivantes :

* Dans la zone Accueil

   * Tous les projets, tâches, problèmes, feuilles de temps, documents et accès en attente de votre approbation s’affichent dans la zone Accueil lorsque vous sélectionnez l’option Tout afficher ou Validations.
   * Les approbations que vous avez envoyées vous-même s’affichent également dans la zone Accueil, dans la section Approbations que j’ai envoyées de la Liste de travail. Pour plus d’informations, voir la section [Réviser le travail que vous soumettez pour approbation dans la zone Accueil](#review-work-you-submit-for-approval-in-the-home-area) dans cet article.
   * Les approbations sont supprimées de la zone d’accueil lorsque le projet, la tâche ou le problème associé est marqué Résolu, En attente, Fermé ou Annulé.

  Pour plus d’informations sur l’utilisation de la page d’accueil, voir [Commencer avec la page d’accueil](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* Dans l’en-tête d’un projet, d’une tâche, d’un problème, d’un document ou d’une épreuve
* Dans la section Approbations d’un projet, d’une tâche ou d’un problème
* Dans un rapport

  >[!NOTE]
  >
  >Vous ne pouvez pas prendre de décision sur une approbation à partir d’un rapport.

  Vous pouvez créer un rapport d’approbation de projet, de tâche, de problème ou de document qui contient les informations d’approbation.

  Pour plus d’informations sur la création de rapports, voir [Créer un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Réviser le travail que vous soumettez pour approbation dans la zone Accueil. {#review-work-you-submit-for-approval-in-the-home-area}

1. Cliquez sur l’icône **Accueil** ![](assets/home-icon-30x29.png) dans le coin supérieur gauche d’Adobe Workfront.

   >[!NOTE]
   >
   >Votre administrateur ou administratrice Workfront peut apporter les modifications suivantes à l’icône Accueil de votre environnement :
   >
   >* La remplacer par une image personnalisée pour illustrer votre entreprise. Dans ce cas, l’icône sera différente de celle présentée dans cet article.
   >* Remplacer la page à laquelle elle est liée par une autre page. Dans ce cas, cliquez sur le **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de la page, puis sur **Accueil**.

1. Sélectionnez **Liste de travail**, puis cliquez sur le menu déroulant **Filtrer** et sélectionnez **Approbations**.
1. Développez la section **Approbations que j’ai envoyées** et recherchez les approbations que vous avez envoyées.

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## Afficher le statut d’approbation d’un objet

Vous pouvez afficher le statut d’approbation d’un objet dans les sections suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Mises à jour </td> 
   <td> <p>Affiche tous les statuts d’approbation lorsqu’ils se produisent. Les statuts d’approbation s’affichent à côté des autres statuts affichés dans la section <strong>Mises à jour</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Approbations</td> 
   <td> <p>Affiche des informations plus détaillées sur le processus d’approbation, telles que les étapes individuelles du processus d’approbation et si les approbateurs et approbatrices ont approuvé ou non.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Utiliser la zone Mises à jour pour afficher le statut d’une approbation {#use-the-updates-area-to-view-an-approval-status}

Lorsqu’une approbation est lancée sur un projet, une tâche ou un problème, un état s’affiche dans l’onglet **Mises à jour** de l’objet, indiquant le statut de la validation. Un nouvel état s’affiche chaque fois que l’objet passe par le processus d’approbation. Cela inclut les événements suivants :

* Un processus d’approbation est lancé sur un objet. Le processus d’approbation est démarré lorsque le statut est modifié.
* L’objet est rejeté.
* L’objet est approuvé.

>[!TIP]
>
>Si une approbation est appliquée à une tâche, les mises à jour de l’approbation sont affichées dans l’onglet Mises à jour de la tâche, et non dans l’onglet Mises à jour du projet dans lequel se trouve la tâche.

### Utiliser la zone Approbations pour afficher le statut d’une approbation {#use-the-approvals-area-to-view-an-approval-status}

Vous pouvez déterminer où se trouve une tâche ou un problème sur lequel vous travaillez actuellement dans le processus d’approbation. Vous pouvez voir les informations suivantes :

* La phase du processus d’approbation.
* Les approbateurs et approbatrices qui l’ont déjà approuvé.
* Les approbateurs et approbatrices qui ne l’ont pas encore approuvé.

Pour voir l’état actuel d’une tâche ou d’un problème dans le processus d’approbation, procédez comme suit :

1. Accédez au projet, à la tâche ou au problème auquel ou à laquelle l’approbation est associée.
1. Dans le panneau de gauche, cliquez sur **Approbations**. Vous devrez peut-être d’abord cliquer sur **Afficher plus**.

   L’onglet Approbations affiche toutes les informations sur tous les parcours et étapes d’approbation précédents. Vous pouvez voir qui a pris une décision sur l’approbation ou si l’approbation est définie pour une équipe, une fonction, ou bien un utilisateur ou une utilisatrice.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Pour plus d’informations sur la création d’un processus d’approbation, voir [Créer un processus d’approbation pour des éléments de travail](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
