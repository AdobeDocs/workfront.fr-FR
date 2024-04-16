---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connexion [!DNL Adobe Workfront Fusion] to [!DNL Google Services] utilisation d’un client OAuth personnalisé
description: Vous pouvez utiliser [!DNL Adobe Workfront Fusion] pour se connecter à [!DNL Google Services] à l’aide d’un client OAuth personnalisé. Cette procédure nécessite une [!DNL Google] compte .
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 7d2b4a9940cb21de1b8b5f2955f53b3d88040e44
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 5%

---

# Connexion [!DNL Adobe Workfront Fusion] to [!DNL Google Services] utilisation d’un client OAuth personnalisé

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>Nouveau : [!UICONTROL Standard]</p><p>Ou</p><p>Actuel : [!UICONTROL Travail] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Actuel : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Hérité : Tout </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Nouveau :</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plan : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan : [!DNL Workfront Fusion] est inclus.</li></ul>
   <p>Ou</p>
   <p>Actuel : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Vous avez besoin d’un [!DNL Google] pour établir cette connexion.

## Connexion de Fusion aux services Google à l’aide d’un client OAuth personnalisé

Pour créer cette connexion, vous devez créer et configurer un projet sur la plateforme Google Cloud, puis configurer la connexion dans Fusion en fonction de ce projet.

* [Créez un projet sur [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Configurer [!UICONTROL Consentement OAuth] paramètres](#configure-oauth-consent-settings)
* [Création d’informations d’identification OAuth](#create-oauth-credentials)
* [Se connecter à [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Cette procédure est destinée à :
>
>* Utilisation personnelle ([!DNL `@gmail.com`] et [!DNL `@googlemail.com`] users)
>* Utilisation interne ([!DNL G Suite] utilisateurs qui préfèrent utiliser un client OAuth personnalisé)

### Créez un projet sur [!DNL Google Cloud Platform]

Pour créer un projet sur [!DNL Google Cloud] Plateforme :

1. Se connecter à [[!DNL Google Cloud] Plateforme](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) en utilisant votre [!DNL Google] informations d’identification.
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Tableau de bord]**.
1. Cliquez sur **[!UICONTROL Créer un projet]** dans le coin supérieur droit de l’écran.
1. Saisissez le **[!UICONTROL Nom du projet]**, puis cliquez sur **[!UICONTROL Créer]**.

1. Cliquez sur le bouton **[!UICONTROL Activation des API et des services]** dans la partie supérieure de l’écran.
1. Dans le **[!UICONTROL Recherche d’API et de services]** dans la partie supérieure de l’écran, saisissez le nom du service que vous souhaitez utiliser (par exemple [!DNL Gmail] API ou [!DNL Google Drive] API).
1. Lorsqu’il s’affiche, cliquez sur l’API ou le service auquel vous souhaitez vous connecter. [!DNL Workfront Fusion].
1. Cliquez sur **[!UICONTROL Activer]** pour activer l’API sélectionnée.
1. Répétez les étapes 6 à 8 pour chaque API à activer.

   >[!NOTE]
   >
   >Vous devez activer [!DNL Google Drive] API ainsi que l’API de tous [!DNL Google] applications que vous souhaitez utiliser (telles que [!DNL Google Sheets] API).

1. Dans l’écran qui s’affiche, cliquez sur **[!UICONTROL Création d’informations d’identification]** dans le coin supérieur droit.
1. Passez à la section [Configuration des paramètres de consentement OAuth](#configure-oauth-consent-settings) dans cet article.

### Configurer [!UICONTROL Consentement OAuth] paramètres

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Écran de consentement OAuth]**.
1. Sélectionner **[!UICONTROL Externe]**, puis cliquez sur **[!UICONTROL Créer]**.

   >[!NOTE]
   >
   >Si vous sélectionnez cette option, aucun frais ne vous sera facturé. Pour plus d’informations, voir [!DNL Google]Informations sur les exceptions aux exigences de vérification de .

1. Renseignez les champs requis comme suit :

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nom de l’application]</p> </td> 
      <td> <p>Saisissez le nom de l’application qui demande le consentement.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Adresse électronique de l’assistance utilisateur]</td> 
      <td>Entrez une adresse électronique à laquelle les utilisateurs pourront vous contacter pour toute question concernant leur consentement lors de la connexion à cette application.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Adresses électroniques]</td> 
      <td>Entrez une ou plusieurs adresses électroniques que Google peut utiliser pour vous informer des modifications apportées à votre projet.</td> 
     </tr> 
    </tbody> 
   </table>

1. Sous [!UICONTROL Domaines autorisés], cliquez sur **[!UICONTROL Ajouter un domaine]**, puis saisissez `workfrontfusion.com`.

1. Cliquez sur **[!UICONTROL Enregistrer et continuer]**.
1. Cliquez sur **[!UICONTROL Ajouter ou supprimer des portées]**.
1. Dans le panneau de droite, activez les portées suivantes :

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

Vous devrez peut-être développer la liste ou accéder à la page suivante de la liste pour toutes les afficher.

1. Cliquez sur **[!UICONTROL Mettre à jour]**.
1. Cliquez sur **[!UICONTROL Enregistrer et continuer]**.
1. (Facultatif) Ajoutez tous les utilisateurs de test au projet.
1. Cliquez sur **[!UICONTROL Enregistrer et continuer]**.
1. Vérifiez l’exactitude de vos informations, puis cliquez sur **[!UICONTROL Retour au tableau de bord]**.

   >[!NOTE]
   >
   >Vous n’avez pas besoin de soumettre votre écran de consentement et votre demande de vérification en [!DNL Google].

1. Passez à [Création d’informations d’identification OAuth](#create-oauth-credentials).

### Création d’informations d’identification OAuth

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Informations d’identification]**.

   >[!NOTE]
   >
   >S’il ne s’agit pas de la première API ou du premier service ([!DNL Gmail] ou [!DNL Google Drive]) que vous avez activé, il n’est pas nécessaire de créer de nouvelles informations d’identification.

1. Cliquez sur **[!UICONTROL Création d’informations d’identification]** près de la partie supérieure de l’écran, puis sélectionnez **[!UICONTROL ID client OAuth]** dans le menu déroulant.

1. Renseignez les champs requis comme suit :

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Type d’application]</td> 
      <td> <p> [!UICONTROL Application Web]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. Sous [!UICONTROL URI de redirection autorisés], cliquez sur **[!UICONTROL Ajouter un URI]** et saisissez **one** de ce qui suit :

   * Pour [!DNL Gmail] ou [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Pour les autres [!DNL Google] apps : `https://app.workfrontfusion.com/oauth/cb/google`

1. Cliquez sur **[!UICONTROL Créer]**.

   La variable [!UICONTROL ID client] et [!UICONTROL Secret du client] s’affiche.

1. Copiez le [!UICONTROL ID client] et [!UICONTROL Secret du client] vers un emplacement sécurisé. Vous les utiliserez pour établir une connexion à [!DNL Workfront Fusion].
1. Passez à [Se connecter à [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Se connecter à [!DNL Google] in [!DNL Workfront Fusion]

Processus de création d’une connexion à [!DNL Google] varie selon que vous utilisez un module à partir d’un [!DNL Google] (par exemple [!DNL Google Sheets] ou [!DNL Google Docs]), ou si vous vous connectez à [!DNL Google] via le [!UICONTROL HTTP] >[!UICONTROL Créer un OAuth2.0] module de requête.

* [Se connecter à [!DNL Google] dans [!DNL Google] service](#connect-to-google-in-a-google-service)
* [Se connecter à [!DNL Google] dans le [!UICONTROL HTTP] > [!UICONTROL Exécution d’une requête OAuth2.0] module](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Se connecter à [!DNL Google] dans [!DNL Google] service

1. Dans [!DNL Workfront Fusion], recherchez la variable [!DNL Google] pour lequel vous devez créer une connexion.
1. Cliquez sur **[!UICONTROL Création d’une connexion]**, puis cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.

1. Saisissez le [!UICONTROL ID client] et [!UICONTROL Secret du client] que vous avez récupéré dans [[!UICONTROL Création d’informations d’identification OAuth]](#create-oauth-credentials) dans les champs respectifs, puis cliquez sur **[!UICONTROL Continuer]**.

1. Connectez-vous avec votre [!DNL Google] compte .

   La variable **[!UICONTROL Cette application n’est pas vérifiée]** s’affiche. Notez que l’&quot;application&quot; mentionnée dans le titre de la fenêtre est le client OAuth que vous avez créé ci-dessus.

1. Cliquez sur **[!UICONTROL Avancé]**, puis cliquez sur **[!UICONTROL Accédez à [!DNL Workfront Fusion] (non sûr)]** pour autoriser l’accès à l’aide de votre client OAuth personnalisé.

1. Cliquez sur **[!UICONTROL Autoriser]** à accorder [!DNL Workfront Fusion] autorisation.
1. Dans la fenêtre qui s’affiche, cliquez sur **[!UICONTROL Autoriser]** pour confirmer vos choix.

   La connexion à la [!DNL Google] Le service utilisant un client OAuth personnalisé est établi.

#### Se connecter à [!DNL Google] dans le [!UICONTROL HTTP] > [!UICONTROL Exécution d’une requête OAuth2.0] module {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Pour obtenir des instructions sur la connexion à [!DNL Google] dans le [!UICONTROL HTTP] > [!UICONTROL Exécution d’une requête OAuth2.0] module, voir [Instructions pour créer une connexion à [!DNL Google] dans le [!UICONTROL HTTP] > [!UICONTROL Exécution d’une requête OAuth 2.0] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) in [[!UICONTROL HTTP] > [!UICONTROL Exécution d’une requête OAuth 2.0] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Message d’erreur possible :[!UICONTROL [403] Accès non configuré]

Si la variable [!UICONTROL `403 Access Not Configured`] message d’erreur s’affiche. Vous devez activer l’API correspondante dans votre plateforme cloud Google. Pour activer l’API, suivez les étapes de la section [Créez un projet sur [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) dans cet article.
