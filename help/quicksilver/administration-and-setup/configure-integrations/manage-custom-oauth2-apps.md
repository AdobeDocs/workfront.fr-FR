---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Afficher et gérer des applications OAuth2 personnalisées
description: En tant qu’administrateur Adobe Workfront, vous pouvez afficher et gérer les applications OAuth2 pour votre instance de Workfront, qui permettent à d’autres applications d’accéder à Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 5%

---

# Afficher et gérer des applications OAuth2 personnalisées

Comme [!DNL Adobe Workfront] administrateur, vous pouvez afficher et gérer les applications OAuth2 pour votre instance de [!DNL Workfront], qui permettent à d’autres applications d’accéder à [!UICONTROL Workfront].

>[!NOTE]
>
>* Dans le contexte d’OAuth2, &quot;Application Oauth2&quot; fait référence à ce type de lien d’accès entre une application et un serveur, tel que [!DNL Workfront]. Pour plus d’informations, voir [Création d’applications OAuth2 pour [!DNL Workfront] intégrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.

* Pour plus d’informations sur la création d’applications OAuth2 personnalisées, voir [Création d’applications OAuth2 pour [!DNL Workfront] intégrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur (flux de code d’autorisation), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 à l’aide de l’authentification du serveur (flux JWT), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Pour obtenir des instructions sur la configuration et l’utilisation de l’application OAuth2 à l’aide de PKCE, voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Formule] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> Vous devez être un [!DNL Workfront] administrateur. </p>
    <p>Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Vous devez créer [!UICONTROL OAuth2] des applications pour votre organisation avant de pouvoir les afficher ou les gérer.

Pour plus d’informations, voir [Création d’applications OAuth2 pour [!DNL Workfront] intégrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Gestion des applications OAuth2 personnalisées

* [Affichage et modification d’applications OAuth2 personnalisées](#view-and-edit-custom-oauth2-applications)
* [Suppression d’applications OAuth2 personnalisées](#delete-custom-oauth2-applications)

### Affichage et modification d’applications OAuth2 personnalisées {#view-and-edit-custom-oauth2-applications}

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Cliquez sur **[!UICONTROL Création d’une intégration d’application]**.
1. Pointez sur l’application, puis cliquez sur **[!UICONTROL Modifier]** ![](assets/edit-icon.png) quand il apparaît à l&#39;extrême droite.
1. (Facultatif) Modifiez les détails de l’application.

   Pour les champs relatifs aux applications OAuth2 et JWT, voir [Création d’applications OAuth2 pour [!DNL Workfront] intégrations](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Suppression d’applications OAuth2 personnalisées {#delete-custom-oauth2-applications}

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Cliquez sur ** **.
1. Pointez sur l’application, puis cliquez sur **[!UICONTROL Supprimer]** ![](assets/delete.png) quand il apparaît à l&#39;extrême droite.

## Gestion des secrets client dans les applications OAuth2

* [Afficher les détails du secret client](#view-client-secret-details)
* [Ajout ou modification de notes pour le secret client](#add-or-edit-notes-for-client-secret)
* [Suppression du secret client](#delete-client-secret)

### Afficher les détails du secret client {#view-client-secret-details}

>[!IMPORTANT]
>
>Vous ne pouvez pas afficher le secret client lui-même. Si vous avez perdu votre secret client, vous devez le supprimer et en créer un nouveau.
>
>* Pour supprimer un secret client, voir [Suppression du secret client](#delete-client-secret) dans cet article.
>* Pour créer un secret client, voir [Création d’une application OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Création d’applications OAuth2 pour [!DNL Workfront] intégrations](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>



1. Cliquez sur le bouton *[!UICONTROL *Menu principal]** icône ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Pointez sur l’application, puis cliquez sur le **[!UICONTROL Modifier]** s’affiche à l’extrême droite.
1. Afficher les détails dans la zone Secret client :

   * Date de création
   * Date de dernière utilisation
   * Notes

     Pour ajouter des notes à un secret client, voir [Ajout ou modification de notes pour le secret client](#add-or-edit-notes-for-client-secret).

### Ajout ou modification de notes pour le secret client {#add-or-edit-notes-for-client-secret}

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Cliquez sur **[!UICONTROL Création d’une intégration d’application]**.
1. Pointez sur l’application, puis cliquez sur le **[!UICONTROL Modifier]** s’affiche à l’extrême droite.
1. Localisez le secret client pour lequel vous souhaitez ajouter ou modifier une note.
1. Cliquez sur la zone contenant les détails du secret client.

   Vous pouvez maintenant ajouter du texte de note ou modifier du texte de note existant.

   >[!NOTE]
   >
   >Le texte de la note peut contenir, au maximum, 64 caractères.

1. Cliquez ou appuyez sur **[!UICONTROL Entrée]** pour enregistrer le texte de la note.

### Suppression du secret client {#delete-client-secret}

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Cliquez sur **[!UICONTROL Création d’une intégration d’application]**.
1. Pointez sur l’application, puis cliquez sur le **[!UICONTROL Modifier]** s’affiche à l’extrême droite.
1. Recherchez le secret client que vous souhaitez supprimer.
1. Cliquez sur le bouton **[!UICONTROL Supprimer]** icon ![](assets/delete.png) en regard du secret client.
