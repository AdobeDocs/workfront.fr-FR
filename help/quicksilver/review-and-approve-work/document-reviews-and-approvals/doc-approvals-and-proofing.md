---
product-area: documents
navigation-topic: approvals
title: Utiliser les approbations et les relectures de nouveaux documents ensemble
description: Vous pouvez utiliser les nouvelles approbations de document avec la relecture.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 4%

---

# Utiliser les approbations et les relectures de nouveaux documents ensemble

Les nouvelles approbations de documents dans Workfront contiennent un nouvel ensemble de fonctionnalités qui vous aident à examiner et approuver des documents. Vous pouvez utiliser le nouveau workflow d’approbation de document avec la visionneuse de relecture existante pour ajouter des commentaires et des balises aux documents en cours de révision.

Il existe des différences clés dans le workflow lorsque vous utilisez à la fois les approbations de nouveaux documents et la relecture :

* Les boutons de décision n’apparaissent pas dans la visionneuse de relecture

* Les participants sont affichés dans le résumé du document, et non dans le workflow de relecture

* Les détails Envoyé, Ouvert, Commentaire, Décision (SOCD) dans la liste de documents sont liés à la relecture et ne reflètent pas le statut de décision du document.

## Charger un document et créer une épreuve

1. Accédez au projet, à la tâche ou au problème auquel vous souhaitez ajouter un document.
1. Cliquez sur l&#39;onglet **Documents**, puis sur le menu déroulant **Ajouter**.
Ou
Glissez-déposez le document dans la liste des documents.

   >[!NOTE]
   >
   >Si vous avez activé l’option **Générer automatiquement des épreuves lors du chargement de documents** dans votre profil utilisateur, le système crée automatiquement une épreuve simple.

1. Pointez sur le document, puis cliquez sur le lien **Créer une épreuve** qui s’affiche sous le nom du document, puis sélectionnez **Épreuve simple**. Vous devez créer un BAT simple, car vous n&#39;utiliserez pas le workflow de BAT pour les approbations.

Les utilisateurs affectés en tant que participants peuvent utiliser la visionneuse de relecture pour ajouter des commentaires et des balises sur le document. Passez à la section suivante pour savoir comment ajouter des participants à la révision.

## Ouvrir le résumé du document et affecter des participants

Vous avez la possibilité d’affecter des réviseurs et des approbateurs, ou une combinaison des deux :

* **Les réviseurs** peuvent ajouter des commentaires et marquer les ressources. Une fois l’opération terminée, ils peuvent marquer leur révision comme terminée. Il n’est pas nécessaire de marquer la révision comme terminée pour que le document progresse dans le processus d’approbation.
* Les **approbateurs** peuvent ajouter des commentaires et marquer des ressources. Ils doivent prendre la décision de faire avancer le processus d&#39;approbation.

Pour affecter des participants :

1. Sélectionnez le document que vous avez chargé et ouvrez le résumé du document.
   ![Ouvrir le résumé du document](assets/open-doc-summary.png)

1. Faites défiler jusqu’à la section Validations , puis cliquez sur **Ajouter**.

1. (Facultatif) Choisissez un modèle d’approbation existant. Les utilisateurs disposant d&#39;une licence Standard peuvent créer des modèles d&#39;approbation réutilisables à partir de la zone Configuration. Pour plus d’informations, voir [Créer un modèle d’approbation pour les ressources et les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facultatif) Définissez une date limite pour l’approbation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant l’échéance spécifiée.

1. Pour ajouter un approbateur, cliquez sur le bouton Approbateur et commencez à saisir un nom d’utilisateur ou d’équipe.

1. Pour ajouter un réviseur, cliquez sur le bouton Réviseur et commencez à saisir un nom d’utilisateur ou d’équipe.

   ![Ajouter des approbateurs](assets/add-approvers.png)

1. Une fois que vous avez ajouté tous les réviseurs et approbateurs, cliquez sur **Soumettre la demande**. Les participants sont avertis par e-mail.

## Créez une version selon vos besoins.

Si vous avez besoin d’un autre cycle de révision et d’approbation, vous pouvez créer une nouvelle version de l’épreuve.  <!-- and add the previous participants, new participants, or a mix of both. --> Vous pouvez afficher des informations sur les versions précédentes et les participants dans le résumé du document.

Pour ajouter une nouvelle version :

1. Effectuez un glisser-déposer du nouveau fichier au-dessus du document précédent dans Workfront. Une nouvelle version est automatiquement créée.

1. Une fois le chargement du document terminé, sélectionnez le document, puis cliquez sur **Créer une épreuve** > **Épreuve simple**.

1. Sélectionnez à nouveau le document, puis ouvrez le résumé du document.
   ![Ouvrir le résumé du document](assets/open-doc-summary.png)

1. Faites défiler jusqu’à la section Validations , puis cliquez sur **Ajouter**.

1. (Facultatif) Choisissez un modèle d’approbation existant. Les utilisateurs disposant d&#39;une licence Standard peuvent créer des modèles d&#39;approbation réutilisables à partir de la zone Configuration. Pour plus d’informations, voir [Créer un modèle d’approbation pour les ressources et les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facultatif) Définissez une date limite pour l’approbation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant l’échéance spécifiée.

1. Pour ajouter un approbateur, cliquez sur le bouton Approbateur et commencez à saisir un nom d’utilisateur ou d’équipe<span class="preview"> ou choisissez un approbateur dans la version précédente.</span>

1. Pour ajouter un réviseur, cliquez sur le bouton Réviseur et commencez à saisir un nom d’utilisateur ou d’équipe, <span class="preview">ou choisissez un réviseur à partir de la version précédente. </span>

   ![Ajouter des approbateurs](assets/add-approvers.png)

1. Une fois que vous avez ajouté tous les réviseurs et approbateurs, cliquez sur **Soumettre la demande**. Les participants sont avertis par e-mail.

<!-- add info about reusing previous participants once released -->


## Examinez le BAT et prenez une décision

Le document ne passe pas à un statut approuvé tant que tous les approbateurs affectés n&#39;ont pas choisi « approuvé ».

Si l&#39;un des approbateurs choisit « Travail nécessaire », le statut du document passe immédiatement à Travail nécessaire. Le document devra être révisé et téléchargé en tant que nouvelle version avec un nouveau workflow d’approbation.

>[!IMPORTANT]
>
>Les boutons de décision du document n&#39;apparaissent pas dans le lecteur de vérification. Vous devez revenir à la page Résumé du document ou Détails du document pour prendre une décision ou marquer votre révision comme terminée.

Pour réviser et approuver un document :

1. Accédez à l’e-mail de notification de révision, puis cliquez sur **Accéder à la révision**.

1. Une fois dans Workfront, cliquez sur **Accéder au BAT**.

1. Passez en revue le contenu et ajoutez des commentaires ou des balises. Pour plus d’informations sur l’utilisation de la visionneuse de relecture, voir [Révision de BAT dans Adobe Workfront : index d’article](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Lorsque vous avez terminé votre révision, fermez le lecteur de vérification.

1. Si vous vous trouvez sur la page Détails du document , les boutons de décision se trouvent dans le coin supérieur droit de l’écran.

1. Sélectionnez l’une des décisions suivantes :

   * **Approuver** : le document n’a pas besoin d’être modifié et est prêt à être utilisé.
   * **Approuver avec modifications** : le document nécessite des modifications et est prêt à l’emploi une fois qu’il a été créé. Aucune approbation supplémentaire n’est requise.
   * **Travail nécessaire** : le document doit être modifié et n’est pas prêt à être utilisé. Une fois les modifications spécifiées effectuées, le document doit être téléchargé en tant que nouvelle version et passer par un autre cycle d&#39;approbations. Pour plus d’informations sur le téléchargement d’une nouvelle version, consultez la section [Créer une version si nécessaire](#create-a-new-version-as-needed) dans cet article.

Une fois la décision prise, le propriétaire du document est averti par e-mail.
