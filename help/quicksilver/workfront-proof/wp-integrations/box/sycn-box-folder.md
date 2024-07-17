---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Dossiers de boîte de synchronisation avec  [!DNL Workfront Proof]
description: Vous pouvez synchroniser un dossier Box avec un dossier dans Workfront Proof. Chaque modification que vous apportez à vos fichiers dans le dossier Box est répercutée dans Workfront Proof (par conséquent, vous devez charger un nouveau fichier, ajouter une nouvelle version, renommer un fichier, etc.).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Synchroniser Les Dossiers [!DNL Box] Avec [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez synchroniser un dossier [!DNL Box] avec un dossier dans [!DNL Workfront Proof]. Chaque modification que vous apportez à vos fichiers dans le dossier Box est répercutée dans Workfront Proof (par conséquent, vous devez charger un nouveau fichier, ajouter une nouvelle version, renommer un fichier, etc.).

Pour plus d’informations sur les dossiers, voir [Gestion des dossiers et de leur contenu dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Seuls les utilisateurs disposant de profils de [!UICONTROL  gestionnaires] ou supérieurs peuvent synchroniser des dossiers. L’utilisateur [!DNL Box] qui charge le fichier dans un dossier synchronisé avec [!DNL Workfront Proof] deviendra le propriétaire du BAT créé dans [!DNL Workfront Proof] (s’il s’agit d’un utilisateur appartenant au même compte [!DNL Workfront Proof]). Si l’utilisateur [!DNL Box] est un utilisateur dans un autre compte [!DNL Workfront Proof] ou n’a pas de compte avec [!DNL Workfront Proof], la personne qui a créé la synchronisation entre les dossiers deviendra le propriétaire du BAT. Pour plus d’informations, voir *&quot;Modification des profils utilisateur et des autorisations.&quot;*

Pour synchroniser un dossier [!DNL Box] avec un dossier dans [!DNL Workfront Proof] :

1. Dans votre compte [!DNL Box], accédez à la page [!UICONTROL Tous les fichiers et dossiers].
1. Cliquez sur le menu **[!UICONTROL Autres options]** en regard du dossier que vous souhaitez synchroniser avec [!DNL Workfront Proof] (1).
1. Sélectionnez **[!UICONTROL Autres actions]** (2).
1. Cliquez sur **[!UICONTROL Synchroniser avec[!DNL Workfront Proof]]** (3).
1. Dans la zone [!UICONTROL Synchroniser le dossier] qui s’affiche (si vous êtes connecté à [!DNL Workfront Proof]), effectuez l’une des opérations suivantes :

   * Cliquez sur un nom de dossier [!DNL Workfront Proof] pour le synchroniser avec le dossier correspondant dans la boîte (4).
   * Cliquez sur **[!UICONTROL Nouveau dossier]** pour créer un dossier dans [!DNL Workfront Proof] (5).\

     ![folder_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Si vous choisissez de créer un dossier, vous êtes invité à fournir des informations sur le nouveau dossier.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   La page [!UICONTROL Détails du dossier] du dossier synchronisé s’ouvre dans [!DNL Workfront Proof]. Cette page contient des informations sur le dossier.\
   Cette page vous permet également de suspendre et de désactiver la synchronisation. Si vous suspendez la synchronisation, le dossier ne sera plus mis à jour avec les modifications de [!DNL Box], mais la synchronisation peut reprendre à tout moment. La désactivation de la synchronisation signifie que la connexion entre les dossiers est rompue et que la synchronisation doit être rétablie à partir du compte [!DNL Box].\
   La page [!UICONTROL Détails du dossier] contient les informations et fonctions suivantes relatives à votre dossier dans [!DNL Box] :

   * **[!UICONTROL Synchronisation des mises en pause]** : le dossier [!DNL Workfront Proof] ne sera plus mis à jour avec les modifications de la boîte. La synchronisation peut être reprise à tout moment (1).
   * **[!UICONTROL Désactiver la synchronisation des dossiers]** : la connexion entre les dossiers est perdue et la synchronisation devra être reconfigurée à partir du compte [!DNL Box] (2).

   * Seul l’utilisateur qui a démarré la synchronisation des dossiers peut la désactiver ou la suspendre. Pour plus d’informations, voir [Gestion des dossiers et de leur contenu dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Accédez au dossier [!DNL Box]** : si vous avez partagé l’URL du dossier (dans les options du dossier [!DNL Box]), cette option devient disponible et vous emmène directement dans le dossier [!DNL Box] (3).
   * **[!UICONTROL Détails sur la synchronisation des dossiers]** : cette section contient des informations sur le dossier [!DNL Box] (4).
   * **[!UICONTROL [!DNL Box]lien du dossier]** : URL du dossier [!DNL Box] (5).
   * **[!UICONTROL Activité] :** Affiche les journaux d’activité du dossier [!DNL Workfront Proof], où vous pouvez vérifier qui a démarré la synchronisation des dossiers (6).
   * ![folder_details__1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* Vous pouvez également synchroniser le dossier [!DNL Box] à partir du menu [!UICONTROL Options du dossier].
>* Si vous disposez de votre propre page de connexion [!DNL Workfront Proof] de marque, vous accédez à cette page au lieu de la page de connexion [!DNL Workfront Proof] standard. Consultez les articles sous [Marque](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) si vous avez besoin d’informations supplémentaires.
>* Si vous avez activé la fonctionnalité [!UICONTROL Authentification unique (SSO)] dans votre compte [!DNL Workfront Proof], vous serez amené à la page de connexion SSO et vous serez invité à saisir vos informations d’identification de connexion SSO, mais seulement si vous utilisez la même adresse électronique pour votre compte [!DNL Box] et [!DNL Workfront Proof]. Si vous avez besoin d’informations supplémentaires, reportez-vous à la section [[!UICONTROL Connexion unique] dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Si vous n&#39;utilisez pas la même adresse électronique pour votre compte [!DNL Box] et votre compte [!DNL Workfront Proof], vous serez toujours dirigé vers la page de connexion [!DNL Workfront Proof] standard.
>


