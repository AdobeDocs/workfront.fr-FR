---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Intégrer  [!DNL Workfront Proof]  à Basecamp Classic
description: Si vous utilisez  [!DNL Basecamp]  pour la gestion de projets, vous pouvez proposer à votre équipe de projet des outils de révision et d’approbation plus riches à l’aide de  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 100%

---

# Intégrer [!DNL Workfront Proof] à [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit [!DNL Workfront Proof] autonome. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Si vous utilisez [!DNL Basecamp] pour la gestion de projets, vous pouvez proposer à votre équipe de projet des outils de révision et d’approbation plus riches à l’aide de [!DNL Workfront Proof].

## Comprendre l’intégration de [!DNL Basecamp] à [!DNL Workfront]

L’intégration à [!DNL Basecamp] permet aux utilisateurs et utilisatrices d’afficher, de réviser et d’approuver des épreuves dans [!DNL Basecamp]. Les utilisateurs et utilisatrices peuvent envoyer des épreuves à votre compte [!DNL Workfront Proof] et les connecter à votre projet [!DNL Basecamp]. Vos réviseurs et réviseuses peuvent [prendre une décision sur une épreuve dans la visionneuse de relecture](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp], à l’aide de la mini-épreuve incorporée dans votre message Basecamp.

Lorsqu’il est intégré à [!DNL Workfront Proof], [!DNL Basecamp] permet aux utilisateurs et utilisatrices d’effectuer les opérations suivantes sur les épreuves :

* Les utilisateurs et utilisatrices peuvent réviser et approuver des épreuves dans [!DNL Basecamp Classic].
* Les utilisateurs et utilisatrices disposent d’outils de révision facilement disponibles.
* Les équipes de révision de projet reçoivent un message dans [!DNL Basecamp] avec une mini-épreuve pour révision et approbation.
* Les utilisateurs et utilisatrices peuvent basculer vers une épreuve en pleine page à des fins de révision et d’approbation.
* Les utilisateurs et utilisatrices peuvent ajouter des commentaires et des annotations aux mini-épreuves et aux épreuves en taille réelle.

  >[!NOTE]
  >
  >Une fois qu’une réponse a été ajoutée à un commentaire, ce dernier ne peut pas être modifié ni supprimé.

* Les réviseurs et réviseuses peuvent répondre aux commentaires et aux balisages d’autres réviseurs et réviseuses.

* Les utilisateurs et utilisatrices sont avertis lorsqu’une nouvelle version de l’épreuve est disponible.
* Les utilisateurs et utilisatrices qui n’utilisent pas [!DNL Workfront Proof] peuvent travailler sur une épreuve dans [!DNL Basecamp].

L’intégration de [!DNL Workfront Proof] à [!DNL Basecamp] doit être configurée à deux niveaux :

* Configurer [!DNL Basecamp] dans [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) : permet d’intégrer Basecamp pour l’ensemble de votre entreprise.
* Pour plus d’informations, voir [Activer l’intégration de  [!DNL Basecamp]  à  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Configurer [!DNL Basecamp] dans [Paramètres personnels](https://support.workfront.com/hc/fr-fr/sections/115000921168-Personal-settings) : permet aux créateurs et créatrices et aux personnes propriétaires d’épreuves de se connecter à leur compte [!DNL Basecamp] personnel et d’autoriser l’accès à [!DNL Workfront Proof]. Pour plus d’informations, voir [Configurer les paramètres personnels](#configuring-personal-settings).

Vous pouvez intégrer [!DNL Workfront] à [!DNL Basecamp] ou [!DNL Basecamp Classic]. Chaque version de [!DNL Basecamp] utilise une API différente et nécessite donc des procédures de configuration différentes.

Pour plus d’informations sur la configuration de [!DNL Basecamp Classic], voir [Activer l’intégration de  [!DNL Basecamp]  à  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) dans cet article.

Pour plus d’informations sur la configuration de [!DNL Basecamp], voir [Intégrer  [!DNL Workfront Proof]  à  [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Activer l’intégration de [!DNL Basecamp] à [!DNL Workfront Proof]

Comme les [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) ou les [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), vous pouvez configurer l’intégration de Basecamp pour l’ensemble du compte dans les [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Accédez à [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).
1. Ouvrez l’onglet **[!UICONTROL Intégrations]** (1).
1. Pour activer l’intégration de Basecamp, cliquez sur **[!UICONTROL Activer]** (2).
1. Vérifiez que [!DNL Basecamp Classic] est la version avec laquelle vous effectuez l’intégration (3).
1. (Le cas échéant) Si aucune URL [!DNL Basecamp] ne s’affiche (4), cliquez sur **[!UICONTROL Modifier]** et saisissez l’URL de votre compte [!DNL Basecamp] (sans http://).
1. Cliquez sur **[!UICONTROL Enregistrer]** (5).\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Facultatif) Vérifiez votre URL [!DNL Basecamp] dans votre navigateur une fois que la connexion est établie à votre compte [!DNL Basecamp Classic] (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   Une fois que vous avez intégré [!DNL Workfront Proof] à [!DNL Basecamp], vos utilisateurs et utilisatrices peuvent configurer leurs paramètres personnels. Pour plus d’informations sur la configuration des paramètres personnels, voir [Configuration des paramètres personnels](#configuring-personal-settings).

   Si vous ne pouvez pas activer l’intégration de [!DNL Basecamp], votre identifiant de compte [!DNL Workfront Proof] peut ne pas être identique à l’identifiant de compte utilisé dans [!DNL Basecamp].

## Configurer les paramètres personnels

Après avoir configuré les [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) pour votre organisation, chaque auteur ou autrice créant/envoyant des épreuves doit définir ses [paramètres personnels](https://support.workfront.com/hc/fr-fr/sections/115000921168-Personal-settings).

>[!NOTE]
>
>Il est plus facile de suivre ces étapes si votre session [!DNL Basecamp] est ouverte dans une fenêtre de navigateur et que votre session [!DNL Workfront Proof] est ouverte dans une autre.

* [Récupérer votre jeton API  [!DNL Basecamp] ](#retrieving-your-basecamp-api-token)
* [Ajouter votre jeton API  [!DNL Basecamp]  à vos paramètres personnels](#adding-your-basecamp-api-token-to-your-personal-settings)

### Récupérer votre jeton API [!DNL Basecamp]

Pour terminer l’intégration au niveau individuel dans [!DNL Workfront Proof], les personnes ont besoin de leur jeton d’authentification individuel pour l’API [!DNL Basecamp].

Pour récupérer votre jeton API [!DNL Basecamp] :

1. Connectez-vous à votre compte [!DNL Basecamp].
1. Cliquez sur **[!UICONTROL Mes informations]** (1) dans le coin supérieur droit de l’écran.\
   La page [!UICONTROL Mes informations] s’affiche.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. Dans la section [!UICONTROL Jetons d’authentification], cliquez sur **[!UICONTROL Afficher vos jetons]** (2) pour afficher vos jetons d’authentification personnels.
1. Sélectionnez le **[!UICONTROL Jeton pour les lecteurs de flux]** ou l’**[!UICONTROL API Basecamp]** (3), puis copiez le jeton dans le presse-papiers.

1. Collez votre jeton d’API [!DNL Basecamp] dans la zone [!UICONTROL Jeton pour les lecteurs de flux] ou [!UICONTROL API Basecamp].\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Ajouter votre jeton API [!DNL Basecamp] à vos paramètres personnels

Pour coller le jeton API [!DNL Basecamp] dans vos [Paramètres personnels](https://support.workfront.com/hc/fr-fr/sections/115000921168-Personal-settings) [!DNL Workfront Proof] :

1. Accédez à [[!UICONTROL Intégrations] - Configuration des utilisateurs et utilisatrices](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) dans vos [Paramètres personnels](https://support.workfront.com/hc/fr-fr/sections/115000921168-Personal-settings) (1).\
   L’équipe d’administration doit d’abord activer l’intégration de [!DNL Basecamp Classic] pour activer vos paramètres personnels. Pour plus d’informations sur la configuration de l’intégration, voir [Activation de l’intégration  [!DNL Basecamp]  avec  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) dans cet article.

1. Dans la zone Jeton API [!DNL Basecamp] (2), collez le jeton que vous venez de copier à partir de votre page [!UICONTROL Mes informations] [!DNL Basecamp] dans le champ (3).\
   Pour plus d’informations sur la copie de votre jeton API [!DNL Basecamp], voir [Récupération de votre jeton API  [!DNL Basecamp] ](#retrieving-your-basecamp-api-token) dans cet article.

1. Cliquez sur **[!UICONTROL Enregistrer]** (4).

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Vos [Paramètres personnels](https://support.workfront.com/hc/fr-fr/sections/115000921168-Personal-settings) [!DNL Workfront Proof] sont désormais intégrés à votre compte [!DNL Basecamp Classic].
