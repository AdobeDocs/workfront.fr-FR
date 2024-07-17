---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connectez-vous  [!DNL Adobe Workfront Fusion]  à un service Web qui utilise l’autorisation de jeton API.
description: Certains services ne permettent pas aux solutions d’intégration telles que  [!DNL Adobe Workfront Fusion] de créer une application que vous pouvez facilement utiliser dans votre scénario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 13%

---

# Connecter [!DNL Adobe Workfront Fusion] à un service Web qui utilise l’autorisation de jeton API

Certains services ne permettent pas aux solutions d’intégration telles que [!DNL Adobe Workfront Fusion] de créer une application que vous pouvez facilement utiliser dans votre scénario.

Il existe une solution à cette situation. Vous pouvez connecter le service (app) souhaité à [!DNL Workfront Fusion] à l’aide du module [!UICONTROL HTTP] de [!DNL Workfront Fusion].

Cet article explique comment connecter pratiquement n’importe quel service Web à [!DNL Workfront Fusion] à l’aide d’une clé API/d’un jeton API.

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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connexion à un service Web qui utilise un jeton API

La procédure de connexion du service via un jeton API est similaire pour la plupart des services web.

1. Créez une application sur le site web du service web, comme expliqué dans la section [Créer une application et obtenir le jeton API](#create-a-new-application-and-obtain-the-api-token) de cet article.
1. Obtenez la clé API ou le jeton API.
1. Ajoutez le module [!UICONTROL HTTP] > [!UICONTROL  Créer une requête] à votre scénario.[!DNL Workfront Fusion]
1. Configurez le module conformément à la documentation de l’API du service Web et exécutez le scénario, comme expliqué dans la section [Configuration du module [!UICONTROL HTTP]](#set-up-the-http-module) de cet article.

>[!NOTE]
>
>Nous utiliserons le service de notification [!DNL Pushover] comme exemple tout au long de cet article.

## Création d’une application et obtention du jeton API

>[!NOTE]
>
>Les services Web peuvent créer et distribuer des clés d’API ou des jetons d’API de différentes manières. Pour obtenir des instructions sur l’obtention d’une clé et d’un jeton d’API pour le service Web souhaité, rendez-vous sur le site Web du service et recherchez &quot;Clé API&quot; ou &quot;Jeton d’API&quot;.
>
>Nous incluons des instructions pour l’obtention d’une clé API push uniquement comme exemple de ce que vous pourriez trouver.

1. Connectez-vous à votre compte [!DNL Pushover].
1. Cliquez sur **[!UICONTROL Créer un jeton d’application/API]** au bas de la page.
1. Renseignez les informations de l&#39;application et cliquez sur **[!UICONTROL Créer une application]**.
1. Stockez le jeton API fourni dans un endroit sûr. Vous en aurez besoin pour le module [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Lancer une requête] pour vous connecter au service Web souhaité ([!DNL Pushover], dans ce cas).

## Configuration du module [!UICONTROL HTTP]

Pour connecter un service Web à votre scénario [!DNL Workfront Fusion], vous devez utiliser le module [!UICONTROL HTTP] >[!UICONTROL Effectuer une requête] dans le scénario et configurer le module conformément à la documentation de l’API du service Web.

1. Ajoutez le module [!UICONTROL HTTP] >[!UICONTROL Make a Request] à votre scénario.
1. Pour envoyer un message en push à l’aide de [!DNL Workfront Fusion], configurez le module HTTP comme suit.

   >[!NOTE]
   >
   >Ces paramètres de module correspondent à la documentation de l’API de service Web [!DNL Pushover]. Les paramètres peuvent être différents pour d’autres services web. Par exemple, le jeton API peut être inséré dans [!UICONTROL Header] et non dans le champ [!UICONTROL Body].

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>Le champ URL contient le point de terminaison que vous trouverez dans la documentation de l’API du service Web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>La méthode utilisée dépend du point de terminaison correspondant. Le point de terminaison push pour la publication de messages utilise la méthode POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>Certains services web peuvent utiliser des en-têtes pour spécifier l’authentification par jeton API ou d’autres paramètres. Ce n’est pas le cas dans notre exemple, car le point de terminaison du Pushover pour la publication de messages utilise Body (voir ci-dessous) pour tous les types de requêtes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Query String]</p> </td> 
      <td> <p>Certains services Web peuvent utiliser une chaîne de requête pour spécifier d’autres paramètres. Ce n’est pas le cas dans notre exemple, car le service Web [!DNL Pushover] utilise [!UICONTROL Body] (voir ci-dessous) pour tous les types de requêtes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>Ce paramètre vous permet de sélectionner le type de contenu JSON dans le champ [!UICONTROL Content Type] ci-dessous.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON est le type de contenu requis par l’application [!UICONTROL Pushover]. Cela peut différer des autres services Web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Demander du contenu]</p> </td> 
      <td> <p>Saisissez le contenu de la requête [!UICONTROL Body] au format JSON. Vous pouvez utiliser le module [!UICONTROL JSON] &gt; [!UICONTROL Créer JSON] comme expliqué dans la section <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">JSON Body Mapped Using the [!UICONTROL JSON] &gt; [!UICONTROL Create JSON] </a> de cet article. Vous pouvez également saisir le contenu JSON manuellement, comme expliqué dans la section <a href="#json-body-entered-manually" class="MCXref xref">JSON Body Entered Manually</a> de cet article.</p> <p>Consultez la documentation de l’API du service Web pour connaître les paramètres requis pour ce service Web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Corps JSON saisi manuellement

Spécifiez les paramètres et les valeurs au format JSON.

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
   <td> <p>Votre jeton API/clé API qui a été généré, vous avez créé votre application [!DNL Pushover].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>Contenu texte de la notification push envoyée aux appareils.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Facultatif) Titre de votre message. Si aucune valeur n’est saisie, le nom de votre application est utilisé. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Corps JSON mappé à l’aide du module [!UICONTROL JSON] >[!UICONTROL Créer JSON]

Le module [!UICONTROL Créer JSON] facilite la spécification de JSON. Il vous donne également la possibilité de définir des valeurs de manière dynamique.

Pour plus d’informations sur les modules JSON, voir [Modules JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Saisissez ou mappez les valeurs à partir desquelles vous souhaitez créer JSON.

   ![](assets/json-values-350x288.png)

1. Connectez le module [!UICONTROL JSON] > [!UICONTROL Créer JSON] au module HTTP > Créer une requête.
1. Mappez la chaîne JSON du module [!UICONTROL  Create JSON] au champ [!UICONTROL Request content] dans le module [!UICONTROL HTTP] >[!UICONTROL Make a Request] .

   Désormais, lorsque vous exécutez le scénario, la notification push est envoyée à l’appareil qui a été enregistré dans votre compte [!DNL Pushover].
