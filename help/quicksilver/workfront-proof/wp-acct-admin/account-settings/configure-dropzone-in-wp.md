---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configuration de la zone de dépôt dans [!DNL Workfront Proof]
description: Comme [!DNL Workfront Proof] administrateur, vous pouvez définir, afficher et modifier les paramètres de zone de dépôt de vos utilisateurs. Pour plus d’informations sur la zone de dépôt, voir Zone de dépôt.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Configuration de la zone de dépôt dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Comme [!DNL Workfront Proof] administrateur, vous pouvez définir, afficher et modifier les paramètres de zone de dépôt de vos utilisateurs. Pour plus d’informations sur Dropzone, voir [Zone de dépôt](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]**, puis ouvrez le **[!UICONTROL Zone de dépôt]** .

1. Apportez l’une des modifications suivantes dans le **[!UICONTROL Détails de la zone de dépôt]** section :

   * **[!UICONTROL Zone de dépôt web]**: Activez ou désactivez la zone de dépôt.
   * **[!UICONTROL URL de la zone de dépôt Web]**: URL que vous devez entrer dans votre navigateur pour envoyer des BAT via la zone de dépôt.
   * **[!UICONTROL Zone de dépôt des emails]**: Activez ou désactivez la zone de dépôt des emails.

      >[!NOTE]
      >
      >L’envoi d’emails aux zones de dépôt n’est plus pris en charge.

   * **[!UICONTROL Propriétaire de la zone de dépôt]**: Définissez ou modifiez le propriétaire de la zone de dépôt. Il s’agit de la personne qui sera informée des nouvelles soumissions à la zone de dépôt. Pour être défini comme propriétaire de la zone de dépôt, l’utilisateur doit être un responsable, un administrateur, un administrateur de facturation ou le créateur du compte. Pour plus d’informations, voir [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Rôle par défaut pour les créateurs]**: Tous les émetteurs sont ajoutés au BAT avec ce rôle comme valeur par défaut.
   * **[!UICONTROL Notification par e-mail pour tous les créateurs]**: Définissez ici la préférence d’alerte par email pour les créateurs de BAT (soumetteurs). Voir [Configuration des paramètres de notification électronique dans [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) pour plus d’informations sur les différents paramètres d’alerte disponibles.

   * **[!UICONTROL Nouvelle fonction de version]**: Activez et désactivez la fonction Nouvelle version sur la zone de dépôt. Cela permet aux utilisateurs d’envoyer de nouvelles versions de BAT via la zone de dépôt, ou les supprime.
   * **[!UICONTROL Supprimer les BAT de brouillon après (jours)]**: Indiquez le nombre de jours après lesquels un brouillon de BAT sera supprimé. Les bons à tirer restent en état de brouillon si l’envoi de la zone de dépôt n’est pas terminé après le téléchargement du fichier vers la zone de dépôt.
   * **[!UICONTROL Masquer le rôle de réviseur]**: Masquez le champ Rôle de réviseur lors de l’ajout de personnes à la zone de dépôt.
   * **[!UICONTROL Envoyer le message du BAT lors de l’activation]**: Configurer [!DNL Workfront Proof] pour envoyer automatiquement aux opérateurs validants des emails de notification de BAT lorsqu&#39;un BAT est activé.
   * **[!UICONTROL Activer le BAT lors de l’envoi]**: Configurer [!DNL Workfront Proof] pour activer automatiquement les bons à tirer lors de l’envoi (en supprimant la nécessité de les activer manuellement).

   * Si un BAT est déplacé hors de la zone de dépôt (par exemple, vers un autre dossier de votre compte), les paramètres de la zone de dépôt ne s’appliqueront plus au BAT. Ceci est particulièrement important pour les paramètres d’alerte par email.

1. Apportez toute modification dans le **[!UICONTROL Champs de zone de dépôt]** pour spécifier les champs qui s’affichent dans la section [!UICONTROL Détails du BAT] de la page d’envoi Zone de dépôt lorsque les bons à tirer sont envoyés via la zone de dépôt.
1. Dans le **[!UICONTROL Domaines autorisés]** , spécifiez les domaines que vous souhaitez autoriser à utiliser la zone de dépôt.

   * Vous pouvez cliquer sur **[!UICONTROL Ajouter un domaine]** pour ajouter un domaine. Une fois l’ajout des détails du domaine terminé, cliquez sur **[!UICONTROL Enregistrer]**.

   * Vous pouvez **[!UICONTROL Modifier]** et **[!UICONTROL Supprimer]** tous les domaines existants que vous avez ajoutés précédemment.

1. Sous **[!UICONTROL Personnes à avertir]**, spécifiez les personnes que vous souhaitez avertir avec le propriétaire de la zone de dépôt lorsque de nouveaux bons à tirer sont envoyés à la zone de dépôt. [Zone de dépôt](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Cliquez sur **[!UICONTROL Ajouter des personnes]**, saisissez les détails du destinataire, puis cliquez sur **[!UICONTROL Enregistrer]**.

   * **[!UICONTROL Supprimer]** les personnes que vous avez déjà ajoutées.
