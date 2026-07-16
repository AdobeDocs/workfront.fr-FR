---
product-area: documents
navigation-topic: approvals
title: Utiliser conjointement les approbations unifiées et la relecture
description: Vous pouvez utiliser les approbations unifiées avec la relecture.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 678
ht-degree: 10%

---

# Utiliser conjointement les approbations unifiées et la relecture

Les approbations unifiées dans Workfront présentent un nouvel ensemble de fonctionnalités qui vous aident à examiner et approuver des documents. Vous pouvez utiliser un workflow Approbations unifiées avec la visionneuse de relecture existante pour ajouter des commentaires et des balises aux documents en cours de révision.

Il existe des différences clés dans le workflow lors de l’utilisation conjointe des validations unifiées et de la relecture :

* Les participants sont affichés dans le résumé du document, et non dans le workflow de relecture.

* Les détails Envoyé, Ouvert, Commentaire, Décision (SOCD) dans la liste de documents sont liés à la relecture et ne reflètent pas le statut de décision du document.

## Charger un document et créer une épreuve

1. Accédez au projet, à la tâche ou au problème auquel vous souhaitez ajouter un document.
1. Cliquez sur l’onglet **Documents**, puis sur le menu déroulant **Ajouter**.
Ou
Glissez-déposez le document dans la liste des documents.

   >[!NOTE]
   >
   >Si vous avez activé l’option **Générer automatiquement des épreuves lors du chargement de documents** dans votre profil utilisateur, le système crée automatiquement une épreuve simple.

1. Pointez sur le document, puis cliquez sur le lien **Créer une épreuve** qui s’affiche sous le nom du document, puis sélectionnez **Épreuve simple**. Vous devez créer un BAT simple, car vous n&#39;utiliserez pas le workflow de BAT pour les approbations.

Les utilisateurs affectés en tant que participants peuvent utiliser la visionneuse de relecture pour ajouter des commentaires et des balises sur le document. Passez à la section suivante pour savoir comment ajouter des participants à la révision.

<!--
## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## Ouvrir le résumé du document et affecter des participants

La boîte de dialogue Demander l’approbation s’ouvre en mode de base par défaut pour une approbation en une seule étape. Passez en mode avancé pour configurer les validations à plusieurs étapes ou les chemins d’accès parallèles.

Pour affecter des participants :

1. Sélectionnez le document que vous avez chargé et ouvrez le résumé du document.

   ![Ouvrir le résumé du document](assets/open-doc-summary.png)

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Créer un workflow**. La boîte de dialogue **Demander la validation** s’ouvre en mode de base.

1. Configurez le workflow de validation. Pour la description des champs, le bouton (bascule) Mode avancé et le flux de chemins d’accès parallèles, voir [Création d’un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Cliquez sur **Demander l’approbation**. Les participants sont avertis par e-mail.

<!--
## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

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

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## Créez une version selon vos besoins.

Si vous avez besoin d’une autre série d’examens et d’approbations, vous pouvez créer une nouvelle version de l’épreuve et ajouter les participants précédents, les nouveaux participants ou une combinaison des deux. Vous pouvez afficher des informations sur les versions précédentes et les participants dans le résumé du document.

La boîte de dialogue Demander l’approbation s’ouvre en mode de base par défaut pour une approbation en une seule étape. Passez en mode avancé pour configurer les validations à plusieurs étapes ou les chemins d’accès parallèles.

Pour ajouter une nouvelle version :

1. Effectuez un glisser-déposer du nouveau fichier au-dessus du document précédent dans Workfront. Workfront crée automatiquement une nouvelle version.

1. Une fois le chargement du document terminé, sélectionnez le document, puis cliquez sur **Créer une épreuve** > **Épreuve simple**.

1. Sélectionnez à nouveau le document, puis ouvrez le résumé du document.

   ![Ouvrir le résumé du document](assets/open-doc-summary.png)

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Créer un workflow**. La boîte de dialogue **Demander la validation** s’ouvre en mode de base.

1. Configurez le workflow de validation. Pour la description des champs, le bouton (bascule) Mode avancé et le flux de chemins d’accès parallèles, voir [Création d’un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Cliquez sur **Demander l’approbation**. Les participants sont avertis par e-mail.

## Examinez le BAT et prenez une décision

Le document ne passe pas à un statut approuvé tant que tous les approbateurs affectés n&#39;ont pas choisi « approuvé ».

Pour réviser et approuver un document :

1. Accédez à l’e-mail de notification de révision, puis cliquez sur **Accéder à la révision**.

1. Une fois dans Workfront, cliquez sur **Accéder au BAT**.

1. Passez en revue le contenu et ajoutez des commentaires ou des balises. Pour plus d’informations sur l’utilisation de la visionneuse de relecture, voir [Révision de BAT dans Adobe Workfront : index d’article](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Sélectionnez l’une des décisions suivantes :

   * **Approuver** : le document n’a pas besoin d’être modifié et est prêt à être utilisé.
   * **Approuver avec modifications** : le document nécessite des modifications et est prêt à l’emploi une fois qu’il a été créé. Aucune approbation supplémentaire n’est requise.
   * **Travail nécessaire** : le document doit être modifié et n’est pas prêt à être utilisé. Une fois les modifications spécifiées effectuées, le document doit être téléchargé en tant que nouvelle version et passer par un autre cycle d&#39;approbations. Pour plus d’informations sur le téléchargement d’une nouvelle version, consultez la section [Créer une version si nécessaire](#create-a-new-version-as-needed) dans cet article.

Une fois la décision prise, le propriétaire du document est averti par e-mail.