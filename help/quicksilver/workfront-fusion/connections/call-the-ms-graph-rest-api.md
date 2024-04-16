---
title: Appelez l’API REST MS Graph via le [!DNL Adobe Workfront Fusion] HTTP &gt; Créer un module de requête OAuth 2.0
description: Appelez l’API REST MS Graph via le [!DNL Adobe Workfront Fusion] HTTP &gt; Créer un module de requête OAuth 2.0
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 9%

---

# Appelez le[!UICONTROL  API REST MS Graph] via le [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Exécution d’une requête OAuth 2.0] module

<!-- Audited: 3/2024-->

Beaucoup [!DNL Microsoft] les services web sont accessibles par l’intermédiaire de la fonction [!DNL Microsoft Graph API]. Vous pouvez créer une connexion à la variable [!DNL Microsoft Graph API], en utilisant la variable [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Exécution d’une requête OAuth 2.0] module .

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

## Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]

Pour créer une connexion à la variable [!DNL Microsoft Graph REST API], vous devez d’abord vous enregistrer [!DNL Adobe Workfront Fusion].

1. Commencer à enregistrer une nouvelle application, comme décrit dans [Enregistrement de votre application](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) dans le [!DNL Microsoft] la documentation.

   Dans le cadre de l&#39;enregistrement, [!DNL Microsoft] requiert les informations suivantes :

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nom de l’application]</td>
        <td>Saisissez un nom pour l’application, par exemple "Mon [!DNL Workfront Fusion] application."</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Une fois l’enregistrement de l’application terminé, prenez note de la [!UICONTROL ID de l’application].

   >[!IMPORTANT]
   >
   >Vous aurez besoin de l’ID d’application pour configurer votre connexion dans [!DNL Workfront Fusion].

1. Générer une [!UICONTROL Secret de l’application]. Prends note de ce secret.

   Pour obtenir des instructions, voir [Enregistrement de votre application](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) dans le [!DNL Microsoft] la documentation.

   >[!IMPORTANT]
   >
   >Vous aurez besoin de la variable [!UICONTROL Secret de l’application] pour configurer votre connexion dans [!DNL Workfront Fusion].

1. Configurez les autorisations de votre application.

   Pour plus d’informations sur la localisation et la configuration de ces champs, voir la section &quot;Configurer les autorisations pour Microsoft Graph&quot; dans [Obtenir un accès sans utilisateur](https://docs.microsoft.com/en-us/graph/auth-v2-service) dans le [!UICONTROL Microsoft] la documentation.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Quel type d’autorisations votre application requiert-elle ?]</td> 
      <td>Sélectionner <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Sélectionner les autorisations]</td> 
      <td> <p>Sélectionnez les autorisations suivantes :</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Toutes les autres autorisations requises par vos intégrations (par exemple : <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Important</b>: vous aurez besoin des autorisations sélectionnées pour configurer votre connexion dans [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passez à [Configurez vos [!DNL MS Graph API] connexion dans [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configurez vos [!DNL MS Graph API] connexion dans [!DNL Workfront Fusion]

Après l’enregistrement [!DNL Workfront Fusion] comme décrit dans [Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), vous pouvez configurer votre connexion dans le [!UICONTROL HTTP] > [!UICONTROL Make an Oauth 2.0] module de requête.

1. Ajoutez un [!UICONTROL HTTP] > [!UICONTROL Effectuer un appel OAuth 2.0] à votre scénario.
1. Cliquez sur **[!UICONTROL Ajouter]** en regard de [!UICONTROL connection] champ .
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
      <td> <p>Saisissez les autorisations sélectionnées à l’étape 4 de la <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Pour chaque portée, cliquez sur <b>[!UICONTROL Ajouter]</b> et saisissez l’autorisation.</p> <p>Exemple : <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Séparateur de portée]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Saisissez l’[!UICONTROL ID de l’application] à l’étape 2 de la section <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Saisissez le [!UICONTROL Clé secrète] que vous avez généré à l’étape 3 de la section <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autoriser les paramètres]</td> 
      <td> <p>Ajoutez les paramètres d’autorisation suivants :</p> 
       <ul> 
        <li> <p>[!UICONTROL Key] :<code> response_mode</code> [!UICONTROL Value] : <code>query</code></p> </li> 
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
        <li value="2"> <p>Dans le <b>[!UICONTROL Key]</b> champ, entrer <code>scope</code>.</p> </li> 
        <li value="3"> <p>Dans le <b>[!UICONTROL Value]</b> , saisissez toutes les portées [!UICONTROL]s que vous avez saisies dans le champ de portée, séparées par des espaces.</p> <p>Exemple : <code>offline_access openid User.Read</code></p> </li> 
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
