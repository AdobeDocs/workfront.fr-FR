---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configurer des informations sur les utilisateurs et utilisatrices grâce à  [!DNL Workfront Proof]
description: Configurer des informations sur les utilisateurs et utilisatrices grâce à  [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 100%

---

# Configurer des informations sur les utilisateurs et utilisatrices grâce à [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

1. Commencez à créer ou modifier un utilisateur ou une utilisatrice comme décrit dans la section [Créer des utilisateurs et utilisatrices grâce à  [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Indiquez les informations suivantes :

   * Dans la section **[!UICONTROL Détails personnels]**, procédez comme suit :

      * **Adresse e-mail :** adresse e-mail de l’utilisateur ou de l’utilisatrice.
      * **Prénom :** prénom de l’utilisateur ou de l’utilisatrice.
      * **Nom :** nom de l’utilisateur ou de l’utilisatrice.
      * **Position :** position de l’utilisateur ou de l’utilisatrice dans l’entreprise.
      * **Profil d’autorisation :** autorisations de l’utilisateur ou de l’utilisatrice sur le compte d’épreuve.
      * **Langue :** langue principale de l’utilisateur ou de l’utilisatrice.
      * **Fuseau horaire :** sélectionnez le fuseau horaire de l’utilisateur ou de l’utilisatrice.
      * **Format de date :** sélectionnez le format de date préféré de l’utilisateur ou de l’utilisatrice.
      * **Opt-in - E-mails relatifs aux produits et au marketing :** indiquez si l’utilisateur ou l’utilisatrice souhaite recevoir les e-mails relatifs aux produits et au marketing.
      * **API uniquement :** permet à l’utilisateur ou l’utilisatrice de se connecter uniquement via l’API.

   * Dans la section **[!UICONTROL Détails sur l’utilisateur ou l’utilisatrice]**, saisissez les coordonnées de l’utilisateur ou de l’utilisatrice, telles que l’adresse postale et le numéro de téléphone.
   * Dans la section **[!UICONTROL Paramètres par défaut de l’épreuve]**, configurez les paramètres qui affectent la manière dont l’utilisateur ou l’utilisatrice crée ou travaille sur les épreuves.

      * **Rôle d’épreuve par défaut :** sélectionnez un rôle d’épreuve par défaut pour l’utilisateur ou l’utilisatrice. Les options de rôle sont **[!UICONTROL Lecture seule]**, **[!UICONTROL Révision]**, **[!UICONTROL Approbation]**, **[!UICONTROL Révision et approbation]**, **[!UICONTROL Création]** ou **[!UICONTROL Modération]**.

        Pour plus d’informations sur les rôles d’épreuve, consultez [Gestion des rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Verrouiller une épreuve lorsque toutes les décisions sont prises :** verrouille automatiquement l’épreuve contre toute modification ultérieure une fois que toutes les décisions relatives à l’épreuve ont été prises.
      * **Connexion requise. L’épreuve ne peut être partagée qu’avec d’autres utilisateurs et utilisatrices :** rend l’épreuve disponible uniquement pour les utilisateurs et utilisatrices disposant d’informations de connexion [!DNL Workfront Proof].
      * **Une seule décision requise :** nécessite une seule décision sur une épreuve.
      * **Téléchargement du fichier d’origine :** permet à l’utilisateur ou à l’utilisatrice de télécharger le fichier d’origine pour une épreuve. Cette option est activée par défaut.

        Pour plus d’informations sur le téléchargement des fichiers d’origine, consultez [Télécharger des fichiers stockés dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Abonnement. Les personnes peuvent s’inscrire à l’épreuve via l’URL publique ou le code intégré :** permet aux réviseurs et réviseuses externes à l’organisation de s’inscrire à l’épreuve via l’URL publique ou le code intégré.

        Lorsque cette option est sélectionnée, l’option **La personne abonnée doit cliquer sur un lien dans un e-mail pour accéder à une épreuve** est également disponible. Sélectionnez cette option pour demander au réviseur ou à la réviseuse externe de cliquer sur un lien dans l’e-mail pour accéder à l’épreuve.
Cette option est activée par défaut si l’option **Partage public** est sélectionnée.

      * **Rôle par défaut pour les nouveaux réviseurs et réviseuses invités :** sélectionnez un rôle de l’épreuve par défaut pour les réviseurs et réviseuses invités. Les options sont identiques à celles dans **Rôle de l’épreuve par défaut**, à l’exception de Modération et de Création.

   * Dans la section **[!UICONTROL Paramètres d’alerte par e-mail par défaut]**, procédez comme suit :

      * **Alerte par e-mail par défaut :** sélectionnez la fréquence à laquelle l’utilisateur ou l’utilisatrice reçoit des mises à jour par e-mail. Sélectionnez **Toutes les activités, réponses à mes commentaires, décisions, décision finale, résumé horaire, résumé quotidien,** ou **Désactivé**.

        Pour plus d’informations sur les options d’alerte par e-mail par défaut, consultez [Configurer les paramètres de notification par e-mail dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

      * **Alertes par e-mail par défaut pour les nouveaux réviseurs et réviseuses invités :** sélectionnez la fréquence à laquelle les réviseurs et réviseuses invités reçoivent les mises à jour par e-mail. Les options sont identiques à celles de **Alerte par e-mail par défaut.**

      * **Envoyer un e-mail de confirmation lorsque les épreuves sont prêtes :** sélectionnez cette option pour envoyer automatiquement à l’utilisateur ou l’utilisatrice un e-mail de confirmation lorsque les épreuves sont prêtes.
      * **Format des e-mails envoyés à cet utilisateur ou cette utilisatrice :** sélectionnez **[!UICONTROL HTML]** ou **[!UICONTROL Texte brut]** comme format par défaut des e-mails envoyés à l’utilisateur ou l’utilisatrice.

   * Dans la section **[!UICONTROL Paramètres des messages personnalisés]** : créez des paramètres pour les modèles d’épreuve.

     Pour plus d’informations sur les modèles, consultez ce qui suit :

      * **Modèle d’objet d’épreuve :** créez un modèle pour l’objet d’épreuve.
      * **Modèle de message d’épreuve :** créez un modèle pour un message d’épreuve et son format.
