---
product-area: documents
navigation-topic: approvals
title: Ajouter des approbateurs ou des réviseurs supplémentaires à un workflow d’approbation de document
description: Vous pouvez ajouter des réviseurs et réviseuses ou des approbateurs et approbatrices supplémentaires à un document ayant déjà des approbations en attente.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 13%

---

# Ajouter des approbateurs ou des réviseurs supplémentaires à un workflow d’approbation de document

Vous pouvez ajouter d&#39;autres approbateurs ou réviseurs à un workflow d&#39;approbation de document qui a déjà des approbations en attente.

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
<p>Tout package de workflow pour gérer les validations à l’aide de l’espace de stockage dans le cloud Adobe</p> </td> 
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
   <td> <p>Accédez en lecture seule ou à un accès plus étendu aux projets, tâches, événements, modèles, portefeuilles, programmes, rapports, tableaux de bord, calendriers et documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher ou avoir un accès supérieur à l’objet associé à l’approbation ou à l’accès à la demande </p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



<!--
## Add additional approvers or reviewers in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To add additional approvers or reviewers from the Document Summary:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document will open.

1. Select the version of the document you would like to add an approver or reviewer to in the version drop-down menu. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Edit workflow**.

   ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## Ajouter des approbateurs ou des réviseurs supplémentaires dans la zone des documents hérités

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, voir [Différences entre le stockage cloud Adobe et le stockage Workfront hérité](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Pour ajouter des approbateurs ou des réviseurs supplémentaires à partir du résumé du document :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document dont vous avez besoin. Le panneau Résumé du document s’ouvre pour ce document.

1. Sélectionnez la version du document auquel vous souhaitez ajouter un approbateur ou un réviseur dans le menu déroulant Version. La dernière version est sélectionnée par défaut.

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Modifier le workflow**. La boîte de dialogue Demander l’approbation s’ouvre dans le mode dans lequel l’approbation a été enregistrée pour la dernière fois : De base pour les approbations en une seule étape ou Avancé pour les approbations en plusieurs étapes et les approbations avec des chemins d’accès parallèles.

1. Ajoutez l’utilisateur, l’équipe ou l’e-mail :

   * En mode de base, saisissez le nom ou l’adresse e-mail dans le champ **Ajouter des noms ou des adresses e-mail**.
   * En mode avancé, sélectionnez le chemin d’accès qui contient l’étape à mettre à jour, puis saisissez le nom ou l’adresse électronique dans le champ **Ajouter des noms ou des adresses électroniques** de l’étape.

1. Pour chaque personne que vous avez ajoutée, choisissez s’il s’agit d’un approbateur ou d’un réviseur.

   ![liste déroulante approbateur ou réviseur](assets/choose-reviewer-or-approver.png)

1. Cliquer sur **Enregistrer**. Les participants que vous avez ajoutés reçoivent une notification par e-mail indiquant que leur approbation ou révision est nécessaire pour le document.

>[!TIP]
>
>Pour transformer une approbation en mode de base en approbation à plusieurs étapes ou à chemins d’accès, cliquez sur **Aller à l’avancé** dans le coin supérieur droit. Vos participants existants sont conservés sous le chemin 1, étape 1. Après l’enregistrement, vous ne pouvez pas revenir au mode de base. Pour plus d’informations, voir [Créer un workflow d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

<!--
## Add additional approvers or reviewers in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page. 

   ![Add approvers in document summary](assets/approvals-icon-new.png)


1. Click **Edit workflow**.

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## Ajoutez d&#39;autres approbateurs ou réviseurs à partir du Résumé du document dans la zone des nouveaux Documents

Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Pour ajouter des approbateurs ou des réviseurs supplémentaires à partir du résumé du document :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document, puis sur l’icône **Validations** sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)

1. Cliquez sur **Modifier le workflow**. La boîte de dialogue Demander l’approbation s’ouvre dans le mode dans lequel l’approbation a été enregistrée pour la dernière fois : De base pour les approbations en une seule étape ou Avancé pour les approbations en plusieurs étapes et les approbations avec des chemins d’accès parallèles.

1. Ajoutez l’utilisateur, l’équipe ou l’e-mail :

   * En mode de base, saisissez le nom ou l’adresse e-mail dans le champ **Ajouter des noms ou des adresses e-mail**.
   * En mode avancé, sélectionnez le chemin d’accès qui contient l’étape à mettre à jour, puis saisissez le nom ou l’adresse électronique dans le champ **Ajouter des noms ou des adresses électroniques** de l’étape.

1. Pour chaque personne que vous avez ajoutée, choisissez s’il s’agit d’un approbateur ou d’un réviseur.

   ![liste déroulante approbateur ou réviseur](assets/choose-reviewer-or-approver.png)

1. Cliquer sur **Enregistrer**. Les participants que vous avez ajoutés reçoivent une notification par e-mail indiquant que leur approbation ou révision est nécessaire pour le document.

>[!TIP]
>
>Pour transformer une approbation en mode de base en approbation à plusieurs étapes ou à chemins d’accès, cliquez sur **Aller à l’avancé** dans le coin supérieur droit. Vos participants existants sont conservés sous le chemin 1, étape 1. Après l’enregistrement, vous ne pouvez pas revenir au mode de base. Pour plus d’informations, voir [Créer un workflow d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).
