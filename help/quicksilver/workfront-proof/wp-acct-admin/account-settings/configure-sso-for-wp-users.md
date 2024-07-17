---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Configuration de l’authentification unique pour les utilisateurs  [!DNL Workfront Proof]
description: Si vous disposez du plan Select ou Premium, vous pouvez fournir une fonctionnalité de connexion unique (SSO) qui vous permet d’utiliser le nom d’utilisateur et le mot de passe de votre organisation existante pour accéder à votre compte  [!DNL Workfront Proof] .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 007a603ef1df2a02959d7fb623ac784bf5b9cb80
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# Configuration de l’authentification unique pour les utilisateurs de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Si vous disposez du plan Select ou Premium, vous pouvez fournir une fonctionnalité de connexion unique (SSO) qui vous permet d’utiliser le nom d’utilisateur et le mot de passe de votre organisation existante pour accéder à votre compte [!DNL Workfront Proof].

Cela signifie que vous vous authentifierez par rapport à votre propre système de connexion, et non par rapport à la page de connexion [!DNL Workfront Proof].

>[!NOTE]
>
>Un sous-domaine ou domaine personnalisé doit être configuré sur votre compte [!DNL Workfront Proof] pour activer SAML. Les sous-domaines personnalisés peuvent être configurés librement. Voir [Marque](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) pour plus d’informations. Vous pouvez en savoir plus sur les domaines entièrement personnalisés sur notre [ site de marque  [!DNL Workfront Proof] avancé](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Activation de l’authentification unique dans [!DNL Workfront Proof]

La fonctionnalité de connexion unique peut être activée dans l’onglet [!UICONTROL Authentification unique] de vos [!UICONTROL  paramètres de compte ]. Elle s’appliquera à tous les utilisateurs de votre compte [!DNL Workfront Proof]. Pour plus d’informations, voir [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) .

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

1. Ouvrez l’onglet **[!UICONTROL Connexion unique]** (1).
1. Saisissez l’ **URL SSO** (2).
Il s’agit du lien vers votre serveur SSO (par exemple, **https://sso.mycompany.com/opensso**).

1. Saisissez l’ **URL de connexion** (3).
Il s’agit de l’URL qui sera appelée pour rediriger les utilisateurs vers votre fournisseur d’identité.

1. Il ne s’agit pas d’une URL réelle que vous saisissez dans le navigateur, mais plutôt d’un point de terminaison qui traitera les informations que nous lui envoyons afin de présenter l’écran de connexion.

Saisissez l’ **URL de déconnexion** (4).
Il s’agit de l’URL à laquelle vous revenez après votre déconnexion, par exemple

**https://www.yourcompany.com/services/logout.asp**

1. Saisissez l’ **empreinte du certificat** (5).
1. L’empreinte numérique SHA1 du certificat SAML fourni par votre fournisseur d’identité SAML.
1. Veillez à inclure les informations clés en les définissant sur votre fournisseur d’identité.
1. Passez **SSO** à **[!UICONTROL Activé]** (6).
Une fois l’authentification unique activée, vous et les autres utilisateurs de votre compte vous connectez à l’aide de votre propre mécanisme d’authentification. Cela signifie que lorsque les utilisateurs accèdent à l’écran de connexion de votre compte [!DNL Workfront Proof] (par exemple, **yourcompany.proofhq.com/login**), ils sont invités à afficher la fenêtre de transfert vers votre propre page de connexion d’authentification.

1. (Facultatif) Activez l’option **Fournir automatiquement des utilisateurs** (7).
Une fois cette option activée, les comptes d’utilisateurs sont automatiquement créés pour les personnes qui n’ont pas leurs propres profils [!DNL Workfront Proof], mais qui accèdent à votre compte [!DNL Workfront Proof] à l’aide de leurs informations d’identification de connexion unique. Cette action sera effectuée uniquement lorsque la limite utilisateur n’est pas encore atteinte pour votre compte.

1. Les autorisations de profil Manager sont attribuées par défaut aux nouveaux utilisateurs configurés. Si vous avez besoin d’informations supplémentaires, reportez-vous à la section [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Activation de l’authentification unique pour les comptes satellites

Lorsque des comptes satellites sont connectés à votre compte hub, vous pouvez les administrer au niveau du compte hub.

L’authentification unique est une fonctionnalité Select et Premium, de sorte que l’authentification unique ne peut être activée que sur les satellites qui sont sur les plans Select et Premium.

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Cliquez sur le compte satellite dans le menu déroulant (2).
1. Ouvrez l’onglet **[!UICONTROL Connexion unique]** (3).
1. Commencez à modifier la configuration SSO (4).
1. ![Enenabling_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Vous disposez ici de deux méthodes (5) de configuration :

1. **Hérité :** SSO avec la configuration prise à partir de votre compte hub.
Si un utilisateur accède à [!DNL Workfront Proof] par l’intermédiaire de la **page de connexion par défaut** ([https://www.proofhq.com/login](https://www.proofhq.com/login)), il y aura **deux niveaux d’autorisation** : il est d’abord demandé à un utilisateur de se connecter à l’aide des [!DNL Workfront Proof] données d’accès (adresse électronique et mot de passe) ; l’utilisateur est transféré via une fenêtre d’authentification unique vers la page de connexion SSO.
Par conséquent, avec le service SSO activé, nous vous recommandons de vous connecter via votre propre sous-domaine/domaine [!DNL Workfront Proof].

   >[!NOTE]
   >
   >Actuellement, lorsque l’authentification unique est activée sur votre compte [!DNL Workfront Proof], vous ne pourrez pas vous connecter à l’application iPhone avec ces informations d’identification.

   1. **Manuel** (par défaut) : SSO avec une configuration différente (pointant par exemple vers un autre fournisseur d’identité).

      >[!NOTE]
      >
      >Si le compte satellite hérite de la configuration SSO du compte hub, l’écran de connexion sera celui du compte hub. Lorsque l’utilisateur du compte satellite renseigne ses détails de connexion SSO sur cette page, il est redirigé vers le compte satellite.

      ![Enenabling_SSO_-_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Cliquez sur **[!UICONTROL Enregistrer]** (6).

## Paramètres d’authentification unique hérités d’un compte Hub

Lorsque vous choisissez d’hériter des paramètres de votre compte hub, vous remarquerez que tous les champs sont désormais renseignés avec les données de votre compte hub (7) et que l’authentification unique est automatiquement activée/désactivée(8) comme sur votre compte principal. Il n’existe plus de liens d’édition dans les champs, car l’ensemble de la configuration d’authentification unique pour le compte satellite est maintenant défini et géré à partir de votre compte central.

![Satellite_Account_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

Dans votre compte hub (9), le champ [!UICONTROL Utilisation de l’authentification unique] indique que cette configuration est utilisée par les comptes satellites (10).\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## SSO configuré manuellement

Si vous avez choisi la configuration d’authentification unique manuelle pour un compte satellite (1), vous devez saisir manuellement les données pour l’authentification unique.

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Ouvrez l’onglet **[!UICONTROL Authentification unique]** .
1. Cliquez sur **[!UICONTROL Modifier],** pour remplir le champ, puis cliquez sur **[!UICONTROL Enregistrer]** (2).

1. Sur la ligne **[!UICONTROL SSO]**, cliquez sur **[!UICONTROL Enabled]** (3).

![Satellite_Account_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## Connexion SSO

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]** (1).

1. Ouvrez l’onglet **[!UICONTROL Authentification unique]** .
1. Assurez-vous que votre domaine/sous-domaine [!DNL Workfront Proof] (1) est configuré et que vos utilisateurs accèdent à votre compte [!DNL Workfront Proof] via ce domaine/sous-domaine personnalisé.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Lorsque l’authentification unique est activée, l’URL de connexion au sous-domaine (yourcompany.proofhq.com/login, par exemple) affiche un écran de transfert (2) qui vous permet d’accéder directement à la page de connexion SSO.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Si un utilisateur accède à [!DNL Workfront Proof] par l’intermédiaire de la **page de connexion par défaut** ([https://www.proofhq.com/login](https://www.proofhq.com/login)), il y aura **deux niveaux d’autorisation**. Un utilisateur est d’abord invité à se connecter à l’aide des données d’accès [!DNL Workfront Proof] (adresse électronique et mot de passe). Ensuite, l’utilisateur est transféré via une fenêtre d’authentification unique (2) vers la page de connexion d’authentification unique.\
   Par conséquent, avec le service SSO activé, nous vous recommandons de vous connecter via votre propre sous-domaine/domaine [!DNL Workfront Proof].

1. Actuellement, lorsque l’authentification unique est activée sur votre compte Workfront Proof, vous ne pourrez pas vous connecter à l’application iPhone avec ces informations d’identification.

## À propos de l’ajout d’un nouvel utilisateur

Lorsque la fonctionnalité de connexion unique est activée sur votre compte [!DNL Workfront Proof], les nouveaux utilisateurs ne reçoivent aucun e-mail de confirmation, car leurs comptes sont automatiquement activés et prêts à l’emploi.

Sur la page de connexion [!DNL Workfront Proof], après avoir cliqué sur le bouton [!UICONTROL Connexion], les utilisateurs sont redirigés vers votre page de connexion SSO et sont invités à saisir vos informations d’identification de connexion à authentification unique.

>[!IMPORTANT]
>
>Les utilisateurs sont identifiés par une adresse électronique au cours du processus d’authentification, ce qui signifie que le compte de messagerie utilisé pour votre connexion SSO doit correspondre à l’adresse électronique de l’utilisateur enregistré dans votre compte.

## Active Directory Federation Services (AD FS)

Active Directory Federation Services (AD FS) est un composant logiciel [!DNL Microsoft] qui peut être installé sur les systèmes d’exploitation Windows Server pour fournir aux utilisateurs un accès de connexion unique aux systèmes et applications situés au-delà des limites organisationnelles. Pour plus d’informations, voir &quot;Active Directory Federation Services&quot; sur le site web de Microsoft Developer Network.

Le système [!DNL Workfront Proof] prend en charge SAML 2.0 et n’est compatible qu’avec AD FS version 2.0 ou supérieure.

Pour obtenir des instructions détaillées, reportez-vous à la section [Connexion unique dans [!DNL Workfront Proof] : configuration AD FS](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) .
