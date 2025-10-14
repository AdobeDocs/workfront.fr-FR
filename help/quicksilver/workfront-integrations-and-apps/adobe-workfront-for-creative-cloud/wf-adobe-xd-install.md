---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Installer et ouvrir Adobe Workfront pour XD
description: Vous pouvez installer le plug-in Adobe Workfront for XD depuis Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: a5c4479833243bb5817196a3af8acaa063a16747
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 85%

---

# Installer et ouvrir [!DNL Adobe Workfront for XD]

Vous pouvez installer le plug-in [!DNL Adobe Workfront for XD] depuis Adobe Marketplace. Le plug-in prend en charge les langues suivantes :

* Anglais
* Français
* Allemand
* Italien
* Espagnol
* Portugais
* Japonais
* Chinois simplifié
* Chinois traditionnel
* Coréen

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Produit</td> 
   <td><p>Vous devez disposer d’une licence [!DNL Adobe Creative Cloud] en plus d’une licence [!DNL Workfront].</p><p>Pour plus d’informations, voir <a href="https://helpx.adobe.com/fr/support/programs/cc-support-policy.html#cce" class="MCXref xref" xrefformat="{para}">Politique de prise en charge Creative Cloud</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou votre administratrice [!DNL Workfront].

+++

## Conditions préalables

* Vous devez installer l’application [!DNL Adobe XD] avant d’installer le plug-in Workfront.

## Installer le plug-in [!DNL Adobe Workfront for XD] pour votre organisation

Si vous êtes un administrateur ou une administratrice [!DNL Adobe Admin Console], vous pouvez inclure le plug-in dans des packages de déploiement [!DNL Creative Cloud]. Pour plus d’informations, voir [Inclure des plug-ins dans votre package](https://helpx.adobe.com/fr/enterprise/using/manage-extensions.html).

[Regardez un tutoriel vidéo ici](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

Les administrateurs et administratrices [!DNL Adobe Admin Console] peuvent également créer des packages de plug-ins seuls à distribuer aux utilisateurs et utilisatrices. Pour plus d’informations, voir [Créer des packages [!UICONTROL [!DNL Adobe Workfront] for [!DNL Creative Cloud]]  pour vos utilisateurs et utilisatrices dans  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md).

## Installer le plug-in [!DNL Adobe Workfront for XD] individuellement

Vous pouvez installer le plug-in [!DNL Adobe Workfront for XD] pour vous-même depuis [!DNL Adobe Exchange].

1. Accédez à la [page d’installation d’Adobe Workfront for XD](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&workflow=share) sur Adobe Exchange.
1. Dans la boîte de dialogue qui apparaît, cliquez sur **Ouvrir l’application de bureau [!DNL Adobe Creative Cloud]**.
1. Lorsque le gestionnaire des plug-ins [!DNL Adobe XD] est ouvert, cliquez sur **[!UICONTROL Installer]**.
1. Lisez les informations de la boîte de dialogue, puis cliquez sur **[!UICONTROL OK]**.
1. Pour plus d’informations sur l’ouverture du plug-in, reportez-vous à la section suivante.

## Ouvrir le plug-in [!DNL Adobe Workfront for XD]

1. Ouvrez [!DNL Adobe XD].

1. Créez un fichier ou ouvrez un fichier existant.

1. Dans le coin inférieur gauche, cliquez sur l’icône **Plug-ins**.

Fenêtre du plug-in XD ![](assets/xd-plugin-window-350x620.png)

1. Dans le **[!UICONTROL panneau des plug-ins]**, recherchez **[!UICONTROL Adobe Workfront for XD]**.

1. Pour plus d’informations sur la connexion au plug-in, reportez-vous à la section suivante.

## Se connecter à [!DNL Adobe Workfront for XD]

1. Vérifiez que le panneau des plug-ins est ouvert, puis cliquez sur **[!DNL Adobe Workfront for XD]**.
1. Saisissez votre domaine, puis cliquez sur **[!UICONTROL Connexion]**. Une page de navigateur s’ouvre.

   >[!TIP]
   >
   >* Pour trouver votre domaine, ouvrez un navigateur, accédez à votre instance [!DNL Workfront] et copiez la première partie de l’URL :\
   >![Localiser le domaine](assets/domain-350x50.png)
   >
   > * Si votre instance Workfront est intégrée à Experience Cloud, demandez à votre équipe d’administration de vous fournir le domaine Workfront situé sous Produit > Workfront dans l’Admin Console.

1. Dans le navigateur, saisissez vos informations d’identification [!DNL Workfront], puis cliquez sur **[!DNL Log in]**. Si votre entreprise utilise une authentification unique (SSO), vous accédez à la page de votre fournisseur d’authentification unique pour vous connecter.

   >[!NOTE]
   >
   >Vous n’aurez peut-être pas besoin de saisir vos informations d’identification [!DNL Workfront] si votre connexion est récente.

   Suivez les invites pour vous connecter à [!DNL Workfront].

   >[!NOTE]
   >
   >* [!DNL Workfront] se connecte à [!DNL Adobe Creative Cloud] en utilisant OAuth 2.0, une norme sécurisée utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs et utilisatrices.
   >* Lorsqu’on vous invite à saisir [le domaine ou l’hôte] de votre compte [!DNL Workfront], saisissez-le au format suivant : *domainedevotreentreprise.my.workfront.com*. Le domaine de votre entreprise est généralement le nom de votre entreprise.

1. Cliquez sur **[!UICONTROL Autoriser l’accès]** pour terminer la connexion et revenir à [!DNL Adobe XD] pour voir votre travail.

### Résolution des erreurs de connexion

**’erreur « Un problème est survenu » s’affiche lors de la tentative de connexion**


Vous ne pouvez pas utiliser une URL commençant par `experience.adobe.com` pour vous connecter au plug-in.

![erreur de connexion](assets/plugin-log-in-error.png) ![domaine](assets/incorrect-domain.png)


Pour résoudre ce problème, procédez comme suit :

1. Désinstallez et réinstallez le plug-in Adobe Workfront for XD pour effacer le domaine et générer l’erreur.

1. Entrez votre domaine Workfront. Le domaine doit être `company-name.my.workfront.com` et non `experience.adobe.com`.

Pour rechercher votre domaine Workfront si vous utilisez l’expérience unifiée Adobe, accédez à
