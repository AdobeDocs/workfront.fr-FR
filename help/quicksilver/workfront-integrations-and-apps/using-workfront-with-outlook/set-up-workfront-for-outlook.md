---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configuration [!DNL Adobe Workfront] pour [!DNL Outlook]
description: Adobe Workfront Fusion offre une intégration à Outlook. Cet article décrit comment commencer à utiliser cette intégration dans vos propres workflows.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: a1569362dee8cd686a91698af3c9c217e920c263
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Configuration [!DNL Adobe Workfront for Outlook]

La variable [!DNL Adobe Workfront] [!DNL Outlook] module complémentaire vous permet d’effectuer les opérations suivantes : [!DNL Workfront] tâches directement depuis Outlook :

* Mettre à jour un projet, une tâche ou un problème existant à l’aide des informations d’un courrier électronique. Pour plus d’informations, voir [Mettre à jour un objet existant à partir d’un [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Créez un [!DNL Workfront] requête basée sur un courrier électronique dans [!DNL Outlook]. Pour plus d’informations, voir [Créez une requête Adobe Workfront à partir d’une [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Ajoutez un email comme tâche dans votre [!UICONTROL Mon travail] zone. Pour plus d’informations, voir [Ajoutez un [!DNL Outlook] envoyer un email en tant que tâche à votre liste de travail ;](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Répondre aux commentaires via [!DNL Workfront] module complémentaire pour [!DNL Outlook]. Pour plus d’informations sur la réponse aux commentaires de Workfront pour [!DNL Outlook], voir [Réponse à un commentaire de [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Créez des tâches et des problèmes à partir de zéro, ou créez-les à partir d’emails existants (à l’aide de la fonctionnalité glisser-déposer). Pour plus d’informations, voir [Ajoutez un [!DNL Outlook] envoyer par courrier électronique à un projet en tant que tâche ou problème ;](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Vous devez ajouter la variable [!DNL Workfront] de votre [!DNL Outlook] avant d’utiliser [!DNL Workfront for Outlook].

Si vous ne parvenez pas à installer le [!DNL Workfront] module complémentaire avec votre [!DNL Outlook] , contactez votre [!DNL Workfront] pour vous assurer que [!DNL Outlook] les modules complémentaires sont activés pour votre organisation.

Pour plus d’informations sur l’activation de la variable [!DNL Outlook] intégration pour votre organisation, voir [Activer [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau plan : Standard </p>
 <p>ou</p> 
<p>Plan actuel : [!UICONTROL Work], [!UICONTROL Plan] </p> 
  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Votre [!DNL Workfront] L’administrateur doit activer [!DNL Outlook for Office] avec [!DNL Workfront] avant de pouvoir utiliser cette intégration.

## Configuration requise

Les applications suivantes sont disponibles :

* **[!DNL Outlook]sur le Web :** La variable [!DNL Workfront] est disponible lors de l’utilisation de [!DNL Outlook] à partir d’un navigateur web, que ce soit sur un ordinateur de bureau ou un périphérique mobile. Cette fonctionnalité est également disponible lors de l’utilisation de la fonction [!DNL Outlook] application web.
* **[!DNL Outlook]Application de bureau :** La variable [!DNL Workfront] est disponible lors de l’utilisation de la fonction [!DNL Windows] et [!DNL Mac] Versions de bureau de [!DNL Outlook] inclus dans la variable [!DNL Office] module.

La variable [!DNL Workfront] module complémentaire pour [!DNL Outlook] est pris en charge dans les environnements qui répondent aux exigences suivantes :

* [Conditions client](#client-requirements-client-requirements)
* [Exigences relatives aux serveurs de messagerie](#mail-server-requirements-mail-server-requirements)

### Conditions client {#client-requirements}

Nous prenons en charge les versions suivantes de [!DNL Outlook]:

* [!DNL Outlook 2013] ou ultérieur [!DNL Windows]
*[!DNL  Outlook 2016] ou ultérieur [!DNL Windows]
* [!DNL Outlook] on [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] on [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] sur le web

Vous devez être connecté à un [!DNL Exchange Server] ou [!DNL Office 365] en utilisant une connexion directe.

Lors de la configuration du client, l&#39;utilisateur doit sélectionner l&#39;un des types de compte suivants :

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B; Si le client est configuré pour se connecter à POP3 ou IMAP, la variable [!DNL Workfront] module complémentaire ne se charge pas.

### Exigences relatives aux serveurs de messagerie {#mail-server-requirements}

Les exigences du serveur de messagerie sont remplies par défaut lorsque vous vous connectez à [!DNL Office 365] ou [!DNL Outlook.com]. Cependant, si vous êtes connecté à une installation on-premise de [!DNL Exchange Server], les exigences suivantes s’appliquent :

* Nous soutenons tous [!DNL Exchange On-Premise] serveurs
* [!DNL Exchange Web Services] (EWS) doit être activé et exposé à Internet.
* Le serveur doit disposer d’un certificat d’authentification valide pour que le serveur puisse émettre des jetons d’identité valides. Nouvelles installations de [!DNL Exchange Server] incluez un certificat d’authentification par défaut.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Pour accéder à la variable [!DNL Workfront] du module complémentaire [[!DNL Office] Magasin](https://store.office.com/), vos serveurs d’accès client doivent pouvoir communiquer avec  [https://store.office.com](https://store.office.com/).

Pour plus d’informations sur les environnements pris en charge, voir [[!DNL Microsoft Office 365] page d&#39;accueil](https://products.office.com/en-us/office-365-home).

## Installation du module complémentaire

Pour plus d’informations sur la configuration de la variable [!DNL Workfront] module complémentaire pour [!DNL Outlook], voir [[!DNL Workfront] - Gestion collaborative du travail.](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)

* [[!DNL Workfront] pour [!DNL Outlook 365]](#workfront-for-outlook-365-workfront-for-outlook-365)
* [[!DNL Workfront] pour [!DNL Outlook] sur le Web](#workfront-for-outlook-on-the-web-workfront-for-outlook-on-the-web)
* [[!DNL Workfront] pour [!DNL Outlook] on [!DNL Windows] ou [!DNL Mac]](#workfront-for-outlook-on-windows-or-mac-workfront-for-outlook-on-windows-or-mac)

### [!DNL Workfront] pour [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Dans [!DNL Outlook 365], cliquez sur le **[!UICONTROL Parcourir les modules complémentaires]** icon ![](assets/outlook-add-in-26x26.png)en haut de l’interface d’Office 365, puis cliquez sur **[!UICONTROL Gestion des modules complémentaires]**.

1. Dans le **[!UICONTROL Rechercher des modules complémentaires]** box, recherchez **[!DNL Workfront]** puis appuyez [!UICONTROL Entrée].

1. Cliquez sur **[!UICONTROL Ajouter]**.

### [!DNL Workfront] pour [!DNL Outlook] sur le Web {#workfront-for-outlook-on-the-web}

1. Ouvrir [!DNL Microsoft Outlook] dans un navigateur web.
1. Cliquez sur le bouton **[!UICONTROL Parcourir] add-ins** icon ![](assets/outlook-add-in-web-version-20x20.png).

   Pour localiser l’icône, voir [Utilisation de modules complémentaires dans [!DNL Outlook] sur le web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) dans la documentation de Microsoft.

1. Recherchez **[!DNL Workfront]** dans le **[!UICONTROL Rechercher des modules complémentaires]** champ, puis appuyez sur **[!UICONTROL Entrée]**.

1. Lorsqu’il apparaît dans la liste, cliquez sur **Ajouter**.

### [!DNL Workfront for Outlook] on [!UICONTROL Windows] ou [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Cliquez sur **[!UICONTROL Accueil]** > **[!UICONTROL Magasin]** sur le ruban.

1. Recherchez **[!DNL Workfront]** dans le **[!UICONTROL Rechercher]** champ, puis appuyez sur **[!UICONTROL Entrée]**.

1. Cliquez sur le bouton bascule pour activer la fonction **[!UICONTROL [!DNL Workfront]add-in]**.

## Connexion à [!DNL Workfront] de [!DNL Outlook]

1. Dans [!DNL Outlook], sélectionnez un message électronique, puis cliquez sur le bouton **[!DNL Workfront]** dans l’en-tête de l’email.
1. Suivez les invites pour vous connecter à [!DNL Workfront] à l’aide d’une authentification améliorée, d’OAuth 2.0 ou de l’URL SAML (Security Assertion Markup Language).

   Avant que les utilisateurs puissent se connecter à la [!DNL Workfront] module complémentaire utilisant SAML, un [!DNL Workfront] L’administrateur doit d’abord activer [!DNL Office 365] des modules complémentaires pour l’authentification à l’aide d’une solution SAML 2.0. Pour plus d’informations, voir la section [Configurer [!DNL Adobe Workfront] avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) dans l’article [Configurer [!DNL Adobe Workfront] avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Lorsque vous êtes invité à saisir le domaine de votre [!DNL Workfront] compte, saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre société correspond généralement au nom de votre société.
   >* L’authentification améliorée n’est pas disponible tant qu’un [!DNL Workfront] L’administrateur l’active pour cette intégration.

