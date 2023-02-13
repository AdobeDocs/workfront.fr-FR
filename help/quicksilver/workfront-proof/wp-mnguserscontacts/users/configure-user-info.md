---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configuration des informations utilisateur à l’aide de [!DNL Workfront Proof]
description: Configuration des informations utilisateur à l’aide de [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Configuration des informations utilisateur à l’aide de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

1. Commencez à créer ou modifier un utilisateur comme décrit dans la section [Création d’utilisateurs à l’aide de [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Indiquez les informations suivantes :

   * Dans le **[!UICONTROL Détails personnels]** section :

      * **Adresse électronique :** Adresse électronique de l’utilisateur.
      * **Prénom :** Prénom de l’utilisateur.
      * **Nom :** Nom de l’utilisateur.
      * **Position :** Position de l’utilisateur dans la société.
      * **Profil d’autorisation :** Autorisations de l’utilisateur sur le compte BAT.
      * **Langue :** La langue Principale de l’utilisateur.
      * **Fuseau horaire :** Sélectionnez le fuseau horaire de l’utilisateur.
      * **Format de date :** Sélectionnez le format de date préféré de l’utilisateur.
      * **Accord préalable - emails de produit et marketing :** Indiquez si l’utilisateur doit accepter les courriers électroniques de produit et de marketing.
      * **API uniquement :** Permet à l’utilisateur de se connecter uniquement via l’API.
   * Dans le **[!UICONTROL Détails de l’utilisateur]** , saisissez les coordonnées de l’utilisateur, telles que l’adresse postale et le numéro de téléphone.
   * Dans le **[!UICONTROL Paramètres de BAT par défaut]** , configurez les paramètres qui affectent la manière dont l’utilisateur crée ou fonctionne sur les bons à tirer.

      * **Rôle de BAT par défaut :** Sélectionnez un rôle de BAT par défaut pour l’utilisateur. Les options de rôle sont **[!UICONTROL Lecture seule]**, **[!UICONTROL Réviseur]**, **[!UICONTROL Approbateur]**, **[!UICONTROL Réviseur et approbateur]**, **[!UICONTROL Auteur]** ou **[!UICONTROL Modérateur]**.

         Pour plus d’informations sur les rôles de BAT, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Verrouillez le BAT lorsque toutes les décisions sont prises :** Verrouille automatiquement le BAT d’autres modifications une fois toutes les décisions prises sur le BAT.
      * **Connexion requise. Le BAT ne peut être partagé qu&#39;avec d&#39;autres utilisateurs :** Rend le BAT disponible uniquement pour les utilisateurs disposant de [!DNL Workfront Proof] informations de connexion.
      * **Une seule décision requise :** Nécessite une seule décision sur un BAT.
      * **Téléchargement du fichier d’origine :** Permet à l’utilisateur de télécharger le fichier d’origine pour un BAT. Cette option est activée par défaut.

         Pour plus d’informations sur le téléchargement des fichiers originaux, voir [Téléchargement des fichiers stockés dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

         <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Abonnement. Les personnes peuvent s&#39;inscrire au BAT via l&#39;URL publique ou le code intégré :** Permet aux réviseurs externes à l’organisation de s’inscrire au BAT via l’URL publique ou le code intégré.

         Lorsque cette option est sélectionnée, **L&#39;abonné doit cliquer sur un lien dans un email pour accéder à un BAT** est également disponible. Sélectionnez cette option pour obliger le validant externe à cliquer sur un lien dans l&#39;email pour accéder au BAT.
Cette option est activée par défaut si la variable **Partage public** est sélectionnée.

      * **Rôle par défaut pour les nouveaux réviseurs invités :** Sélectionnez un rôle de BAT par défaut pour les réviseurs invités. Les options sont identiques à celles de la variable **Rôle de BAT par défaut.**
   * Dans le **[!UICONTROL Paramètres d’alerte par défaut]** section :

      * **Alerte par défaut :** Sélectionnez la fréquence à laquelle l’utilisateur reçoit les mises à jour par courrier électronique. Sélectionner **Toutes les activités, Réponses à mes commentaires, décisions, décision finale, résumé horaire, résumé quotidien,** ou **Désactivé**.

         Pour plus d’informations sur les options d’alerte par défaut, voir [Configuration des paramètres de notification électronique dans [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Alertes par défaut pour les nouveaux réviseurs invités :** Sélectionnez la fréquence à laquelle les réviseurs invités reçoivent les mises à jour des emails. Les options sont identiques à celles de **Alerte par défaut.**

      * **Envoyez un email de confirmation lorsque les bons à tirer sont prêts :** Sélectionnez cette option pour envoyer automatiquement à l’utilisateur un email de confirmation lorsque les bons à tirer sont prêts.
      * **Format des emails envoyés à cet utilisateur :** Sélectionner **[!UICONTROL HTML]** ou **[!UICONTROL Texte brut]** comme format par défaut des emails envoyés à l’utilisateur.
   * Dans le **[!UICONTROL Paramètres des messages personnalisés]** section : Créez des paramètres pour les modèles de BAT.

      Pour plus d’informations sur les modèles, voir :

      * **Modèle d’objet du bon à tirer :** Créez un modèle pour l’objet du BAT.
      * **Modèle de message de BAT :** Créez un modèle pour un message de BAT et son format.
