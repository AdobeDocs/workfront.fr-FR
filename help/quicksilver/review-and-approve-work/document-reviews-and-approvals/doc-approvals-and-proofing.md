---
product-area: documents
navigation-topic: approvals
title: Utiliser ensemble les nouvelles validations de documents et la vérification
description: Vous pouvez utiliser de nouvelles validations de documents avec la vérification.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 8dc9df69bbce86f141ac451381fcc41a112ca0bc
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 1%

---


# Utiliser ensemble les nouvelles validations de documents et la vérification

Les nouvelles approbations de documents dans Workfront s’accompagnent d’un nouvel ensemble de fonctions qui vous permettent de réviser et d’approuver des documents. Vous pouvez utiliser le nouveau processus d’approbation de documents avec la visionneuse de vérification existante pour ajouter des commentaires et des balises aux documents en révision.

Il existe des différences clés dans le workflow lors de l’utilisation conjointe de nouvelles validations de document et de la vérification :

* Les boutons de décision n’apparaissent pas dans la visionneuse de vérification

* Les participants sont affichés dans le résumé du document, et non dans le workflow de vérification

* Les détails envoyés, ouverts, de commentaire, de décision (SOCD) dans la liste des documents sont liés à la vérification et ne reflètent pas l’état de décision du document.

## Télécharger un document et créer un BAT

1. Accédez au projet, à la tâche ou au problème auquel vous souhaitez ajouter un nouveau document.
1. Cliquez sur l’onglet **Documents** , puis sur le menu déroulant **Ajouter nouveau** .
Ou
Faites glisser et déposez le document dans la liste des documents.

   >[!NOTE]
   >
   >Si **Générer automatiquement des bons à tirer lors du téléchargement de documents** est activé dans votre profil utilisateur, le système crée automatiquement un bon à tirer simple.

1. Passez la souris sur le document, puis cliquez sur le lien **Créer un bon à tirer** qui apparaît sous le nom du document, et sélectionnez **Bon à tirer simple**. Vous devez créer un BAT simple car vous n&#39;utiliserez pas le workflow de validation des validations.

Les utilisateurs affectés en tant que participants peuvent utiliser la visionneuse de vérification pour ajouter des commentaires et des balises au document. Passez à la section suivante pour savoir comment ajouter des participants à la révision.

## Ouvrez le résumé du document et affectez des participants.

Vous avez la possibilité d’affecter des réviseurs, des approbateurs ou un mélange des deux :

* **Les réviseurs** peuvent ajouter des commentaires et marquer des ressources. Une fois la révision terminée, ils peuvent la marquer comme terminée. Le fait de marquer la révision comme terminée n’est pas nécessaire pour que le document puisse avancer dans le processus d’approbation.
* **Les approbateurs** peuvent ajouter des commentaires et marquer des ressources. Ils doivent prendre la décision de faire avancer le processus d’approbation.

Pour affecter des participants :

1. Sélectionnez le document que vous avez téléchargé et ouvrez le résumé du document.
   ![](assets/open-doc-summary.png)

1. Faites défiler l’écran jusqu’à la section Approbations , puis cliquez sur **Ajouter**.

1. (Facultatif) Choisissez un modèle de validation existant. Les utilisateurs disposant d’une licence Standard peuvent créer des modèles d’approbation fiables à partir de la zone Configuration . Pour plus d’informations, voir [Création d’un modèle d’approbation pour les ressources et les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facultatif) Définissez une date limite de validation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date limite spécifiée.

1. Pour ajouter un approbateur, cliquez sur le bouton Approbateur et commencez à saisir le nom d’un utilisateur ou d’une équipe.

1. Pour ajouter un réviseur, cliquez sur le bouton Réviseur et commencez à saisir le nom d’un utilisateur ou d’une équipe.

   ![](assets/add-approvers.png)

1. Une fois que vous avez ajouté tous les réviseurs et approbateurs, cliquez sur **Submit Request**. Les participants sont informés par email.

## Créez une version selon les besoins.

Si vous avez besoin d’un autre cycle de révision et d’approbation, vous pouvez créer une version de BAT.  <!-- and add the previous participants, new participants, or a mix of both. --> Vous pouvez afficher des informations sur les versions précédentes et les participants dans le résumé du document.

Pour ajouter une nouvelle version :

1. Glissez-déposez le nouveau fichier en haut du document précédent dans Workfront. Cela crée automatiquement une nouvelle version.

1. Une fois le téléchargement du document terminé, sélectionnez le document, puis cliquez sur **Créer un BAT** > **BAT simple**.

1. Sélectionnez à nouveau le document, puis ouvrez le résumé du document.
   ![](assets/open-doc-summary.png)

1. Faites défiler l’écran jusqu’à la section Approbations , puis cliquez sur **Ajouter**.

1. (Facultatif) Choisissez un modèle de validation existant. Les utilisateurs disposant d’une licence Standard peuvent créer des modèles d’approbation fiables à partir de la zone Configuration . Pour plus d’informations, voir [Création d’un modèle d’approbation pour les ressources et les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Facultatif) Définissez une date limite de validation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date limite spécifiée.

1. Pour ajouter un approbateur, cliquez sur le bouton Approbateur et commencez à saisir le nom d’un utilisateur ou d’une équipe.

1. Pour ajouter un réviseur, cliquez sur le bouton Réviseur et commencez à saisir le nom d’un utilisateur ou d’une équipe.

   ![](assets/add-approvers.png)

1. Une fois que vous avez ajouté tous les réviseurs et approbateurs, cliquez sur **Submit Request**. Les participants sont informés par email.

<!-- add info about reusing previous participants once released -->


## Vérifier le BAT et prendre une décision

Le document ne passe pas à l’état approuvé tant que tous les approbateurs affectés n’ont pas sélectionné &quot;approuvé&quot;.

Si un approbateur sélectionne &quot;nécessite du travail&quot;, l’état du document passe immédiatement à &quot;Nécessite du travail&quot;. Le document devra être révisé et téléchargé en tant que nouvelle version avec un nouveau workflow d’approbation.

>[!IMPORTANT]
>
>Les boutons de décision de document n’apparaissent pas dans la visionneuse de vérification. Vous devez revenir à la page Résumé du document ou Détails du document pour prendre votre décision ou marquer la fin de votre révision.

Pour réviser et approuver un document :

1. Accédez à votre notification électronique de révision, puis cliquez sur **Aller à la révision**.

1. Une fois que vous êtes dans Workfront, cliquez sur **Aller à BAT**.

1. Passez en revue le contenu et ajoutez des commentaires ou des balises. Pour plus d’informations sur l’utilisation de la visionneuse de vérification, voir [Vérification des bons à tirer dans Adobe Workfront : index de l’article](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Une fois la révision terminée, fermez la visionneuse de vérification.

1. Si vous vous trouvez sur la page Détails du document, les boutons de décision se trouvent dans le coin supérieur droit de l’écran.

1. Choisissez l’une des décisions suivantes :

   * **Approve** : le document n’a pas besoin de modifications et est prêt à l’emploi.
   * **Approuver avec des modifications** : le document nécessite des modifications et est prêt à l’emploi une fois qu’il a été modifié. Aucune validation supplémentaire n’est requise.
   * **Travail requis** : le document nécessite des modifications et n’est pas prêt à l’emploi. Une fois les modifications spécifiées effectuées, le document doit être téléchargé en tant que nouvelle version et passer par un autre cycle de validations. Pour plus d&#39;informations sur le téléchargement d&#39;une nouvelle version, voir [Créer une version selon les besoins](#create-a-new-version-as-needed) dans cet article.

Une fois que vous avez pris une décision, le propriétaire du document est informé par courrier électronique.

