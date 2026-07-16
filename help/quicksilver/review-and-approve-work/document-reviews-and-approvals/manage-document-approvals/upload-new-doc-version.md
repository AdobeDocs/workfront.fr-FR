---
product-area: documents
navigation-topic: approvals
title: Charger une nouvelle version du document et demander une approbation
description: Vous pouvez charger une nouvelle version du document et demander l’approbation d’autres utilisateurs dans Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66a134507a06c0ce0b4fd78bfa5e32bd95f8f08c
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 14%

---

# Charger une nouvelle version du document et demander une approbation

Si un document est marqué « A besoin d’être retravaillé » lors d’une révision précédente, vous pouvez charger une nouvelle version dans le document d’origine et commencer une nouvelle série d’approbations. Une fois que vous avez chargé une nouvelle version du document, les versions précédentes sont verrouillées.

Si le nom de fichier de la nouvelle version est différent de celui de la version précédente, Workfront affiche le document avec le nom de fichier le plus récent.

Lorsqu&#39;une nouvelle version est ajoutée à un document avec des approbations en attente, l&#39;approbation de la version précédente indique « Retiré ». Le processus d’approbation précédent se termine, même si certains participants n’ont pas encore pris de décision.

Si la dernière version du document est supprimée, les versions précédentes restent verrouillées. Si vous devez modifier une version précédente, vous devez la déverrouiller manuellement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les approbations à l’aide du stockage Workfront hérité</p>
<p>Tout package de workflow pour gérer les validations à l’aide de l’espace de stockage dans le cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td> <p>Requête ou supérieure</p>
   <p>Contributeur ou supérieur</p>
   <p>Si vous utilisez l'intégration Frame.io, vous devez disposer d'une licence Standard pour créer des workflows d'approbation.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux documents</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès Modifier à l’objet associé au document</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



<!--
## Use drag-and-drop to add a new version in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-drop does not work with Internet Explorer.


If you need another round of review and approval on a document, you can create a new document version in Workfront.

You can add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page. 

To add a new version:

1. Navigate to the document in Workfront.
1. Drag and drop the new file on top of the previous document. This automatically creates a new version. 

1. Once the document finishes uploading, select the document to open the Document Summary panel. Here you'll see the version number at the top of the panel.


1. Scroll down to the **Approvals** section.

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
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



1. (Optional) To add an existing approval template, select a template from the left side of the dialog.

   >[!TIP]
   >
   >   Users with a Standard license can create reusable Approval Templates from the Setup area. For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Once you have added all the stages and participants you need, click **Request approval**.

   The approval workflow starts and the approvers receive a notification that their approval is needed on the new document version. The previous document version is locked and any outstanding approvals on the previous version are withdrawn.

    ![request approval](assets/request-approval.png)
-->

<!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

## Effectuez un glisser-déposer pour ajouter une nouvelle version dans la zone des documents hérités

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, voir [Différences entre le stockage cloud Adobe et le stockage Workfront hérité](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Glisser-déposer ne fonctionne pas avec Internet Explorer.

Si vous avez besoin d’une autre phase de révision et d’approbation d’un document, vous pouvez créer une nouvelle version du document dans Workfront. Vous pouvez ajouter les participants précédents, de nouveaux participants ou une combinaison des deux. Vous pouvez afficher des informations sur les versions précédentes et les participants sur la page Détails du document .

La boîte de dialogue Demander l’approbation s’ouvre en mode de base par défaut pour une approbation en une seule étape. Passez en mode avancé pour configurer les validations à plusieurs étapes ou les chemins d’accès parallèles.

Pour ajouter une nouvelle version et demander l’approbation :

1. Accédez au document dans Workfront.

1. Glissez-déposez le nouveau fichier en haut du document précédent. Workfront crée automatiquement une nouvelle version.

1. Une fois le chargement du document terminé, sélectionnez le document pour ouvrir le panneau Résumé du document . Le numéro de version s’affiche en haut du panneau.

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Créer un workflow**. La boîte de dialogue **Demander la validation** s’ouvre en mode de base.

1. Configurez le workflow de validation. Pour la description des champs, le bouton (bascule) Mode avancé et le flux de chemins d’accès parallèles, voir [Création d’un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Pour copier les mêmes réviseurs et approbateurs de la version précédente du document, cliquez sur **Copier**.
1. Cliquez sur **Demander l’approbation**.

   Le workflow d’approbation démarre et les approbateurs reçoivent une notification indiquant que leur approbation est nécessaire pour la nouvelle version du document. La version précédente du document est verrouillée et toutes les approbations en attente sur la version précédente sont retirées.

## Effectuez un glisser-déposer pour ajouter une nouvelle version dans la zone des nouveaux Documents

Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

>[!NOTE]
>
>Glisser-déposer ne fonctionne pas avec Internet Explorer.

Si vous avez besoin d’une autre phase de révision et d’approbation d’un document, vous pouvez créer une nouvelle version du document dans Workfront. Vous pouvez ajouter un workflow d’approbation à la nouvelle version du document.

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

La boîte de dialogue Demander l’approbation s’ouvre en mode de base par défaut pour une approbation en une seule étape. Passez en mode avancé pour configurer les validations à plusieurs étapes ou les chemins d’accès parallèles.

Pour ajouter une nouvelle version et demander l’approbation :

1. Accédez au document dans Workfront.

1. Glissez-déposez le nouveau fichier en haut du document précédent. Workfront crée automatiquement une nouvelle version.

1. Une fois le chargement du document terminé, sélectionnez le document pour ouvrir le panneau Résumé . La dernière version du document est sélectionnée par défaut.

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Créer un workflow**. La boîte de dialogue **Demander la validation** s’ouvre en mode de base.

1. Configurez le workflow de validation. Pour la description des champs, le bouton (bascule) Mode avancé et le flux de chemins d’accès parallèles, voir [Création d’un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Pour copier les mêmes réviseurs et approbateurs de la version précédente du document, cliquez sur **Copier**.
1. Cliquez sur **Demander l’approbation**.

   Le workflow d’approbation démarre et les approbateurs reçoivent une notification indiquant que leur approbation est nécessaire pour la nouvelle version du document. La version précédente du document est verrouillée et toutes les approbations en attente sur la version précédente sont retirées.
