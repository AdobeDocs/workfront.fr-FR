---
title: Création d’applications OAuth2 pour les intégrations  [!DNL Workfront]
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: En tant qu’administrateur ou administratrice  [!DNL Adobe Workfront] , vous pouvez créer des applications OAuth2 pour votre instance de  [!DNL Workfront], qui permet à d’autres applications d’accéder à Workfront. Vos utilisateurs et utilisatrices peuvent alors autoriser ces autres applications à accéder à leurs données Workfront. Vous pouvez ainsi intégrer Workfront aux applications de votre choix, y compris à vos propres applications internes.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 09f7e854c2df1291feb150d2169fa6ccd5cdb1d6
workflow-type: tm+mt
source-wordcount: '1981'
ht-degree: 98%

---

# Créer des applications OAuth2 pour les intégrations [!DNL Workfront]

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez créer des applications OAuth2 pour votre instance de [!DNL Workfront], qui permettent à d’autres applications d’accéder à [!DNL Workfront]. Vos utilisateurs et utilisatrices peuvent alors autoriser ces autres applications à accéder à leurs données [!DNL Workfront]. Vous pouvez ainsi intégrer les applications de votre choix, y compris vos propres applications internes.

Lorsque vous créez une application [!UICONTROL OAuth2], vous générez un ID et un secret client. Vos utilisateurs et utilisatrices peuvent ensuite utiliser l’ID client dans les appels API pour une intégration à l’application que vous avez créée.

>[!NOTE]
>
>Dans le contexte d’OAuth2, « créer une application » fait référence au processus de création de ce type de lien d’accès entre une application et un serveur, tel que [!DNL Workfront].

* Pour obtenir des instructions sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur ou utilisatrice (flux de code d’autorisation), voir [Configurer et utiliser des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 à l’aide de l’authentification du serveur (flux JWT), voir [Configurer et utiliser les applications OAuth2 personnalisées de votre entreprise à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Pour obtenir des instructions sur la configuration et l’utilisation de l’application OAuth2 à l’aide de PKCE, voir [Configurer et utiliser des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

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
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> Vous devez être administrateur ou administratrice [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble d’OAuth2

Imaginez qu’une application puisse extraire certaines informations spécifiques de [!DNL Workfront]. Une application qui demande des informations est appelée client. Dans cet exemple, le nom du client est ClientApp. ClientApp doit avoir accès aux informations d’un utilisateur ou d’une utilisatrice spécifique et doit donc accéder à [!DNL Workfront] en tant qu’utilisateur. Si votre utilisateur ou utilisatrice donne à ClientApp son nom d’utilisateur ou d’utilisatrice et son mot de passe, il peut accéder à toutes les données auxquelles l’utilisateur ou l’utilisatrice peut accéder. Il s’agit d’un risque de sécurité, car ClientApp n’a besoin que d’un petit ensemble d’informations spécifiques.

Lorsque vous créez une application OAuth2 pour ClientApp, vous indiquez essentiellement à [!DNL Workfront] que ClientApp est autorisé à accéder à [!DNL Workfront], mais uniquement si la personne dont le compte auquel accède ClientApp donne l’autorisation d’accès.

## Créer une application OAuth2

Lors de la création d’une application OAuth2, choisissez le type d’application qui répond le mieux aux besoins de votre intégration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d’application</th> 
   <th>Idéale pour</th> 
   <th>Méthode d’authentification</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Application machine-machine</p> </td> 
   <td> <p>Idéale pour les interfaces de ligne de commande, les démons ou les scripts exécutés sur votre serveur</p> <p>Exemples :</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Authentification via le jeton web JSON avec codage de paire de clés publique/privée.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Application web monopage</p> </td> 
   <td> <p>Idéale pour les applications web mobiles ou monopages</p> <p>Exemples :</p> 
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
   <td> <p>Idéale pour les applications côté serveur qui gèrent les informations d’identification et les jetons sur le serveur.</p> <p>Exemples :</p> 
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
>Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.

* [Créer une application OAuth2 à l’aide de l’authentification du serveur (flux JWT)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Créer une application OAuth2 à l’aide d’informations d’identification d’utilisateur ou d’utilisatrice (flux de code d’autorisation)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Créer une application web OAuth2 monopage à l’aide de PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Créer une application OAuth2 à l’aide de l’authentification du serveur (flux JWT) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth2]**.
1. Cliquez sur **[!UICONTROL Créer l’intégration d’application]**.
La zone **Nouvelle application OAuth2** s’affiche.
1. Dans la zone **Nouvelle application OAuth2**, sélectionnez **[!UICONTROL Application machine à machine]**.
1. Saisissez un nom pour la nouvelle application, par exemple « [!DNL Workfront] pour ClientApp ».
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
      <td> <p>Ce champ est généré automatiquement.</p> <p><b>IMPORTANT</b> :  <p>copiez le contenu de ce champ dans un autre fichier sécurisé avant de fermer cette page. Vous ne pourrez plus voir cette clé secrète.</p> <p>Si vous perdez cette clé, supprimez-la et créez un secret client.</p> 
        <ol> 
         <li value="1"> <p>Cliquez sur l’icône <b>[!UICONTROL Delete]</b> <img src="assets/delete.png"> pour supprimer le secret client actuel.</p> </li> 
         <li value="2"> <p>Cliquez sur <b>[!UICONTROL Add client secret]</b> pour générer un nouveau secret client.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>Les applications serveur à serveur utilisent des clés publiques et privées pour l’authentification. Utilisez l’une des méthodes suivantes :</p> 
       <ul> 
        <li> <p>Cliquez sur <b>[!UICONTROL Add a public key]</b> et saisissez la clé publique de l’autre application.</p> </li> 
        <li> <p>Cliquez sur <b>[!UICONTROL Generate a public/private keypair]</b>, puis partagez la clé publique avec l’autre application.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Il s’agit du nom que vous avez donné à l’application. Ce champ ne doit pas être vide.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour l’intégration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur ou de l’utilisatrice (flux de code d’autorisation), voir la section [Configurer et utiliser les applications OAuth 2 personnalisées de votre organisation à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).

### Créer une application OAuth2 à l’aide d’informations d’identification d’utilisateur ou d’utilisatrice (flux de code d’autorisation) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

>[!NOTE]
>
>Si vous créez une application pour vous connecter à Workfront Fusion, utilisez l’une des URL de redirection suivantes :
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-workfront`
>* `https://app-eu.workfrontfusion.com/oauth/cb/workfront-workfront` (centre de données de l’UE)
>* `https://app-az.workfrontfusion.com/oauth/cb/workfront-workfront` (Azure Data Center)

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth2]**.
1. Cliquez sur **[!UICONTROL Créer l’intégration de l’application]**.

   La **Nouvelle application OAuth2** s’affiche.
1. Dans la zone **Nouvelle application OAuth2**, sélectionnez **[!UICONTROL Application web]**.
1. Saisissez un nom pour la nouvelle application OAuth2, tel que « [!DNL Workfront] pour ClientApp ».
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
      <td> <p>Ce champ est généré automatiquement.</p> <p><b>IMPORTANT</b> :  <p>copiez le contenu de ce champ dans un autre fichier sécurisé avant de fermer cette page. Vous ne pourrez plus voir cette clé secrète.</p> <p>Si vous perdez cette clé, supprimez-la et créez un secret client.</p> 
        <ol> 
         <li value="1"> <p>Cliquez sur l’icône <b>[!UICONTROL Delete]</b> <img src="assets/delete.png"> pour supprimer le secret client actuel.</p> </li> 
         <li value="2"> <p>Cliquez sur <b>[!UICONTROL Add client secret]</b> pour générer un nouveau secret client.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirect URLs]</td> 
      <td>Les utilisateurs et utilisatrices seront redirigés vers ce chemin après s’être authentifiés auprès de [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Refresh token rotation]</td> 
      <td>Activez cette option pour émettre un nouveau jeton d’actualisation lorsque le jeton d’actualisation est utilisé. Votre application doit stocker le nouveau jeton après chaque actualisation.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute refresh token expiration]</td> 
      <td> <p>Sélectionnez la durée d’existence d’un jeton d’actualisation avant son expiration. À son expiration, vos utilisateurs et utilisatrices doivent à nouveau se connecter à l’intégration. Sélectionnez « [!UICONTROL No expiration] » si vous ne souhaitez pas que le jeton d’actualisation expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Expiration du jeton d’actualisation d’inactivité</td> 
      <td> <p>Sélectionnez la durée au bout de laquelle le jeton d’actualisation d’un utilisateur ou d’une utilisatrice en inactivité expire. </p> <p>Par exemple, si l’expiration du jeton d’actualisation pour inactivité est de 6 mois et que l’utilisateur ou utilisatrice ne se connecte pas pendant six mois, le jeton d’actualisation expire même si l’expiration du jeton d’actualisation absolu est définie pour une plus longue durée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Vous pouvez ajouter un logo pour rendre cette application plus reconnaissable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Il s’agit du nom que vous avez donné à l’application. Ce champ ne doit pas être vide.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour l’intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL App Description URL]</td> 
      <td>Il peut s’agir d’un lien vers une page « À propos de nous » ou d’une page contenant plus d’informations sur l’intégration.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur ou utilisatrice (flux de code d’autorisation), voir [Configurer et utiliser les applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).

### Créer une application web OAuth2 monopage à l’aide de PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Système]**, puis sélectionnez **[!UICONTROL Applications OAuth2]**.
1. Cliquez sur **[!UICONTROL Créer l’intégration d’application]**.

   La boîte de dialogue **Nouvelle application OAuth2** s’affiche.
1. Dans la boîte de dialogue **Nouvelle application OAuth2**, sélectionnez **[!UICONTROL Application web monopage]**.
1. Saisissez un nom pour la nouvelle application [!UICONTROL OAuth2], tel que « [!DNL Workfront] pour ClientApp ».
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
      <td role="rowheader">[!UICONTROL Redirect URLs]</td> 
      <td>Les utilisateurs et utilisatrices seront redirigés vers ce chemin après s’être authentifiés auprès de Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Rotate refresh token every time it is used]</td> 
      <td>Activez cette option pour émettre un nouveau jeton d’actualisation lorsque le jeton d’actualisation est utilisé. Votre application doit stocker le nouveau jeton après chaque actualisation.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute expiration]</td> 
      <td> <p>Sélectionnez la durée d’existence d’un jeton d’actualisation avant son expiration. À son expiration, vos utilisateurs et utilisatrices doivent à nouveau se connecter à l’intégration. Sélectionnez « [!UICONTROL No expiration] » si vous ne souhaitez pas que le jeton d’actualisation expire.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Inactivity expiration]</td> 
      <td> <p>Sélectionnez la durée au bout de laquelle le jeton d’actualisation d’un utilisateur ou d’une utilisatrice en inactivité expire. </p> <p>Par exemple, si l’expiration du jeton d’actualisation pour inactivité est de 6 mois et que l’utilisateur ou utilisatrice ne se connecte pas pendant six mois, le jeton d’actualisation expire même si l’expiration du jeton d’actualisation absolu est définie pour une plus longue durée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Vous pouvez ajouter un logo pour rendre cette application plus reconnaissable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Il s’agit du nom que vous avez donné à l’application. Ce champ ne doit pas être vide.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour l’intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Developer name]</td> 
      <td>Il s’agit du nom du développeur ou de la développeuse qui configure l’application OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Developer email address]</td> 
      <td>Il s’agit de l’adresse électronique du développeur ou de la développeuse qui configure l’application OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Privacy policy URL]</td> 
      <td>Il s’agit du lien vers l’emplacement où votre entreprise stocke sa politique de confidentialité.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Configurer et utiliser l’application OAuth2 créée

La configuration et l’utilisation avancées de l’application OAuth2 créée nécessitent des connaissances techniques, qui incluent les appels API.

* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 avec les informations d’identification de l’utilisateur ou de l’utilisatrice (flux de code d’autorisation), voir [Configurer et utiliser les applications OAuth2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 à l’aide de l’authentification du serveur (flux JWT), voir [Configurer et utiliser les applications OAuth2 personnalisées de votre entreprise à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Pour plus d’informations sur la configuration et l’utilisation de l’application OAuth2 à l’aide de PKCE, voir [Configurer et utiliser les applications OAuth2 personnalisées de votre entreprise à l’aide du flux PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Processus OAuth2 pour le flux de code d’autorisation

>[!NOTE]
>
>Vos utilisateurs et vos utilisatrices accèdent à l’application [!UICONTROL OAuth2] par le biais de l’API. Cette section décrit les fonctionnalités en termes généraux et est fournie à titre d’information uniquement.
>
>Pour obtenir des instructions spécifiques sur l’utilisation de l’application OAuth2, y compris les appels API spécifiques, voir [Configurer et utiliser les applications OAuth2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).

### Autoriser avec un code d’autorisation et un jeton d’accès {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp a besoin de certaines informations de [!DNL Workfront], elle envoie donc une requête au point d’entrée de l’API [!DNL Workfront] `/authorize`. La requête inclut l’instruction [!UICONTROL response_type] `code`, qui indique que la requête doit renvoyer un code d’autorisation.
1. Cela déclenche dans [!DNL Workfront] l’envoi d’une invite d’authentification à l’utilisateur ou à l’utilisatrice. L’utilisateur ou l’utilisatrice peut saisir ses informations d’identification dans l’invite, ce qui accorde à [!DNL Workfront] l’autorisation de communiquer avec ClientApp. Si la personne est déjà connectée à [!DNL Workfront], cette étape peut être ignorée.
1. L’API [!DNL Workfront] envoie un code d’autorisation à ClientApp.
1. ClientApp envoie les informations suivantes dans une requête au point d’entrée de l’API [!DNL Workfront] `/token` :

   * Le code d’autorisation envoyé à ClientApp à l’étape 3. Cela identifie l’instance spécifique d’autorisation de l’utilisateur ou de l’utilisatrice.
   * Le secret client généré lors de la configuration de l’application ClientApp OAuth2 dans [!DNL Workfront]. Cela permet à [!DNL Workfront] de savoir que la demande provient de ClientApp.

1. Si le code d’autorisation et le secret client sont corrects, [!DNL Workfront] envoie un jeton d’accès à ClientApp. Ce jeton d’accès est envoyé directement de [!DNL Workfront] à l’application cliente et ne peut pas être visualisé, copié ou utilisé par un autre utilisateur, une autre utilisatrice ou une autre application cliente.
1. ClientApp envoie le jeton d’accès à [!DNL Workfront] ainsi que la demande d’informations spécifique.
1. Étant donné que le jeton d’accès est correct, [!DNL Workfront] envoie les informations à ClientApp.

#### Actualiser les jetons d’accès

Pour des raisons de sécurité, les jetons d’accès expirent après un court laps de temps. Pour obtenir de nouveaux jetons d’accès sans avoir à saisir des informations d’identification à chaque fois, [!DNL OAuth2] utilise des jetons d’actualisation. Les jetons d’actualisation sont stockés par le client.

Le processus d’acquisition d’un jeton d’actualisation est identique à celui décrit dans la section [Autorisation avec un code d’autorisation et un jeton d’accès](#authorizing-with-an-authorization-code-and-access-token). La requête de code d’autorisation inclut la portée `offline_access`, qui indique que la requête doit renvoyer un jeton de requête avec le code d’autorisation.
