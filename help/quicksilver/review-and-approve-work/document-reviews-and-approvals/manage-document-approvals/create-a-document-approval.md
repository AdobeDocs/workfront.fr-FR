---
product-area: documents
navigation-topic: approvals
title: Create a document approval workflow
description: Vous pouvez demander l’approbation d’un document à d’autres utilisateurs et utilisatrices dans Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 23%

---

# Create a document approval workflow

Vous pouvez demander à d’autres personnes ou équipes d’approuver un document dans Adobe Workfront, ou leur demander de réviser un document sans avoir à l’approuver.

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus d’approbation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les approbations à l’aide du stockage Workfront hérité</p>
<p>Tout package de workflow pour gérer les approbations à l’aide du stockage d’entreprise Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td>  
   <td>
   <p>Contributeur ou supérieur</p>
   <p>Révision ou supérieur</p>
   <p>Si vous utilisez l'intégration Frame.io, vous devez disposer d'une licence Standard pour créer des workflows d'approbation.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Affichage ou accès supérieur pour Projets, Tâches, Problèmes, Modèles, Portfolios, Programmes, Rapports, Tableaux de bord, Calendriers et Documents</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès à l’objet associé à la demande d’accès ou d’approbation </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create an approval workflow from the Summary panel in the legacy documents area

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, consultez la section [Stockage Workfront par rapport au stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

To create an approval workflow:

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le panneau Résumé du document correspondant.

1. Sélectionnez la version du document pour laquelle vous souhaitez créer une approbation dans le menu déroulant de la version. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)


## Create an approval workflow from the Summary panel in the new document area

Si votre entreprise utilise le stockage d’entreprise, la nouvelle zone de documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise](/help/quicksilver/review-and-approve-work/esm-overview.md).

Pour créer un workflow de validation :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Click on the document, then click the Approvals icon on the right side of the page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)

1. Cliquez sur **Créer un workflow**, puis renseignez les informations suivantes :

   <table>
   <tr>
   <td><strong>Nom de l’étape</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Ajouter des noms ou des adresses e-mail</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
