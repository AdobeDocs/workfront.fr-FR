---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Intégrer [!DNL Workfront Proof] avec [!DNL Basecamp]
description: Si vous utilisez [!DNL Basecamp] pour la gestion de projet, vous pouvez proposer à votre équipe de projet des outils d’examen et d’approbation plus riches en utilisant [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 0%

---

# Intégrer [!DNL Workfront Proof] avec [!DNL Basecamp]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

Si vous utilisez [!DNL Basecamp] pour la gestion de projet, vous pouvez proposer à votre équipe de projet des outils d’examen et d’approbation plus riches en utilisant [!DNL Workfront Proof].

## Présentation de la fonction [!DNL Basecamp] Intégration avec [!DNL Workfront]

Intégration avec [!DNL Basecamp] permet aux utilisateurs d’afficher, de réviser et d’approuver les bons à tirer dans [!DNL Basecamp]. Les utilisateurs peuvent envoyer des bons à tirer à votre [!DNL Workfront Proof] et connectez-les à votre [!DNL Basecamp] projet. Vos réviseurs peuvent commenter et prendre des décisions via [!DNL Basecamp], à l’aide du mini-BAT incorporé dans votre message Basecamp .

Lorsqu’il est intégré à [!DNL Workfront Proof], [!DNL Basecamp] dispose de la fonctionnalité de vérification suivante :

* Les utilisateurs peuvent consulter et approuver des BAT dans [!DNL Basecamp Classic].
* Les utilisateurs disposent d’outils de révision facilement disponibles.
* Les équipes d’examen de projet reçoivent un message dans [!DNL Basecamp] avec un mini BAT pour révision et validation.
* Les utilisateurs peuvent passer à un BAT de page entière pour révision et approbation.
* Les utilisateurs peuvent ajouter des commentaires et des annotations aux mini-bons à tirer et aux bons à tirer.

   >[!NOTE]
   >
   >Une fois qu’un commentaire a reçu une réponse, il ne peut pas être modifié ni supprimé.

* Les réviseurs peuvent répondre aux balises et effectuées par d’autres réviseurs.
* Les utilisateurs sont avertis lorsqu’une nouvelle version du BAT est disponible.
* Utilisateurs qui ne sont pas [!DNL Workfront Proof] les utilisateurs peuvent travailler sur un BAT dans [!DNL Basecamp].

L’intégration de [!DNL Workfront Proof] avec [!DNL Basecamp] doit être configuré à deux niveaux :

* Configurer [!DNL Basecamp] in [Paramètres du compte :](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Cela permet l’intégration Basecamp pour l’ensemble de votre organisation. Pour plus d’informations, voir [Activation de l’intégration Basecamp avec [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Configurer [!DNL Basecamp] in [Paramètres personnels](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Cela permet aux créateurs et aux propriétaires de BAT de se connecter à leur compte Basecamp personnel et d’autoriser [!DNL Workfront Proof] accès. Pour plus d’informations, voir [Configuration des paramètres personnels](#configuring-personal-settings).

Vous pouvez intégrer des [!DNL Workfront] avec [!DNL Basecamp] ou [!DNL Basecamp Classic]. Chaque version de [!DNL Basecamp] utilise une API différente et nécessite donc des procédures de configuration différentes.

Pour plus d’informations sur la configuration [!DNL Basecamp Classic], voir [Intégration [!DNL Workfront Proof] avec [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Activation de la variable [!DNL Basecamp] Intégration avec [!DNL Workfront Proof]

Comme [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) ou [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), vous pouvez configurer la variable [!DNL Basecamp] intégration pour l’ensemble du compte dans votre [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Dans [!UICONTROL Basecamp], collectez les informations suivantes :

   * L’URL de votre [!DNL Basecamp] account
   * L’URL trouvée dans le[!UICONTROL Mes informations]section &quot;

1. Déconnexion de [!DNL Basecamp].
1. Cliquez sur **[!UICONTROL Paramètres du compte]** près du coin supérieur droit.
1. Cliquez sur le bouton **[!UICONTROL Intégrations]** .
1. Dans le **[!UICONTROL [!DNL Basecamp]]** , à droite de **[!UICONTROL [!DNL Basecamp]integration]**, cliquez sur **[!UICONTROL Activer]**.

1. En regard de **[!UICONTROL [!DNL Basecamp]version]**, vérifiez la variable **[!UICONTROL Version classique]** est la version avec laquelle vous effectuez l’intégration.

1. (Conditionnel) Si non [!DNL Basecamp] L’URL s’affiche, cliquez sur **[!UICONTROL Modifier]**, saisissez l’URL de votre [!DNL Basecamp] sans inclure &quot;http://&quot;, puis cliquez sur **[!UICONTROL Enregistrer]**.

1. Dans le coin supérieur droit de la fenêtre, cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres personnels]**.

1. Cliquez sur le bouton **[!UICONTROL Intégrations]** .
1. Sous **[!DNL Basecamp]**, à droite de **[!UICONTROL Intégration de Basecamp]**, cliquez sur **[!UICONTROL Activer]**.

1. Dans les options qui s’affichent, à droite de **[!UICONTROL [!DNL Basecamp]Jeton API]**, cliquez sur **[!UICONTROL Modifier]**.

1. Dans la zone qui s’affiche, saisissez l’URL figurant dans le[!UICONTROL Mes informations]&quot; dans la section [!DNL Basecamp], puis cliquez sur **[!UICONTROL Enregistrer]**.\
   Une fois que vous avez intégré [!DNL Workfront Proof] avec [!DNL Basecamp], vos utilisateurs peuvent configurer leurs paramètres personnels. Pour plus d’informations sur la configuration des paramètres personnels, voir [Configuration des paramètres personnels](#configuring-personal-settings)

1. Si vous ne pouvez pas activer [!DNL Basecamp] intégration, votre [!DNL Workfront Proof] L’identifiant de compte peut ne pas être identique à l’identifiant de compte utilisé dans [!DNL Basecamp].
1. Une fois que vous avez intégré [!DNL Workfront Proof] avec [!DNL Basecamp], vos utilisateurs peuvent configurer leurs paramètres personnels. Pour plus d’informations sur la configuration des paramètres personnels, voir [Configuration des paramètres personnels](#configuring-personal-settings).

## Configuration des paramètres personnels

Après avoir configuré [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) pour votre organisation, chacun de vos auteurs qui crée/envoie des bons à tirer doit définir leur  [paramètres personnels.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Accédez à **[!UICONTROL Paramètres**&#x200B;**personnels]**.

1. Ouvrez le **[!UICONTROL Intégrations]** (1).
1. Pour activer la variable [!DNL Basecamp] intégration, cliquez sur **[!UICONTROL Activer]** (2).
1. Cliquez sur **[!UICONTROL Connectez-vous à votre [!DNL Basecamp] account]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Connectez-vous à [!DNL Basecamp] compte (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Cliquez sur **[!UICONTROL Oui, j’autorise l’accès]** autoriser [!DNL Workfront Proof] accès à votre compte (2).\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Facultatif) Lorsque votre intégration personnelle est principale (3), vous pouvez basculer facilement entre vos [!DNL Basecamp] comptes.

   1. Cliquer **[!UICONTROL Basculer [!DNL Basecamp] account]** (4).\

      ![Basecamp_switch_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      Le [!UICONTROL Basecamp Compte] vous conduit à la fonction [!UICONTROL Paramètres personnels] où vous pouvez choisir laquelle de vos [!DNL Basecamp] comptes que vous souhaitez intégrer à vos [!DNL Workfront Proof] compte .

   1. Cliquez sur **[!UICONTROL Réintégrer avec[!DNL Basecamp]]** (5) avant de choisir la variable [!DNL Basecamp] account\

      Cette opération actualise la variable [!UICONTROL Paramètres personnels] et affiche la liste la plus récente des [!DNL Basecamp] comptes.

   1. Cliquez sur **[!UICONTROL Intégration à ce compte]** pour la connecter à [!DNL Workfront Proof].\

      ![Basecamp_switch_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Vous pouvez maintenant ajouter des bons à tirer à [!DNL Basecamp] projets.
