---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Affichage et gestion des applications OAuth2 personnalisées
description: En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez afficher et gérer les applications OAuth2 pour votre instance de Workfront, qui permettent à d’autres applications d’accéder à Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 31e5f5e039e25fa25f3038c23ee579ba1f830bb7
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 80%

---

# Afficher et gérer des applications OAuth2 personnalisées

En tant qu’administrateur ou administratrice d’[!DNL Adobe Workfront], vous pouvez afficher et gérer les applications OAuth2 pour votre instance de [!DNL Workfront], qui permettent à d’autres applications d’accéder à [!UICONTROL Workfront].

>[!NOTE]
>
>* Dans le contexte d’OAuth2, « Application OAuth2 » fait référence à ce type de lien d’accès entre une application et un serveur tel que [!DNL Workfront]. Pour plus d’informations, voir [Créer des applications OAuth2 pour les intégrations de  [!DNL Workfront] ](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>* Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.

* Pour plus d’informations, d’instructions et de détails sur la création d’applications OAuth2 personnalisées, voir [Création d’applications OAuth2 pour  [!DNL Workfront]  intégrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Pour plus d’informations, d’instructions et de détails sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur (flux de code d’autorisation), voir [ Configurer et utiliser les applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).
* Pour plus d’informations, d’instructions et de détails sur la configuration et l’utilisation de l’application OAuth2 à l’aide de l’authentification du serveur (flux JWT), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Pour obtenir des instructions sur la configuration et l’utilisation de l’application OAuth2 à l’aide de PKCE, voir [Configurer et utiliser des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur ou une administratrice Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous devez créer les applications [!UICONTROL OAuth2] de votre entreprise avant de pouvoir les afficher ou les gérer.

Pour plus d’informations, voir [Créer des applications OAuth2 pour les intégrations de  [!DNL Workfront] ](../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Gérer des applications OAuth2 personnalisées

* [Afficher et modifier des applications OAuth2 personnalisées](#view-and-edit-custom-oauth2-applications)
* [Supprimer des applications OAuth2 personnalisées](#delete-custom-oauth2-applications)

### Afficher et modifier des applications OAuth2 personnalisées {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Cliquez sur **[!UICONTROL Créer l’intégration d’application]**.
1. Pointez sur l’application et cliquez sur **[!UICONTROL Modifier]** ![Icône Modifier](assets/edit-icon.png) lorsqu’elle s’affiche à l’extrémité droite.
1. (Facultatif) Modifiez les détails de l’application.

   Pour les champs relatifs aux applications OAuth2 et JWT, voir [Créer des applications OAuth2 pour les intégrations de  [!DNL Workfront] ](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Supprimer des applications OAuth2 personnalisées {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Pointez sur l’application et cliquez sur **[!UICONTROL Supprimer]** ![Supprimer](assets/delete.png) lorsqu’elle s’affiche à l’extrême droite.

## Gérer des secrets clients dans les applications OAuth2

* [Afficher les détails du secret client](#view-client-secret-details)
* [Ajouter ou modifier des notes pour le secret client](#add-or-edit-notes-for-client-secret)
* [Supprimer le secret client](#delete-client-secret)

### Afficher les détails du secret client {#view-client-secret-details}

>[!IMPORTANT]
>
>Vous ne pouvez pas afficher le secret client. Si vous avez perdu votre secret client, vous devez le supprimer et en créer un nouveau.
>
>* Pour supprimer un secret client, voir [Supprimer le secret client](#delete-client-secret) dans cet article.
>* Pour créer un secret client, voir [Créer une application OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) dans [Créer des applications OAuth2 pour les intégrations de  [!DNL Workfront] ](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Pointez sur l’application, puis cliquez sur l’icône **[!UICONTROL Modifier]** lorsqu’elle apparaît tout à droite.
1. Affichez les détails dans la zone Secret client :

   * Date de création
   * Date de dernière utilisation
   * Notes

     Pour ajouter des notes à un secret client, voir [Ajouter ou modifier des notes pour le secret client](#add-or-edit-notes-for-client-secret).

### Ajouter ou modifier des notes pour le secret client {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Cliquez sur **[!UICONTROL Créer l’intégration d’application]**.
1. Pointez sur l’application, puis cliquez sur l’icône **[!UICONTROL Modifier]** lorsqu’elle apparaît tout à droite.
1. Localisez le secret client pour lequel vous souhaitez ajouter ou modifier une note.
1. Cliquez sur la zone contenant les détails du secret client.

   Vous pouvez maintenant ajouter du texte pour la note ou modifier le texte de la note existant.

   >[!NOTE]
   >
   >Le texte de la note peut contenir jusqu’à 64 caractères.

1. Cliquez hors de la zone ou appuyez sur **[!UICONTROL Entrée]** pour enregistrer le texte de la note.

### Supprimer le secret client {#delete-client-secret}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth]**.
1. Cliquez sur **[!UICONTROL Créer l’intégration d’application]**.
1. Pointtez sur l’application, puis cliquez sur l’icône **[!UICONTROL Modifier]** lorsqu’elle apparaît tout à droite.
1. Recherchez le secret client que vous souhaitez supprimer.
1. Cliquez sur l’icône **[!UICONTROL Supprimer]** ![Supprimer](assets/delete.png) en regard du secret client.
