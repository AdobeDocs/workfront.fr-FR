---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connecter  [!DNL Adobe Workfront Fusion]  à  [!DNL Google Services]  en utilisant un client OAuth personnalisé
description: Vous pouvez utiliser  [!DNL Adobe Workfront Fusion]  pour vous connecter à  [!DNL Google Services]  à l’aide d’un client OAuth personnalisé. Cette procédure nécessite l’existence d’un compte  [!DNL Google] .
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 100%

---

# Connecter [!DNL Adobe Workfront Fusion] à [!DNL Google Services] en utilisant un client OAuth personnalisé

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Actuelle : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Héritée : n’importe laquelle. </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Nouveau :</p> <ul><li>Forfait [!DNL Workfront] [!UICONTROL Select] ou [!UICONTROL Prime] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Forfait [!DNL Workfront] [!UICONTROL Ultimate] : [!DNL Workfront Fusion] est inclus.</li></ul>
   <p>Ou</p>
   <p>Actuel : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Vous devez disposer d’un compte [!DNL Google] pour établir cette connexion.

## Connecter Fusion aux services Google à l’aide d’un client OAuth personnalisé

Pour établir cette connexion, vous devez créer et configurer un projet sur la plateforme Google Cloud, puis configurer la connexion dans Fusion en fonction de ce projet.

* [Créer un projet dans  [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Configurer les paramètres de [!UICONTROL consentement OAuth]](#configure-oauth-consent-settings)
* [Créer des informations d’identification OAuth](#create-oauth-credentials)
* [Se connecter à  [!DNL Google]  dans  [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Cette procédure est destinée à :
>
>* un usage personnel (utilisateurs ou utilisatrices [!DNL `@gmail.com`] et [!DNL `@googlemail.com`]) ;
>* un usage interne (utilisateurs ou utilisatrices [!DNL Google Workspace] qui préfèrent utiliser un client OAuth personnalisé).

### Créer un projet dans [!DNL Google Cloud Platform]

Pour créer un projet sur la plateforme [!DNL Google Cloud], procédez comme suit :

1. Connectez-vous à la plateforme [[!DNL Google Cloud] ](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) à l’aide de vos informations d’identification [!DNL Google].
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Tableau de bord]**.
1. Cliquez sur **[!UICONTROL Créer un projet]** dans le coin supérieur droit de l’écran.
1. Saisissez le **[!UICONTROL Nom du projet]**, puis cliquez sur **[!UICONTROL Créer]**.

1. Cliquez sur l’onglet **[!UICONTROL Activer les API et les services]** en haut de l’écran.
1. Dans le champ **[!UICONTROL Rechercher les API et les services]** en haut de l’écran, saisissez le nom du service que vous voulez utiliser (par exemple, API [!DNL Gmail] ou API [!DNL Google Drive]).
1. Lorsqu’il s’affiche, cliquez sur l’API ou le service que vous souhaitez connecter à [!DNL Workfront Fusion].
1. Cliquez sur **[!UICONTROL Activer]** pour activer l’API sélectionnée.
1. Répétez les étapes 6 à 8 pour chaque API que vous souhaitez activer.

   >[!NOTE]
   >
   >Vous devez activer l’API [!DNL Google Drive] ainsi que l’API de toutes les applications [!DNL Google] que vous souhaitez utiliser (comme l’API [!DNL Google Sheets]).

1. Dans l’écran qui s’affiche, cliquez sur **[!UICONTROL Créer des informations d’identification]** dans le coin supérieur droit.
1. Passez à la section [Configurer les paramètres de consentement OAuth](#configure-oauth-consent-settings) dans cet article.

### Configurer les paramètres de [!UICONTROL consentement OAuth]

1. Dans le panneau de gauche, cliquez sur l’**[!UICONTROL écran de consentement OAuth]**.
1. Sélectionnez **[!UICONTROL Externe]**, puis cliquez sur **[!UICONTROL Créer]**.

   >[!NOTE]
   >
   >Cette option ne vous sera pas facturée. Pour plus d’informations, consultez les informations de [!DNL Google] sur les exceptions aux exigences de vérification.

1. Remplissez les champs obligatoires comme suit :

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Saisissez le nom de l’application qui demande un consentement.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL User support email]</td> 
      <td>Saisissez une adresse e-mail pour que les utilisateurs et utilisatrices puissent vous contacter en cas de questions sur le consentement au moment de se connecter à cette application.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email addresses]</td> 
      <td>Saisissez une ou plusieurs adresses e-mail que Google peut utiliser pour vous informer de toute modification apportée à votre projet.</td> 
     </tr> 
    </tbody> 
   </table>

1. Dans [!UICONTROL Domaines autorisés], cliquez sur **[!UICONTROL Ajouter un domaine]**, et saisissez `workfrontfusion.com`.

1. Cliquez sur **[!UICONTROL Enregistrer et continuer]**.
1. Cliquez sur **[!UICONTROL Ajouter ou supprimer des portées]**.
1. Dans le panneau de droite, activez les portées suivantes :

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Service/API</th> 
      <th>Portées requises</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

Il se peut que vous deviez développer la liste ou passer à la page suivante de la liste pour les voir toutes.

1. Cliquez sur **[!UICONTROL Mettre à jour]**.
1. Cliquez sur **[!UICONTROL Enregistrer et continuer]**.
1. (Facultatif) Ajoutez des utilisateurs et utilisatrices de test au projet.
1. Cliquez sur **[!UICONTROL Enregistrer et continuer]**.
1. Vérifiez l’exactitude de vos informations, puis cliquez sur **[!UICONTROL Retour au tableau de bord]**.

   >[!NOTE]
   >
   >Vous n’avez pas besoin d’envoyer votre écran de consentement et votre demande de vérification à [!DNL Google].

1. Passez à [Créer des informations d’identification OAuth](#create-oauth-credentials).

### Créer des informations d’identification OAuth

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Informations d’identification]**.

   >[!NOTE]
   >
   >Si ce n’est pas la première API ou le premier service ([!DNL Gmail] ou [!DNL Google Drive]) que vous activez, vous n’avez pas besoin de créer de nouvelles informations d’identification.

1. Cliquez sur **[!UICONTROL Créer des informations d’identification]** en haut de l’écran, puis sélectionnez **[!UICONTROL ID client OAuth]** dans le menu déroulant.

1. Remplissez les champs obligatoires comme suit :

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Sous [!UICONTROL URI de redirection autorisés], cliquez sur **[!UICONTROL Ajouter un URI]** et saisissez **un** des éléments suivants :

   * Pour [!DNL Gmail] ou [!DNL Google Drive] : `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Pour d’autres applications [!DNL Google] : `https://app.workfrontfusion.com/oauth/cb/google`

1. Cliquez sur **[!UICONTROL Créer]**.

   L’[!UICONTROL ID client] et le [!UICONTROL secret client] s’affichent.

1. Copiez l’[!UICONTROL ID client] et le [!UICONTROL secret client] dans un endroit sûr. Vous les utiliserez pour vous connecter à [!DNL Workfront Fusion].
1. Continuez vers [Se connecter à  [!DNL Google]  dans  [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Se connecter à [!DNL Google] dans [!DNL Workfront Fusion]

Le processus de création d’une connexion à [!DNL Google] diffère selon que vous utilisez un module d’un service [!DNL Google] (tel que [!DNL Google Sheets] ou [!DNL Google Docs]), ou que vous vous connectez à [!DNL Google] via le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth2.0].

* [Se connecter à  [!DNL Google]  dans un service  [!DNL Google] ](#connect-to-google-in-a-google-service)
* [Se connecter à  [!DNL Google]  dans le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth2.0]](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Se connecter à [!DNL Google] dans un service [!DNL Google]

1. Dans [!DNL Workfront Fusion], localisez le module [!DNL Google] pour lequel vous devez créer une connexion.
1. Cliquez sur **[!UICONTROL Créer une connexion]**, puis cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.

1. Saisissez l’[!UICONTROL ID client] et le [!UICONTROL secret client] que vous avez récupérés dans [[!UICONTROL Créer des informations d’identfication OAuth]](#create-oauth-credentials) dans les champs respectifs, puis cliquez sur **[!UICONTROL Continuer]**.

1. Connectez-vous avec votre compte [!DNL Google].

   La fenêtre **[!UICONTROL Cette application n’est pas vérifiée]** s’affiche. Notez que l’« application » mentionnée dans le titre de la fenêtre est le client OAuth que vous avez créé ci-dessus.

1. Cliquez sur **[!UICONTROL Avancé]**, puis sur **[!UICONTROL Accéder à [!DNL Workfront Fusion] (risqué)]** pour autoriser l’accès à l’aide de votre client OAuth personnalisé.

1. Cliquez sur **[!UICONTROL Autoriser]** pour accorder l’autorisation à [!DNL Workfront Fusion].
1. Dans la fenêtre qui s’affiche, cliquez à nouveau sur **[!UICONTROL Autoriser]** pour confirmer vos choix.

   La connexion au service [!DNL Google] souhaité est établie à l’aide d’un client OAuth personnalisé.

#### Se connecter à [!DNL Google] dans le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth2.0] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Pour savoir comment se connecter à [!DNL Google] dans le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth2.0], voir [Instructions pour créer une connexion à  [!DNL Google]  dans le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) dans le module [[!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Message d’erreur possible : [!UICONTROL [403] Accès non configuré]

Si le message d’erreur [!UICONTROL `403 Access Not Configured`] s’affiche, vous devez activer l’API correspondante dans votre plateforme Google Cloud. Pour activer l’API, suivez les étapes de la section [Créer un projet sur  [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) de cet article.
