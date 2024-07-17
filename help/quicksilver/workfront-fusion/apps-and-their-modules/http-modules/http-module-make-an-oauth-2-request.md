---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: http-modules
title: HTTP &gt; Make an OAuth 2.0 request module
description: Pour envoyer une requête  [!DNL Adobe Workfront Fusion] HTTP(S) aux serveurs nécessitant une autorisation OAuth 2.0, vous devez d’abord créer une connexion OAuth. [!DNL Adobe Workfront Fusion] s’assure que tous les appels effectués avec cette connexion comportent les en-têtes d’autorisation appropriés et actualisent automatiquement les jetons associés si nécessaire.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '2236'
ht-degree: 10%

---

# [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une licence [!DNL Adobe Workfront].

Pour envoyer une requête HTTP(S) [!DNL Adobe Workfront Fusion] aux serveurs nécessitant une autorisation OAuth 2.0, vous devez d’abord créer une connexion OAuth. [!DNL Adobe Workfront Fusion] s’assure que tous les appels effectués avec cette connexion comportent les en-têtes d’autorisation appropriés et actualisent automatiquement les jetons associés si nécessaire.

[!DNL Workfront Fusion] prend en charge les flux d’authentification OAuth 2.0 suivants :

* Flux de code d’autorisation
* Flux implicite

D’autres flux, tels que Flux d’informations d’identification de mot de passe du propriétaire des ressources et Flux d’informations d’identification du client, ne sont pas automatiquement pris en charge par ce module.

Pour plus d’informations sur l’authentification OAuth 2.0, voir [The OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749).

>[!NOTE]
>
>Si vous vous connectez à un produit Adobe qui ne possède pas encore de connecteur dédié, il est recommandé d&#39;utiliser le module Adobe Authenticator.
>
>Pour plus d’informations, voir [Module Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Création d&#39;une connexion pour une requête [!DNL OAuth]

* [Instructions générales pour créer une connexion dans le module de requête HTTP > Make an OAuth 2.0](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [Instructions pour créer une connexion à Google dans le module de requête HTTP >[!UICONTROL Make] an OAuth 2.0](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [Instructions pour la connexion à l’API Microsoft Graph via HTTP > Make an OAuth 2.0 request module](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### Instructions générales pour la création d’une connexion dans le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]

1. Créez un client OAuth dans le service [!DNL target] avec lequel vous souhaitez que [!DNL Adobe Workfront Fusion] communique. Cette option se trouve probablement dans la section [!UICONTROL Développeur] du service donné.

   1. Lors de la création d’un client, saisissez l’URL appropriée dans le champ `[!UICONTROL Redirect URL]` ou `[!UICONTROL Callback URL]` :

      | Amériques/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. Une fois le client créé, le service donné affiche 2 clés : `[!UICONTROL Client ID]` et `[!UICONTROL Client Secret]`. Certains services appellent ces `[!UICONTROL App Key]` et `[!UICONTROL App Secret]` . Enregistrez la clé et le secret dans un emplacement sécurisé afin de pouvoir les fournir lors de la création de la connexion dans Workfront Fusion.

1. Recherchez les `[!UICONTROL Authorize URI]` et `[!UICONTROL Token URI]` dans la documentation API du service donné. Il s’agit d’adresses URL par lesquelles [!DNL Workfront Fusion] communique avec le service [!DNL target]. Les adresses servent à l’autorisation OAuth.

   >[!NOTE]
   >
   >Si le service utilise le flux Implicit, vous n’aurez besoin que de `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**Exemple :** Adresses Yahoo :
   >
   >* Authorize URI :
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* URI du jeton :
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (Conditionnel) Si le service cible utilise des portées (droits d’accès), vérifiez comment le service sépare les portées individuelles et assurez-vous de définir le séparateur dans les paramètres avancés en conséquence. Si le séparateur n’est pas défini correctement, [!DNL Workfront Fusion] ne parvient pas à créer la connexion et vous recevez une erreur de plage non valide.
1. Après avoir suivi les étapes ci-dessus, vous pouvez commencer à créer la connexion OAuth dans [!DNL Workfront Fusion]. Ajoutez le module de traitement des requêtes et réponses HTTP(S) OAuth 2.0 à votre scénario.
1. Dans le champ Connexion du module, cliquez sur **[!UICONTROL Ajouter]**.

1. Renseignez les champs suivants pour créer une connexion :

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>Saisissez le nom de la connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Type de flux]</p> </td> 
      <td> <p>Sélectionnez le flux permettant d’obtenir les jetons.</p> 
       <ul> 
        <li><strong>[!UICONTROL Authorization Code]</strong> : saisissez les <code>[!UICONTROL Authorize URI]</code> et <code>[!UICONTROL Token URI]</code> de la documentation de l’API du service.</li> 
        <li><strong>[!UICONTROL Implicit]</strong> : saisissez le <code>[!UICONTROL Authorize URI]</code> de la documentation de l’API du service.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>Ajoutez des portées individuelles. Vous trouverez ces informations dans la documentation destinée aux développeurs (API) du service donné.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Séparateur de portée] </td> 
      <td> <p>Sélectionnez les portées saisies ci-dessus à séparer. Vous trouverez ces informations dans la documentation destinée aux développeurs (API) du service donné.</p> <p>Avertissement : si le séparateur n’est pas défini correctement, [!DNL Workfront Fusion] ne parvient pas à créer la connexion et vous recevez une erreur de plage non valide.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>Saisissez l’ID client. Vous avez obtenu l’identifiant du client lorsque vous avez créé un client OAuth dans le service que vous souhaitez connecter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p> Saisissez le secret client. Vous avez obtenu le secret client lorsque vous avez créé un client OAuth dans le service que vous souhaitez connecter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autoriser les paramètres]</p> </td> 
      <td> <p>Ajoutez tous les paramètres que vous souhaitez inclure dans l’appel d’autorisation. Les paramètres standard suivants sont toujours automatiquement inclus et ne doivent pas être ajoutés.</p> <p>Paramètres standard :</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code> pour [!UICONTROL Flux de code d’autorisation] et <code>token </code> pour [!UICONTROL Flux implicite]</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Amériques/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> Identifiant client que vous avez reçu lors de la création du compte</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Paramètres du jeton d’accès]</p> </td> 
      <td> <p>Ajoutez les paramètres que vous souhaitez inclure dans l’appel de jeton. Les paramètres standard suivants sont toujours automatiquement inclus et ne doivent pas être ajoutés.</p> <p>Paramètres standard :</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong> : <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">Amériques/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong> : l’ID client que vous avez reçu lors de la création du compte est automatiquement inclus dans le corps de la requête.</li> 
        <li><strong>client_secret</strong> : le secret client que vous avez reçu lors de la création du compte est automatiquement inclus dans le corps de la requête.</li> 
        <li><strong>code</strong> : code renvoyé par la demande d’autorisation</li> 
       </ul> <p>Remarque :  <p>La norme OAuth 2.0 prend en charge au moins 2 méthodes d’authentification du client au cours de cette étape (<code>[!UICONTROL client_secret_basic]</code> et <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] envoie automatiquement l’ID client spécifié et le secret par le biais de la méthode <code>[!UICONTROL client_secret_post]</code>. Par conséquent, ces paramètres sont inclus automatiquement dans le corps de la requête de jeton. </p> <p>Pour plus d’informations sur l’authentification OAuth 2.0, voir <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Paramètres du jeton d’actualisation]</p> </td> 
      <td> <p>Ajoutez les paramètres que vous souhaitez inclure dans l’appel de jeton. Les paramètres standard suivants sont toujours automatiquement inclus et ne doivent pas être ajoutés.</p> <p>Paramètres standard :</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong> : <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong> : jeton d’actualisation le plus récent obtenu par le service auquel vous vous connectez.</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> : l’ID client que vous avez reçu lors de la création du compte est automatiquement inclus dans le corps de la requête.</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong> : le secret client que vous avez reçu lors de la création du compte est automatiquement inclus dans le corps de la requête</p> </li> 
       </ul> <p>Remarque :  <p>La norme OAuth 2.0 prend en charge au moins 2 méthodes d’authentification du client au cours de cette étape (<code>[!UICONTROL client_secret_basic]</code> et <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] envoie automatiquement l’ID client spécifié et le secret par le biais de la méthode <code>[!UICONTROL client_secret_post]</code>. Par conséquent, ces paramètres sont inclus automatiquement dans le corps de la requête de jeton. </p> <p>Pour plus d’informations sur l’authentification OAuth 2.0, voir <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL En-têtes personnalisés]</p> </td> 
      <td> <p>Indiquez les clés et valeurs supplémentaires à inclure dans l’en-tête des étapes [!UICONTROL Token] et R[!UICONTROL Actualiser le jeton] .</p> <p>Remarque :  <p>La norme OAuth 2.0 prend en charge au moins 2 méthodes d’authentification du client au cours de cette étape (<code>[!UICONTROL client_secret_basic]</code> et <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] ne prend pas automatiquement en charge la méthode <code>[!UICONTROL client_secret_basic]</code>. Si le service que vous vous connectez à suppose que l’identifiant du client et le secret du client soient combinés en une seule chaîne, puis codés en base64 dans l’en-tête Authorization, vous devez ajouter cet en-tête et cette valeur key ici.</p> <p> Pour plus d’informations sur l’authentification OAuth 2.0, voir <a href="https://tools.ietf.org/html/rfc6749">The OAuth 2.0 Authorization Framework</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Token placement]</p> </td> 
      <td> <p>Choisissez d’envoyer le jeton dans l’[!UICONTROL en-tête], la [!UICONTROL chaîne de requête] ou dans les deux lors de la connexion à l’URL spécifiée.</p> <p>Les jetons sont le plus souvent envoyés dans l’en-tête de la requête.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom du jeton d’en-tête] </td> 
      <td> <p>Saisissez le nom du jeton d’autorisation dans l’en-tête . Valeur par défaut : <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom du paramètre de chaîne de requête] </td> 
      <td> <p>Saisissez le nom du jeton d’autorisation dans la chaîne de requête. Valeur par défaut : <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer les paramètres de connexion.
1. Passez à la [configuration du module de requête OAuth 2.0](#oauth-20-request-module-setup).

### Instructions de création d’une connexion à [!DNL Google] dans le [!UICONTROL HTTP] >[!UICONTROL Créer un module de requête OAuth 2.0]

L’exemple suivant montre comment utiliser le module de requête [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0] pour se connecter à [!DNL Google].

1. Assurez-vous d’avoir créé un projet, configuré les paramètres OAuth et généré vos informations d’identification comme décrit dans [Se connecter [!DNL Adobe Workfront Fusion] à [!DNL Google Services] à l’aide d’un client OAuth personnalisé](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. Ouvrez le module [!UICONTROL HTTP] >[!UICONTROL Créer une requête OAuth 2.0] .
1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone de connexion.
1. Saisissez les valeurs suivantes :

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>Saisissez le nom de la connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Type de flux]</p> </td> 
      <td> <p>[!UICONTROL Authorization Code]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autoriser l’URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>Ajoutez des portées individuelles. Pour plus d’informations sur les portées, voir <a href="https://developers.google.com/identity/protocols/oauth2/scopes">Portées OAuth 2.O pour les [!DNL Google] APIs</a> dans la documentation [!DNL Google].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Séparateur de portée] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>Saisissez votre ID client [!DNL Google]. </p> <p>Pour créer un ID client, voir <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Création des informations d’identification OAuth</a> dans <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] vers [!DNL Google Services] à l’aide d’un client OAuth personnalisé</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>Saisissez votre secret client [!DNL Google]. </p> <p>Pour créer un secret client, voir <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Création des informations d’identification OAuth</a> dans <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] vers [!DNL Google] Services à l’aide d’un client OAuth personnalisé</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autoriser les paramètres]</p> </td> 
      <td> <p>Ajoutez <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>paire clé-valeur.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>Remarque : Si vous rencontrez des problèmes d’authentification, par exemple avec l’actualisation des jetons, essayez d’ajouter la paire <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>clé-valeur.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer les paramètres de connexion.
1. Passez à la [configuration du module de requête OAuth 2.0](#oauth-20-request-module-setup).

### Instructions pour se connecter à [!DNL Microsoft Graph API] via le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]

Pour obtenir des instructions sur [!DNL Microsoft Graph API], voir [Appel de  [!DNL MS Graph REST API]  via le  [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Lancer une requête OAuth 2.0] module](../../../workfront-fusion/connections/call-the-ms-graph-rest-api.md).

## Configuration du module de requête OAuth 2.0

Lorsque vous avez établi une connexion [!DNL Oauth 2].0 comme décrit dans [Création d’une connexion pour une  [!DNL OAuth] requête](#creating-a-connection-for-an-oauth-request), continuez à configurer le module suivant vos besoins. Tous les jetons d’autorisation sont automatiquement inclus dans cette requête, ainsi que dans toute autre requête qui utilise la même connexion.

Lorsque vous configurez le module [!UICONTROL HTTP] >[!UICONTROL Make an OAuth 2.0 request] , [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la configuration d’une connexion, voir <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">Création d’une connexion pour une requête OAuth</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Évaluer tous les états comme des erreurs (sauf 2xx et 3xx]) </td> 
   <td> <p>Utilisez cette option pour configurer la gestion des erreurs.</p> <p>Pour plus d’informations, voir <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Gestion des erreurs dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Saisissez l’URL à laquelle vous souhaitez envoyer une requête, par exemple un point de terminaison API, un site web, etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Entrez les paires clé-valeur de requête souhaitées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type de corps]</p> </td> 
   <td> <p>Le corps HTTP est l’octet de données transmis dans un message de transaction HTTP immédiatement après les en-têtes s’il y a un élément à utiliser.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Le type de corps brut est généralement adapté à la plupart des requêtes de corps HTTP, même dans les cas où la documentation du développeur ne spécifie aucune donnée à envoyer.</p> <p>Spécifiez un formulaire d’analyse des données dans le champ [!UICONTROL Type de contenu] .</p> <p>Malgré le type de contenu sélectionné, les données sont entrées dans n’importe quel format requis ou indiqué par la documentation du développeur.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]{1</strong> </p> <p>Ce type de corps est destiné aux données de POST utilisant <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>Pour <code>[!UICONTROL application/x-www-form-urlencoded]</code>, le corps du message HTTP envoyé au serveur est essentiellement une chaîne de requête. Les clés et les valeurs sont codées en paires clé-valeur séparées par <code>&amp;</code> et avec une <code>=</code> entre la clé et la valeur. </p> <p>Pour les données binaires, <code>use [!UICONTROL multipart/form-data]</code> à la place.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Exemple : </b></span></span> 
       <p>Exemple du format de requête HTTP obtenu :</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] est une requête HTTP multipart utilisée pour envoyer des fichiers et des données. Il est généralement utilisé pour charger des fichiers sur le serveur.</p> <p>Ajoutez les champs à envoyer dans la requête. Chaque champ doit contenir une paire clé-valeur.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Texte]</strong> </p> <p>Saisissez la clé et la valeur à envoyer dans le corps de la requête.</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Saisissez la clé et indiquez le fichier source à envoyer dans le corps de la requête.</p> <p>Mappez le fichier que vous souhaitez charger à partir du module précédent (par exemple [!UICONTROL HTTP] &gt;[!UICONTROL Obtenir un fichier] ou [!UICONTROL Google Drive] &gt;[!UICONTROL Télécharger un fichier]), ou saisissez manuellement le nom du fichier et les données du fichier.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Réponse d’analyse]</p> </td> 
   <td> <p>Activez cette option pour analyser automatiquement les réponses et convertir les réponses JSON et XML afin que vous n’ayez pas à utiliser les modules [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] ou [!UICONTROL XML] &gt; [!UICONTROL Parse XML].</p> <p>Avant de pouvoir utiliser du contenu JSON ou XML analysé, exécutez le module une fois manuellement afin que le module puisse reconnaître le contenu de la réponse et vous permettre de le mapper dans les modules suivants.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>Saisissez le délai d’attente de la requête en secondes (1 à 300). La valeur par défaut est de 40 secondes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partage de cookies avec d’autres modules HTTP]</td> 
   <td> <p> Activez cette option pour partager les cookies du serveur avec tous les modules HTTP de votre scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificat auto-signé]</td> 
   <td> <p> Téléchargez votre certificat si vous souhaitez utiliser TLS à l’aide de votre certificat auto-signé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rejeter les connexions qui utilisent des certificats non vérifiés (auto-signés)] </td> 
   <td> <p>Activez cette option pour rejeter les connexions qui utilisent des certificats TLS non vérifiés.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suivre la redirection]</td> 
   <td> <p> Activez cette option pour suivre les redirections d’URL avec les réponses 3xx.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suivre toutes les redirections] </td> 
   <td> <p>Activez cette option pour suivre les redirections d’URL avec tous les codes de réponse.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Désactivation de la sérialisation de plusieurs mêmes clés de chaîne de requête en tant que tableaux]</p> </td> 
   <td> <p>Par défaut, [!DNL Workfront Fusion] gère plusieurs valeurs pour la même clé de paramètre de chaîne de requête d’URL que les tableaux. Par exemple, <code>www.test.com?foo=bar&amp;foo=baz</code> sera converti en <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Activez cette option pour désactiver cette fonction. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Demander du contenu compressé]</td> 
   <td> <p> Activez cette option pour demander une version compressée du site web.</p> <p>Cela ajoute un en-tête <code>[!UICONTROL Accept-Encoding]</code> pour demander du contenu compressé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Utiliser TLS Mutuel]</td> 
   <td> <p>Activez cette option pour utiliser le protocole TLS mutuel dans la requête HTTP.</p> <p>Pour plus d’informations sur Mutual TLS, voir <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Utilisation de Mutual TLS dans les modules HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
