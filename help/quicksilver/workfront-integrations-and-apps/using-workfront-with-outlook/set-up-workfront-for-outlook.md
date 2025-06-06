---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configurer  [!DNL Adobe Workfront]  pour  [!DNL Outlook]
description: Le module complémentaire  [!DNL Adobe Workfront] [!DNL Outlook] vous permet d’effectuer les tâches clés de  [!DNL Workfront]  directement à partir d’Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 75%

---

# Configurer [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>[Microsoft est en train de désactiver la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le complément Workfront Outlook pour l&#39;authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et continuera à être déployée par phases jusqu’en octobre 2025.
>
>* **Une fois que Microsoft a complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionne plus.**
>
>Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière dont les jetons sont réactivés. Après le **30 juin 2025**, les administrateurs ne pourront plus réactiver les jetons eux-mêmes. Seule la prise en charge de Microsoft peut accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Les exceptions ne seront pas accordées.**

Le module complémentaire [!DNL Adobe Workfront] [!DNL Outlook] vous permet d’effectuer les tâches clés [!DNL Workfront] suivantes directement à partir d’Outlook :

* Mettre à jour un projet, une tâche ou un problème existant à l’aide des informations contenues dans un e-mail. Pour plus d’informations, voir [Mettre à jour un objet existant à partir d’un e-mail  [!DNL Outlook] ](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Créez une demande [!DNL Workfront] sur la base d’un e-mail dans [!DNL Outlook]. Pour plus d’informations, voir [Créer une demande Adobe Workfront à partir d’un e-mail  [!DNL Outlook] ](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Ajoutez un e-mail comme tâche dans votre zone [!UICONTROL Mon travail]. Pour plus d’informations, voir [Ajouter un e-mail  [!DNL Outlook]  comme tâche à votre liste de travail](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Répondez aux commentaires via le module complémentaire [!DNL Workfront] pour [!DNL Outlook]. Pour plus d’informations sur la manière de répondre aux commentaires de Workfront pour [!DNL Outlook], voir [Répondre à un commentaire à partir d’ [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Créez des tâches et des problèmes à partir de zéro ou à partir d’e-mails existants (grâce à la fonctionnalité Glisser-déposer). Pour plus d’informations, voir [Ajouter un e-mail  [!DNL Outlook]  à un projet en tant que tâche ou problème](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Vous devez ajouter le module complémentaire [!DNL Workfront] à votre compte [!DNL Outlook] avant de pouvoir utiliser [!DNL Workfront for Outlook].

Si vous ne parvenez pas à installer le module complémentaire [!DNL Workfront] avec votre compte [!DNL Outlook], contactez votre équipe d’administration [!DNL Workfront] pour vous assurer que les modules complémentaires [!DNL Outlook] sont activés pour votre organisation.

Pour plus d’informations sur l’activation de l’intégration d’[!DNL Outlook] pour votre organisation, voir [Activer [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> 
   <p>Nouveau plan : [!UICONTROL Standard]</p> 
   <p>Plan actuel : [!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Votre équipe d’administration [!DNL Workfront] doit activer [!DNL Outlook for Office] avec [!DNL Workfront] avant de pouvoir utiliser cette intégration.

## Configuration requise

Les applications suivantes sont disponibles :

* **[!DNL Outlook]sur le web :** le module complémentaire [!DNL Workfront] est disponible lorsque vous utilisez [!DNL Outlook] à partir d’un navigateur web, que ce soit sur un ordinateur de bureau ou un appareil mobile. Cette fonctionnalité est également disponible lorsque vous utilisez l’application web [!DNL Outlook].
* Application de bureau **[!DNL Outlook] :** le module complémentaire [!DNL Workfront] est disponible lorsque vous utilisez les versions de bureau de [!DNL Windows] et [!DNL Mac] d’[!DNL Outlook] incluses dans le package [!DNL Office].

Le module complémentaire [!DNL Workfront] pour [!DNL Outlook] est pris en charge dans les environnements qui répondent aux exigences suivantes :

* [Exigences relatives au client](#client-requirements-client-requirements)
* [Exigences relatives au serveur de messagerie](#mail-server-requirements-mail-server-requirements)

### Exigences relatives au client {#client-requirements}

Workfront prend en charge les versions suivantes d’[!DNL Outlook] :

* [!DNL Outlook 2013] ou version ultérieure sur [!DNL Windows]
* [!DNL Outlook 2016] ou version ultérieure sur [!DNL Windows]
* [!DNL Outlook] sur [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] sur [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] sur le web

Vous devez vous connecter à un [!DNL Exchange Server] ou à [!DNL Office 365] à l’aide d’une connexion directe.

Lors de la configuration du client, vous devez sélectionner l’un des types de compte suivants :

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] Si le client est configuré pour se connecter avec POP3 ou IMAP, le complément [!DNL Workfront] ne se charge pas.

### Exigences relatives au serveur de messagerie {#mail-server-requirements}

Les conditions requises pour le serveur de messagerie sont remplies par défaut lorsque vous vous connectez à [!DNL Office 365] ou [!DNL Outlook.com]. Toutefois, si vous vous connectez à une installation On-Premise d’[!DNL Exchange Server], les conditions suivantes s’appliquent :

* Workfront prend en charge tous les serveurs [!DNL Exchange On-Premise].
* [!DNL Exchange Web Services] (EWS) doit être activé et doit être exposé à l’Internet.
* Le serveur doit disposer d’un certificat d’authentification valide pour pouvoir délivrer des jetons d’identité valides. Les nouvelles installations d’[!DNL Exchange Server] incluent un certificat d’authentification par défaut.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Afin d’accéder au module complémentaire [!DNL Workfront] à partir de la boutique [[!DNL Office] ](https://store.office.com/), vos serveurs d’accès client doivent pouvoir communiquer avec [https://store.office.com](https://store.office.com/).

Pour plus d’informations sur les environnements pris en charge, voir la page d’accueil [[!DNL Microsoft Office 365] ](https://products.office.com/fr-fr/office-365-home).

## Installer le module complémentaire

Vous pouvez obtenir le module complémentaire Workfront pour Outlook dans le [Microsoft Store](https://appsource.microsoft.com/fr-fr/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] pour [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Dans [!DNL Outlook 365], cliquez sur l&#39;icône **[!UICONTROL Parcourir les compléments]** ![Parcourir les compléments](assets/outlook-add-in-26x26.png)en haut de l&#39;interface Office 365, puis cliquez sur **[!UICONTROL Gérer les compléments]**.

1. Dans la boîte de dialogue **[!UICONTROL Rechercher des modules complémentaires]**, recherchez **[!DNL Workfront]** puis appuyez sur [!UICONTROL Entrée].

1. Cliquez sur **[!UICONTROL Ajouter]**.

### [!DNL Workfront] pour [!DNL Outlook] sur le web {#workfront-for-outlook-on-the-web}

1. Ouvrez [!DNL Microsoft Outlook] dans un navigateur web.
1. Cliquez sur l’icône **[!UICONTROL Parcourir] modules complémentaires** ![Parcourir les modules complémentaires](assets/outlook-add-in-web-version-20x20.png).

   Pour localiser l’icône, voir [Utiliser des modules complémentaires dans  [!DNL Outlook]  sur le web](https://support.microsoft.com/fr-fr/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) dans la documentation Microsoft.

1. Recherchez **[!DNL Workfront]** dans le champ **[!UICONTROL Rechercher des modules complémentaires]**, puis appuyez sur **[!UICONTROL Entrée]**.

1. Lorsqu’il apparaît dans la liste, cliquez sur **Ajouter**.

### [!DNL Workfront for Outlook] sur [!UICONTROL Windows] ou [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Cliquez sur **[!UICONTROL Accueil]** > **[!UICONTROL Boutique]** sur le ruban.

1. Recherchez **[!DNL Workfront]** dans le champ **[!UICONTROL Rechercher]**, puis appuyez sur **[!UICONTROL Entrée]**.

1. Cliquez sur le bouton (bascule) pour activer le module complémentaire **[!UICONTROL [!DNL Workfront]]**.

## Connectez-vous à [!DNL Workfront] à partir d’[!DNL Outlook].

1. Dans [!DNL Outlook], sélectionnez un e-mail, puis cliquez sur l’icône **[!DNL Workfront]** dans l’en-tête de l’e-mail.
1. Sur la page de connexion, cliquez sur **Connexion à Workfront**.
1. Suivez les invites pour vous connecter à [!DNL Workfront] à l’aide d’OAuth 2.0. <!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* Si vous êtes invité à saisir le domaine de votre compte [!DNL Workfront], saisissez-le au format suivant : *yourCompany&#39;sDomain.my.workfront.com*. Le domaine de votre entreprise est généralement le nom de votre entreprise.

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
