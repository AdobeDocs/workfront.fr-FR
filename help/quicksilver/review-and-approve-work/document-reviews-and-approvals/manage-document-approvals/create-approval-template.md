---
product-area: documents
navigation-topic: approvals
title: Create an approval workflow template for documents
description: Vous pouvez créer des modèles d’approbation afin d’optimiser votre processus d’approbation.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 37%

---

# Create an approval workflow template for documents

In the Workfront Setup area, users with a Standard license can create reusable Approval Templates. Une fois créés, les modèles d’approbation peuvent être appliqués aux ressources dans la zone Documents d’un projet, d’une tâche ou d’un problème.

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
   <td><p>Any Workfront package to manage approvals using legacy Workfront storage</p>
<p>Any Workflow package to manage approvals using Adobe enterprise storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Plan</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++
ß

## Créer un modèle d’approbation

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Révision et approbation** > **Modèles d’approbation**.
1. Cliquez sur **Nouveau modèle** sur le côté droit de la page.

1. Fill in the following details:

   <table>
     <tr>
   <td><strong>Nom de modèle</strong></td>
   <td>Add a template name. </td>
   </tr>
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
   <td><strong>Jours ouvrés jusqu’à échéance</strong></td>
   <td>Choose how many workdays until the approval is due after a stage is activated.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)

1. Cliquez sur **Enregistrer**.

Once the template is created, it can be applied to documents in the Documents area of a project, task, or issue to begin the formal review and approval process in Workfront.



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
