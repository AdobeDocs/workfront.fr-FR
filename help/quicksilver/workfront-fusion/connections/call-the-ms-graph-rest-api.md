---
title: Appelez l’API REST MS Graph via le module de requête  [!DNL Adobe Workfront Fusion] HTTP &gt; Make an OAuth 2.0
description: Appelez l’API REST MS Graph via le module de requête  [!DNL Adobe Workfront Fusion] HTTP &gt; Make an OAuth 2.0
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 12%

---

# Appelez l’[!UICONTROL  API REST MS Graph] via le module [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]

<!-- Audited: 3/2024-->

De nombreux services Web [!DNL Microsoft] sont accessibles par le biais de [!DNL Microsoft Graph API]. Vous pouvez créer une connexion à [!DNL Microsoft Graph API] à l’aide du module [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Créer une requête OAuth 2.0] .

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

## Enregistrez [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]

Pour créer une connexion à [!DNL Microsoft Graph REST API], vous devez d&#39;abord enregistrer [!DNL Adobe Workfront Fusion].

1. Commencez à enregistrer une nouvelle application comme décrit dans [Enregistrement de votre application](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) dans la documentation [!DNL Microsoft].

   Dans le cadre de l&#39;enregistrement, [!DNL Microsoft] nécessite les informations suivantes :

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nom de l’application]</td>
        <td>Saisissez un nom pour l’application, par exemple "Mon application [!DNL Workfront Fusion]".</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Une fois l’enregistrement de l’application terminé, prenez note de l’[!UICONTROL ID de l’application].

   >[!IMPORTANT]
   >
   >Vous aurez besoin de l’ID d’application pour configurer votre connexion dans [!DNL Workfront Fusion].

1. Générez un [!UICONTROL secret d’application]. Prends note de ce secret.

   Pour obtenir des instructions, voir [Enregistrement de votre application](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) dans la documentation [!DNL Microsoft].

   >[!IMPORTANT]
   >
   >Vous aurez besoin du [!UICONTROL secret d&#39;application] pour configurer votre connexion dans [!DNL Workfront Fusion].

1. Configurez les autorisations de votre application.

   Pour plus d&#39;informations sur la localisation et la configuration de ces champs, consultez la section &quot;Configurer les autorisations pour Microsoft Graph&quot; dans [Obtenir l&#39;accès sans utilisateur](https://docs.microsoft.com/en-us/graph/auth-v2-service) dans la documentation [!UICONTROL Microsoft].

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Quel type d’autorisations votre application requiert-elle ?]</td> 
      <td>Sélectionnez <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Sélectionner les autorisations]</td> 
      <td> <p>Sélectionnez les autorisations suivantes :</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Toutes les autres autorisations requises par vos intégrations (exemple : <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Important</b> : vous aurez besoin des autorisations sélectionnées pour configurer votre connexion dans [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passez à [Configuration de votre [!DNL MS Graph API] connexion dans [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configurer votre connexion [!DNL MS Graph API] dans [!DNL Workfront Fusion]

Après avoir enregistré [!DNL Workfront Fusion] comme décrit dans [Register [!DNL Workfront Fusion] dans le  [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), vous pouvez configurer votre connexion dans le module de requête [!UICONTROL HTTP] > [!UICONTROL Make an Oauth 2.0] .

1. Ajoutez un module [!UICONTROL HTTP] > [!UICONTROL Lancer un appel OAuth 2.0] à votre scénario.
1. Cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL connexion] .
1. Configurez les champs de connexion comme suit :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td>Saisissez le nom de la connexion.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Type de flux]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autoriser l’URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Saisissez les autorisations que vous avez sélectionnées à l’étape 4 de <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Pour chaque portée, cliquez sur <b>[!UICONTROL Ajouter]</b> et saisissez l’autorisation.</p> <p>Exemple : <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Séparateur de portée]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Saisissez l’[!UICONTROL ID d’application] de l’étape 2 dans <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Saisissez le [!UICONTROL Clé secrète] que vous avez généré à l’étape 3 dans <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autoriser les paramètres]</td> 
      <td> <p>Ajoutez les paramètres d’autorisation suivants :</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Value]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key] : <code>prompt </code>[!UICONTROL Value] : <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Paramètres du jeton d’accès]</td> 
      <td>Vous n’avez rien à saisir dans ce champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Paramètres du jeton d’actualisation]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Cliquez sur <b>[!UICONTROL Ajouter]</b>.</p> </li> 
        <li value="2"> <p>Dans le champ <b>[!UICONTROL Key]</b>, saisissez <code>scope</code>.</p> </li> 
        <li value="3"> <p>Dans le champ <b>[!UICONTROL Valeur]</b>, saisissez toutes les [!UICONTROL Portée] que vous avez entrées dans le champ Portée, séparées par des espaces.</p> <p>Exemple : <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL En-têtes personnalisés]</td> 
      <td>Vous n’avez rien à saisir dans ce champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre qui s’affiche, cliquez sur **[!UICONTROL Accepter]** pour terminer la connexion et revenir au module.
