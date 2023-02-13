---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Présentation de l’authentification unique dans Adobe Workfront
description: Workfront fournit une configuration de connexion unique (SSO) centralisée qui intègre facilement Workfront à votre solution d’authentification unique d’entreprise existante. Cette configuration est facile à configurer et à gérer. Elle est disponible pour les clients OnDemand et OnPremise Enterprise.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Présentation de l’authentification unique dans Adobe Workfront

{{important-admin-console-onboard}}


Workfront fournit une configuration de connexion unique (SSO) centralisée qui intègre facilement Workfront à votre solution d’authentification unique d’entreprise existante. Cette configuration est facile à configurer et à gérer. Elle est disponible pour les clients OnDemand et OnPremise Enterprise.

Pour utiliser la fonctionnalité SSO dans Workfront, votre entreprise doit configurer une application SSO. Vous pouvez ensuite configurer Workfront afin qu’il puisse communiquer avec votre solution SSO.

Les solutions fédérées permettent aux utilisateurs de se connecter à toutes leurs applications en saisissant leur nom d’utilisateur et leur mot de passe dans un portail de connexion centralisé.

![](assets/overview-sso-wf.png)


## Configuration de votre pare-feu

Lors de l’utilisation d’une solution d’authentification unique, Workfront établit une connexion à votre serveur sur le port spécifié.

Si vous vous abonnez à Workfront à la demande et si vous avez configuré votre pare-feu ou votre serveur de messagerie pour autoriser l’accès uniquement à des fournisseurs spécifiques, vous devez ajouter certaines adresses IP Workfront à la liste autorisée de votre pare-feu. Pour plus d’informations, voir [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configuration de l’authentification unique

Workfront s’intègre aux solutions d’authentification unique suivantes :

* Solutions fédérées qui prennent en charge SAML 2.0

   Pour plus d’informations sur l’intégration de Workfront à SAML 2.0, voir [Configuration d’Adobe Workfront avec SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* Solutions fédérées qui prennent en charge SAML 2.0 à l’aide d’ADFS

   Pour plus d’informations sur l’intégration de Workfront avec SAML 2.0 à l’aide d’ADFS, voir [Configuration d’Adobe Workfront avec SAML 2.0 à l’aide d’ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
