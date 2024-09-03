---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installer  [!DNL Adobe Workfront]  pour  [!DNL Salesforce]
description: Pour installer l’application avant qu’elle ne soit disponible sur AppExchange  [!DNL Salesforce] , voir Installer  [!DNL Workfront]  pour Salesforce avant qu’elle ne soit disponible sur AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: b088c305cbd16aea1b6b79a9f3a9c5ac326cd0b8
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 92%

---

# Installer [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>Pour installer l’application avant qu’elle ne soit disponible sur [!DNL Salesforce AppExchange], voir [Installer  [!DNL Workfront for Salesforce]  avant qu’elle ne soit disponible sur  [!DNL AppExchange]  Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

En tant qu’administrateur ou administratrice [!DNL Salesforce] et [!DNL Adobe Workfront], vous pouvez installer [!DNL Workfront for Salesforce] pour permettre à vos utilisateurs et utilisatrices [!DNL Salesforce] de soumettre des demandes [!DNL Workfront] et de créer automatiquement des projets sans jamais quitter Salesforce.

Pour une compréhension générale de ce que vous pouvez attendre de l’installation de [!DNL Workfront for Salesforce], voir Vue d’ensemble de [[!DNL Adobe Workfront for Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Conditions préalables à l’installation et à l’utilisation de  [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installer  [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des accès suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables à l’installation et à l’utilisation de [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Vous devez disposer d’une instance [!DNL Salesforce] avec accès à un compte d’administrateur ou d’administratrice système afin d’installer l’application.
* Vous devez disposer d’une instance [!DNL Workfront] avec accès à un compte d’administrateur ou d’administratrice système afin de configurer l’intégration.
* Les utilisateurs et utilisatrices de [!UICONTROL Salesforce] doivent disposer d’un compte [!DNL Workfront] afin de pouvoir :

   * Créer des demandes [!DNL Workfront] à partir de [!DNL Salesforce].
   * Voir les demandes ou les projets [!DNL Workfront] dans Salesforce.

## Installer [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

Vous devez être un administrateur ou une administratrice système [!DNL Salesforce] et [!DNL Workfront] pour installer et configurer [!DNL Workfront for Salesforce].

Les sous-sections suivantes décrivent comment installer [!DNL Workfront] pour votre environnement de production [!DNL Salesforce]. Vous pouvez suivre les mêmes étapes pour installer [!DNL Workfront] dans votre environnement Sandbox [!DNL Salesforce].

* [Installer  [!DNL Workfront for Salesforce]  avant qu’il ne soit disponible sur  [!DNL AppExchange]  Marketplace.](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installer  [!DNL Workfront for Salesforce]  dans le cadre  [!DNL Salesforce Classic] ](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installer  [!DNL Workfront for Salesforce]  dans le cadre  [!DNL Salesforce Lightning Experience] ](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installer [!DNL Workfront for Salesforce] avant qu’il ne soit disponible sur [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] sera bientôt disponible sur [!DNL Salesforce AppExchange].

Pour installer l’application avant qu’elle ne soit disponible :

1. Dans votre environnement de production, accédez à

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   Dans votre environnement Sandbox, accédez à

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >Vous devez vous connecter à Salesforce pour accéder à ces pages.

1. Cochez la case **[!UICONTROL Oui, autoriser l’accès à ces sites web tiers]**.

   Un écran de chargement s’affiche. L’installation peut prendre un certain temps.

1. Cliquez sur **[!UICONTROL Terminé]** lorsque l’installation est terminée.

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Sécurité] Contrôles** > **[!UICONTROL Paramètres des sites distants]**.
1. (Le cas échéant) Sélectionnez Workfront dans la liste.

   Ou

   Si votre URL [!DNL Workfront] ne figure pas dans la liste **[!UICONTROL Tous les sites distants]**, cliquez sur **[!UICONTROL Nouveau site distant]**.

1. (Le cas échéant) Si vous ajoutez le site, indiquez le **[!UICONTROL nom du site distant]**.

   Par exemple, *[!DNL Workfront]*.

1. (Le cas échéant) Si vous ajoutez le site, indiquez l’**[!UICONTROL URL du site distant]**.

   Par exemple, *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   L’application [!DNL Workfront] est maintenant installée sur votre instance [!DNL Salesforce] et les pages **[!UICONTROL WorkfrontOpportunities]** et **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] ont été créées dans votre environnement.

   Les utilisateurs et utilisatrices de [!DNL Salesforce] peuvent utiliser l’application une fois que vous avez ajouté la section [!DNL Workfront] à leur disposition des pages [!UICONTROL Opportunité] ou [!UICONTROL Compte].\
   Pour plus d’informations sur la configuration de la section Workfront pour les personnes, voir [Configurer la section Adobe Workfront pour les utilisateurs et utilisatrices de Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installer [!DNL Workfront] pour [!DNL Salesforce] dans le framework [!DNL Salesforce Classic] 

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur ou administratrice système.
1. Accédez à **Configuration**.
1. Dans la section **Créer**, cliquez sur **AppExchange Marketplace**.

1. Dans la zone **Rechercher des apps AppExchange**, saisissez **Workfront**.

1. Cliquez sur l’application Workfront lorsque vous la trouvez, puis cliquez sur **Obtenir maintenant**.
1. Cliquez sur **[!UICONTROL Installer en production]** pour installer l’application [!DNL Workfront] dans votre environnement de production [!DNL Salesforce]. (Recommandé)
1. Après avoir lu et accepté les conditions générales, activez le champ **[!UICONTROL J’ai lu et j’accepte les conditions générales]**.
1. Cliquez sur **[!UICONTROL Confirmer et installer]**.
1. Sélectionnez **[!UICONTROL Installer pour toutes les personnes]** (recommandé), puis cliquez sur **[!UICONTROL Installer]**.

1. (Le cas échéant) Si l’on vous demande si vous voulez approuver l’accès d’une tierce partie, vous devez sélectionner **[!UICONTROL Oui, accorder l’accès à ces sites web tiers]**, puis cliquer sur **[!UICONTROL Continuer]**.

1. Cliquez sur **[!UICONTROL Terminé]** lorsque l’installation est terminée.

   L’application [!DNL Workfront] est répertoriée sous **[!UICONTROL Packages installés]**.


1. Accédez à **[!UICONTROL Configuration > Contrôle de sécurités > Paramètres de site distant]**.
1. (Le cas échéant) Si votre URL [!DNL Workfront] ne figure pas dans la liste **[!UICONTROL Tous les sites distants]**, cliquez sur **[!UICONTROL Nouveau site distant]**.

1. (Le cas échéant) Si vous ajoutez le site, spécifiez le **[!UICONTROL nom du site distant]**.
Par exemple, *[!DNL Workfront]*.

1. (Le cas échéant) Si vous ajoutez le site, indiquez l’**[!UICONTROL URL du site distant]**.
Par exemple, *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.\
   L’application [!DNL Workfront] est maintenant installée sur votre instance [!DNL Salesforce]. Les pages **[!UICONTROL WorkfrontOpportunities]** et **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] ont été créées dans votre environnement.\
   Les utilisateurs et utilisatrices de [!DNL Salesforce] ne peuvent pas encore utiliser l’application tant que vous n’avez pas ajouté la section [!DNL Workfront] à leurs mises en page des pages [!UICONTROL Opportunité] ou [!UICONTROL Compte].\
   Pour plus d’informations sur la configuration de la section [!DNL Workfront] pour les personnes, voir [Configurer la section  [!DNL Adobe Workfront]  pour les utilisateurs et utilisatrices de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installer [!DNL Workfront for Salesforce] dans le framework [!DNL Salesforce Lightning Experience]

1. Connectez-vous à [!DNL Salesforce] en tant qu’administrateur ou administratrice système.
1. Cliquez sur l’icône **[!UICONTROL Configuration]**, puis cliquez sur **[!UICONTROL Configuration]**.

1. Dans la section **[!UICONTROL OUTILS DE PLATEFORME]**, développez **[!UICONTROL Apps].**

1. Cliquez sur **[!DNL AppExchange Marketplace]**.
1. Dans la zone **[!UICONTROL Rechercher des applications[!DNL AppExchange]]**, saisissez **[!DNL Workfront]**.

1. Cliquez sur l’application Workfront lorsque vous la trouvez, puis cliquez sur **Obtenir maintenant**.
1. Cliquez sur **[!UICONTROL Ouvrir l’écran de connexion]**.\
   Vous devez vous connecter avec votre compte administrateur ou administratrice [!DNL Workfront] pour [!DNL Salesforce].

1. Cliquez sur **[!UICONTROL Autoriser]**.
1. Dans la zone **[!UICONTROL Installer dans cette organisation]**, cliquez sur **[!UICONTROL Installer ici]** pour installer [!DNL Workfront] dans votre environnement de production [!DNL Salesforce]. (Recommandé)

1. Après avoir lu et accepté les conditions générales, activez le champ **[!UICONTROL J’ai lu et j’accepte les conditions générales]**.
1. Cliquez sur **[!UICONTROL Confirmer et installer]**.
1. Sélectionnez **[!UICONTROL Installer pour toutes les personnes]** (recommandé), puis cliquez sur **[!UICONTROL Installer]**.

1. (Le cas échéant) Si l’on vous demande si vous voulez approuver l’accès d’une tierce partie, vous devez sélectionner **[!UICONTROL Oui, accorder l’accès à ces sites web tiers]**, puis cliquer sur **[!UICONTROL Continuer]**.

1. Cliquez sur **[!UICONTROL Terminé]** lorsque l’installation est terminée.

   L’application [!DNL Workfront] est répertoriée sous **[!UICONTROL Packages installés]**.

1. Accédez à **[!UICONTROL Configuration].**
1. Dans la section **[!UICONTROL Paramètres]**, développez **[!UICONTROL Sécurité].**

1. Cliquez sur **[!UICONTROL Paramètres du site distant]**.
1. (Le cas échéant) Si votre URL [!DNL Workfront] ne figure pas dans la liste **[!UICONTROL Tous les sites distants]**, cliquez sur **[!UICONTROL Nouveau site distant]**.

1. (Le cas échéant) Si vous ajoutez le site, spécifiez le **[!UICONTROL nom du site distant]**.
Par exemple, *[!DNL Workfront]*.

1. (Le cas échéant) Si vous ajoutez le site, indiquez l’**[!UICONTROL URL du site distant]**.
Par exemple, *yourDomain.my.workfront.com*.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   L’application [!DNL Workfront] est désormais installée sur votre instance [!DNL Salesforce], et le composant **[!DNL Workfront]** est désormais ajouté à votre environnement.

   Les utilisateurs et utilisatrices de [!UICONTROL Salesforce] peuvent utiliser l’application [!DNL Workfront] une fois que vous avez ajouté la section [!DNL Workfront] à leurs dispositions de page [!UICONTROL Opportunité] ou [!UICONTROL Compte].\
   Pour plus d’informations sur la configuration de la section [!DNL Workfront] pour les utilisateurs et utilisatrices, voir [Configurer la section [!DNL Adobe Workfront] pour les utilisateurs et utilisatrices [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Configuration des autorisations pour l’intégration Workfront for Salesforce

### Autorisations pour `workfront_business`

1. Accédez à **Configuration** > **Sécurité** > **URL de confiance**.
1. Sélectionnez `workfront_business` dans la liste.
1. Cliquez sur **Modifier**.
1. Sous Directives CSP , vérifiez les options suivantes :

   * connect-src (scripts)
   * font-src (fonts)
   * frame-src (contenu iframe)
   * img-src (images)
   * media-src (audio et vidéo)
   * style-src (feuilles de style)

1. Cliquer sur **Enregistrer**.


### Autorisations pour workfront_session

1. Accédez à **Configuration** > **Sécurité** > **URL de confiance**.
1. Sélectionnez `workfront_session` dans la liste.
1. Cliquez sur **Modifier**.
1. Sous Directives CSP , vérifiez les options suivantes :

   * connect-src (scripts)
   * font-src (fonts)
   * frame-src (contenu iframe)
   * img-src (images)
   * media-src (audio et vidéo)
   * style-src (feuilles de style)

1. Cliquer sur **Enregistrer**.

