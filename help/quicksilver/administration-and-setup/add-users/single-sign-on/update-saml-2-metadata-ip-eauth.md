---
title: Mettre à jour les métadonnées SAML 2.0 dans votre fournisseur d’identité lors de l’utilisation de l’authentification améliorée
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez intégrer l’authentification unique (SSO) Workfront à n’importe quel fournisseur d’identité prenant en charge le protocole SAML (Security Assertion Markup Language) 2.0.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 98%

---

# Mettre à jour les métadonnées SAML 2.0 dans votre IDP avec l’authentification renforcée

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez intégrer l’authentification unique (SSO) Workfront à n’importe quel fournisseur d’identité prenant en charge le protocole SAML (Security Assertion Markup Language) 2.0.

Les sections suivantes décrivent le processus d’intégration lorsque votre compte Workfront a été mis à niveau vers une expérience d’authentification améliorée (qui n’est pas encore disponible pour toutes les organisations). Pour plus d’informations sur l’expérience d’authentification améliorée, voir [Vue d’ensemble de l’authentification améliorée](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Pour plus d’informations sur la configuration de SAML avant votre migration vers l’expérience d’authentification améliorée, voir [Mettre à jour les métadonnées SAML 2.0 dans votre fournisseur d’identité](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Utiliser Okta comme fournisseur d’identité

Okta est un exemple de fournisseur d’identité qui prend en charge SAML 2.0. Cette section décrit comment utiliser Okta en tant que fournisseur d’identité. Des étapes similaires sont requises lors de la configuration d’un autre fournisseur d’identité prenant en charge SAML 2.0.

>[!NOTE]
>
>Les personnes sont mappées en fonction de leur adresse e-mail. Pour se connecter à Workfront à l’aide d’Okta, une personne doit avoir la même adresse e-mail (sans respect de la casse) que celle créée dans son compte Workfront.

Renseignez les sections suivantes pour configurer Okta en tant que fournisseur d’identité dans Workfront.

* [Créer une application Workfront dans Okta](#create-a-workfront-app-in-okta)
* [Ajouter votre instance Okta en tant que fournisseur d’identité dans Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Créer une application Workfront dans Okta {#create-a-workfront-app-in-okta}

1. Connectez-vous à votre environnement Okta.
1. Assurez-vous que l’option **IU classique** est sélectionnée dans le coin supérieur gauche de l’interface d’Okta.
1. Dans le menu, cliquez sur **Applications** > **Applications**.

1. Cliquez sur **Ajouter une application**, puis cliquez sur **Créer une application**.

1. Dans la boîte de dialogie **Créer une intégration d’application**, sélectionnez **SAML 2.0**, puis cliquez sur **Créer**.

1. Attribuez un nom à votre application Workfront, puis cliquez sur **Suivant**.
1. Dans la page Paramètres SAML qui s’affiche, recherchez les informations requises pour la page Paramètres SAML :

   1. Sans quitter l’onglet du navigateur dans lequel s’affiche l’interface d’Okta, ouvrez un onglet ou une fenêtre de navigateur distinct.
   1. Spécifiez l’URL suivante dans le navigateur :

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Dans le fichier XML obtenu, identifiez les valeurs **entityID** et **Emplacement**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copiez la valeur du champ **entityID** vers le presse-papiers du système. Ne fermez pas cet onglet du navigateur.

1. Revenez à la page Paramètres SAML que vous avez ouverte à l’étape 6.
1. Collez la valeur du champ **entityID** dans le champ **URI d’audience (ID d’entité SP)**.

1. Dans le fichier XML de l’autre onglet du navigateur, copiez la valeur du champ **Emplacement**.
1. Collez la valeur du champ **Emplacement** dans le champ **URL** d’**authentification unique**.

1. Faites défiler l’écran jusqu’à la section **Instructions d’attribut (facultatif)**.
1. Dans le champ **Nom**, spécifiez **e-mail**.

1. Dans le champ **Valeur**, spécifiez **e-mail utilisateur ou utilisatrice**.

1. (Facultatif) Ajoutez toute valeur avancée.
1. Cliquez sur **Suivant**.
1. Sélectionnez **Je suis un client ou une cliente Okta qui ajoute une application interne**, puis cliquez sur **Terminer**.

### Ajouter votre instance Okta en tant que fournisseur d’identité dans Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Cette procédure fournit des informations essentielles pour configurer Okta en tant que fournisseur d’identité dans Workfront. Pour plus d’informations sur d’autres mappages ou options de configuration, consultez la section [Configurer Adobe Workfront avec SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Téléchargez les métadonnées du fournisseur d’identité pour votre instance Okta :

   1. Connectez-vous à votre environnement Okta.
   1. Assurez-vous que l’option **IU classique** est sélectionnée dans le coin supérieur gauche de l’interface d’Okta.
   1. Dans le menu, cliquez sur **Applications** > **Applications**.

   1. Cliquez sur l’application Workfront que vous avez créée, comme décrit dans la section [Créer une application Workfront dans Okta.](#create-a-workfront-app-in-okta)
   1. Sur l’onglet **Authentification**, cliquez sur **Métadonnées du fournisseur d’identité**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Les métadonnées s’ouvrent au format XML dans un nouvel onglet du navigateur.

   1. Copiez l’URL affichée dans le champ URL du navigateur.

1. Connectez-vous à Workfront en tant que personne membre de l’administration Workfront.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Authentification unique (SSO)**.

1. (Le cas échéant) Si deux onglets s’affichent, cliquez sur l’onglet **Nouveaux fournisseurs d’authentification unique**.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Ne supprimez pas vos paramètres de configuration SSO existants dans l’onglet **Fournisseur SSO actuel** jusqu’à ce que votre compte soit mis à jour vers l’expérience d’authentification améliorée et que la nouvelle configuration SSO soit entièrement fonctionnelle.

1. Cliquez sur **Nouveau fournisseur SSO**.
1. Spécifiez un nom, tel qu’Okta IDP, puis une description.
1. Dans la section **Renseigner les champs à partir des métadonnées du fournisseur d’identité**, collez l’URL que vous avez copiée à l’étape 1 dans le champ **URL de métadonnées**.\
   Vous pouvez également cliquer sur **Choisir un fichier** pour charger un fichier .xml, mais nous vous recommandons de coller l’URL.

1. Dans la section **Mapper les attributs d’utilisateur ou d’utilisatrice**, dans le champ **Attribut de répertoire**, saisissez **e-mail**. (**Adresse e-mail** est déjà renseigné dans le champ **Attribut d’utilisateur ou d’utilisatrice Workfront**).

1. (Facultatif) Activez **Fournisseur SSO par défaut** pour rediriger les utilisateurs et les utilisatrices dont l’authentification n’a pas été effectuée vers l’écran de connexion du fournisseur d’identité au lieu de l’écran de connexion de Workfront pour leur authentification. Nous vous recommandons d’activer cette option uniquement si l’ensemble des utilisateurs et des utilisatrices de votre système accèdent à Workfront par l’intermédiaire du fournisseur d’identité.
1. Cochez la case **Activer**. Avant de procéder, assurez-vous que les utilisateurs et les utilisatrices de votre système connaissent la nouvelle expérience de connexion afin de s’assurer qu’ils n’ont pas perdu l’accès au système Workfront.
1. Cliquez sur **Tester la connexion**.\
   Un message vous indique que la connexion a réussi.

1. Cliquer sur **Enregistrer**.

## Utiliser d’autres fournisseurs d’identité

Lorsque vous utilisez des fournisseurs d’identité autres que Okta (tels que Ping ou Centrify), vous devez charger à nouveau les métadonnées Workfront sur votre fournisseur d’identité.
