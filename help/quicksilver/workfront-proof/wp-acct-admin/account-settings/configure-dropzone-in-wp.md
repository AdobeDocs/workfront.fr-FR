---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Configuration de la zone de dépôt dans [!DNL Workfront Proof]
description: En tant qu'administrateur  [!DNL Workfront Proof] , vous pouvez définir, afficher et modifier les paramètres de zone de dépôt de vos utilisateurs. Pour plus d’informations sur la zone de dépôt, voir Zone de dépôt.
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
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

En tant qu’administrateur [!DNL Workfront Proof], vous pouvez définir, afficher et modifier les paramètres de zone de dépôt de vos utilisateurs. Pour plus d’informations sur Dropzone, voir [The Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]**, puis ouvrez l’onglet **[!UICONTROL Zone de dépôt]** .

1. Apportez l’une des modifications suivantes à la section **[!UICONTROL Détails de la zone de dépôt]** :

   * **[!UICONTROL Zone de dépôt web]** : activez ou désactivez la zone de dépôt.
   * **[!UICONTROL URL de zone de dépôt web]** : URL que vous devez entrer dans votre navigateur pour envoyer des bons à tirer via la zone de dépôt.
   * **[!UICONTROL Zone de dépôt des emails]** : activez ou désactivez la zone de dépôt des emails.

     >[!NOTE]
     >
     >L’envoi par courrier électronique aux zones de dépôt n’est plus pris en charge.

   * **[!UICONTROL Propriétaire de la zone de dépôt]** : définissez ou modifiez le propriétaire de la zone de dépôt. Il s’agit de la personne qui sera informée des nouvelles soumissions à la zone de dépôt. Pour être défini comme propriétaire de la zone de dépôt, l’utilisateur doit être un responsable, un administrateur, un administrateur de facturation ou le créateur du compte. Pour plus d’informations, voir [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Rôle par défaut pour les créateurs]** : tous les envoyeurs sont ajoutés au BAT avec ce rôle par défaut.
   * **[!UICONTROL Notification par e-mail pour tous les créateurs]** : définissez ici les préférences d’alerte par e-mail pour les créateurs de BAT (soumis). Voir [Configuration des paramètres de notification électronique dans [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) pour plus d’informations sur les différents paramètres d’alerte disponibles.

   * **[!UICONTROL Nouvelle fonction de version]** : activez et désactivez la fonction Nouvelle version sur Dropzone. Cela permet aux utilisateurs d’envoyer de nouvelles versions de BAT via la zone de dépôt, ou les supprime.
   * **[!UICONTROL Supprimer les BAT de brouillon après (jours)]** : spécifiez le nombre de jours après lesquels un BAT de brouillon sera supprimé. Les bons à tirer restent en état de brouillon si l’envoi de la zone de dépôt n’est pas terminé après le téléchargement du fichier vers la zone de dépôt.
   * **[!UICONTROL Masquer le rôle de réviseur]** : masquez le champ rôle de réviseur lors de l’ajout de personnes à la zone de dépôt.
   * **[!UICONTROL Envoyer le message du BAT lors de l&#39;activation]** : configurez [!DNL Workfront Proof] pour envoyer automatiquement aux réviseurs des e-mails de notification du BAT lorsqu&#39;un BAT est activé.
   * **[!UICONTROL Activer le BAT lors de l’envoi]** : configurez [!DNL Workfront Proof] pour activer automatiquement les bons à tirer lors de l’envoi (supprimant la nécessité de les activer manuellement).

   * Si un BAT est déplacé hors de la zone de dépôt (par exemple, vers un autre dossier de votre compte), les paramètres de la zone de dépôt ne s’appliqueront plus au BAT. Ceci est particulièrement important pour les paramètres d’alerte par email.

1. Apportez toute modification à la section **[!UICONTROL Champs de la zone de dépôt]** pour spécifier les champs qui s’affichent dans la section [!UICONTROL  Détails du bon à tirer] de la page d’envoi de la zone de dépôt lorsque les bons à tirer sont envoyés par l’intermédiaire de la zone de dépôt.
1. Dans la section **[!UICONTROL Domaines autorisés]** , spécifiez les domaines que vous souhaitez autoriser à utiliser la zone de dépôt.

   * Vous pouvez cliquer sur **[!UICONTROL Ajouter un domaine]** pour ajouter un domaine. Lorsque vous avez terminé d’ajouter les détails du domaine, cliquez sur **[!UICONTROL Enregistrer]**.

   * Vous pouvez **[!UICONTROL Modifier]** et **[!UICONTROL Supprimer]** tous les domaines existants que vous avez ajoutés précédemment.

1. Sous **[!UICONTROL Personnes à avertir]**, spécifiez les personnes que vous souhaitez avertir avec le propriétaire de la zone de dépôt lorsque de nouveaux bons à tirer sont envoyés à la zone de dépôt [La zone de dépôt](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Cliquez sur **[!UICONTROL Ajouter des personnes]**, entrez les détails du destinataire, puis cliquez sur **[!UICONTROL Enregistrer]**.

   * **[!UICONTROL Supprimez]** les personnes que vous avez déjà ajoutées.
