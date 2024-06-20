---
product-area: documents
navigation-topic: approvals
title: Créer une demande de révision ou d’approbation de document
description: Vous pouvez demander l’approbation d’un document à d’autres utilisateurs et utilisatrices dans Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: e8116a6778d5952ba583cfdfb94b761757adc030
workflow-type: ht
source-wordcount: '500'
ht-degree: 100%

---

# Créer une demande de révision ou d’approbation de document

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elles sont disponibles uniquement dans l’environnement de prévisualisation de sandbox.</span>

Vous pouvez demander l’approbation d’un document à d’autres utilisateurs et utilisatrices ou équipes dans Adobe Workfront, ou leur demander de réviser un document sans devoir l’approuver.

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus d’approbation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Affichage ou accès supérieur pour Projets, Tâches, Problèmes, Modèles, Portfolios, Programmes, Rapports, Tableaux de bord, Calendriers et Documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès à l’objet associé à la demande d’accès ou d’approbation </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer d’une demande de révision ou d’approbation de document à partir de la page du document

1. Pointez sur le document, puis cliquez sur sélectionnez Détails du document.
   ![](assets/doc-details.png)


1. À côté du nom du document, sélectionnez la version du document pour laquelle créer une approbation dans le menu déroulant de la version. La version la plus récente est sélectionnée par défaut.

1. Cliquez sur **Approbations** dans le volet de gauche.

1. <span class="preview">(Facultatif) Définissez un échéance pour l’approbation. Les utilisateurs et utilisatrices et les équipes sont informés par e-mail 72 heures, puis 24 heures avant l’échéance spécifiée.</span>

1. Pour ajouter un approbateur ou une approbatrice, cliquez sur **Approbateur** et commencez à saisir le nom d’un utilisateur, d’une utilisatrice ou d’une équipe.

1. Pour ajouter un réviseur ou une réviseuse, cochez la case **Réviseur** et commencez à saisir le nom d’un utilisateur, d’une utilisatrice ou d’une équipe.

   ![](assets/add-approver-and-deadline.png)

1. Répétez l’étape précédente pour ajouter d’autres approbateurs, approbatrices, réviseurs ou réviseuses.

## Créer une demande de révision ou d’approbation de document à partir du volet Résumé du document

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le volet Résumé du document.

1. Sélectionnez la version du document pour laquelle créer une approbation dans le menu déroulant de la version. La version la plus récente est sélectionnée par défaut.

1. Faites défiler la page jusqu’à la section **Approbations** dans le volet Résumé du document, puis cliquez sur **Ajouter**.

![](assets/doc-summary-add-approvers.png)

1. <span class="preview">(Facultatif) Définissez une échéance pour l’approbation. Les utilisateurs et utilisatrices et les équipes sont informés par e-mail 72 heures, puis 24 heures avant l’échéance spécifiée.</span>

1. Pour ajouter un approbateur ou une approbatrice, cliquez sur **Approbateur** et commencez à saisir le nom d’un utilisateur, d’une utilisatrice ou d’une équipe.

1. Pour ajouter un réviseur ou une réviseuse, cochez la case **Réviseur** et commencez à saisir le nom d’un utilisateur, d’une utilisatrice ou d’une équipe.

   ![](assets/add-approver-and-deadline.png)

1. Répétez l’étape précédente pour ajouter d’autres approbateurs, approbatrices, réviseurs ou réviseuses.

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![](assets/nwe-resubmit-approval-350x149.png)
-->
