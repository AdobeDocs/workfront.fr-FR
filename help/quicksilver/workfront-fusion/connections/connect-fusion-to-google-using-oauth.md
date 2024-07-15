---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Connectez-vous  [!DNL Adobe Workfront Fusion] à  [!DNL Google Services] à l’aide d’un client OAuth personnalisé
description: Vous pouvez utiliser  [!DNL Adobe Workfront Fusion]  pour vous connecter à  [!DNL Google Services]  à l’aide d’un client OAuth personnalisé. Cette procédure nécessite un compte  [!DNL Google] existant.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 6%

---

# Connectez [!DNL Adobe Workfront Fusion] à [!DNL Google Services] à l’aide d’un client OAuth personnalisé.

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
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Actuel : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Hérité : Tout </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Nouveau :</p> <ul><li>Formule [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront] : [!DNL Workfront Fusion] est inclus.</li></ul>
   <p>Ou</p>
   <p>Actuel : votre organisation doit acheter [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Vous avez besoin d&#39;un compte [!DNL Google] existant pour établir cette connexion.

## Connexion de Fusion aux services Google à l’aide d’un client OAuth personnalisé

Pour créer cette connexion, vous devez créer et configurer un projet sur la plateforme Google Cloud, puis configurer la connexion dans Fusion en fonction de ce projet.

* [Création d’un projet sur [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [ Configuration des paramètres [!UICONTROL OAuth consent]](#configure-oauth-consent-settings)
* [Création d’informations d’identification OAuth](#create-oauth-credentials)
* [Se connecter à [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Cette procédure est destinée à :
>
>* Utilisation personnelle ([!DNL `@gmail.com`] et [!DNL `@googlemail.com`] utilisateurs)
>* Utilisation interne ([!DNL Google Workspace] utilisateurs qui préfèrent utiliser un client OAuth personnalisé)

### Créez un projet sur [!DNL Google Cloud Platform]

Pour créer un projet sur la plateforme [!DNL Google Cloud] :

1. Connectez-vous à [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) à l’aide de vos informations d’identification [!DNL Google].
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Tableau de bord]**.
1. Cliquez sur **[!UICONTROL Créer un projet]** dans le coin supérieur droit de l’écran.
1. Saisissez le **[!UICONTROL nom du projet]**, puis cliquez sur **[!UICONTROL Créer]**.

1. Cliquez sur l’onglet **[!UICONTROL Activer les API et services]** près de la partie supérieure de l’écran.
1. Dans le champ **[!UICONTROL Rechercher des API et des services]** en haut de l’écran, saisissez le nom du service que vous souhaitez utiliser (par exemple, l’API [!DNL Gmail] ou l’API [!DNL Google Drive]).
1. Lorsqu&#39;il s&#39;affiche, cliquez sur l&#39;API ou le service auquel vous souhaitez vous connecter [!DNL Workfront Fusion].
1. Cliquez sur **[!UICONTROL Activer]** pour activer l’API sélectionnée.
1. Répétez les étapes 6 à 8 pour chaque API à activer.

   >[!NOTE]
   >
   >Vous devez activer l’API [!DNL Google Drive] ainsi que l’API de toutes les applications [!DNL Google] que vous souhaitez utiliser (comme l’API [!DNL Google Sheets]).

1. Sur l’écran qui s’affiche, cliquez sur **[!UICONTROL Créer des informations d’identification]** dans le coin supérieur droit.
1. Passez à la section [Configuration des paramètres de consentement OAuth](#configure-oauth-consent-settings) de cet article.

### Configuration des paramètres de [!UICONTROL consentement OAuth]

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Écran de consentement OAuth]**.
1. Sélectionnez **[!UICONTROL External]**, puis cliquez sur **[!UICONTROL Créer]**.

   >[!NOTE]
   >
   >Si vous sélectionnez cette option, aucun frais ne vous sera facturé. Pour plus d’informations, voir les informations de [!DNL Google] sur les exceptions aux exigences de vérification.

1. Renseignez les champs requis comme suit :

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nom de l’application]</p> </td> 
      <td> <p>Saisissez le nom de l’application qui demande le consentement.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
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
1. Vérifiez la précision de vos informations, puis cliquez sur **[!UICONTROL Retour au tableau de bord]**.

   >[!NOTE]
   >
   >Vous n&#39;avez pas besoin d&#39;envoyer votre écran de consentement et votre demande de vérification par [!DNL Google].

1. Passez à [Créer des informations d’identification OAuth](#create-oauth-credentials).

### Création d’informations d’identification OAuth

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Credentials]**.

   >[!NOTE]
   >
   >S’il ne s’agit pas de la première API ou service ([!DNL Gmail] ou [!DNL Google Drive]) que vous avez activée, vous n’avez pas à créer de nouvelles informations d’identification.

1. Cliquez sur **[!UICONTROL Créer des informations d’identification]** près du haut de l’écran, puis sélectionnez **[!UICONTROL ID client OAuth]** dans le menu déroulant.

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

1. Sous [!UICONTROL URI de redirection autorisés], cliquez sur **[!UICONTROL Ajouter un URI]** et saisissez **un** parmi les éléments suivants :

   * Pour [!DNL Gmail] ou [!DNL Google Drive] : `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Pour les autres [!DNL Google] applications : `https://app.workfrontfusion.com/oauth/cb/google`

1. Cliquez sur **[!UICONTROL Créer]**.

   Les [!UICONTROL ID client] et [!UICONTROL Secret client] s&#39;affichent.

1. Copiez l&#39;[!UICONTROL identifiant du client] et le [!UICONTROL secret du client] vers un emplacement sécurisé. Vous les utiliserez pour établir une connexion dans [!DNL Workfront Fusion].
1. Passez à [Se connecter à [!DNL Google] dans [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Connexion à [!DNL Google] dans [!DNL Workfront Fusion]

Le processus de création d’une connexion à [!DNL Google] varie selon que vous utilisez un module à partir d’un service [!DNL Google] (tel que [!DNL Google Sheets] ou [!DNL Google Docs]) ou si vous vous connectez à [!DNL Google] via le module de requête [!UICONTROL HTTP] >[!UICONTROL Make an OAuth2.0].

* [Connectez-vous à [!DNL Google] dans un  [!DNL Google] service](#connect-to-google-in-a-google-service)
* [Connectez-vous à  [!DNL Google] dans le module [!UICONTROL HTTP] > [!UICONTROL Créer une requête OAuth2.0]](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Connexion à [!DNL Google] dans un service [!DNL Google]

1. Dans [!DNL Workfront Fusion], recherchez le module [!DNL Google] pour lequel vous devez créer une connexion.
1. Cliquez sur **[!UICONTROL Créer une connexion]**, puis sur **[!UICONTROL Afficher les paramètres avancés]**.

1. Saisissez l’ [!UICONTROL  identifiant client] et le [!UICONTROL  secret client] que vous avez récupérés dans les champs respectifs [[!UICONTROL Créer des informations d’identification OAuth]](#create-oauth-credentials) , puis cliquez sur **[!UICONTROL Continuer]**.

1. Connectez-vous avec votre compte [!DNL Google].

   La fenêtre **[!UICONTROL Cette application n&#39;est pas vérifiée]** s&#39;affiche. Notez que l’&quot;application&quot; mentionnée dans le titre de la fenêtre est le client OAuth que vous avez créé ci-dessus.

1. Cliquez sur **[!UICONTROL Avancé]**, puis sur **[!UICONTROL Accéder à [!DNL Workfront Fusion] (non sécurisé)]** pour autoriser l’accès à l’aide de votre client OAuth personnalisé.

1. Cliquez sur **[!UICONTROL Autoriser]** pour accorder l’autorisation [!DNL Workfront Fusion].
1. Dans la fenêtre qui s’affiche, cliquez de nouveau sur **[!UICONTROL Autoriser]** pour confirmer vos choix.

   La connexion au service [!DNL Google] souhaité à l’aide d’un client OAuth personnalisé est établie.

#### Connectez-vous à [!DNL Google] dans le module [!UICONTROL HTTP] > [!UICONTROL  Créer une requête OAuth2.0] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Pour obtenir des instructions sur la connexion à [!DNL Google] dans le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth2.0], voir [Instructions pour la création d’une connexion à  [!DNL Google]  dans [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) sur [[!UICONTROL HTTP] > [!UICONTROL  4}Effectuez une requête OAuth 2.0] module](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Message d’erreur possible :[!UICONTROL [403] Accès non configuré]

Si le message d’erreur [!UICONTROL `403 Access Not Configured`] s’affiche, vous devez activer l’API correspondante dans votre plateforme Google Cloud. Pour activer l’API, suivez les étapes de la section [Créer un projet sur [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) de cet article.
