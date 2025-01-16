---
title: Appeler l’API REST MS Graph via le module  [!DNL Adobe Workfront Fusion]  HTTP > Effectuer une requête OAuth 2.0
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 87%

---

# Appeler l’[!UICONTROL API REST MS Graph] via le module [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Appeler l’API REST MS Graph](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/call-the-ms-graph-rest-api.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

<!-- Audited: 3/2024-->

De nombreux services web de [!DNL Microsoft] sont accessibles par l’intermédiaire de l’[!DNL Microsoft Graph API]. Vous pouvez créer une connexion à l’[!DNL Microsoft Graph API] à l’aide du module [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0].

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou niveau supérieur</p> </td> 
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

## Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]

Pour créer une connexion à [!DNL Microsoft Graph REST API], vous devez d’abord enregistrer [!DNL Adobe Workfront Fusion].

1. Commencez à enregistrer une nouvelle application, tel que décrit dans [Enregistrer votre application](https://learn.microsoft.com/en-us/graph/auth-register-app-v2) dans la documentation de [!DNL Microsoft].

   Dans le cadre de l’enregistrement, [!DNL Microsoft] requiert les informations suivantes :

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Saisissez un nom pour l’application, par exemple « Mon application [!DNL Workfront Fusion] ».</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Une fois l’enregistrement de l’application terminé, prenez note de l’[!UICONTROL ID de l’application].

   >[!IMPORTANT]
   >
   >Vous aurez besoin de l’ID de l’application pour configurer votre connexion dans [!DNL Workfront Fusion].

1. Générer une [!UICONTROL clé secrète]. Prenez note de cette clé secrète.

   Pour obtenir des instructions, voir [Enregistrer votre application](https://learn.microsoft.com/en-us/graph/auth-register-app-v2) dans la documentation de [!DNL Microsoft].

   >[!IMPORTANT]
   >
   >Vous aurez besoin de la [!UICONTROL clé secrète] pour configurer votre connexion dans [!DNL Workfront Fusion].

1. Configurez les autorisations de votre application.

   Pour plus d’informations sur la localisation et la configuration de ces champs, voir la section « Configurer les autorisations pour Microsoft Graph » dans [Obtenir un accès sans utilisateur ou utilisatrice](https://docs.microsoft.com/en-us/graph/auth-v2-service) dans la documentation de [!UICONTROL Microsoft].

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL What type of permissions does your application require?]</td> 
      <td>Sélectionnez <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Select permissions]</td> 
      <td> <p>Sélectionnez les autorisations suivantes :</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Toutes les autres autorisations requises par vos intégrations (par exemple : <code>User.Read</code>).</p> </li> 
       </ul> <p><b>Important</b> : vous aurez besoin des autorisations sélectionnées pour configurer votre connexion dans [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passez à [Configurer votre connexion  [!DNL MS Graph API]  dans  [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configurer votre connexion [!DNL MS Graph API] dans [!DNL Workfront Fusion]

Après l’enregistrement de [!DNL Workfront Fusion] tel que décrit dans [Enregistrer  [!DNL Workfront Fusion]  dans le  [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), vous pouvez configurer votre connexion dans le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0].

1. Ajoutez un module [!UICONTROL HTTP] > [!UICONTROL Effectuer un appel OAuth 2.0] à votre scénario.
1. Cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Configurez les champs de connexion comme suit :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td>Saisissez un nom pour la connexion.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Flow type]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Saisissez les autorisations sélectionnées à l’étape 4 d’<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Pour chaque portée, cliquez sur <b>[!UICONTROL Add]</b> et saisissez l’autorisation.</p> <p>Exemple : <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Saisissez l’[!UICONTROL Application ID] de l’étape 2 d’<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Saisissez la [!UICONTROL Application Secret] que vous avez générée à l’étape 3 d’<a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Enregistrer [!DNL Workfront Fusion] dans le [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize parameters]</td> 
      <td> <p>Ajoutez les paramètres d’autorisation suivants :</p> 
       <ul> 
        <li> <p>[!UICONTROL Key] :<code> response_mode</code> [!UICONTROL Value] : <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key] : <code>prompt </code>[!UICONTROL Value] : <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access token parameters]</td> 
      <td>Vous n’avez rien à saisir dans ce champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Refresh token parameters]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Cliquez sur <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>Dans le champ <b>[!UICONTROL Key]</b>, saisissez <code>scope</code>.</p> </li> 
        <li value="3"> <p>Dans le champ <b>[!UICONTROL Value]</b>, saisissez toutes les [!UICONTROL scope]s que vous avez saisies dans le champ de portée, séparées par des espaces.</p> <p>Exemple : <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Headers]</td> 
      <td>Vous n’avez rien à saisir dans ce champ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre qui s’affiche, cliquez sur **[!UICONTROL Accepter]** pour terminer la connexion et revenir au module.
