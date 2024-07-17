---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Intégrer [!DNL Workfront Proof]  avec Basecamp Classic
description: Si vous utilisez  [!DNL Basecamp] pour la gestion de projet, vous pouvez offrir à votre équipe de projet des outils de révision et d'approbation plus riches en utilisant [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Intégrer [!DNL Workfront Proof] avec [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Si vous utilisez [!DNL Basecamp] pour la gestion de projet, vous pouvez offrir à votre équipe de projet des outils de révision et d&#39;approbation plus riches en utilisant [!DNL Workfront Proof].

## Présentation de l’intégration [!DNL Basecamp] avec [!DNL Workfront]

L’intégration à [!DNL Basecamp] permet aux utilisateurs d’afficher, de réviser et d’approuver les bons à tirer tous dans [!DNL Basecamp]. Les utilisateurs peuvent envoyer des bons à tirer à votre compte [!DNL Workfront Proof] et les connecter à votre projet [!DNL Basecamp]. Vos réviseurs peuvent et font [ une décision sur un BAT dans la visionneuse de correctifs ](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp], en utilisant le mini-BAT incorporé dans votre message Basecamp.

Lorsqu&#39;il est intégré à [!DNL Workfront Proof], [!DNL Basecamp] permet aux utilisateurs d&#39;effectuer les opérations suivantes avec des bons à tirer :

* Les utilisateurs peuvent consulter et approuver les bons à tirer dans [!DNL Basecamp Classic].
* Les utilisateurs disposent d’outils de révision facilement disponibles.
* Les équipes d’examen de projet reçoivent un message dans [!DNL Basecamp] avec un mini BAT pour révision et approbation.
* Les utilisateurs peuvent passer à un BAT de page entière pour révision et approbation.
* Les utilisateurs peuvent ajouter des commentaires et des annotations aux mini-bons à tirer et aux bons à tirer.

  >[!NOTE]
  >
  >Une fois qu’un commentaire a reçu une réponse, il ne peut pas être modifié ni supprimé.

* Les réviseurs peuvent répondre aux balises et effectuées par d’autres réviseurs.
* Les utilisateurs sont avertis lorsqu’une nouvelle version du BAT est disponible.
* Les utilisateurs qui ne sont pas [!DNL Workfront Proof] peuvent travailler sur un BAT dans [!DNL Basecamp].

L’intégration de [!DNL Workfront Proof] avec [!DNL Basecamp] doit être configurée à deux niveaux :

* Configurez [!DNL Basecamp] dans [Paramètres du compte :](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Cela permet l’intégration Basecamp pour l’ensemble de votre organisation.
* Pour plus d’informations, voir [Activation de l’ [!DNL Basecamp] intégration avec [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Configurez [!DNL Basecamp] dans [Paramètres personnels](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) : cela permet aux créateurs et aux propriétaires de BAT de se connecter à leur compte personnel [!DNL Basecamp] et d&#39;autoriser l&#39;accès à [!DNL Workfront Proof]. Pour plus d’informations, voir [Configuration des paramètres personnels](#configuring-personal-settings).

Vous pouvez intégrer [!DNL Workfront] à [!DNL Basecamp] ou [!DNL Basecamp Classic]. Chaque version de [!DNL Basecamp] utilise une API différente et nécessite donc des procédures de configuration différentes.

Pour plus d&#39;informations sur la configuration de [!DNL Basecamp Classic], voir [Activation de l&#39; [!DNL Basecamp] intégration avec [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) dans cet article.

Pour plus d&#39;informations sur la configuration de [!DNL Basecamp], voir [Intégrer [!DNL Workfront Proof] avec [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Activation de l’intégration [!DNL Basecamp] avec [!DNL Workfront Proof]

En tant que [ {Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) ou [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), vous pouvez configurer l’intégration Basecamp pour l’ensemble du compte dans les [paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Accédez à [Paramètres du compte.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Ouvrez l’onglet **[!UICONTROL Intégrations]** (1).
1. Pour activer l’intégration Basecamp, cliquez sur **[!UICONTROL Activer]** (2).
1. Vérifiez que [!DNL Basecamp Classic] est la version que vous intégrez à (3).
1. (Conditionnel) Si aucune URL [!DNL Basecamp] ne s’affiche (4), cliquez sur **[!UICONTROL Modifier]** et saisissez l’URL de votre compte [!DNL Basecamp] (sans le http://).
1. Cliquez sur **[!UICONTROL Enregistrer]** (5).\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Facultatif) Vérifiez l’URL [!DNL Basecamp] dans votre navigateur après vous être connecté à votre compte [!DNL Basecamp Classic] (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   Une fois que vous avez intégré [!DNL Workfront Proof] à [!DNL Basecamp], vos utilisateurs peuvent configurer leurs paramètres personnels. Pour plus d’informations sur la configuration des paramètres personnels, voir [Configuration des paramètres personnels](#configuring-personal-settings).

   Si vous ne pouvez pas activer l&#39;intégration [!DNL Basecamp], votre ID de compte [!DNL Workfront Proof] peut ne pas être identique à l&#39;ID de compte que vous utilisez dans [!DNL Basecamp].

## Configuration des paramètres personnels

Après avoir configuré les [ paramètres du compte ](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) pour votre organisation, chacun des auteurs qui créent/envoient des bons à tirer doit définir ses [ paramètres personnels.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Il est plus facile de suivre ces étapes si votre session [!DNL Basecamp] est ouverte dans une fenêtre de navigateur et que votre session [!DNL Workfront Proof] est ouverte dans une autre fenêtre.

* [Récupération de votre  [!DNL Basecamp] jeton API](#retrieving-your-basecamp-api-token)
* [Ajout de votre jeton API  [!DNL Basecamp] à vos paramètres personnels](#adding-your-basecamp-api-token-to-your-personal-settings)

### Récupération de votre jeton d’API [!DNL Basecamp]

Pour terminer l’intégration au niveau individuel dans [!DNL Workfront Proof], les utilisateurs ont besoin de leur jeton d’authentification individuel pour l’API [!DNL Basecamp].

Pour récupérer votre jeton d’API [!DNL Basecamp] :

1. Connectez-vous à votre compte [!DNL Basecamp].
1. Cliquez sur **[!UICONTROL My Info]** (1) dans le coin supérieur droit de l’écran.\
   La page [!UICONTROL My Info] s’affiche.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. Dans la section [!UICONTROL jetons d’authentification], cliquez sur **[!UICONTROL Afficher vos jetons]** (2) pour afficher vos jetons d’authentification personnels.
1. Sélectionnez le **[!UICONTROL jeton pour les lecteurs de flux]** ou l’ **[!UICONTROL API Basecamp]** (3), puis copiez le jeton dans le presse-papiers.

1. Collez votre jeton d’API [!DNL Basecamp] dans la zone [!UICONTROL Jeton pour les lecteurs de flux] ou [!UICONTROL API Basecamp].\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Ajout de votre jeton d’API [!DNL Basecamp] à vos paramètres personnels

Pour coller le jeton d&#39;API [!DNL Basecamp] dans vos [!DNL Workfront Proof] [Paramètres personnels](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) :

1. Accédez à [[!UICONTROL Intégrations] - Configuration utilisateur](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) dans vos [Paramètres personnels](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1).\
   Un administrateur doit d’abord activer l’intégration [!DNL Basecamp Classic] pour que vous puissiez activer vos paramètres personnels. Pour plus d&#39;informations sur la configuration de l&#39;intégration, voir [Activation de l&#39; [!DNL Basecamp] intégration avec [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) dans cet article.

1. Dans la zone de jeton API [!DNL Basecamp] (2), collez le jeton que vous venez de copier de votre page [!DNL Basecamp] [!UICONTROL My Info] dans le champ (3).\
   Pour plus d’informations sur la copie de votre jeton d’API [!DNL Basecamp], voir [Récupération de votre [!DNL Basecamp] jeton d’API](#retrieving-your-basecamp-api-token) dans cet article.

1. Cliquez sur **[!UICONTROL Enregistrer]** (4).

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Vos [!DNL Workfront Proof] [paramètres personnels](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) sont désormais intégrés à votre compte [!DNL Basecamp Classic].
