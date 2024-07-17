---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installer [!DNL Adobe Workfront] pour [!DNL Salesforce]
description: Pour installer l’application avant qu’elle ne soit disponible dans l’AppExchange  [!DNL Salesforce] , voir Installation de  [!DNL Workfront]  pour Salesforce avant qu’elle ne devienne disponible dans AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: c0e7340e2bf650b6f9931ae12aee07c5f7d5292b
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 3%

---

# Installer [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>Pour installer l’application avant qu’elle ne soit disponible dans le [!DNL Salesforce AppExchange], voir [Installation [!DNL Workfront for Salesforce] avant qu’elle ne devienne disponible dans le  [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

En tant qu&#39;administrateur [!DNL Salesforce] et [!DNL Adobe Workfront], vous pouvez installer [!DNL Workfront for Salesforce] pour permettre à vos utilisateurs [!DNL Salesforce] d&#39;envoyer des requêtes [!DNL Workfront] et de créer automatiquement des projets sans jamais quitter Salesforce.

Pour une compréhension générale de ce que vous pouvez attendre en installant [!DNL Workfront for Salesforce], voir [[!DNL Adobe Workfront for Salesforce] overview](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Conditions préalables pour l’installation et l’utilisation de [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installation de [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables pour l’installation et l’utilisation de [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Pour installer l’application, vous devez disposer d’une instance [!DNL Salesforce] ayant accès à un compte administrateur système.
* Pour configurer l’intégration, vous devez disposer d’une instance [!DNL Workfront] ayant accès à un compte administrateur système.
* Les utilisateurs de [!UICONTROL Salesforce] doivent avoir un compte [!DNL Workfront] pour pouvoir :

   * Créer [!DNL Workfront] requêtes de [!DNL Salesforce]
   * Affichage de [!DNL Workfront] requêtes ou projets dans Salesforce

## Installation de [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

Vous devez être un administrateur système [!DNL Salesforce] et [!DNL Workfront] pour installer et configurer [!DNL Workfront for Salesforce].

Les sous-sections suivantes décrivent comment installer [!DNL Workfront] pour votre environnement de production [!DNL Salesforce]. Vous pouvez suivre les mêmes étapes pour installer [!DNL Workfront] pour votre environnement [!DNL Salesforce] Sandbox.

* [Installation de  [!DNL Workfront for Salesforce] avant qu’il ne devienne disponible sur  [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installation de  [!DNL Workfront for Salesforce]  dans le  [!DNL Salesforce Classic] Framework](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installation de  [!DNL Workfront for Salesforce]  dans le  [!DNL Salesforce Lightning Experience] Framework](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installation de [!DNL Workfront for Salesforce] avant qu’il ne devienne disponible sur le [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] sera bientôt disponible dans le [!DNL Salesforce AppExchange].

Pour installer l’application avant qu’elle ne soit disponible :

1. Dans votre environnement de production, accédez à

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   Dans votre environnement Sandbox, accédez à

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >Vous devez être connecté à Salesforce pour accéder à ces pages.

1. Cochez la case **[!UICONTROL Oui, accorder l’accès à ces sites web tiers]** .

   Un écran de chargement s’affiche. L’installation peut prendre du temps.

1. Cliquez sur **[!UICONTROL Terminé]** une fois l’installation terminée.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Contrôles de sécurité]** > **[!UICONTROL Paramètres du site distant]**.
1. (Conditionnel) Sélectionnez Workfront dans la liste.

   Ou

   Si votre URL [!DNL Workfront] n’est pas répertoriée dans la liste **[!UICONTROL Tous les sites distants]**, cliquez sur **[!UICONTROL Nouveau site distant]**.

1. (Conditionnel) Si vous ajoutez le site, spécifiez le **[!UICONTROL nom du site distant]**.

   Par exemple, *[!DNL Workfront]*.

1. (Conditionnel) Si vous ajoutez le site, spécifiez l’ **[!UICONTROL URL du site distant]**.

   Par exemple, *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   L’application [!DNL Workfront] est maintenant installée sur votre instance [!DNL Salesforce] et les **[!UICONTROL WorkfrontOpportunities]** et **[!UICONTROL WorkfrontAccount]** [!UICONTROL Visualforce] Les pages ont été créées dans votre environnement.

   Les utilisateurs de [!DNL Salesforce] peuvent utiliser l’application une fois que vous avez ajouté la section [!DNL Workfront] à leurs mises en page [!UICONTROL Opportunité] ou [!UICONTROL Compte].\
   Pour plus d’informations sur la configuration de la section Workfront pour les utilisateurs, voir [Configuration de la section Adobe Workfront pour les utilisateurs Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installation de [!DNL Workfront] pour [!DNL Salesforce] dans la structure [!DNL Salesforce Classic]

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur système.
1. Accédez à **Configuration.**
1. Dans la section **Build** , cliquez sur **AppExchange Marketplace**.

1. Dans la zone **Rechercher dans les applications d&#39;AppExchange**, saisissez **Workfront**.

1. Cliquez sur l’application Workfront lorsque vous la trouvez, puis cliquez sur **Obtenir maintenant**.
1. Cliquez sur **[!UICONTROL Installer en production]** pour installer l’application [!DNL Workfront] dans votre environnement de production [!DNL Salesforce]. (recommandé).
1. Après avoir lu et accepté les conditions générales, activez le champ **[!UICONTROL J’ai lu et accepté les conditions générales]** .
1. Cliquez sur **[!UICONTROL Confirmer et installer]**.
1. Sélectionnez **[!UICONTROL Installer pour tous les utilisateurs]** (recommandé), puis cliquez sur **[!UICONTROL Installer]**.

1. (Conditionnel) Si vous devez approuver un accès tiers, vous devez sélectionner **[!UICONTROL Oui, accorder l’accès à ces sites Web tiers]**, puis cliquer sur **[!UICONTROL Continuer]**.

1. Cliquez sur **[!UICONTROL Terminé]** une fois l’installation terminée.

   L’application [!DNL Workfront] est répertoriée sous **[!UICONTROL Packages installés]**.


1. Accédez à **[!UICONTROL Configuration>Contrôles de sécurité>Paramètres du site distant]**.
1. (Conditionnel) Si votre URL [!DNL Workfront] ne figure pas dans la liste **[!UICONTROL Tous les sites distants]**, cliquez sur **[!UICONTROL Nouveau site distant]**.

1. (Conditionnel) Si vous ajoutez le site, spécifiez le **[!UICONTROL nom du site distant]**.
Par exemple, *[!DNL Workfront]*.

1. (Conditionnel) Si vous ajoutez le site, spécifiez l’ **[!UICONTROL URL du site distant]**.
Par exemple, *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   L’application [!DNL Workfront] est désormais installée sur votre instance [!DNL Salesforce]. Les pages **[!UICONTROL WorkfrontOpportunities]** et **** [!UICONTROL Visualforce] ont été créées dans votre environnement.\
   Les utilisateurs de [!DNL Salesforce] ne peuvent pas encore utiliser l’application tant que vous n’avez pas ajouté la section [!DNL Workfront] à leurs mises en page [!UICONTROL Opportunité] ou [!UICONTROL Compte].\
   Pour plus d&#39;informations sur la configuration de la section [!DNL Workfront] pour les utilisateurs, voir [Configuration de la section  [!DNL Adobe Workfront] pour les  [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installation de [!DNL Workfront for Salesforce] dans la structure [!DNL Salesforce Lightning Experience]

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur système.
1. Cliquez sur l&#39;icône **[!UICONTROL Setup]**, puis sur **[!UICONTROL Setup]**.

1. Dans la section **[!UICONTROL OUTILS PLATFORM]**, développez **[!UICONTROL Applications].**

1. Cliquez sur **[!DNL AppExchange Marketplace]**.
1. Dans la zone **[!UICONTROL Search [!DNL AppExchange] Apps]** , saisissez **[!DNL Workfront]**.

1. Cliquez sur l’application Workfront lorsque vous la trouvez, puis cliquez sur **Obtenir maintenant**.
1. Cliquez sur **[!UICONTROL Ouvrir l’écran de connexion]**.\
   Vous devez vous connecter avec votre compte administrateur [!DNL Workfront] pour [!DNL Salesforce].

1. Cliquez sur **[!UICONTROL Autoriser]**.
1. Dans la zone **[!UICONTROL Installer dans cette organisation]**, cliquez sur **[!UICONTROL Installer ici]** pour installer [!DNL Workfront] dans votre environnement de production [!DNL Salesforce]. (recommandé).

1. Après avoir lu et accepté les conditions générales, activez le champ **[!UICONTROL J’ai lu et accepté les conditions générales]** .
1. Cliquez sur **[!UICONTROL Confirmer et installer]**.
1. Sélectionnez **[!UICONTROL Installer pour tous les utilisateurs]** (recommandé), puis cliquez sur **[!UICONTROL Installer]**.

1. (Conditionnel) Si vous devez approuver un accès tiers, vous devez sélectionner **[!UICONTROL Oui, accorder l’accès à ces sites Web tiers]**, puis cliquer sur **[!UICONTROL Continuer]**.

1. Cliquez sur **[!UICONTROL Terminé]** une fois l’installation terminée.

   L’application [!DNL Workfront] est répertoriée sous **[!UICONTROL Packages installés]**.

1. Accédez à **[!UICONTROL Setup].**
1. Dans la section **[!UICONTROL SETTINGS]**, développez **[!UICONTROL Security].**

1. Cliquez sur **[!UICONTROL Paramètres du site distant]**.
1. (Conditionnel) Si votre URL [!DNL Workfront] ne figure pas dans la liste **[!UICONTROL Tous les sites distants]**, cliquez sur **[!UICONTROL Nouveau site distant]**.

1. (Conditionnel) Si vous ajoutez le site, spécifiez le **[!UICONTROL nom du site distant]**.
Par exemple, *[!DNL Workfront]*.

1. (Conditionnel) Si vous ajoutez le site, spécifiez l’ **[!UICONTROL URL du site distant]**.
Par exemple, *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   L’application [!DNL Workfront] est maintenant installée sur votre instance [!DNL Salesforce] et le composant **[!DNL Workfront]** est maintenant ajouté à votre environnement.

   Les utilisateurs de [!UICONTROL Salesforce] peuvent utiliser l’application [!DNL Workfront] une fois que vous avez ajouté la section [!DNL Workfront] à leurs mises en page [!UICONTROL Opportunity] ou [!UICONTROL Account].\
   Pour plus d&#39;informations sur la configuration de la section [!DNL Workfront] pour les utilisateurs, voir [Configuration de la section  [!DNL Adobe Workfront] pour les  [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
