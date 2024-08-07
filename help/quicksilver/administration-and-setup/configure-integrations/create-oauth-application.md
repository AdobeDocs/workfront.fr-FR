---
title: Créer des applications OAuth2 pour les intégrations  [!DNL Workfront]
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: En tant qu’administrateur  [!DNL Adobe Workfront] , vous pouvez créer des applications OAuth2 pour votre instance de [!DNL Workfront], ce qui permet à d’autres applications d’accéder à Workfront. Vos utilisateurs peuvent alors autoriser ces autres applications à accéder à leurs données Workfront. Ainsi, vous pouvez intégrer Workfront aux applications de votre choix, y compris vos propres applications internes.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 9%

---

# Créer des applications OAuth2 pour les intégrations [!DNL Workfront]

En tant qu&#39;administrateur [!DNL Adobe Workfront], vous pouvez créer des applications OAuth2 pour votre instance de [!DNL Workfront], qui permettent à d&#39;autres applications d&#39;accéder à [!DNL Workfront]. Vos utilisateurs peuvent alors autoriser ces autres applications à accéder à leurs données [!DNL Workfront]. Ainsi, vous pouvez intégrer   avec les applications de votre choix, y compris vos propres applications internes.

Lorsque vous créez une application [!UICONTROL OAuth2], vous générez un identifiant client et un secret client. Vos utilisateurs peuvent ensuite utiliser l’ID client dans les appels API pour s’intégrer à l’application que vous avez créée.

>[!NOTE]
>
>Dans le contexte d’OAuth2, &quot;création d’une application&quot; fait référence au processus de création de ce type de lien d’accès entre une application et un serveur tel que [!DNL Workfront].

* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur (flux de code d’autorisation), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 à l’aide de l’authentification du serveur (flux JWT), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 à l’aide de PKCE, voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide de PKCE flow](../../wf-api/api/oauth-app-pkce-flow.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuel :[!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> Vous devez être un administrateur ou une administratrice de [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

+++

## Présentation d’OAuth2

Imaginez qu’une application doit extraire certaines informations spécifiques de [!DNL Workfront]. Une application qui demande des informations est appelée client. Dans cet exemple, le nom du client est ClientApp. ClientApp doit accéder aux informations d’un utilisateur particulier et doit donc accéder à [!DNL Workfront] en tant qu’utilisateur. Si votre utilisateur donne à ClientApp son nom d’utilisateur et son mot de passe, il peut accéder à toutes les données auxquelles il peut accéder. Il s’agit d’un risque de sécurité, car ClientApp n’a besoin que d’un petit ensemble d’informations spécifiques.

Lorsque vous créez une application OAuth2 pour ClientApp, vous indiquez essentiellement à [!DNL Workfront] que ClientApp est autorisé à accéder à [!DNL Workfront], mais seulement si l’utilisateur dont le compte Accès à ClientApp donne l’autorisation d’accès.

## Créer une application OAuth2

Lors de la création d’une application OAuth2, choisissez le type d’application qui répond le mieux aux besoins de votre intégration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d’application</th> 
   <th>Meilleur pour</th> 
   <th>Méthode d’authentification</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Application machine-machine</p> </td> 
   <td> <p>Solution recommandée pour les interfaces de ligne de commande, les démons ou les scripts exécutés sur votre serveur</p> <p>Exemples :</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Authentification via le jeton web JSON avec codage de paire de clés publique/privée.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Application web monopage</p> </td> 
   <td> <p>Le meilleur pour les applications web mobiles ou mono-page</p> <p>Exemples :</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>Authentification via le flux de code d’autorisation OAuth 2.0 avec PKCE (Proof Key for Code Exchange).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Application web</p> </td> 
   <td> <p>Solution recommandée pour les applications côté serveur qui gèrent les informations d’identification et les jetons sur le serveur</p> <p>Exemples :</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>Authentification via le flux de code d’autorisation OAuth 2.0.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.

* [Créer une application OAuth2 à l’aide de l’authentification du serveur (flux JWT)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Création d’une application OAuth2 à l’aide des informations d’identification de l’utilisateur (flux de code d’autorisation)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Créer une application web OAuth2 mono-page à l’aide de PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Créer une application OAuth2 à l’aide de l’authentification du serveur (flux JWT) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL System]**, puis sélectionnez **[!UICONTROL OAuth2 Applications]**.
1. Cliquez sur **[!UICONTROL Créer une intégration d’application]**.
La zone **Nouvelle application OAuth2** s’affiche.
1. Dans la zone **Nouvelle application OAuth2**, sélectionnez **[!UICONTROL Machine to Machine Application]**.
1. Saisissez un nom pour la nouvelle application, par exemple &quot;[!DNL Workfront] pour ClientApp&quot;.
1. Cliquez sur **[!UICONTROL Créer]**.
1. Renseignez les champs de la nouvelle application.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Ce champ est généré automatiquement.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Ce champ est généré automatiquement</p> <p><b>IMPORTANT</b> :  <p>Copiez le contenu de ce champ dans un autre fichier sécurisé avant de fermer cette page. Vous ne pourrez plus voir cette clé secrète.</p> <p>Si vous perdez cette clé, supprimez-la et créez un secret client.</p> 
        <ol> 
         <li value="1"> <p>Cliquez sur l’icône <b>[!UICONTROL Supprimer]</b> <img src="assets/delete.png"> pour supprimer le secret client actuel.</p> </li> 
         <li value="2"> <p>Cliquez sur <b>[!UICONTROL Ajouter le secret client]</b> pour générer un nouveau secret client.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>Les applications serveur à serveur utilisent des clés publiques et privées pour l’authentification. Utilisez l’une des méthodes suivantes :</p> 
       <ul> 
        <li> <p>Cliquez sur <b>[!UICONTROL Ajouter une clé publique]</b> et saisissez la clé publique de l’autre application.</p> </li> 
        <li> <p>Cliquez sur <b>[!UICONTROL Générer une paire de clés publique/privée]</b>, puis partagez la clé publique avec l’autre application.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>C'est le même nom que celui que vous avez donné à l'application. Ce champ ne peut pas être vide.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour l’intégration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur (flux de code d’autorisation), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).

### Création d’une application OAuth2 à l’aide des informations d’identification de l’utilisateur (flux de code d’autorisation) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL System]**, puis sélectionnez **[!UICONTROL OAuth2 Applications]**.
1. Cliquez sur **[!UICONTROL Créer une intégration d’application]**.

   **Nouvelle application OAuth2** s’affiche.
1. Dans la zone **Nouvelle application OAuth2**, sélectionnez **[!UICONTROL Application Web]**.
1. Saisissez un nom pour la nouvelle application OAuth2, par exemple &quot;[!DNL Workfront] pour ClientApp&quot;.
1. Cliquez sur **[!UICONTROL Créer]**.
1. Renseignez les champs de la nouvelle application.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Ce champ est généré automatiquement.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Ce champ est généré automatiquement</p> <p><b>IMPORTANT</b> :  <p>Copiez le contenu de ce champ dans un autre fichier sécurisé avant de fermer cette page. Vous ne pourrez plus voir cette clé secrète.</p> <p>Si vous perdez cette clé, supprimez-la et créez un secret client.</p> 
        <ol> 
         <li value="1"> <p>Cliquez sur l’icône <b>[!UICONTROL Supprimer]</b> <img src="assets/delete.png"> pour supprimer le secret client actuel.</p> </li> 
         <li value="2"> <p>Cliquez sur <b>[!UICONTROL Ajouter le secret client]</b> pour générer un nouveau secret client.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de redirection]</td> 
      <td>Les utilisateurs seront redirigés vers ce chemin après s’être authentifiés avec [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Actualiser la rotation du jeton]</td> 
      <td>Activez cette option pour émettre un nouveau jeton d’actualisation lorsque le jeton d’actualisation est utilisé. Votre application doit stocker le nouveau jeton après chaque actualisation.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Expiration absolue du jeton d’actualisation]</td> 
      <td> <p>Sélectionnez la durée pendant laquelle vous souhaitez qu’un jeton d’actualisation existe avant son expiration. À son expiration, vos utilisateurs doivent à nouveau se connecter à l’intégration. Sélectionnez "[!UICONTROL No expiration]" si vous ne souhaitez pas que le jeton d’actualisation expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Expiration du jeton d’actualisation d’inactivité</td> 
      <td> <p>Sélectionnez la durée au bout de laquelle, si l’utilisateur n’a pas été actif dans votre système, son jeton d’actualisation expire. </p> <p>Par exemple, si l’expiration du jeton d’actualisation d’inactivité est de 6 mois et que l’utilisateur ne se connecte pas pendant six mois, le jeton d’actualisation expire même si l’expiration du jeton d’actualisation absolu peut être définie pour plus longtemps.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Vous pouvez ajouter un logo pour rendre cette application plus identifiable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>C'est le même nom que celui que vous avez donné à l'application. Ce champ ne peut pas être vide.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour l’intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de description de l’application]</td> 
      <td>Il peut s’agir d’un lien vers une page "À propos de nous" ou d’une page contenant plus d’informations sur l’intégration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur (flux de code d’autorisation), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).

### Créer une application web OAuth2 mono-page à l’aide de PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL System]**, puis sélectionnez **[!UICONTROL OAuth2 Applications]**.
1. Cliquez sur **[!UICONTROL Créer une intégration d’application]**.

   La zone **Nouvelle application OAuth2** s’affiche.
1. Dans la zone **Nouvelle application OAuth2**, sélectionnez **[!UICONTROL Application Web Mono-Page]**.
1. Saisissez un nom pour la nouvelle application [!UICONTROL OAuth2], par exemple &quot;[!DNL Workfront] pour ClientApp&quot;.
1. Cliquez sur **[!UICONTROL Créer]**.
1. Renseignez les champs de la nouvelle application.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Ce champ est généré automatiquement.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de redirection]</td> 
      <td>Les utilisateurs seront redirigés vers ce chemin après s’être authentifiés auprès de Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Rotation du jeton d’actualisation à chaque utilisation]</td> 
      <td>Activez cette option pour émettre un nouveau jeton d’actualisation lorsque le jeton d’actualisation est utilisé. Votre application doit stocker le nouveau jeton après chaque actualisation.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Expiration absolue]</td> 
      <td> <p>Sélectionnez la durée d’existence d’un jeton d’actualisation avant son expiration. À son expiration, vos utilisateurs doivent à nouveau se connecter à l’intégration. Sélectionnez "[!UICONTROL No expiration]" si vous ne souhaitez pas que le jeton d’actualisation expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Délai d’expiration de l’inactivité]</td> 
      <td> <p>Sélectionnez la durée au bout de laquelle, si l’utilisateur n’a pas été actif dans votre système, son jeton d’actualisation expire. </p> <p>Par exemple, si l’expiration du jeton d’actualisation d’inactivité est de 6 mois et que l’utilisateur ne se connecte pas pendant six mois, le jeton d’actualisation expire même si l’expiration du jeton d’actualisation absolu peut être définie pour plus longtemps.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Vous pouvez ajouter un logo pour rendre cette application plus identifiable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>C'est le même nom que celui que vous avez donné à l'application. Ce champ ne peut pas être vide.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour l’intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom du développeur]</td> 
      <td>Il s’agit du nom du développeur qui configure l’application OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Adresse électronique du développeur]</td> 
      <td>Il s’agit de l’adresse électronique du développeur qui configure l’application OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL URL de la politique de confidentialité]</td> 
      <td>Il s’agit du lien vers lequel votre entreprise stocke la politique de confidentialité.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Configuration et utilisation de l’application OAuth2 créée

La configuration et l’utilisation ultérieures de l’application OAuth2 créée nécessitent quelques connaissances techniques, y compris les appels d’API.

* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur (flux de code d’autorisation), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 à l’aide de l’authentification du serveur (flux JWT), voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 à l’aide de PKCE, voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide de PKCE flow](../../wf-api/api/oauth-app-pkce-flow.md).

## Processus OAuth2 pour le flux de code d’autorisation

>[!NOTE]
>
>Vos utilisateurs accèdent à l’application [!UICONTROL OAuth2] via l’API. Cette section décrit les fonctionnalités en termes généraux et est fournie à titre d’information uniquement.
>
>Pour obtenir des instructions spécifiques sur l’utilisation de l’application OAuth2, y compris des appels d’API spécifiques, voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorisation avec un code d’autorisation et un jeton d’accès {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp a besoin de certaines informations de [!DNL Workfront], de sorte qu’il envoie une requête au point de terminaison [!DNL Workfront] de l’API `/authorize`. La requête inclut le [!UICONTROL response_type] `code`, ce qui indique que la requête doit renvoyer un code d’autorisation.
1. Cela déclenche [!DNL Workfront] pour envoyer une invite d’authentification à l’utilisateur. L’utilisateur peut saisir ses informations d’identification dans l’invite, qui autorise [!DNL Workfront] à communiquer avec ClientApp. Si l’utilisateur est déjà connecté à [!DNL Workfront], cette étape peut être ignorée.
1. L’API [!DNL Workfront] envoie un code d’autorisation à ClientApp.
1. ClientApp envoie les informations suivantes dans une requête à l’ [!DNL Workfront] API `/token`   endpoint :

   * Code d’autorisation envoyé à ClientApp à l’étape 3. Cela identifie l’instance spécifique de l’autorisation utilisateur.
   * Secret client généré lors de la configuration de l’application OAuth2 ClientApp dans [!DNL Workfront]. Cela permet à [!DNL Workfront] de savoir que la demande provient de ClientApp.

1. Si le code d’autorisation et le secret client sont corrects, [!DNL Workfront] envoie un jeton d’accès à ClientApp. Ce jeton d’accès est envoyé directement de [!DNL Workfront] à ClientApp et ne peut pas être affiché, copié ou utilisé par un autre utilisateur ou une autre application cliente.
1. ClientApp envoie le jeton d&#39;accès à [!DNL Workfront] avec la demande d&#39;informations spécifique.
1. Comme le jeton d’accès est correct, [!DNL Workfront] envoie les informations à ClientApp.

#### Actualisation des jetons d’accès

Pour la sécurité, les jetons d’accès expirent après un court laps de temps. Pour obtenir de nouveaux jetons d’accès sans avoir à saisir d’informations d’identification à chaque fois, [!DNL OAuth2] utilise des jetons d’actualisation. Les jetons d’actualisation sont stockés par le client.

Le processus d’acquisition d’un jeton d’actualisation est identique à celui décrit dans la section [Autorisation avec un code d’autorisation et un jeton d’accès](#authorizing-with-an-authorization-code-and-access-token). La requête pour le code d’autorisation inclut la portée `offline_access`, qui indique que la requête doit renvoyer un jeton de requête avec le code d’autorisation.
