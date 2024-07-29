---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Installer et ouvrir Adobe Workfront pour XD
description: Vous pouvez installer le module externe Adobe Workfront for XD depuis Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: 4256e1ecd16179d0a2aa8e623b05be754d8bbd2d
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 9%

---

# Installer et ouvrir [!DNL Adobe Workfront for XD]

Vous pouvez installer le module externe [!DNL Adobe Workfront for XD] à partir d’Adobe Marketplace. Le module externe prend en charge les langues suivantes :

* Anglais
* Français
* Allemand
* Italien
* Espagnol
* Portuge
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
   <td><p>Vous devez disposer d’une licence [!DNL Adobe Creative Cloud] en plus d’une licence [!DNL Workfront].</p><p>Pour plus d’informations, voir la <a href="https://helpx.adobe.com/support/programs/cc-support-policy.html#cce" class="MCXref xref" xrefformat="{para}">Stratégie de prise en charge des Creative Cloud</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

+++

## Conditions préalables

* Vous devez installer l’application [!DNL Adobe XD] avant d’installer le module externe Workfront.

## Installation du module externe [!DNL Adobe Workfront for XD] pour votre organisation

Si vous êtes administrateur [!DNL Adobe Admin Console], vous pouvez inclure le module externe dans les modules de déploiement [!DNL Creative Cloud]. Pour plus d’informations, voir [Inclusion de modules externes dans votre package](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[Affichez un tutoriel vidéo ici](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

Les administrateurs [!DNL Adobe Admin Console] peuvent également créer des modules externes uniquement pour distribution aux utilisateurs. Pour plus d’informations, voir [Création de packages [!UICONTROL [!DNL Adobe Workfront] pour [!DNL Creative Cloud]] pour vos utilisateurs dans le [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Installez le module externe [!DNL Adobe Workfront for XD] individuellement

Vous pouvez installer le module externe [!DNL Adobe Workfront for XD] à partir de [!DNL Adobe Exchange].

1. Accédez à la [page d’installation d’Adobe Workfront pour XD](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&amp;workflow=share) sur l’Adobe Exchange.
1. Dans la boîte de dialogue qui s’affiche, cliquez sur **Ouvrir l’appli de bureau [!DNL Adobe Creative Cloud]**.
1. Une fois le gestionnaire de modules externes [!DNL Adobe XD] ouvert, cliquez sur **[!UICONTROL Installer]**.
1. Lisez les informations dans la boîte de dialogue, puis cliquez sur **[!UICONTROL OK]**.
1. Pour plus d’informations sur l’ouverture du module externe, reportez-vous à la section suivante.

## Ouvrez le module externe [!DNL Adobe Workfront for XD]

1. Ouvrez [!DNL Adobe XD].

1. Créez un fichier ou ouvrez un fichier existant.

1. Dans le coin inférieur gauche, cliquez sur l’icône **Plugins** .

![](assets/xd-plugin-window-350x620.png)

1. Dans le **[!UICONTROL panneau Plugins]**, recherchez **[!UICONTROL Adobe Workfront for XD]**.

1. Pour plus d’informations sur la connexion au module externe, reportez-vous à la section suivante.

## Connectez-vous à [!DNL Adobe Workfront for XD]

1. Assurez-vous que le panneau du module externe est ouvert, puis cliquez sur **[!DNL Adobe Workfront for XD]**.
1. Entrez votre domaine, puis cliquez sur **[!UICONTROL Se connecter]**. Une page de navigateur s’ouvre.

   >[!TIP]
   >
   >* Pour trouver votre domaine, ouvrez un navigateur, accédez à votre instance [!DNL Workfront] et copiez la première partie de l’URL :\
   >![](assets/domain-350x50.png)
   >
   > * Si votre instance Workfront est intégrée à Experience Cloud, demandez à votre administrateur de vous fournir le domaine Workfront situé sous Produit > Workfront dans l’Admin Console.

1. Dans le navigateur, saisissez vos informations d’identification [!DNL Workfront], puis cliquez sur **[!DNL Log in]**. Si votre entreprise utilise une authentification unique (SSO), vous serez dirigé vers la page de votre fournisseur d’authentification unique pour vous connecter.

   >[!NOTE]
   >
   >Si vous vous êtes connecté récemment, il se peut que vous ne soyez pas invité à saisir vos informations d’identification [!DNL Workfront].

   Suivez les invites pour vous connecter à [!DNL Workfront].

   >[!NOTE]
   >
   >* [!DNL Workfront] se connecte à [!DNL Adobe Creative Cloud] à l’aide d’OAuth 2.0, une norme sécurisée utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs.
   >* Lorsque vous êtes invité à saisir le [domaine ou hôte] de votre compte [!DNL Workfront], saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre société correspond généralement au nom de votre société.

1. Cliquez sur **[!UICONTROL Autoriser l’accès]** pour terminer la connexion, puis revenez à [!DNL Adobe XD] pour voir votre travail.

 
