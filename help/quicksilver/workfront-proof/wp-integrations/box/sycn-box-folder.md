---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Dossiers de boîte de synchronisation avec [!DNL Workfront Proof]
description: Vous pouvez synchroniser un dossier Box avec un dossier dans Workfront BAT. Chaque modification apportée à vos fichiers dans le dossier Box est répercutée dans le BAT Workfront (par conséquent, le téléchargement d’un nouveau fichier, l’ajout d’une nouvelle version, le changement de nom d’un fichier, etc.).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Synchronisation [!DNL Box] Dossiers avec [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez synchroniser une [!DNL Box] dossier contenant un dossier [!DNL Workfront Proof]. Chaque modification apportée à vos fichiers dans le dossier Box est répercutée dans le BAT Workfront (par conséquent, le téléchargement d’un nouveau fichier, l’ajout d’une nouvelle version, le changement de nom d’un fichier, etc.).

Pour plus d’informations sur les dossiers, voir [Gestion des dossiers et de leur contenu dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Uniquement les utilisateurs dotés de profils [!UICONTROL Chefs] ou les versions ultérieures peuvent synchroniser les dossiers. Le [!DNL Box] utilisateur qui charge le fichier dans un dossier synchronisé avec [!DNL Workfront Proof], sera le propriétaire du BAT créé dans [!DNL Workfront Proof] (s’il s’agit d’un utilisateur du même [!DNL Workfront Proof] ). Si la variable [!DNL Box] un utilisateur est un utilisateur dans un autre [!DNL Workfront Proof] compte ou ne possède pas de compte avec [!DNL Workfront Proof], la personne qui a créé la synchronisation entre les dossiers deviendra le propriétaire du BAT. Pour plus d’informations, voir *&quot;Modification des profils utilisateur et des autorisations.&quot;*

Pour synchroniser une [!DNL Box] dossier contenant un dossier [!DNL Workfront Proof]:

1. Dans votre [!DNL Box] , accédez au [!UICONTROL Tous les fichiers et dossiers] page.
1. Cliquez sur le bouton **[!UICONTROL Autres options]** en regard du dossier avec lequel vous souhaitez effectuer la synchronisation [!DNL Workfront Proof] (1).
1. Sélectionner **[!UICONTROL Autres actions]** (2).
1. Cliquez sur **[!UICONTROL Synchroniser avec[!DNL Workfront Proof]]** (3).
1. Dans le [!UICONTROL Dossier de synchronisation] s’affiche (si vous êtes connecté à [!DNL Workfront Proof]), effectuez l’une des opérations suivantes :

   * Cliquez sur un [!DNL Workfront Proof] nom du dossier pour le synchroniser avec le dossier correspondant dans la boîte (4).
   * Cliquez sur **[!UICONTROL Nouveau dossier]** pour créer un dossier dans [!DNL Workfront Proof] (5).\

      ![folder_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Si vous choisissez de créer un dossier, vous êtes invité à fournir des détails sur le nouveau dossier.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   Le [!UICONTROL Détails du dossier] La page du dossier synchronisé s’ouvre dans [!DNL Workfront Proof]. Cette page contient des informations sur le dossier.\
   Cette page vous permet également de suspendre et de désactiver la synchronisation. Si vous suspendez la synchronisation, le dossier ne sera plus mis à jour avec les modifications de [!DNL Box], mais la synchronisation peut être reprise à tout moment. La désactivation de la synchronisation signifie que la connexion entre les dossiers est rompue et que la synchronisation doit être rétablie à partir du [!DNL Box] compte .\
   Le [!UICONTROL Détails du dossier] contient les informations et fonctions suivantes relatives à votre dossier dans [!DNL Box]:

   * **[!UICONTROL Synchronisation des pauses]**: Le [!DNL Workfront Proof] ne sera plus mis à jour avec les modifications de la boîte de dialogue. La synchronisation peut être reprise à tout moment (1).
   * **[!UICONTROL Désactiver la synchronisation des dossiers]**: La connexion entre les dossiers est perdue et la synchronisation doit être reconfigurée à partir de la fonction [!DNL Box] compte (2).

   * Seul l’utilisateur qui a démarré la synchronisation des dossiers peut la désactiver ou la suspendre. Pour plus d’informations, voir  [Gestion des dossiers et de leur contenu dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Accédez à [!DNL Box] folder**: Si vous avez partagé l’URL du dossier (dans la variable [!DNL Box] (options de dossier), cette option devient disponible et vous emmène directement vers la [!DNL Box] dossier (3).
   * **[!UICONTROL Détails de la synchronisation des dossiers]**: Cette section contient des informations sur les [!DNL Box] dossier (4).
   * **[!UICONTROL [!DNL Box]lien du dossier]**: URL de la [!DNL Box] dossier (5).
   * **[!UICONTROL Activité]:** Affiche les journaux d’activité de la variable [!DNL Workfront Proof] , ici, vous pouvez vérifier qui a démarré la synchronisation des dossiers (6).
   * ![folder_details__1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* Vous pouvez également synchroniser la variable [!DNL Box] à partir du dossier [!UICONTROL Options du dossier] .
>* Si vous avez votre propre marque [!DNL Workfront Proof] page de connexion, vous accédez à cette page au lieu de la page standard. [!DNL Workfront Proof] page de connexion. Voir les articles sous [Marques](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) si vous avez besoin de plus d’informations.
>* Si vous avez activé la variable [!UICONTROL Authentification unique (SSO)] de votre [!DNL Workfront Proof] , vous serez redirigé vers la page de connexion SSO et invité à saisir vos informations d’identification de connexion SSO, mais seulement si vous utilisez la même adresse électronique pour votre [!DNL Box] compte et [!DNL Workfront Proof]. Si vous avez besoin d’informations supplémentaires, reportez-vous à la section [[!UICONTROL Authentification unique] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Si vous n’utilisez pas la même adresse électronique pour vos [!DNL Box] et votre compte [!DNL Workfront Proof] , vous serez toujours porté à la norme [!DNL Workfront Proof] page de connexion.
>



