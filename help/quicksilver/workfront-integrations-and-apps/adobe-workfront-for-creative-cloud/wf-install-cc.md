---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Installation et ouverture [!DNL Adobe Workfront for design and video]
description: Vous pouvez installer le module externe Workfront for Creative Cloud à partir d’Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: f4fbae93-b54b-4d08-82c3-72a9a760c317
source-git-commit: 9baddd29b84c3b5d77f8b2e708be53d4150e6e92
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 1%

---

# Installation et ouverture [!DNL Adobe Workfront for design and video]

Vous pouvez installer le [!DNL Adobe Workfront for design and video] du module externe [!DNL Adobe Marketplace]. Ce module externe prend en charge les applications de Creative Cloud suivantes :

{{cc-plugin-app-list}}

Le module externe prend en charge les langues suivantes :

* Anglais
* Français
* Allemand
* Italien
* Espagnol
* Japonais
* Portugais
* Chinois simplifié
* Chinois traditionnel
* Coréen

>[!NOTE]
>
>Il existe des instructions d’installation distinctes pour [!DNL Photoshop] et [!DNL XD]. Pour plus d’informations, voir [Installer [!DNL Adobe Workfront for Photoshop]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) et [Installer [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).


## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td>Vous devez disposer d’un [!DNL Adobe Creative Cloud] en plus d’une [!DNL Workfront] licence.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

* Vous devez installer le [!DNL Creative Cloud] de l’application que vous souhaitez utiliser avant d’installer le module externe.

## Installez le [!DNL Adobe Workfront for design and video] plugin

>[!TIP]
>
>Si vous êtes un [!DNL Adobe Admin Console] administrateur, vous pouvez inclure le module externe dans [!DNL Creative Cloud] packages de déploiement. Pour plus d’informations, voir [Inclusion de modules externes dans votre module](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

Pour installer le [!DNL Adobe Workfront for design and video] module externe :

1. Ouvrez le [!DNL Adobe Creative Cloud] application.
1. Cliquez sur le bouton **[!UICONTROL Marketplace]** à proximité de la partie supérieure de la fenêtre.
1. Dans le **[!UICONTROL Rechercher tous les modules externes]** box, type *Workfront*, puis appuyez sur **[!UICONTROL Entrée]**.

   ![](assets/adobe-marketplace-350x218.png)

1. When [!DNL Adobe Workfront for design and video] s’affiche dans les résultats de la recherche, cliquez sur **[!UICONTROL Get]**.
1. Lisez les informations de la boîte de dialogue, puis cliquez sur **[!UICONTROL OK]**.
1. Une fois le module externe installé, ouvrez la [!DNL Creative Cloud] de l’application dont vous avez besoin et recherchez le module externe Workfront dans le panneau du module externe.

   <!-- new screen -->

1. Pour plus d’informations sur l’ouverture du module externe, reportez-vous à la section suivante.

## Ouvrez le [!DNL Adobe Workfront for design and video] plugin

1. Ouvrez le module de Creative Cloud que vous souhaitez utiliser.

1. Créez un projet ou ouvrez un projet existant.

1. Dans le menu supérieur, cliquez sur **Windows** > **Extensions** > **Menu Adobe Workfront**.

   >[!NOTE]
   >
   >Si vous utilisez Premiere Pro, un projet doit être ouvert pour accéder à ce menu.

   ![](assets/adobe-workfront-menu.png)


   >[!TIP]
   >
   >Si le module externe ne s’affiche pas après son ouverture à partir du menu Extensions, il peut se trouver derrière l’application de Creative Cloud. Essayez de réduire l’application pour trouver le module externe.

1. Pour plus d’informations sur la connexion au module externe, reportez-vous à la section suivante.


## Connectez-vous à [!DNL Adobe Workfront for design and video]

1. Dans la **[!UICONTROL Modules externes]** dans la partie supérieure de l’écran, sélectionnez **[!UICONTROL Panneau du module externe]**.
1. Sélectionner **[!DNL Adobe Workfront for design and video]**.
1. Saisissez votre domaine, puis cliquez sur **[!UICONTROL Connexion]**. Une page de navigateur s’ouvre.

   >[!TIP]
   >
   >* Pour trouver votre domaine, ouvrez un navigateur et accédez à [!DNL Workfront] et copiez la première partie de l’URL :\
      >![](assets/domain-350x50.png)
   >
   > * Si votre instance Workfront est intégrée à Experience Cloud, demandez à votre administrateur de vous fournir le domaine Workfront situé sous Produit > Workfront dans le Admin Console.


1. Dans le navigateur, saisissez votre [!DNL Workfront] informations d’identification, puis cliquez sur **[!UICONTROL Connexion]**. Si votre entreprise utilise une authentification unique (SSO), vous serez dirigé vers la page de votre fournisseur d’authentification unique pour vous connecter.

   >[!NOTE]
   >
   >Il se peut que vous ne soyez pas invité à saisir votre [!DNL Workfront] informations d’identification si vous vous êtes connecté récemment.

1. Suivez les invites pour vous connecter à [!DNL Workfront].

   >[!NOTE]
   >
   >* [!DNL Workfront] se connecte à [!DNL Adobe Creative Cloud] en utilisant OAuth 2.0, une norme sécurisée utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs.
   >* Lorsque vous êtes invité à saisir la variable [domaine ou hôte] de votre [!DNL Workfront] compte, saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre société correspond généralement au nom de votre société.


1. Cliquez sur **[!UICONTROL Autoriser l’accès]** pour terminer la connexion.
1. Revenir à [!DNL Adobe Photoshop] pour voir votre travail.

