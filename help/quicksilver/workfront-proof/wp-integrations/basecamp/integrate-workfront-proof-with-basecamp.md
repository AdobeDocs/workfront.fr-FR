---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Intégrer [!DNL Workfront Proof] avec [!DNL Basecamp]
description: Si vous utilisez  [!DNL Basecamp] pour la gestion de projet, vous pouvez offrir à votre équipe de projet des outils de révision et d'approbation plus riches en utilisant [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Intégrer [!DNL Workfront Proof] avec [!DNL Basecamp]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Si vous utilisez [!DNL Basecamp] pour la gestion de projet, vous pouvez offrir à votre équipe de projet des outils de révision et d&#39;approbation plus riches en utilisant [!DNL Workfront Proof].

## Présentation de l’intégration [!DNL Basecamp] avec [!DNL Workfront]

L’intégration à [!DNL Basecamp] permet aux utilisateurs d’afficher, de réviser et d’approuver les bons à tirer tous dans [!DNL Basecamp]. Les utilisateurs peuvent envoyer des bons à tirer à votre compte [!DNL Workfront Proof] et les connecter à votre projet [!DNL Basecamp]. Vos réviseurs peuvent commenter et prendre des décisions via [!DNL Basecamp], en utilisant le mini-BAT incorporé dans votre message Basecamp.

Lorsqu&#39;il est intégré à [!DNL Workfront Proof], [!DNL Basecamp] dispose de la fonctionnalité de vérification de l&#39;intégrité suivante :

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

* Configurez [!DNL Basecamp] dans [Paramètres du compte :](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Cela permet l’intégration Basecamp pour l’ensemble de votre organisation. Pour plus d’informations, voir [Activation de l’intégration Basecamp avec [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Configurez [!DNL Basecamp] dans [Paramètres personnels](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) : cela permet aux créateurs et aux propriétaires de BAT de se connecter à leur compte Basecamp personnel et d&#39;autoriser l&#39;accès à [!DNL Workfront Proof]. Pour plus d’informations, voir [Configuration des paramètres personnels](#configuring-personal-settings).

Vous pouvez intégrer [!DNL Workfront] à [!DNL Basecamp] ou [!DNL Basecamp Classic]. Chaque version de [!DNL Basecamp] utilise une API différente et nécessite donc des procédures de configuration différentes.

Pour plus d&#39;informations sur la configuration de [!DNL Basecamp Classic], voir [Intégration [!DNL Workfront Proof] avec [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Activation de l’intégration [!DNL Basecamp] avec [!DNL Workfront Proof]

En tant que [ {Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) ou [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), vous pouvez configurer l’intégration [!DNL Basecamp] de l’ensemble du compte dans les [paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Dans [!UICONTROL Basecamp], collectez les informations suivantes :

   * URL de votre compte [!DNL Basecamp]
   * URL trouvée dans la section &quot;[!UICONTROL My info]&quot;

1. Déconnectez-vous de [!DNL Basecamp].
1. Cliquez sur **[!UICONTROL Paramètres du compte]** près du coin supérieur droit.
1. Cliquez sur l’onglet **[!UICONTROL Intégrations]** .
1. Dans la section **[!UICONTROL [!DNL Basecamp]]**, à droite de l&#39;intégration **[!UICONTROL [!DNL Basecamp]]**, cliquez sur **[!UICONTROL Activer]**.

1. En regard de **[!UICONTROL [!DNL Basecamp]version]**, vérifiez que la **[!UICONTROL version classique]** est la version que vous intégrez.

1. (Conditionnel) Si aucune URL [!DNL Basecamp] ne s’affiche, cliquez sur **[!UICONTROL Modifier]**, saisissez l’URL de votre compte [!DNL Basecamp], sans inclure &quot;http://&quot;, puis cliquez sur **[!UICONTROL Enregistrer]**.

1. Dans le coin supérieur droit de la fenêtre, cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres personnels]**.

1. Cliquez sur l’onglet **[!UICONTROL Intégrations]** .
1. Sous **[!DNL Basecamp]**, à droite de **[!UICONTROL Basecamp integration]**, cliquez sur **[!UICONTROL Activer]**.

1. Dans les options qui s’affichent, à droite de **[!UICONTROL [!DNL Basecamp]API Token]**, cliquez sur **[!UICONTROL Modifier]**.

1. Dans la zone qui s’affiche, saisissez l’URL trouvée dans la section &quot;[!UICONTROL My info]&quot; dans [!DNL Basecamp], puis cliquez sur **[!UICONTROL Save]**.\
   Une fois que vous avez intégré [!DNL Workfront Proof] à [!DNL Basecamp], vos utilisateurs peuvent configurer leurs paramètres personnels. Pour plus d’informations sur la configuration des paramètres personnels, voir [Configuration des paramètres personnels](#configuring-personal-settings)

1. Si vous ne pouvez pas activer l&#39;intégration [!DNL Basecamp], votre ID de compte [!DNL Workfront Proof] peut ne pas être identique à l&#39;ID de compte que vous utilisez dans [!DNL Basecamp].
1. Une fois que vous avez intégré [!DNL Workfront Proof] à [!DNL Basecamp], vos utilisateurs peuvent configurer leurs paramètres personnels. Pour plus d’informations sur la configuration des paramètres personnels, voir [Configuration des paramètres personnels](#configuring-personal-settings).

## Configuration des paramètres personnels

Une fois que vous avez configuré les [ paramètres du compte ](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) pour votre organisation, chacun de vos auteurs qui crée/envoie des bons à tirer doit définir ses [ paramètres personnels.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Accédez à **[!UICONTROL Personal** **settings]**.

1. Ouvrez l’onglet **[!UICONTROL Intégrations]** (1).
1. Pour activer l’intégration [!DNL Basecamp], cliquez sur **[!UICONTROL Activer]** (2).
1. Cliquez sur **[!UICONTROL Se connecter à votre compte [!DNL Basecamp]]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Connectez-vous à votre compte [!DNL Basecamp] (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Cliquez sur **[!UICONTROL Oui, j&#39;autorise l&#39;accès]** pour autoriser l&#39;accès [!DNL Workfront Proof] à votre compte (2).\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Facultatif) Lorsque votre intégration personnelle est active (3), vous pouvez facilement basculer entre vos comptes [!DNL Basecamp].

   1. Cliquez sur **[!UICONTROL Changer de compte [!DNL Basecamp]]** (4).\

      ![ Basecamp_switch_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      Le [!UICONTROL  compte de basculement de base] vous conduit à la page [!UICONTROL  paramètres personnels ], sur laquelle vous pouvez choisir les comptes [!DNL Basecamp] que vous souhaitez intégrer à votre compte [!DNL Workfront Proof].

   1. Cliquez sur **[!UICONTROL Réintégrer à[!DNL Basecamp]]** (5) avant de choisir le compte [!DNL Basecamp]\

      Cette opération actualise la page [!UICONTROL Paramètres personnels] et affiche la liste de vos comptes [!DNL Basecamp] les plus récents.

   1. Cliquez sur **[!UICONTROL Intégrer à ce compte]** pour le connecter à [!DNL Workfront Proof].\

      ![Basecamp_switch_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Vous pouvez désormais ajouter des bons à tirer aux projets [!DNL Basecamp].
