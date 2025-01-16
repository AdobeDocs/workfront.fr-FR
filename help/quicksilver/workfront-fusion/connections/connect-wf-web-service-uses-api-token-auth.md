---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connecter  [!DNL Adobe Workfront Fusion]  à un service web qui utilise l’autorisation de jeton d’API
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 91%

---

# Connecter [!DNL Adobe Workfront Fusion] à un service web qui utilise l’autorisation de jeton d’API

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Connectez Adobe Workfront Fusion à un service web qui utilise l’autorisation de jeton API](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-wf-web-service-uses-api-token-auth.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Certains services n’autorisent pas les solutions d’intégration telles qu’[!DNL Adobe Workfront Fusion] pour créer une application que vous pouvez facilement utiliser dans votre scénario.

Il existe une solution à cette situation. Vous pouvez connecter le service souhaité (application) à [!DNL Workfront Fusion] à l’aide du module [!UICONTROL HTTP] de [!DNL Workfront Fusion].

Cet article explique comment connecter pratiquement n’importe quel service web à [!DNL Workfront Fusion] à l’aide d’une clé d’API/d’un jeton d’API.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Se connecter à un service web qui utilise un jeton d’API

La procédure de connexion du service via un jeton d’API est similaire pour la plupart des services web.

1. Créez une application sur le site web du service web comme expliqué dans la section [Créer une application et obtenir le jeton d’API](#create-a-new-application-and-obtain-the-api-token) de cet article.
1. Obtenez la clé d’API ou le jeton d’API.
1. Ajoutez à votre scénario le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête] de [!DNL Workfront Fusion].
1. Configurez le module conformément à la documentation de l’API du service web et exécutez le scénario comme expliqué dans la section [Configurer le module [!UICONTROL HTTP] ](#set-up-the-http-module) de cet article.

>[!NOTE]
>
>Nous utiliserons le service de notification [!DNL Pushover] comme exemple tout au long de cet article.

## Créer une application et obtenir le jeton d’API

>[!NOTE]
>
>Les services web peuvent créer et distribuer des clés d’API ou des jetons d’API de nombreuses manières. Pour obtenir des instructions sur l’obtention d’une clé et d’un jeton d’API pour le service web souhaité, rendez-vous sur le site web du service et recherchez « Clé d’API » ou « Jeton d’API ».
>
>Nous incluons des instructions pour l’obtention d’une clé d’API Pushover uniquement à titre d’exemple de ce que vous pourriez trouver.

1. Connectez-vous à votre compte [!DNL Pushover].
1. Cliquez sur **[!UICONTROL Créer une application/un jeton d’API]** au bas de la page.
1. Renseignez les informations de l’application et cliquez sur **[!UICONTROL Créer une application]**.
1. Stockez le jeton d’API fourni dans un endroit sûr. Vous en aurez besoin pour le module [!UICONTROL HTTP] >[!UICONTROL Effectuer une requête] de [!DNL Workfront Fusion] afin de vous connecter au service web souhaité ([!DNL Pushover] dans ce cas).

## Configurer le module [!UICONTROL HTTP]

Pour connecter un service web à votre scénario [!DNL Workfront Fusion], vous devez utiliser le module [!UICONTROL HTTP] >[!UICONTROL Effectuer une requête] dans le scénario et configurer le module conformément à la documentation de l’API du service web.

1. Ajoutez à votre scénario le module [!UICONTROL HTTP] >[!UICONTROL Effectuer une requête].
1. Pour envoyer un message push à l’aide de [!DNL Workfront Fusion], configurez le module HTTP comme suit.

   >[!NOTE]
   >
   >Ces paramètres de module correspondent à la documentation de l’API de service web [!DNL Pushover]. Les paramètres peuvent être différents pour d’autres services web. Par exemple, le jeton d’API peut être inséré dans l’[!UICONTROL En-tête] et non dans le champ [!UICONTROL Corps].

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>Le champ URL contient le point d’entrée que vous trouverez dans la documentation de l’API du service web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>La méthode utilisée dépend du point d’entrée correspondant. Le point d’entrée de Pushover pour la publication de messages utilise la méthode POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>Certains services web peuvent utiliser des en-têtes pour spécifier l’authentification par jeton API ou d’autres paramètres. Ce n’est pas le cas dans notre exemple, car le point d’entrée de Pushover pour la publication de messages utilise Body (voir ci-dessous) pour tous les types de requêtes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Query String]</p> </td> 
      <td> <p>Certains services web peuvent utiliser une chaîne de requête pour spécifier d’autres paramètres. Ce n’est pas le cas dans notre exemple puisque le service web [!DNL Pushover] utilise [!UICONTROL Body] (voir ci-dessous) pour tous les types de requêtes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Ce paramètre vous permet de sélectionner le type de contenu JSON dans le champ [!UICONTROL Content Type] ci-dessous.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON est le type de contenu requis par l’application [!UICONTROL Pushover]. Cela peut différer des autres services web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Request Content]</p> </td> 
      <td> <p>Saisissez le contenu de la requête [!UICONTROL Body] au format JSON. Vous pouvez utiliser le module [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] comme expliqué dans la section <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Corps JSON mappé à l’aide du module [!UICONTROL JSON] &gt; [!UICONTROL Create JSON]</a> dans cet article. Vous pouvez également saisir le contenu JSON manuellement, tel qu’expliqué à la section <a href="#json-body-entered-manually" class="MCXref xref">Corps JSON saisi manuellement</a> dans cet article.</p> <p>Consultez la documentation de l’API du service web pour connaître les paramètres requis pour ce service web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Corps JSON saisi manuellement

Spécifiez les paramètres et les valeurs au format JSON.

>[!INFO]
>
>**Exemple :**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>Votre USER_KEY. Vous pouvez le trouver dans votre tableau de bord [!DNL Pushover].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Votre jeton API/clé API généré lorsque vous avez créé votre application [!DNL Pushover].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>Contenu texte de la notification push envoyée à l’appareil ou aux appareils.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Facultatif) Titre de votre message. Si aucune valeur n’est saisie, le nom de votre application est utilisé. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Corps JSON mappé à l’aide du module [!UICONTROL JSON] >[!UICONTROL Créer JSON]

Le module [!UICONTROL Créer JSON] facilite la spécification de JSON. Il vous donne également la possibilité de définir des valeurs de manière dynamique.

Pour plus d’informations sur les modules JSON, voir [Modules JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Saisissez ou mappez les valeurs à partir desquelles vous souhaitez créer JSON.

   ![](assets/json-values-350x288.png)

1. Connectez le module [!UICONTROL JSON] > [!UICONTROL Créer JSON] au module HTTP > Créer une requête.
1. Mappez la chaîne JSON, du module [!UICONTROL Créer JSON] au champ [!UICONTROL Demander du contenu] dans le module [!UICONTROL HTTP] >[!UICONTROL Effectuer une requête].

   Maintenant, lorsque vous exécutez le scénario, la notification push est envoyée à l’appareil qui a été enregistré dans votre compte [!DNL Pushover].
