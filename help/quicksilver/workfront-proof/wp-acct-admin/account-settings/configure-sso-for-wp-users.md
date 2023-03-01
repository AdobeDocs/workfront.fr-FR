---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Configuration de l’authentification unique pour [!DNL Workfront Proof] utilisateurs
description: Si vous disposez du plan Select ou Premium, vous pouvez fournir une fonctionnalité de connexion unique (SSO) qui vous permet d’utiliser le nom d’utilisateur et le mot de passe de votre organisation existante pour accéder à votre [!DNL Workfront Proof] compte .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 007a603ef1df2a02959d7fb623ac784bf5b9cb80
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 0%

---

# Configuration de l’authentification unique pour [!DNL Workfront Proof] utilisateurs

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Si vous disposez du plan Select ou Premium, vous pouvez fournir une fonctionnalité de connexion unique (SSO) qui vous permet d’utiliser le nom d’utilisateur et le mot de passe de votre organisation existante pour accéder à votre [!DNL Workfront Proof] compte .

Cela signifie que vous vous authentifierez par rapport à votre propre système de connexion, et non par rapport au [!DNL Workfront Proof] page de connexion.

>[!NOTE]
>
>Un sous-domaine ou un domaine personnalisé doit être configuré sur votre [!DNL Workfront Proof] pour activer SAML. Les sous-domaines personnalisés peuvent être configurés librement. Voir [Marques](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) pour plus d’informations. Pour en savoir plus sur les domaines entièrement personnalisés, consultez notre [Marque [!DNL Workfront Proof] site - advanced](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Activation de l’authentification unique dans [!DNL Workfront Proof]

La fonctionnalité de connexion unique peut être activée sur le [!UICONTROL Authentification unique] de votre [!UICONTROL Paramètres du compte], qui s’appliquera à tous les utilisateurs de votre [!DNL Workfront Proof] compte . Voir [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) pour plus d’informations.

## ID d’entité

En tant que fournisseur de services, nous avons publié notre identifiant d’entité ici :

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (où &quot;votre sous-domaine&quot; est le sous-domaine de votre compte)

[!DNL Workfront Proof] requiert l’adresse électronique de l’utilisateur comme identifiant unique, qui peut être transmis comme l’un des attributs suivants :

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* mail
* email
* emailAddress

Pour configurer SSO :

1. Ouvrez le **[!UICONTROL Authentification unique]** (1).
1. Saisissez le **URL SSO** (2).
Il s’agit du lien vers votre serveur SSO (par exemple : **https://sso.mycompany.com/opensso**).

1. Saisissez le **URL de connexion** (3).
Il s’agit de l’URL qui sera appelée pour rediriger les utilisateurs vers votre fournisseur d’identité.

1. Il ne s’agit pas d’une URL réelle que vous saisissez dans le navigateur, mais plutôt d’un point de terminaison qui traitera les informations que nous lui envoyons afin de présenter l’écran de connexion.

Saisissez le **URL de déconnexion** (4).
Il s’agit de l’URL à laquelle vous revenez après votre déconnexion, par exemple

**https://www.yourcompany.com/services/logout.asp**

1. Saisissez le **empreinte du certificat** (5).
1. L’empreinte numérique SHA1 du certificat SAML fourni par votre fournisseur d’identité SAML.
1. Veillez à inclure les informations clés en les définissant sur votre fournisseur d’identité.
1. Basculer **SSO** to **[!UICONTROL Activé]** (6).
Une fois l’authentification unique activée, vous et les autres utilisateurs de votre compte vous connectez à l’aide de votre propre mécanisme d’authentification. Cela signifie que lorsque les utilisateurs accèdent à votre [!DNL Workfront Proof] écran de connexion au compte (par exemple, **yourcompany.proofhq.com/login**), vous serez invité à saisir la fenêtre de transfert de votre propre page de connexion à l’authentification.

1. (Facultatif) Activez **Configuration automatique des utilisateurs** (7).
Une fois cette option activée, les comptes d’utilisateurs sont automatiquement créés pour les personnes qui n’ont pas le leur. [!DNL Workfront Proof] , mais accède à vos [!DNL Workfront Proof] compte à l’aide de leurs identifiants de connexion unique. Cette action sera effectuée uniquement lorsque la limite utilisateur n’est pas encore atteinte pour votre compte.

1. Les autorisations de profil Manager sont attribuées par défaut aux nouveaux utilisateurs configurés. Si vous avez besoin d’informations supplémentaires, reportez-vous à la section [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Activation de l’authentification unique pour les comptes satellites

Lorsque des comptes satellites sont connectés à votre compte hub, vous pouvez les administrer au niveau du compte hub.

L’authentification unique est une fonctionnalité Select et Premium, de sorte que l’authentification unique ne peut être activée que sur les satellites qui sont sur les plans Select et Premium.

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Cliquez sur le compte satellite dans le menu déroulant (2).
1. Ouvrez le **[!UICONTROL Authentification unique]** (3).
1. Commencez à modifier la configuration SSO (4).
1. ![Activation_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Vous disposez ici de deux méthodes (5) de configuration :

1. **Hérité :** SSO avec la configuration prise à partir de votre compte hub.
Si un utilisateur accède à [!DNL Workfront Proof] via la **page de connexion par défaut** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) il y aura **deux niveaux d’autorisation**: Tout d’abord, un utilisateur est invité à se connecter à l’aide de [!DNL Workfront Proof] les données d&#39;accès (email et mot de passe) ; l’utilisateur est ensuite transféré via une fenêtre SSO vers la page de connexion SSO.
Par conséquent, avec le service SSO activé, nous vous recommandons de vous connecter par l’intermédiaire de votre propre [!DNL Workfront Proof] sous-domaine/domaine.

   >[!NOTE]
   >
   >Actuellement, lorsque l’authentification unique est activée sur votre [!DNL Workfront Proof] , vous ne pourrez pas vous connecter à l’application iPhone avec ces informations d’identification.

   1. **Manuel** (par défaut) : SSO avec une configuration différente (par exemple, pointant vers un autre fournisseur d’identité).

      >[!NOTE]
      >
      >Si le compte satellite hérite de la configuration SSO du compte hub, l’écran de connexion sera celui du compte hub. Lorsque l’utilisateur du compte satellite renseigne ses détails de connexion SSO sur cette page, il est redirigé vers le compte satellite.

      ![Activation_SSO_-_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Cliquez sur **[!UICONTROL Enregistrer]** (6).

## Paramètres d’authentification unique hérités d’un compte Hub

Lorsque vous choisissez d’hériter des paramètres de votre compte hub, vous remarquerez que tous les champs sont désormais renseignés avec les données de votre compte hub (7) et que l’authentification unique est automatiquement activée/désactivée(8) comme sur votre compte principal. Il n’existe plus de liens d’édition dans les champs, car l’ensemble de la configuration d’authentification unique pour le compte satellite est maintenant défini et géré à partir de votre compte central.

![Satellite_Account_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

Dans votre compte hub (9), la variable [!UICONTROL Utilisation du service unique] indique que cette configuration est utilisée par les comptes satellites (10).\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## SSO configuré manuellement

Si vous avez choisi la configuration d’authentification unique manuelle pour un compte satellite (1), vous devez saisir manuellement les données pour l’authentification unique.

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Ouvrez le **[!UICONTROL Authentification unique]** .
1. Cliquez sur **[!UICONTROL Modifier],** renseignez le champ, puis cliquez sur **[!UICONTROL Enregistrer]** (2).

1. Sur le **[!UICONTROL SSO]** ligne, cliquez sur **[!UICONTROL Activé]** (3).

![Satellite_Account_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## Connexion SSO

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Ouvrez le **[!UICONTROL Authentification unique]** .
1. Assurez-vous que la variable [!DNL Workfront Proof] domaine/sous-domaine (1) est configuré et que vos utilisateurs accèdent à vos [!DNL Workfront Proof] par le biais de ce domaine/sous-domaine personnalisé.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Lorsque votre authentification unique est activée, votre URL de connexion de sous-domaine (yourcompany.proofhq.com/login, par exemple) affiche un écran de transfert (2) qui vous permet d’accéder directement à la page de connexion SSO.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Si un utilisateur accède à [!DNL Workfront Proof] via la **page de connexion par défaut** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) il y aura **deux niveaux d’autorisation**. Tout d’abord, un utilisateur est invité à se connecter à l’aide de [!DNL Workfront Proof] données d&#39;accès (email et mot de passe). Ensuite, l’utilisateur est transféré via une fenêtre d’authentification unique (2) vers la page de connexion d’authentification unique.\
   Par conséquent, avec le service SSO activé, nous vous recommandons de vous connecter par l’intermédiaire de votre propre [!DNL Workfront Proof] sous-domaine/domaine.

1. Actuellement, lorsque l’authentification unique est activée sur votre compte Workfront BAT, vous ne pourrez pas vous connecter à l’application iPhone avec ces informations d’identification.

## À propos de l’ajout d’un nouvel utilisateur

Lorsque la fonctionnalité de connexion unique est activée sur votre [!DNL Workfront Proof] , les nouveaux utilisateurs ne recevront aucun email de confirmation, car leurs comptes seront automatiquement activés et prêts à l’emploi.

À partir de [!DNL Workfront Proof] Connectez-vous à la page , après avoir cliqué sur le bouton [!UICONTROL Connexion] , les utilisateurs sont redirigés vers votre page de connexion SSO et invités à saisir vos informations d’identification de connexion à authentification unique.

>[!IMPORTANT]
>
>Les utilisateurs sont identifiés par une adresse électronique au cours du processus d’authentification, ce qui signifie que le compte de messagerie utilisé pour votre connexion SSO doit correspondre à l’adresse électronique de l’utilisateur enregistré dans votre compte.

## Services de fédération principale Directory (AD FS)

Les services de fédération Principale Directory (AD FS) sont un [!DNL Microsoft] composant logiciel pouvant être installé sur les systèmes d’exploitation Windows Server afin de fournir aux utilisateurs un accès de connexion unique aux systèmes et applications situés au-delà des limites organisationnelles. Pour plus d’informations, voir &quot;Principale Directory Federation Services&quot; sur le site web de Microsoft Developer Network.

Le [!DNL Workfront Proof] Le système prend en charge SAML 2.0 et n’est compatible qu’avec AD FS version 2.0 ou ultérieure.

Voir [Connexion unique [!DNL Workfront Proof]: Configuration AD FS](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) pour obtenir des instructions détaillées.
