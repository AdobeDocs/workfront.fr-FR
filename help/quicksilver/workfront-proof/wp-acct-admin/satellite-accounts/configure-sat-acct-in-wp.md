---
product-previous: workfront-proof
product-area: documents;system-administration;setup
navigation-topic: satellite-accounts
title: Configuration d’un compte satellite dans [!DNL Workfront Proof]
description: Les comptes satellites sont des comptes payants que vous configurez et gérez à partir de vos propres comptes. [!DNL Workfront] Compte de preuve. Pour plus d’informations, voir "Comptes satellites dans [!DNL Workfront] Preuve.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 82c6dff3-6187-4145-951c-3f5312049b59
source-git-commit: 5be053a6ee99404673f6f3258a423ef5e5c7f431
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 1%

---

# Configuration d’un compte satellite dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Les comptes satellites sont des comptes payants que vous configurez et gérez à partir de vos propres comptes. [!DNL Workfront Proof] compte . Pour plus d’informations, voir [Comptes satellites dans [!DNL Workfront] Bon à tirer](../../../workfront-proof/wp-acct-admin/satellite-accounts/sat-accts-in-wp.md).

Tout administrateur de facturation peut créer un compte satellite. Pour plus d’informations sur les administrateurs de facturation, voir [[!UICONTROL Profils d’autorisations de BAT] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
> Les comptes satellites doivent être définis sur l’une de nos [!UICONTROL Standard] ou des plans supérieurs.

## Création d’un compte satellite {#creating-a-satellite-account}

Pour créer un compte Satellite :

1. Accédez au [!UICONTROL Facturation] page.\
   Pour plus d’informations sur la page de facturation, voir  [Le [!DNL Workfront Proof] [!UICONTROL Facturation] Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. Cliquez sur le bouton **[!UICONTROL Nouveau satellite]** bouton Compte . (1)

   Une fenêtre contextuelle s’affiche.

   ![New_Satellite_Account.png](assets/new-satellite-account-350x156.png)

1. Saisissez les détails de votre client, y compris les codes promotionnels appropriés.
1. Cliquer sur **[!UICONTROL Enregistrer]**. Le compte satellite s’affiche automatiquement dans la variable [!UICONTROL Comptes] menu déroulant en haut de la page [!UICONTROL Facturation] page.
1. Sélectionnez le nouveau compte satellite dans le menu déroulant.
1. Passez à la [Sélection d’un plan pour votre compte satellite](#selecting-a-plan-for-your-satellite-account) pour mettre à niveau votre compte Satellite.

## Sélection d’un plan pour votre compte satellite {#selecting-a-plan-for-your-satellite-account}

Après avoir configuré le compte satellite, comme décrit dans la section [Création d’un compte satellite](#creating-a-satellite-account), vous devez le mettre à niveau selon le plan souhaité.

1. Accédez au [!UICONTROL Facturation] page.\
   Pour plus d’informations sur la page de facturation, voir  [Le [!DNL Workfront Proof] [!UICONTROL Facturation] Page](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. Dans le **[!UICONTROL Vos comptes]** dans le menu déroulant situé en haut de la page (1), sélectionnez le compte satellite approprié.

   La page de facturation du compte satellite s’affiche et les informations de contact de facturation de votre compte sont automatiquement répliquées.

   ![Satellite_Account_Change_Plan.png](assets/satellite-account-change-plan-350x156.png)

1. Cliquez sur le bouton **[!UICONTROL Plan de modification]** dans le coin supérieur droit de la page. (2)\
   Ou\
   Ouvrez la fenêtre contextuelle en cliquant sur le nom du plan actuel ou suivant. (3)

1. Effectuez une mise à niveau ou rétrogradez votre plan.

## Ajout d’utilisateurs à votre compte Satellite

Après avoir mis à niveau le compte Satellite vers le plan de votre choix, vous devez ajouter des utilisateurs au compte.

1. Connectez-vous à [!DNL Workfront Proof] comme la propriété [!DNL Workfront Proof] administrateur.
1. Cliquez sur **[!UICONTROL Paramètres du compte]**.
1. Dans le menu déroulant situé en haut de la page, sélectionnez le compte satellite approprié. (1)\
   La page des paramètres du compte pour le compte satellite s’affiche.
1. Cliquez sur le bouton **[!UICONTROL Nouvel utilisateur]** dans le coin supérieur droit de la page. (2)\
   Le [!DNL New User] s’affiche.

1. Saisissez les détails de l’utilisateur, puis cliquez sur **[!UICONTROL Enregistrer]**.\
   L&#39;utilisateur reçoit une notification par email lui permettant d&#39;accéder au compte.

Les utilisateurs ajoutés au compte Satellite apparaissent en tant que membres dans la liste de contacts du compte hub.

De même, les utilisateurs du compte hub apparaissent comme des membres dans les contacts du compte satellite.

Pour afficher la liste complète de tous les utilisateurs dans le compte satellite, cliquez sur le bouton **[!UICONTROL Utilisateurs]** .

![SA_New_User.png](assets/sa-new-user-350x156.png)

## Liaison de comptes distincts existants à votre compte hub

Si vous avez précédemment créé d’autres comptes distincts pour vos clients, ceux-ci peuvent être convertis en comptes satellites.

Nous prendrons soin de cela pour vous en les liant à votre [!DNL Workfront Proof] (en faisant un compte hub).

Tout ce que vous avez à faire est de nous fournir les détails suivants :

* Le nom de votre [!DNL Workfront Proof] compte et l’adresse électronique que vous avez utilisée pour le configurer
* Les noms des comptes distincts que vous souhaitez lier à votre compte et les adresses électroniques utilisées pour configurer les comptes distincts.
