---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Synchroniser les dossiers Box avec  [!DNL Workfront Proof].
description: Vous pouvez synchroniser un dossier Box avec un dossier dans Workfront Proof. Chaque modification que vous apportez à vos fichiers dans le dossier Box sera reflétée dans Workfront Proof (donc charger un nouveau fichier, ajouter une nouvelle version, renommer un fichier, etc.).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 100%

---

# Synchroniser les dossiers [!DNL Box] avec [!DNL Workfront Proof].

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez synchroniser un dossier [!DNL Box] avec un dossier dans [!DNL Workfront Proof]. Chaque modification que vous apportez à vos fichiers dans le dossier Box sera reflétée dans Workfront Proof (donc charger un nouveau fichier, ajouter une nouvelle version, renommer un fichier, etc.).

Pour plus d’informations sur les dossiers, consultez [Gérer les dossiers et leur contenu dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Seules les personnes avec un profil de [!UICONTROL Personne gestionnaire] ou supérieur peuvent synchroniser les dossiers. La personne [!DNL Box] qui charge le fichier dans un dossier synchronisé avec [!DNL Workfront Proof] sera désignée propriétaire de l’épreuve créée dans [!DNL Workfront Proof] (s’il s’agit d’une personne du même compte [!DNL Workfront Proof]). Si l’utilisateur ou l’utilisatrice [!DNL Box] l’est également dans un autre compte [!DNL Workfront Proof] ou ne possède pas de compte [!DNL Workfront Proof], la personne qui a créé la synchronisation entre les dossiers deviendra propriétaire de l’épreuve. Pour plus d’informations, voir *« Modification des profils et des autorisations des personnes »*.

Pour synchroniser un dossier [!DNL Box] avec un dossier [!DNL Workfront Proof], procédez comme suit :

1. Dans votre compte [!DNL Box], accédez à la page [!UICONTROL Tous les fichiers et dossiers].
1. Cliquez sur le menu **[!UICONTROL Autres options]** à côté du dossier que vous souhaitez synchroniser avec [!DNL Workfront Proof] (1).
1. Sélectionnez **[!UICONTROL Autres actions]** (2).
1. Cliquez sur **[!UICONTROL Synchroniser avec[!DNL Workfront Proof]]** (3).
1. Dans le [!UICONTROL Dossier de synchronisation] qui s’affiche (si votre connexion à [!DNL Workfront Proof] est effective), effectuez l’une des opérations suivantes :

   * Cliquez sur le nom d’un dossier [!DNL Workfront Proof] pour le synchroniser avec le dossier correspondant dans Box (4).
   * Cliquez sur **[!UICONTROL Nouveau dossier]** pour créer un dossier dans [!DNL Workfront Proof] (5).

     ![folder_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Si vous choisissez de créer un dossier, vous recevez une invitation à fournir des détails sur le nouveau dossier.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   La page [!UICONTROL Détails du dossier] du dossier synchronisé s’ouvre dans [!DNL Workfront Proof]. Cette page contient des informations sur le dossier.\
   Cette page vous permet également de mettre en pause et de désactiver la synchronisation. Si vous suspendez la synchronisation, le dossier ne sera plus mis à jour avec les modifications de [!DNL Box], mais la synchronisation peut être reprise à tout moment. La désactivation de la synchronisation signifie que la connexion entre les dossiers est rompue et que la synchronisation doit être rétablie à partir du compte [!DNL Box].\
   La page [!UICONTROL Détails du dossier] contient les informations et fonctions suivantes relatives à votre dossier dans [!DNL Box] :

   * **[!UICONTROL Suspendre la synchronisation]** : le dossier [!DNL Workfront Proof] ne sera plus mis à jour avec les modifications apportées par Box. La synchronisation peut être reprise à tout moment (1).
   * **[!UICONTROL Désactiver la synchronisation des dossiers]** : la connexion entre les dossiers est perdue et la synchronisation doit être reconfigurée à partir du compte [!DNL Box] (2).

   * Seule la personne qui a démarré la synchronisation des dossiers peut la désactiver ou la suspendre. Pour plus d’informations, voir [Gérer les dossiers et leur contenu dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Accédez au dossier [!DNL Box]** : si vous avez partagé l’URL du dossier (dans les options du dossier [!DNL Box]), cette option devient disponible et vous emmène directement vers le dossier [!DNL Box] (3).
   * **[!UICONTROL Détails de la synchronisation du dossier]** : cette section contient des informations sur le dossier [!DNL Box] (4).
   * Lien du dossier **[!UICONTROL [!DNL Box]]** : URL vers le dossier [!DNL Box] (5).
   * **[!UICONTROL Activité] :** affiche les journaux d’activité du dossier [!DNL Workfront Proof]. Vous pouvez y vérifier qui a démarré la synchronisation du dossier (6).
   * ![folder_details__1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* Vous pouvez également synchroniser le dossier [!DNL Box] à partir du menu [!UICONTROL Options du dossier].
>* Si vous avez votre propre page de connexion de marque [!DNL Workfront Proof], vous accédez à cette page au lieu de la page de connexion standard de [!DNL Workfront Proof]. Pour plus d’informations, reportez-vous aux articles sous [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding).
>* Si vous avez activé la fonctionnalité [!UICONTROL Authentification unique (SSO)] dans votre compte [!DNL Workfront Proof], vous accédez à la page de connexion SSO et devez saisir vos informations d’identification de connexion SSO, mais seulement si vous utilisez la même adresse e-mail pour votre compte [!DNL Box] et [!DNL Workfront Proof]. Pour plus d’informations, voir [[!UICONTROL Authentification unique] dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Si vous n’utilisez pas la même adresse e-mail pour vos comptes [!DNL Box] et [!DNL Workfront Proof], vous accédez toujours à la page de connexion standard de [!DNL Workfront Proof].
>


