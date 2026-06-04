---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Authentification unique dans  [!DNL Workfront Proof]
description: L’authentification unique (SSO) permet à vos utilisateurs et utilisatrices de se connecter à  [!DNL Workfront Proof]  à l’aide du nom d’utilisateur ou d’utilisatrice et du mot de passe existants de votre organisation.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
TQID: https://experienceleague.adobe.com/rQkypJthOpKg1gQBH0tUjtwkbaxLn1k-lrpZj9hCQ5o
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 100%

---

# Authentification unique dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Une formule [!UICONTROL Entreprise] [!DNL Workfront] est requise pour utiliser cette fonctionnalité. Pour plus d’informations sur les différentes formules disponibles, voir [Formules Workfront](https://business.adobe.com/products/workfront/pricing.html).

L’authentification unique (SSO) permet à vos utilisateurs et utilisatrices de se connecter à [!DNL Workfront Proof] à l’aide du nom d’utilisateur ou d’utilisatrice et du mot de passe existants de votre organisation.

Pour offrir cette fonctionnalité, nous utilisons [!DNL Security Assertion Markup Language] (SAML) 2.0, un protocole XML qui vous permet d’autoriser les données et d’échanger l’authentification entre un fournisseur d’identité et un service web.

Cela signifie que vous vous authentifierez avec votre propre système de connexion, et non pas avec la page de connexion de [!DNL Workfront Proof].

Un sous-domaine ou un domaine personnalisé doit être configuré sur votre compte [!DNL Workfront] Proof pour activer SAML :

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Pour en savoir plus sur les domaines entièrement personnalisés, consultez [Personnaliser le branding du site [!DNL Workfront Proof]  - Avancé](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Consultez [Configurer l’authentification unique pour les utilisateurs et les utilisatrices de  [!DNL Workfront Proof] ](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) pour plus d’informations sur la configuration de l’authentification unique sur votre compte.
