---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installer [!DNL Adobe Workfront] pour [!DNL Salesforce]
description: Pour installer l’application avant qu’elle ne soit disponible dans le [!DNL Salesforce] AppExchange, voir Installation [!DNL Workfront] pour Salesforce avant qu’elle ne devienne disponible dans AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# Installer [!DNL Adobe Workfront for Salesforce]

Pour installer l’application avant qu’elle ne soit disponible dans le [!DNL Salesforce AppExchange], voir [Installation [!DNL Workfront for Salesforce] avant qu’elle ne devienne disponible dans la variable [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

Comme [!DNL Salesforce] et [!DNL Adobe Workfront] administrateur, vous pouvez installer [!DNL Workfront for Salesforce] pour autoriser votre [!DNL Salesforce] utilisateurs à envoyer [!DNL Workfront] demande et crée automatiquement des projets sans quitter Salesforce.

Pour une compréhension générale de ce à quoi vous pouvez vous attendre en installant [!DNL Workfront for Salesforce], voir [[!DNL Adobe Workfront for Salesforce] aperçu](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Conditions préalables pour l’installation et l’utilisation [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installation [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables pour l’installation et l’utilisation [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Vous devez disposer d’un [!DNL Salesforce] avec accès à un compte administrateur système pour installer l’application.
* Vous devez disposer d’un [!DNL Workfront] avec accès à un compte administrateur système afin de configurer l’intégration.
* [!UICONTROL Salesforce] Les utilisateurs doivent disposer d’un [!DNL Workfront] afin de pouvoir

   * Créer [!DNL Workfront] de [!DNL Salesforce] ou
   * Affichage [!DNL Workfront] demandes ou projets dans Salesforce.

## Installation [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

Vous devez être un [!DNL Salesforce] et un [!DNL Workfront] administrateur système pour installer et configurer [!DNL Workfront for Salesforce].

Les sous-sections suivantes décrivent comment installer [!DNL Workfront] pour votre [!DNL Salesforce] Environnement de production. Vous pouvez suivre les mêmes étapes pour installer [!DNL Workfront] pour votre [!DNL Salesforce] Environnement Sandbox.

* [Installation [!DNL Workfront for Salesforce] avant qu’elle ne devienne disponible dans la variable [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installation [!DNL Workfront for Salesforce] dans le [!DNL Salesforce Classic] Framework](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installation [!DNL Workfront for Salesforce] dans le [!DNL Salesforce Lightning Experience] Framework](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installation [!DNL Workfront for Salesforce] avant qu’elle ne devienne disponible dans la variable [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] est disponible dans la variable [!DNL Salesforce AppExchange] bientôt.

Pour installer l’application avant qu’elle ne soit disponible :

1. Dans votre environnement de production, accédez à

   `https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY`

   Dans votre environnement Sandbox, accédez à

   `https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY`

1. Vérifiez les **[!UICONTROL Oui, accorder l’accès à ces sites web tiers]** de la boîte.

   Un écran de chargement s’affiche et l’installation peut prendre un certain temps.

1. Cliquez sur **[!UICONTROL Terminé]** une fois l’installation terminée.

1. Accédez à **[!UICONTROL Configuration > Contrôles de sécurité > Paramètres du site distant]**.
1. (Conditionnel) Si vous ne voyez pas votre [!DNL Workfront] URL répertoriée dans le **[!UICONTROL Tous les sites distants]** liste, cliquez sur **[!UICONTROL Nouveau site distant]**.

1. Spécifiez la variable **[!UICONTROL Nom du site distant]**.

   Par exemple, *[!DNL Workfront]*.

1. Spécifiez la variable **[!UICONTROL URL du site distant]**.

   Par exemple : *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Le [!DNL Workfront] L’application est désormais installée sur votre [!DNL Salesforce] et l’instance **[!UICONTROL WorkfrontOpportunities]** et **[!UICONTROL WorkfrontComptes]** [!UICONTROL Visualforce] Des pages ont été créées dans votre environnement.

   [!DNL Salesforce] les utilisateurs peuvent utiliser l’application une fois que vous avez ajouté la variable [!DNL Workfront] à leurs [!UICONTROL Opportunité] ou [!UICONTROL Compte] mises en page.\
   Pour plus d’informations sur la configuration de la section Workfront pour les utilisateurs, voir [Configuration de la section Adobe Workfront pour les utilisateurs Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installation [!DNL Workfront] pour [!DNL Salesforce] dans le [!DNL Salesforce Classic] Framework

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur système.
1. Accédez à **Configuration.**
1. Dans le **Build** , cliquez sur **AppExchange Marketplace**.

1. Dans le **Rechercher des applications d’AppExchange** box, type **Workfront**.

1. Cliquez sur l’application lorsque vous la trouvez, puis cliquez sur **Obtenir maintenant**.
1. Cliquez sur **[!UICONTROL Installation en production]** pour installer le [!DNL Workfront] dans votre application [!DNL Salesforce] Environnement de production. (recommandé)
1. Sélectionnez la **[!UICONTROL J&#39;ai lu et j&#39;accepte les conditions générales]** après avoir lu et accepté les conditions générales.
1. Cliquez sur **[!UICONTROL Confirmation et installation]**.
1. Sélectionner **[!UICONTROL Installation pour tous les utilisateurs]** (recommandé), puis cliquez sur **[!UICONTROL Installer]**.

1. (Conditionnel) Si vous êtes invité à approuver un accès tiers, vous devez sélectionner **[!UICONTROL Oui, accorder l’accès à ces sites web tiers]**, puis cliquez sur **[!UICONTROL Continuer]**.

1. Cliquez sur **[!UICONTROL Terminé]** une fois l’installation terminée.

   Le [!DNL Workfront] L’application est répertoriée sous **[!UICONTROL Packages installés]**.


1. Accédez à **[!UICONTROL Configuration > Contrôles de sécurité > Paramètres du site distant]**.
1. (Conditionnel) Si vous ne voyez pas votre [!DNL Workfront] URL répertoriée dans le **[!UICONTROL Tous les sites distants]** liste, cliquez sur **[!UICONTROL Nouveau site distant]**.\

1. Spécifiez la variable **[!UICONTROL Nom du site distant]**.\
   Par exemple, *[!DNL Workfront]*.

1. Spécifiez la variable **[!UICONTROL URL du site distant]**.\
   Par exemple : *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   Le [!DNL Workfront] L’application est désormais installée sur votre [!DNL Salesforce] et l’instance **[!UICONTROL WorkfrontOpportunities]** et **[!UICONTROL WorkfrontComptes]** [!UICONTROL Visualforce] Des pages ont été créées dans votre environnement.\
   [!DNL Salesforce] Les utilisateurs ne peuvent pas encore utiliser l’application tant que vous n’avez pas ajouté la variable [!DNL Workfront] à leurs [!UICONTROL Opportunité] ou [!UICONTROL Compte] mises en page.\
   Pour plus d’informations sur la configuration de la variable [!DNL Workfront] pour les utilisateurs, voir [Configurez la variable [!DNL Adobe Workfront] section pour [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installation [!DNL Workfront for Salesforce] dans le [!DNL Salesforce Lightning Experience] Framework

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur système.
1. Cliquez sur le bouton **[!UICONTROL Configuration] icon**, puis cliquez sur **[!UICONTROL Configuration]**.

1. Dans le **[!UICONTROL OUTILS PLATFORM]** , développez **[!UICONTROL Applications].**

1. Cliquez sur **[!DNL AppExchange Marketplace]**.
1. Dans le **[!UICONTROL Rechercher [!DNL AppExchange] Applications]** box, type **[!DNL Workfront]**.

1. Cliquez sur l’application lorsque vous la trouvez, puis cliquez sur **[!UICONTROL Obtenir maintenant]**.
1. Cliquez sur **[!UICONTROL Ouvrir l’écran de connexion]**.\
   Vous devez vous connecter avec votre [!DNL Workfront] compte administrateur pour [!DNL Salesforce].

1. Cliquez sur **[!UICONTROL Autoriser]**.
1. Dans le **[!UICONTROL Installation dans cette organisation]** , cliquez sur **[!UICONTROL Installer ici]** pour installer [!DNL Workfront] dans votre [!DNL Salesforce] Environnement de production. (recommandé)

1. Sélectionnez la **[!UICONTROL J&#39;ai lu et j&#39;accepte les conditions générales]** après avoir lu et accepté les conditions générales.
1. Cliquez sur **[!UICONTROL Confirmation et installation]**.
1. Sélectionner **[!UICONTROL Installation pour tous les utilisateurs]** (recommandé), puis cliquez sur **[!UICONTROL Installer]**.

1. (Conditionnel) Si vous êtes invité à approuver un accès tiers, vous devez sélectionner **[!UICONTROL Oui, accorder l’accès à ces sites web tiers]**, puis cliquez sur **[!UICONTROL Continuer]**.

1. Cliquez sur **[!UICONTROL Terminé]** une fois l’installation terminée.

   Le [!DNL Workfront] L’application est répertoriée sous **[!UICONTROL Packages installés]**.

1. Accédez à **[!UICONTROL Configuration].**
1. Dans le **[!UICONTROL PARAMÈTRES]** , développez &#x200B;**[!UICONTROL Sécurité].**

1. Cliquez sur **[!UICONTROL Paramètres du site distant]**.
1. (Conditionnel) Si vous ne voyez pas votre [!DNL Workfront] URL répertoriée dans le **[!UICONTROL Tous les sites distants]** liste, cliquez sur **[!UICONTROL Nouveau site distant]**.

1. Spécifiez la variable **[!UICONTROL Nom du site distant]**.

   Par exemple, *[!DNL Workfront]*.

1. Spécifiez la variable **[!UICONTROL URL du site distant]**.

   Par exemple : *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Le [!DNL Workfront] L’application est désormais installée sur votre [!DNL Salesforce] et la variable **[!DNL Workfront]** est maintenant ajouté à votre environnement.

   [!UICONTROL Salesforce] Les utilisateurs peuvent utiliser la variable [!DNL Workfront] une fois que vous avez ajouté l’application [!DNL Workfront] à leurs [!UICONTROL Opportunité] ou [!UICONTROL Compte] mises en page.\
   Pour plus d’informations sur la configuration de la variable [!DNL Workfront] pour les utilisateurs, voir [Configurez la variable [!DNL Adobe Workfront] section pour [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
