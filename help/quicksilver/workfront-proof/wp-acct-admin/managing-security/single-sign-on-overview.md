---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Authentification unique dans  [!DNL Workfront Proof]
description: L’authentification unique (SSO) permet à vos utilisateurs de se connecter à  [!DNL Workfront Proof] à l’aide du nom d’utilisateur et du mot de passe existants de votre entreprise.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 7%

---

# Connexion unique dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Un abonnement [!UICONTROL Enterprise] [!DNL Workfront] est requis pour utiliser cette fonctionnalité. Pour plus d’informations sur les différentes formules disponibles, voir [Formules Workfront](https://www.workfront.com/plans?lang=fr).

L’authentification unique (SSO) permet à vos utilisateurs de se connecter à [!DNL Workfront Proof] à l’aide du nom d’utilisateur et du mot de passe existants de votre entreprise.

Pour fournir cette fonctionnalité, nous utilisons [!DNL Security Assertion Markup Language] (SAML) 2.0, un protocole XML qui vous permet d’autoriser l’authentification des données et des exchanges entre un fournisseur d’identité et un service Web.

Cela signifie que vous vous authentifierez par rapport à votre propre système de connexion, et non par rapport à la page de connexion de [!DNL Workfront Proof].

Pour activer SAML, vous devez configurer un sous-domaine ou un domaine personnalisé sur votre compte BAT [!DNL Workfront] :

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Vous pouvez en savoir plus sur les domaines entièrement personnalisés dans [Brand the [!DNL Workfront Proof] site - advanced](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Voir [Configuration de l’authentification unique pour les  [!DNL Workfront Proof] utilisateurs](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) pour plus d’informations sur la configuration de l’authentification unique sur votre compte.
