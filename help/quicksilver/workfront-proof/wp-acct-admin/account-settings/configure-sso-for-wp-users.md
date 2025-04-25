---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Configuration de l’authentification unique pour les utilisateurs et utilisatrices  [!DNL Workfront Proof] '
description: Si vous disposez de la formule Select ou Premium, vous pouvez fournir une fonctionnalité d’authentification unique (SSO) qui vous permet d’utiliser le nom d’utilisateur ou d’utilisatrice et le mot de passe de votre organisation pour accéder à votre compte  [!DNL Workfront Proof] .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 94%

---

# Configuration de l’authentification unique pour les utilisateurs et utilisatrices [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Si vous disposez de la formule Select ou Premium, vous pouvez fournir une fonctionnalité d’authentification unique (SSO) qui vous permet d’utiliser le nom d’utilisateur ou d’utilisatrice et le mot de passe de votre organisation pour accéder à votre compte [!DNL Workfront Proof].

Cela signifie que vous vous authentifierez avec votre propre système de connexion, et non pas avec la page de connexion [!DNL Workfront Proof].

>[!NOTE]
>
>Un sous-domaine ou un domaine personnalisé doit être configuré sur votre compte [!DNL Workfront Proof] pour activer SAML. Les sous-domaines personnalisés peuvent être configurés gratuitement. Voir [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) pour plus d’informations. Pour en savoir plus sur les domaines entièrement personnalisés, consultez notre [ Marque du site  [!DNL Workfront Proof]  - avancé](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Activation de l’authentification unique dans [!DNL Workfront Proof]

La fonctionnalité d’authentification unique peut être activée sur l’onglet [!UICONTROL Authentification unique] de vos [!UICONTROL Paramètres du compte], et s’appliquera à tous les utilisateurs et utilisatrices de votre compte [!DNL Workfront Proof]. Consultez les [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) pour en savoir plus.

## ID d’entité

En tant que fournisseur, nous avons publié notre ID d’entité ici :

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (où « yoursubdomain » est le sous-domaine de votre compte)

[!DNL Workfront Proof] requiert l’adresse e-mail de l’utilisateur ou de l’utilisatrice comme identifiant unique, qui peut être transmis comme l’un des attributs suivants :

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* mail
* email
* emailAddress

Pour configurer l’authentification unique :

1. Ouvrez l’onglet **[!UICONTROL Authentification unique]** (1).
1. Saisissez l’**URL d’authentifiation unique** (2).
Il s’agit du lien vers votre serveur d’authentification unique (par exemple : **https://sso.mycompany.com/opensso**).

1. Saisissez l’**URL de connexion** (3).
Il s’agit de l’URL qui sera appelée pour rediriger les utilisateurs et utilisatrices vers votre fournisseur d’identité.

   Il ne s’agit pas d’une URL réelle que vous saisissez dans le navigateur, mais plutôt d’un point d’entrée qui traite les informations que nous lui envoyons afin de présenter l’écran de connexion.

1. Saisissez l’**URL de déconnexion** (4).
Il s’agit de l’URL à laquelle vous revenez après votre déconnexion, par exemple.

   **https://www.yourcompany.com/services/logout.asp**

1. Saisissez l’**empreinte du certificat** (5).
1. L’empreinte SHA1 du certificat SAML fourni par votre fournisseur d’identité SAML.
1. Veillez à inclure les informations clés en définissant ce qui suit sur votre fournisseur d’identité.
1. Définissez **SSO** sur **[!UICONTROL Activée]** (6).
Une fois l’authentification unique activée, vous et les autres utilisateurs et utilisatrices de votre compte vous connectez à l’aide de votre propre mécanisme d’authentification. Cela signifie que lorsque les utilisateurs et utilisatrices accèdent à votre écran de connexion au compte [!DNL Workfront Proof] (par exemple, **yourcompany.proofhq.com/login**), il leur sera demandé d’ouvrir la fenêtre de transfert de votre propre page de connexion à l’authentification.

1. (Facultatif) Activez **Allouer automatiquement les utilisateurs et utilisatrices** (7).
Une fois cette option activée, les comptes d’utilisateurs sont automatiquement créés pour les personnes qui n’ont pas leur propre profil [!DNL Workfront Proof], mais qui accèdent à votre compte [!DNL Workfront Proof] à l’aide de leurs identifiants d’authentification unique. Cette action sera effectuée uniquement si la limite d’utilisateur et d’utilisatrice n’est pas encore atteinte pour votre compte.

1. Les autorisations de profil Manager sont attribuées par défaut aux nouveaux utilisateurs et nouvelles utilisatrices alloués. Pour en savoir plus, voir [Profils d’autorisations ds épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Activation de l’authentification unique pour les comptes satellites

Lorsque des comptes satellites sont connectés à votre compte hub, vous pouvez les administrer au niveau du compte hub.

L’authentification unique est une fonctionnalité Select et Premium, et peut donc être activée uniquement sur les satellites des formules Select et Premium.

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Cliquez sur le compte satellite dans le menu déroulant (2).
1. Ouvrez l’onglet **[!UICONTROL Authentification unique]** (3).
1. Vous pouvez maintenant modifier la configuration de l’authentification unique (4).
1. ![Enabling_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Vous disposez ici de deux méthodes (5) de configuration :

1. **Héritée :** authentification unique avec la configuration extraite de votre compte hub.
Si un utilisateur accède à [!DNL Workfront Proof] par le biais de la **page de connexion par défaut** ([https://business.adobe.com/products/workfront/proofing-approvals.html](https://business.adobe.com/products/workfront/proofing-approvals.html) **), deux niveaux d&#39;autorisation s&#39;appliquent** : tout d&#39;abord, il est invité à se connecter à l&#39;aide des données d&#39;accès [!DNL Workfront Proof] (adresse e-mail et mot de passe), puis l&#39;utilisateur est transféré par le biais d&#39;une fenêtre SSO vers la page de connexion SSO.
Par conséquent, avec le service d’authentification unique activé, nous vous recommandons de vous connecter par l’intermédiaire de votre propre sous-domaine/domaine [!DNL Workfront Proof].

   >[!NOTE]
   >
   >Pour le moment, lorsque l’authentification unique est activée sur votre compte [!DNL Workfront Proof], vous ne pouvez pas vous connecter à l’application iPhone avec ces informations d’identification.

   1. **Manuelle** (par défaut) : authentification unique avec une configuration différente (pointant par exemple vers un autre fournisseur d’identité).

      >[!NOTE]
      >
      >Si le compte satellite hérite de la configuration d’authentification unique du compte hub, l’écran de connexion sera celui du compte hub. Lorsque la personne du compte satellite renseigne ses détails de connexion via authentification unique sur cette page, elle est redirigée vers le compte satellite.

      ![Activation_SSO_-_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Cliquez sur **[!UICONTROL Enregistrer]** (6).

## Paramètres d’authentification unique hérités d’un compte hub

Lorsque vous choisissez d’hériter des paramètres de votre compte hub, vous remarquerez que tous les champs sont désormais renseignés avec les données de votre compte hub (7) et que l’authentification unique est automatiquement activée/désactivée (8) comme sur votre compte principal. Il n’existe plus de liens de modification dans les champs, car l’ensemble de la configuration d’authentification unique pour le compte satellite est maintenant définie et gérée à partir de votre compte hub.

![Satellite_Account_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

Dans votre compte hub (9), le champ [!UICONTROL Utilisation de l’authentification unique] indique que cette configuration est utilisée par les comptes satellites (10).\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## Authentification unique configurée manuellement

Si vous avez choisi la configuration d’authentification unique manuelle pour un compte satellite (1), vous devez saisir manuellement les données de l’authentification unique.

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Ouvrez l’onglet **[!UICONTROL Authentification unique]**.
1. Cliquez sur **[!UICONTROL Modifier],** renseignez le champ, puis cliquez sur **[!UICONTROL Enregistrer]** (2).

1. Sur la ligne **[!UICONTROL SSO]**, cliquez sur **[!UICONTROL Activé]** (3).

![Satellite_Account_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## Connexion via authentification unique

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Ouvrez l’onglet **[!UICONTROL Authentification unique]**.
1. Assurez-vous que votre domaine/sous-domaine [!DNL Workfront Proof] (1) est configuré et que vos utilisateurs et utilisatrices accèdent à votre compte [!DNL Workfront Proof] par le biais de ce domaine/sous-domaine personnalisé.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Lorsque l’authentification unique est activée, l’URL de connexion au sous-domaine (yourcompany.proofhq.com/login, par exemple) affiche un écran de transfert (2) qui vous permet d’accéder directement à votre page de connexion via authentification unique.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Si un utilisateur accède à [!DNL Workfront Proof] via la page de connexion **par défaut** ([https://business.adobe.com/products/workfront/proofing-approvals.html](https://business.adobe.com/products/workfront/proofing-approvals.html)), il y aura **deux niveaux d’autorisation**. D’abord, la personne doit se connecter à l’aide des données d’accès [!DNL Workfront Proof] (adresse e-mail et mot de passe). Ensuite, elle est transférée via une fenêtre d’authentification unique (2) vers la page de connexion via authentification unique.\
   Par conséquent, avec le service d’authentification unique activé, nous vous recommandons de vous connecter par l’intermédiaire de votre propre sous-domaine/domaine [!DNL Workfront Proof].

1. Pour le moment, lorsque l’authentification unique est activée sur votre compte Workfront Proof, vous ne pouvez pas vous connecter à l’application iPhone avec ces informations d’identification.

## À propos de l’ajout d’un nouvel utilisateur ou d’une nouvelle utilisatrice

Lorsque la fonctionnalité d’authentification unique est activée sur votre compte [!DNL Workfront Proof], les nouveaux utilisateurs et utilisatrices ne reçoivent aucun e-mail de confirmation, car leurs comptes sont automatiquement activés et prêts à l’emploi.

À partir de votre page de connexion [!DNL Workfront Proof], après avoir cliqué sur le bouton [!UICONTROL Connexion], les utilisateurs et utilisatrices sont redirigés vers votre page de connexion via authentification unique et invités à saisir leurs informations d’identification de connexion via authentification unique.

>[!IMPORTANT]
>
>Les utilisateurs et utilisatrices sont identifiés par une adresse e-mail au cours du processus d’authentification, ce qui signifie que le compte de messagerie utilisé pour votre connexion via authentification unique doit correspondre à l’adresse e-mail de la personne enregistrée dans votre compte.

## Services de fédération Active Directory (AD FS)

Les services de fédération Active Directory (AD FS) constituent un composant logiciel [!DNL Microsoft] qui peut être installé sur les systèmes d’exploitation Windows Server afin de fournir aux utilisateurs et utilisatrices un accès via authentification unique aux systèmes et applications situés au-delà des limites organisationnelles. Pour plus d’informations, voir « Services de fédération Active Directory » sur le site web de Microsoft Developer Network.

Le système [!DNL Workfront Proof] prend en charge SAML 2.0 et n’est compatible qu’avec AD FS version 2.0 ou ultérieure.

Voir [Authentification unique dans  [!DNL Workfront Proof] : configuration AD FS](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) pour obtenir des instructions détaillées.
