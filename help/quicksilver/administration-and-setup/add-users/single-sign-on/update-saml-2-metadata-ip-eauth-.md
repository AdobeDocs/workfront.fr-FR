---
title: Mise à jour des métadonnées SAML 2.0 dans votre IDP lors de l’utilisation de l’authentification améliorée
description: En tant qu’administrateur d’Adobe Workfront, vous pouvez intégrer l’authentification unique (SSO) Workfront à n’importe quel fournisseur d’identité prenant en charge le protocole SAML (Security Assertion Markup Language) 2.0.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: b6fc4775953e47a1b9d84d7537a6d9f5d35b1f2c
workflow-type: tm+mt
source-wordcount: '935'
ht-degree: 0%

---

# Mise à jour des métadonnées SAML 2.0 dans votre IDP lors de l’utilisation de l’authentification améliorée

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

En tant qu’administrateur d’Adobe Workfront, vous pouvez intégrer l’authentification unique (SSO) Workfront à n’importe quel fournisseur d’identité prenant en charge le protocole SAML (Security Assertion Markup Language) 2.0.

Les sections suivantes décrivent le processus d’intégration lorsque votre compte Workfront a été mis à niveau vers une expérience d’authentification améliorée (qui n’est pas encore disponible pour toutes les organisations). Pour plus d’informations sur l’expérience d’authentification améliorée, voir [Présentation de l’authentification améliorée](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Pour plus d’informations sur la configuration de SAML avant votre migration vers l’expérience d’authentification améliorée, voir [Mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Utiliser Okta comme fournisseur d’identité

Okta est un exemple de fournisseur d’identité qui prend en charge SAML 2.0. Cette section décrit comment utiliser Okta comme fournisseur d’identité. Des étapes similaires sont requises lors de la configuration d’un autre fournisseur d’identité prenant en charge SAML 2.0.

>[!NOTE]
>
>Les utilisateurs sont mappés en fonction de leur adresse électronique. Pour vous connecter à Workfront à l’aide d’Okta, vous devez avoir un utilisateur disposant de la même adresse électronique (insensible à la casse) créée dans votre client Workfront.

Renseignez les sections suivantes pour configurer Okta en tant que fournisseur d’identité dans Workfront.

* [Création d’une application Workfront dans Okta](#create-a-workfront-app-in-okta)
* [Ajout de votre instance Okta en tant que fournisseur d’identité dans Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Création d’une application Workfront dans Okta {#create-a-workfront-app-in-okta}

1. Connectez-vous à votre environnement Okta.
1. Assurez-vous que **IU classique** est sélectionné dans le coin supérieur gauche de l’interface d’Okta.
1. Dans le menu, cliquez sur **Applications** > **Applications**.

1. Cliquez sur **Ajouter une application**, puis cliquez sur **Créer une application**.

1. Dans le **Création d’une boîte de dialogue d’intégration d’application** , sélectionnez **SAML 2.0**, puis cliquez sur **Créer**.

1. Attribuez un nom à votre application Workfront, puis cliquez sur **Suivant**.
1. Dans la page Paramètres SAML qui s’affiche, recherchez les informations requises pour la page Paramètres SAML :

   1. Sans quitter l’onglet du navigateur dans lequel s’affiche l’interface d’Okta, ouvrez un onglet ou une fenêtre de navigateur distinct.
   1. Spécifiez l’URL suivante dans le navigateur :

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Dans le fichier XML obtenu, identifiez les valeurs de **entityID** et **Emplacement**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copiez la valeur de la propriété **entityID** du Presse-papiers du système. Ne fermez pas cet onglet du navigateur.

1. Revenez à la page Paramètres SAML que vous avez ouverte à l’étape 6.
1. Collez la valeur de la variable **entityID** dans le champ **Audience URI (ID d’entité SP)** champ .

1. Dans le fichier XML de l’autre onglet du navigateur, copiez la valeur de la variable **Emplacement** champ .
1. Collez la valeur de la variable **Emplacement** dans le champ **Authentification unique** **URL** champ .

1. Faites défiler l’écran jusqu’à **Instructions d’attribut (facultatif)** .
1. Dans le **Nom** champ, spécifiez **email**.

1. Dans le **Valeur** champ, spécifiez **user.email**.

1. (Facultatif) Ajoutez toute valeur avancée.
1. Cliquez sur **Suivant**.
1. Sélectionner, **Je suis un client Okta qui ajoute une application interne**, puis cliquez sur **Terminer**.

### Ajout de votre instance Okta en tant que fournisseur d’identité dans Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Cette procédure fournit des informations essentielles pour configurer Okta en tant que fournisseur d’identité dans Workfront. Pour plus d’informations sur d’autres mappages ou options de configuration, voir [Configuration d’Adobe Workfront avec SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Téléchargez les métadonnées du fournisseur d’identité pour votre instance Okta :

   1. Connectez-vous à votre environnement Okta.
   1. Assurez-vous que **IU classique** est sélectionné dans le coin supérieur gauche de l’interface d’Okta.
   1. Dans le menu, cliquez sur **Applications** > **Applications**.

   1. Cliquez sur l’application Workfront que vous avez créée, comme décrit dans la section , [Création d’une application Workfront dans Okta](#create-a-workfront-app-in-okta)
   1. Sur le **Se connecter** , cliquez sur **Métadonnées du fournisseur d’identité**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Les métadonnées s’ouvrent au format XML dans un nouvel onglet du navigateur.

   1. Copiez l’URL affichée dans le champ URL du navigateur.

1. Connectez-vous à Workfront en tant qu’administrateur Workfront.
1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Système** > **Authentification unique (SSO)**.

1. (Conditionnel) Si deux onglets s’affichent, cliquez sur le bouton **Nouveaux fournisseurs d’authentification unique** .

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Ne supprimez pas vos paramètres de configuration SSO existants dans **Fournisseur d’authentification unique actuel** jusqu’à ce que votre compte soit mis à jour vers l’expérience d’authentification améliorée et que la nouvelle configuration SSO soit entièrement fonctionnelle.

1. Cliquez sur **Nouveau fournisseur d’authentification unique**.
1. Spécifiez un nom, tel qu’Okta IDP, puis une description.
1. Dans le **Renseignement des champs à partir des métadonnées du fournisseur d’identité** , collez l’URL que vous avez copiée à l’étape 1 dans la section **URL de métadonnées** champ .\
   Vous pouvez également cliquer sur **Choisir un fichier** pour télécharger un fichier .xml, mais nous vous recommandons de coller l’URL.

1. Dans le **Mappage des attributs utilisateur** , dans la section **Attribut de répertoire** champ, type **email**. (**Adresse électronique** est déjà renseigné dans la variable **Attribut utilisateur Workfront** ).

1. (Facultatif) Activez **Rendre le fournisseur d’authentification unique par défaut** pour envoyer des utilisateurs non authentifiés à l’écran de connexion du fournisseur d’identité plutôt qu’à l’écran de connexion de Workfront pour authentification. Nous vous recommandons d’activer cette option uniquement si tous les utilisateurs de votre système accèdent à Workfront par l’intermédiaire du fournisseur d’identité.
1. Sélectionnez la **Activer** . Avant de procéder, assurez-vous que les utilisateurs de votre système connaissent la nouvelle expérience de connexion afin de s’assurer qu’ils n’ont pas perdu l’accès au système Workfront.
1. Cliquez sur **Tester la connexion**.\
   Un message vous indique que la connexion a réussi.

1. Cliquer sur **Enregistrer**.

## Utilisation d’autres fournisseurs d’identité

Lorsque vous utilisez des fournisseurs d’identité autres que Okta (tels que Ping ou Centrify), vous devez charger à nouveau les métadonnées Workfront sur votre fournisseur d’identité.
