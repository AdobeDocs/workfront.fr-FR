---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configurer [!DNL Adobe Workfront] pour [!DNL Outlook]
description: Le module complémentaire  [!DNL Adobe Workfront] [!DNL Outlook] vous permet d’effectuer les tâches clé [!DNL Workfront]  directement depuis Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 5%

---

# Configurer [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

Le module complémentaire [!DNL Adobe Workfront] [!DNL Outlook] vous permet d’effectuer les tâches clés suivantes [!DNL Workfront] directement depuis Outlook :

* Mettre à jour un projet, une tâche ou un problème existant à l’aide des informations d’un courrier électronique. Pour plus d&#39;informations, voir [Mettre à jour un objet existant à partir d&#39;un [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Créez une requête [!DNL Workfront] basée sur un courrier électronique dans [!DNL Outlook]. Pour plus d’informations, voir [Création d’une requête Adobe Workfront à partir d’un  [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Ajoutez un email comme tâche dans votre zone [!UICONTROL Mon travail]. Pour plus d’informations, voir [Ajout d’un  [!DNL Outlook] email en tant que tâche à votre liste de travail](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Répondez aux commentaires via le module complémentaire [!DNL Workfront] pour [!DNL Outlook]. Pour plus d’informations sur la réponse aux commentaires de Workfront pour [!DNL Outlook], voir [Réponse à un commentaire de [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Créez des tâches et des problèmes à partir de zéro, ou créez-les à partir d’emails existants (à l’aide de la fonctionnalité glisser-déposer). Pour plus d’informations, voir [Ajout d’un [!DNL Outlook] email à un projet en tant que tâche ou problème](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Vous devez ajouter le module [!DNL Workfront] à votre compte [!DNL Outlook] avant de pouvoir utiliser [!DNL Workfront for Outlook].

Si vous ne parvenez pas à installer le module complémentaire [!DNL Workfront] avec votre compte [!DNL Outlook], contactez votre administrateur [!DNL Workfront] pour vous assurer que les modules complémentaires [!DNL Outlook] sont activés pour votre organisation.

Pour plus d’informations sur l’activation de l’intégration [!DNL Outlook] pour votre organisation, voir [Activer [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> 
   <p>Nouveau plan : [!UICONTROL Standard]</p> 
   <p>Plan actuel :[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Votre administrateur [!DNL Workfront] doit activer [!DNL Outlook for Office] avec [!DNL Workfront] avant de pouvoir utiliser cette intégration.

## Configuration requise

Les applications suivantes sont disponibles :

* **[!DNL Outlook]sur le Web :** Le module complémentaire [!DNL Workfront] est disponible lorsque vous utilisez [!DNL Outlook] depuis un navigateur Web, que ce soit sur un ordinateur de bureau ou un appareil mobile. Cette fonctionnalité est également disponible lors de l’utilisation de l’application web [!DNL Outlook].
* **[!DNL Outlook]Application de bureau :** Le module complémentaire [!DNL Workfront] est disponible lors de l’utilisation des versions de bureau [!DNL Windows] et [!DNL Mac] de [!DNL Outlook] incluses dans le package [!DNL Office].

Le module complémentaire [!DNL Workfront] pour [!DNL Outlook] est pris en charge dans les environnements qui répondent aux exigences suivantes :

* [Conditions client](#client-requirements-client-requirements)
* [Exigences relatives aux serveurs de messagerie](#mail-server-requirements-mail-server-requirements)

### Conditions client {#client-requirements}

Workfront prend en charge les versions suivantes de [!DNL Outlook] :

* [!DNL Outlook 2013] ou version ultérieure le [!DNL Windows]
*[!DNL  Outlook 2016] ou version ultérieure sur [!DNL Windows]
* [!DNL Outlook] sur [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] sur [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] sur le web

Vous devez être connecté à un [!DNL Exchange Server] ou [!DNL Office 365] à l’aide d’une connexion directe.

Lors de la configuration du client, l&#39;utilisateur doit sélectionner l&#39;un des types de compte suivants :

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] &#x200B;**&#x200B;** Si le client est configuré pour se connecter avec POP3 ou IMAP, le module complémentaire [!DNL Workfront] ne se charge pas.

### Exigences relatives aux serveurs de messagerie {#mail-server-requirements}

Les exigences du serveur de messagerie sont remplies par défaut lorsque vous vous connectez à [!DNL Office 365] ou [!DNL Outlook.com]. Toutefois, si vous êtes connecté à une installation on-premise de [!DNL Exchange Server], les conditions suivantes s’appliquent :

* Workfront prend en charge tous les [!DNL Exchange On-Premise] serveurs
* [!DNL Exchange Web Services] (EWS) doit être activé et exposé à Internet.
* Le serveur doit disposer d’un certificat d’authentification valide pour que le serveur puisse émettre des jetons d’identité valides. Les nouvelles installations de [!DNL Exchange Server] incluent un certificat d’authentification par défaut.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Pour accéder au module complémentaire [!DNL Workfront] à partir de [[!DNL Office] Store](https://store.office.com/), vos serveurs d&#39;accès client doivent pouvoir communiquer avec [https://store.office.com](https://store.office.com/).

Pour plus d&#39;informations sur les environnements pris en charge, consultez la [[!DNL Microsoft Office 365] page d&#39;accueil](https://products.office.com/en-us/office-365-home).

## Installation du module complémentaire

Vous pouvez obtenir le module complémentaire Workfront pour Outlook à partir du [Microsoft store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] pour [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Dans [!DNL Outlook 365], cliquez sur l’icône **[!UICONTROL Parcourir les modules complémentaires]** ![](assets/outlook-add-in-26x26.png) en haut de l’interface Office 365, puis cliquez sur **[!UICONTROL Gérer les modules complémentaires]**.

1. Dans la zone **[!UICONTROL Rechercher des modules complémentaires]**, recherchez **[!DNL Workfront]**, puis appuyez sur [!UICONTROL Entrée].

1. Cliquez sur **[!UICONTROL Ajouter]**.

### [!DNL Workfront] pour [!DNL Outlook] sur le Web {#workfront-for-outlook-on-the-web}

1. Ouvrez [!DNL Microsoft Outlook] dans un navigateur web.
1. Cliquez sur l’icône **[!UICONTROL Parcourir] des modules complémentaires** ![](assets/outlook-add-in-web-version-20x20.png).

   Pour localiser l’icône, reportez-vous à la section [Utilisation des modules complémentaires dans  [!DNL Outlook]  sur le web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) de la documentation Microsoft.

1. Recherchez **[!DNL Workfront]** dans le champ **[!UICONTROL Rechercher des modules complémentaires]**, puis appuyez sur **[!UICONTROL Entrée]**.

1. Lorsqu’il apparaît dans la liste, cliquez sur **Ajouter**.

### [!DNL Workfront for Outlook] sur [!UICONTROL Windows] ou [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Cliquez sur **[!UICONTROL Home]** > **[!UICONTROL Store]** sur le ruban.

1. Recherchez **[!DNL Workfront]** dans le champ **[!UICONTROL Rechercher]**, puis appuyez sur **[!UICONTROL Entrée]**.

1. Cliquez sur le bouton bascule pour activer le module complémentaire **[!UICONTROL [!DNL Workfront]]**.

## Connectez-vous à [!DNL Workfront] depuis [!DNL Outlook]

1. Dans [!DNL Outlook], sélectionnez un message électronique, puis cliquez sur l’icône **[!DNL Workfront]** dans l’en-tête de l’email.
1. Suivez les invites pour vous connecter à [!DNL Workfront] à l’aide de l’authentification améliorée, d’OAuth 2.0 ou de l’URL SAML (Security Assertion Markup Language).

   Avant que les utilisateurs puissent se connecter au module complémentaire [!DNL Workfront] à l’aide de SAML, un administrateur [!DNL Workfront] doit d’abord activer les modules complémentaires [!DNL Office 365] pour s’authentifier à l’aide d’une solution SAML 2.0. Pour plus d’informations, reportez-vous à la section [Configuration [!DNL Adobe Workfront] avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) de l’article [Configuration [!DNL Adobe Workfront] avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Lorsque vous êtes invité à saisir le domaine de votre compte [!DNL Workfront], saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre société correspond généralement au nom de votre société.
   >* L’authentification améliorée n’est pas disponible tant qu’un administrateur [!DNL Workfront] ne l’a pas activée pour cette intégration.

