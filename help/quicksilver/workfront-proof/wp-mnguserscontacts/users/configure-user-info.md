---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Configuration des informations utilisateur à l’aide de [!DNL Workfront Proof]
description: Configuration des informations utilisateur à l’aide de [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 1%

---

# Configuration des informations utilisateur à l’aide de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

1. Commencez à créer ou modifier un utilisateur comme décrit dans [Créer des utilisateurs à l’aide de [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Indiquez les informations suivantes :

   * Dans la section **[!UICONTROL Personal Details]** :

      * **Adresse électronique :** adresse électronique de l’utilisateur.
      * **Prénom :** prénom de l’utilisateur.
      * **Nom :** Nom de l’utilisateur.
      * **Position :** position de l’utilisateur dans la société.
      * **Profil d’autorisation :** autorisations de l’utilisateur sur le compte du BAT.
      * **Langue :** Langue principale de l’utilisateur.
      * **Fuseau horaire :** sélectionnez le fuseau horaire de l’utilisateur.
      * **Format de date :** sélectionnez le format de date préféré de l’utilisateur.
      * **Opt-in - email de produit et de marketing :** Indiquez si l’utilisateur doit opt-in pour les emails de produit et marketing.
      * **API uniquement :** Permet à l’utilisateur de se connecter uniquement via l’API.

   * Dans la section **[!UICONTROL User Details]**, saisissez les coordonnées de l’utilisateur, telles que l’adresse postale et le numéro de téléphone.
   * Dans la section **[!UICONTROL Paramètres par défaut du BAT]**, configurez les paramètres qui affectent la manière dont l’utilisateur crée ou travaille sur des BAT.

      * **Rôle de BAT par défaut :** Sélectionnez un rôle de BAT par défaut pour l’utilisateur. Les options de rôle sont **[!UICONTROL Lecture seule]**, **[!UICONTROL Réviseur]**, **[!UICONTROL Approbateur]**, **[!UICONTROL Réviseur et approbateur]**, **[!UICONTROL Auteur]** ou **[!UICONTROL Modérateur]**.

        Pour plus d’informations sur les rôles de BAT, voir [Gestion des rôles de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Verrouiller le BAT lorsque toutes les décisions sont prises :** verrouille automatiquement le BAT d’autres modifications une fois toutes les décisions du BAT effectuées.
      * **Connexion requise. Le BAT ne peut être partagé qu’avec d’autres utilisateurs :** met le BAT à la disposition des utilisateurs disposant des informations de connexion [!DNL Workfront Proof].
      * **Une seule décision requise :** nécessite une seule décision sur un BAT.
      * **Téléchargement du fichier d’origine :** permet à l’utilisateur de télécharger le fichier d’origine pour un BAT. Cette option est activée par défaut.

        Pour plus d’informations sur le téléchargement des fichiers originaux, voir [Téléchargement des fichiers stockés dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Abonnement. Les personnes peuvent s’inscrire au BAT via l’URL publique ou le code incorporé :** Permet aux réviseurs externes à l’organisation de s’inscrire au BAT via l’URL publique ou le code incorporé.

        Lorsque cette option est sélectionnée, **L&#39;abonné doit cliquer sur un lien dans un email pour accéder à un BAT** est également disponible. Sélectionnez cette option pour obliger le validant externe à cliquer sur un lien dans l&#39;email pour accéder au BAT.
Cette option est activée par défaut si l’option **Partage public** est sélectionnée.

      * **Rôle par défaut pour les nouveaux réviseurs invités :** Sélectionnez un rôle de BAT par défaut pour les réviseurs invités. Les options sont identiques à celles du **rôle de BAT par défaut**, à l’exception du modérateur et de l’auteur.

   * Dans la section **[!UICONTROL Paramètres d’alerte par défaut]** :

      * **Alerte par défaut :** sélectionnez la fréquence à laquelle l’utilisateur reçoit des mises à jour de courrier électronique. Sélectionnez **Toutes les activités, Réponses à mes commentaires, Décisions, Décision finale, Résumé horaire, Résumé quotidien,** ou **Désactivé**.

        Pour plus d’informations sur les options d’alerte par défaut, voir [Configuration des paramètres de notification électronique dans [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Alerte par défaut pour les nouveaux réviseurs invités :** Sélectionnez la fréquence à laquelle les réviseurs invités reçoivent des mises à jour de courrier électronique. Les options sont identiques à celles de **Alerte par défaut.**

      * **Envoyez un email de confirmation lorsque les bons à tirer sont prêts :** Sélectionnez cette option pour envoyer automatiquement à l’utilisateur un email de confirmation lorsque les bons à tirer sont prêts.
      * **Format des emails envoyés à cet utilisateur :** Sélectionnez **[!UICONTROL HTML]** ou **[!UICONTROL Texte brut]** comme format par défaut pour les emails envoyés à l’utilisateur.

   * Dans la section **[!UICONTROL Paramètres de message personnalisés]** : créez des paramètres pour les modèles de BAT.

     Pour plus d’informations sur les modèles, voir :

      * **Modèle d’objet BAT :** Créez un modèle pour un objet BAT.
      * **Modèle de message BAT :** Créez un modèle pour un message BAT et son format.
