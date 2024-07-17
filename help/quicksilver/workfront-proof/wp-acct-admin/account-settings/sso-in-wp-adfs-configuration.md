---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Connexion unique en [!DNL Workfront Proof] : configuration AD FS'
description: Si vous êtes administrateur sur votre serveur AD, vous pouvez installer et configurer AD FS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Connexion unique dans [!DNL Workfront Proof] : configuration AD FS

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Si vous êtes administrateur sur votre serveur AD, vous pouvez installer et configurer AD FS.

## Installation et configuration d’AD FS

1. Téléchargez [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) sur votre ordinateur.
1. Ouvrez le fichier AdfsSetup.exe téléchargé pour démarrer l’assistant d’installation ADFS (Active Directory Federation Services).
1. Dans l’écran Rôle du serveur , sélectionnez l’une des options (vous avez besoin d’un serveur de fédération au minimum).
1. Si vous ne souhaitez pas exposer IIS sur votre serveur AD à Internet (ports 80 et 443 pour HTTP et HTTPS), vous pouvez d’abord configurer un serveur de fédération derrière le pare-feu, puis créer un second proxy de serveur de fédération qui transmet les requêtes via le pare-feu au serveur de fédération.
1. Une fois la configuration AD FS terminée, sélectionnez **[!UICONTROL Démarrer le module de gestion AD FS 2.0]**, puis cliquez sur **[!UICONTROL Terminer]**. Une fois cette opération terminée, la fenêtre Gestion AD FS 2.0 doit s’ouvrir immédiatement. Dans le cas contraire, vous pouvez l’ouvrir à partir de **[!UICONTROL Démarrer]** > **[!UICONTROL Outils d’administration]** > **[!UICONTROL Gestion AD FS 2.0]**. Il s’agit de la principale application de contrôle AD FS.

1. Commencez par cliquer sur Assistant de configuration du serveur de fédération AD FS 2.0.
Cela vous aidera à configurer AD FS et à le connecter à Internet via IIS et à AD.
1. Si vous configurez un nouveau serveur AD FS, sélectionnez **[!UICONTROL Create a new Federation Service]**.
1. Sélectionnez **[!UICONTROL Serveur de fédération autonome]** (à des fins de test et d’évaluation).

1. Pour une haute disponibilité et un équilibrage de charge, cliquez sur Nouvelle batterie de serveurs de fédération.
1. Indiquez le nom de votre service de fédération.
Par défaut, l&#39;assistant de configuration récupère le certificat SSL associé au site Web par défaut dans IIS et utilise le nom d&#39;objet qui y est spécifié. Si vous utilisez un certificat générique, vous devez saisir le nom du service de fédération.
Si aucun certificat SSL n’est configuré dans IIS, l’assistant de configuration recherche dans la boutique de certificats de l’ordinateur local les certificats valides. Ils s’affichent dans la liste déroulante des certificats SSL. Si aucun certificat n’a été trouvé, vous pouvez utiliser le générateur de certificats du serveur dans IIS pour en créer un.

1. Poursuivez la configuration, puis cliquez sur **[!UICONTROL Fermer]** une fois la configuration terminée.

## Configuration de l’authentification unique [!DNL Workfront Proof]

Si vous êtes administrateur [!DNL Workfront Proof], vous pouvez configurer l’authentification unique du côté [!DNL Workfront Proof]. Pour plus d’informations, voir [Connexion unique dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]**, puis ouvrez l’onglet **[!UICONTROL Connexion unique]** .

1. Dans la zone **URL SSO**, collez votre ID d’entité.
Voici un exemple d’identifiant d’entité :
http://*&lt;adfs.your-company.com>*/adfs/services/trust
Votre ID d’entité se trouve dans votre fichier XML de métadonnées de fédération.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. Les métadonnées de fédération se trouvent dans le dossier du composant logiciel enfichable AD FS 2.0 > Service > Points de fin . Dans la section Métadonnées , recherchez celle qui possède le type de métadonnées de fédération . Pour afficher les métadonnées, collez ce point de terminaison dans votre navigateur. Vous pouvez également accéder directement à ce lien : https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml après avoir remplacé le fichier {adfs.your-company.com} par vos propres détails.
1. Dans la zone **[!UICONTROL Login URL]**, collez votre connexion SSO.
1. Voici un exemple de connexion SSO :
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Ce lien se trouve dans le fichier XML des métadonnées de fédération.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. Dans la zone **[!UICONTROL URL de déconnexion]**, saisissez le lien et enregistrez.
Voici un exemple d’URL de déconnexion :
https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Accédez à votre gestionnaire AD FS > Relations de confiance > Approbation de partie de confiance - propriétés ProofHQ.
   1. Sous Points de fin, cliquez sur [!UICONTROL Ajouter et entrer] avec les détails suivants :

      * Type de point d’entrée = Déconnexion SAML
      * Liaison = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * Cette étape peut être effectuée après la configuration de l’Approbation de partie de confiance (voir ci-dessous) dans votre AD FS.
   1. Dans la zone **[!UICONTROL Certificate empreinte]**, saisissez les données de votre certificat.
   1. Accédez à votre composant logiciel enfichable ADFS 2.0 à Service > Certificats > Signature des jetons.
   1. Cliquez avec le bouton droit sur cette entrée pour afficher le certificat.
   1. Dans l’onglet [!UICONTROL  Certificate Details], copiez l’empreinte numérique et collez-la dans l’onglet de configuration **[!UICONTROL Authentification unique Workfront Proof]**.

   1. Les caractères d’empreinte peuvent être séparés par des deux-points ou des espaces, mais nous vous recommandons de les supprimer. Si vous rencontrez des problèmes avec votre configuration de connexion unique, contactez l’équipe d’assistance clientèle.


## Ajouter une confiance du parti de confiance

Une fois la configuration terminée, vous devez travailler dans la section Fidélisation dans votre AD FS.

1. Accédez au dossier **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trust]** , puis cliquez sur **[!UICONTROL Add a Relying Party Trust]** pour lancer l’assistant de configuration.

1. Sélectionnez votre source de données.
Toutes les métadonnées de votre compte [!DNL ProofHQ] se trouvent sous un lien comme celui-ci :
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
Cela va configurer la plus grande partie de la confiance du Parti qui dépend.

   >[!NOTE]
   >
   >* Si vous rencontrez des problèmes lors de l’établissement de la connexion à partir de l’URL, enregistrez les métadonnées sous forme de fichier et choisissez d’importer les données d’un fichier.
   >* Lorsque vous avez un domaine personnalisé complet (par exemple, www.your-proofing.com) configuré sur votre compte [!DNL ProofHQ], remplacez la partie &quot;{yoursubdomain}.proofhq.com&quot; entière par votre propre domaine pour créer votre lien de métadonnées [!DNL ProofHQ].


## Configuration des règles de réclamation

Une fois la configuration Approbation de partie de confiance terminée, vous êtes prêt à configurer les règles de réclamation pour terminer la configuration. Vous allez configurer deux règles de réclamation pour ProofHQ : Email et Nom ID.

1. Ouvrez la boîte de dialogue **[!UICONTROL Modifier les règles de réclamation]** .
1. Accédez à **[!UICONTROL ProofHQ Relying Party Trust]**, puis cliquez sur **[!UICONTROL Modifier les règles de réclamation]** (1).\
   La fenêtre contextuelle doit s’ouvrir automatiquement si vous avez sélectionné cette option à la fin de la configuration de l’approbation.

1. Cliquez sur **[!UICONTROL Ajouter une règle]** (2) pour ouvrir la fenêtre de configuration des revendications.

   * Courrier électronique (envoyer des attributs LDAP en tant que modèle de règle de revendications)
   * NomID (transformer un modèle de règle de réclamation entrante)
