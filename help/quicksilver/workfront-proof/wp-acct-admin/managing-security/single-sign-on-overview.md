---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Connexion unique [!DNL Workfront Proof]
description: L’authentification unique (SSO) permet à vos utilisateurs de se connecter. [!DNL Workfront Proof] à l’aide du nom d’utilisateur et du mot de passe existants de votre entreprise.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Connexion unique [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Un [!UICONTROL Entreprise] [!DNL Workfront] Planifiez l’utilisation de cette fonctionnalité. Pour plus d’informations sur les différents plans disponibles, voir [Formules Workfront](https://www.workfront.com/plans).

L’authentification unique (SSO) permet à vos utilisateurs de se connecter. [!DNL Workfront Proof] à l’aide du nom d’utilisateur et du mot de passe existants de votre entreprise.

Pour offrir cette fonctionnalité, nous utilisons [!DNL Security Assertion Markup Language] (SAML) 2.0, un protocole XML qui vous permet d’autoriser les données et d’échanger l’authentification entre un fournisseur d’identité et un service Web.

Cela signifie que vous vous authentifierez par rapport à votre propre système de connexion, et non par rapport à [!DNL Workfront Proof]de la page de connexion de .

Vous devez configurer un sous-domaine ou un domaine personnalisé sur votre [!DNL Workfront] Compte BAT pour activer SAML :

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Vous pouvez en savoir plus sur les domaines entièrement personnalisés dans  [Marque [!DNL Workfront Proof] site - advanced](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Voir [Configuration de l’authentification unique pour [!DNL Workfront Proof] utilisateurs](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) pour plus d’informations sur la configuration de l’authentification unique sur votre compte.
