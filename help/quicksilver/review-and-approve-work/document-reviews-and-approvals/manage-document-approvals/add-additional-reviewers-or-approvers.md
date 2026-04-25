---
product-area: documents
navigation-topic: approvals
title: Add additional approvers or reviewers to a document approval workflow
description: Vous pouvez ajouter des réviseurs et réviseuses ou des approbateurs et approbatrices supplémentaires à un document ayant déjà des approbations en attente.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 17%

---

# Add additional approvers or reviewers to a document approval workflow

You can add additional approvers or reviewers to a document approval workflow that already has pending approvals.

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus d’approbation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
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
   <td> <p>View or higher access to Projects, Tasks, Issues, Templates, Portfolios, Programs, Reports, Dashboards, Calendars, and Documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher ou avoir un accès supérieur à l’objet associé à l’approbation ou à l’accès à la demande </p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Add additional approvers or reviewers from the Document Summary in the legacy documents area

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, consultez la section [Stockage Workfront par rapport au stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

To add additional approvers or reviewers from the Document Summary:

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Click on the document you need and the Document Summary panel for that document will open.

1. Select the version of the document you would like to add an approver or reviewer to in the version drop-down menu. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Edit workflow**.

   ![modifier le workflow d’approbation](assets/edit-approval-in-legacy.png)

1. Locate the stage you would like to add approvers or reviewers to, then add the user&#39;s name or email in the text box. You can also add an entire team if needed.

1. Once their name is added, choose if they are an approver or reviewer.

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
Once you save, the participants added receive an email notification that their approval or review is needed on the document.



## Add additional approvers or reviewers from the Document Summary in the new documents area

Si votre entreprise utilise le stockage d’entreprise, la nouvelle zone de documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document, puis sur l’icône **Validations** sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)


1. Cliquez sur **Modifier le workflow**.

1. Localisez l’étape à laquelle vous souhaitez ajouter des approbateurs ou des réviseurs, puis ajoutez le nom ou l’adresse électronique de l’utilisateur dans la zone de texte. Vous pouvez également ajouter une équipe entière si nécessaire.

1. Une fois leur nom ajouté, choisissez s’ils sont approbateurs ou réviseurs.

   ![liste déroulante approbateur ou réviseur](assets/choose-approver-or-reviewer.png)

1. Répétez les étapes 5 à 6 pour ajouter d’autres approbateurs ou réviseurs ou réviseuses.
Une fois le document enregistré, les participants ajoutés reçoivent une notification par e-mail indiquant que leur approbation ou révision est nécessaire pour le document.







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
