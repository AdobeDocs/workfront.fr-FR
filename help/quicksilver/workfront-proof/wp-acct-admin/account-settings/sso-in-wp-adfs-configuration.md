---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Authentification unique dans  [!DNL Workfront Proof] : configuration AD FS'
description: Si vous êtes administrateur ou administratrice sur votre serveur AD, vous pouvez installer et configurer AD FS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: 690b0817dfe4ff200982ffe8d67ad93e563e30ac
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 99%

---

# SSO dans [!DNL Workfront Proof] : configuration AD FS

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Si vous êtes administrateur ou administratrice sur votre serveur AD, vous pouvez installer et configurer AD FS.

## Installer et configurer AD FS

1. Téléchargez Microsoft AD FS 2.0 sur votre ordinateur.
1. Ouvrez le fichier AdfsSetup.exe téléchargé pour démarrer l’assistant d’installation ADFS (Active Directory Federation Services).
1. Dans l’écran Rôle du serveur, sélectionnez l’une des options (vous avez besoin au minimum d’un serveur de fédération).
1. Si vous ne souhaitez pas exposer IIS sur votre serveur AD à Internet (ports 80 et 443 pour HTTP et HTTPS), vous pouvez d’abord configurer un serveur de fédération derrière le pare-feu, puis créer un second proxy de serveur de fédération qui transmet les demandes via le pare-feu au serveur de fédération.
1. Une fois la configuration d’AD FS terminée, sélectionnez **[!UICONTROL Démarrer le composant logiciel enfichable Gestion d’AD FS 2.0]**, puis cliquez sur **[!UICONTROL Terminer]**. Une fois cette opération terminée, la fenêtre Gestion d’AD FS 2.0 doit s’ouvrir immédiatement. Dans le cas contraire, vous pouvez l’ouvrir à partir de **[!UICONTROL Démarrer]** > **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion d’AD FS 2.0]**. Il s’agit de la principale application de contrôle AD FS.

1. Commencez par cliquer sur Assistant de configuration du serveur de fédération AD FS 2.0.
Cela vous aidera à configurer AD FS et à le connecter à Internet via IIS et à AD.
1. Si vous configurez un nouveau serveur AD FS, sélectionnez **[!UICONTROL Créer un service de fédération]**.
1. Sélectionnez **[!UICONTROL Serveur de fédération autonome]** (à des fins de test et d’évaluation).

1. Pour une haute disponibilité et un équilibrage de charge, cliquez sur Nouvelle batterie de serveurs de fédération.
1. Indiquez le nom de votre service de fédération.
Par défaut, l’assistant de configuration récupère le certificat SSL associé au site web par défaut dans IIS et utilise le nom d’objet qui y est indiqué. Si vous utilisez un certificat générique, vous devez saisir le nom du service de fédération.
Si aucun certificat SSL n’est configuré dans IIS, l’assistant de configuration recherche dans la boutique de certificats de l’ordinateur local les certificats valides. Ils s’affichent dans la liste déroulante des certificats SSL. Si aucun certificat n’a été trouvé, vous pouvez utiliser le générateur de certificats du serveur dans IIS pour en créer un.

1. Poursuivez la configuration, puis cliquez sur **[!UICONTROL Fermer]** une fois l’opération terminée.

## Configurer la SSO pour [!DNL Workfront Proof]

Si vous êtes administrateur ou administratrice [!DNL Workfront Proof], vous pouvez configurer l’authentification unique du côté de [!DNL Workfront Proof]. Pour plus d’informations, voir [SSO dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]**, puis ouvrez l’onglet **[!UICONTROL Authentification unique]**.

1. Dans la boîte **URL SSO**, collez votre identifiant d’entité.
Voici un exemple d’identifiant d’entité :
http://*&lt;adfs.your-company.com>*/adfs/services/trust
Votre identifiant d’entité se trouve dans votre fichier XML de métadonnées de fédération.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. Les métadonnées de fédération se trouvent dans le dossier Composant logiciel enfichable AD FS 2.0 > Service > Points d’entrée. Dans la section Métadonnées, recherchez celles qui possèdent le type de métadonnées de fédération. Pour afficher les métadonnées, collez ce point d’entrée dans votre navigateur. Vous pouvez également accéder directement à ce lien : https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml après avoir remplacé {adfs.your-company.com} par vos propres détails.
1. Dans la zone **[!UICONTROL URL de connexion]**, collez votre connexion SSO.
1. Voici un exemple de connexion SSO :
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Ce lien se trouve dans le fichier XML des métadonnées de fédération.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. Dans la boite **[!UICONTROL URL de déconnexion]**, saisissez le lien et enregistrez.
Voici un exemple d’URL de déconnexion :
https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Accédez à votre gestionnaire AD FS > Relations de confiance > Parties de confiance - propriétés ProofHQ.
   1. Sous Points d’entrée, cliquez sur [!UICONTROL Ajouter et saisir] avec les détails suivants :

      * Type de point d’entrée = Déconnexion SAML
      * Liaison = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * Cette étape peut être effectuée après la configuration de la Partie de confiance (voir ci-dessous) dans votre AD FS.
   1. Dans la zone **[!UICONTROL Empreinte du certificat]**, saisissez les données de votre certificat.
   1. Dans votre service ADFS 2.0, accédez à Service > Certificats > Signature des jetons.
   1. Cliquez avec le bouton droit de la souris sur cette entrée pour afficher le certificat.
   1. Dans l’onglet [!UICONTROL Détails du certificat], copiez l’empreinte puis collez-la dans l’onglet de configuration **[!UICONTROL Authentification unique Workfront Proof]**.

   1. Les caractères de l’empreinte peuvent être séparés par des deux-points ou des espaces, mais nous vous recommandons de supprimer ces séparateurs. Si vous rencontrez des problèmes avec la configuration de votre authentification unique, contactez l’équipe de l’assistance clientèle.


## Ajouter une Partie de confiance

Une fois la configuration terminée, vous devez travailler dans la section Parties de confiance dans votre AD FS.

1. Accédez au dossier **[!UICONTROL Relations de confiance]** > **[!UICONTROL Parties de confiance]**, puis cliquez sur **[!UICONTROL Ajouter une partie confiance]** pour lancer l’assistant de configuration.

1. Sélectionnez votre source de données.
Toutes les métadonnées de votre compte [!DNL ProofHQ] sont accessibles via un lien comme celui-ci :
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
Cela effectue la majorité de la configuration de la partie de confiance.

   >[!NOTE]
   >
   >* Si vous rencontrez des problèmes lors de l’établissement de la connexion à partir de l’URL, enregistrez les métadonnées sous forme de fichier et choisissez d’importer les données à partir d’un fichier.
   >* Si vous disposez d’un domaine personnalisé complet (par exemple, www.votre-relecture.com) configuré sur votre compte [!DNL ProofHQ] remplacez tout la partie « {yoursubdomain}.proofhq.com » par votre propre domaine pour créer votre lien de métadonnées [!DNL ProofHQ].


## Configurer des règles de revendication

Une fois la configuration de la partie de confiance terminée, vous êtes en mesure de configurer les règles de revendication pour terminer la configuration. Vous allez configurer deux règles de revendication pour ProofHQ : E-mail et Identifiant nom.

1. Ouvrez la boîte de dialogue **[!UICONTROL Modifier des règles de revendication]**.
1. Accédez à **[!UICONTROL Partie de confiance ProofHQ]**, puis cliquez sur **[!UICONTROL Modifier des règles de revendication]** (1).\
   La fenêtre contextuelle doit s’ouvrir automatiquement si vous avez sélectionné cette option à la fin de la configuration de la partie de confiance.

1. Cliquez sur **[!UICONTROL Ajouter une règle]** (2) pour ouvrir la fenêtre de configuration des revendications.

   * E-mail (envoyer des attributs LDAP en tant que modèle de règle de revendications)
   * Identifiant nom (transformer un modèle de règle de revendication entrante)
