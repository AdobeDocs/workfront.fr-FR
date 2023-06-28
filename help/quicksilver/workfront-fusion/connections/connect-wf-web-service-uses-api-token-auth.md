---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connexion [!DNL Adobe Workfront Fusion] vers un service Web qui utilise l’autorisation de jeton API
description: Certains services n’autorisent pas les solutions d’intégration telles que [!DNL Adobe Workfront Fusion] pour créer une application que vous pouvez facilement utiliser dans votre scénario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Connexion [!DNL Adobe Workfront Fusion] vers un service Web qui utilise l’autorisation de jeton API

Certains services n’autorisent pas les solutions d’intégration telles que [!DNL Adobe Workfront Fusion] pour créer une application que vous pouvez facilement utiliser dans votre scénario.

Il existe une solution à cette situation. Vous pouvez connecter le service (application) souhaité à [!DNL Workfront Fusion] using [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] module .

Cet article explique comment connecter pratiquement n’importe quel service Web à [!DNL Workfront Fusion] à l’aide d’une clé API/d’un jeton API.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connexion à un service Web qui utilise un jeton API

La procédure de connexion du service via un jeton API est similaire pour la plupart des services web.

1. Créez une application sur le site web du service Web, comme expliqué dans la section . [Création d’une application et obtention du jeton API](#create-a-new-application-and-obtain-the-api-token) dans cet article.
1. Obtenez la clé API ou le jeton API.
1. Ajouter [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] > [!UICONTROL Lancer une requête] à votre scénario.
1. Configurez le module conformément à la documentation de l’API du service Web et exécutez le scénario, comme expliqué dans la section . [Configurez les [!UICONTROL HTTP] module](#set-up-the-http-module) dans cet article.

>[!NOTE]
>
>Nous utiliserons la variable [!DNL Pushover] service de notification comme exemple tout au long de cet article.

## Création d’une application et obtention du jeton API

>[!NOTE]
>
>Les services Web peuvent créer et distribuer des clés d’API ou des jetons d’API de différentes manières. Pour obtenir des instructions sur l’obtention d’une clé et d’un jeton d’API pour le service Web souhaité, rendez-vous sur le site Web du service et recherchez &quot;Clé API&quot; ou &quot;Jeton d’API&quot;.
>
>Nous incluons des instructions pour l’obtention d’une clé API push uniquement comme exemple de ce que vous pourriez trouver.

1. Connectez-vous à [!DNL Pushover] compte .
1. Cliquez sur **[!UICONTROL Création d’un jeton d’application/API]** au bas de la page.
1. Renseignez les informations de l’application et cliquez sur **[!UICONTROL Création d’une application]**.
1. Stockez le jeton API fourni dans un endroit sûr. Vous en aurez besoin pour la variable [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Lancer une requête] pour se connecter au service Web souhaité ([!DNL Pushover], dans ce cas).

## Configurez les [!UICONTROL HTTP] module

Pour connecter un service Web à votre [!DNL Workfront Fusion] , vous devez utiliser la variable [!UICONTROL HTTP] >[!UICONTROL Effectuer une requête] dans le scénario et configurez le module conformément à la documentation de l’API du service web.

1. Ajoutez la variable [!UICONTROL HTTP] >[!UICONTROL Lancer une requête] à votre scénario.
1. Pour envoyer un message en push à l’aide de [!DNL Workfront Fusion], configurez le module HTTP comme suit.

   >[!NOTE]
   >
   >Ces paramètres de module correspondent à la variable [!DNL Pushover] documentation de l’API de service Web. Les paramètres peuvent être différents pour d’autres services web. Par exemple, le jeton API peut être inséré dans la variable [!UICONTROL En-tête] et non au [!UICONTROL Corps] champ .

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>Le champ URL contient le point de terminaison que vous trouverez dans la documentation de l’API du service Web.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Méthode [!UICONTROL]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>La méthode utilisée dépend du point de terminaison correspondant. Le point de terminaison push pour la publication de messages utilise la méthode POST.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>Certains services web peuvent utiliser des en-têtes pour spécifier l’authentification par jeton API ou d’autres paramètres. Ce n’est pas le cas dans notre exemple, car le point de terminaison du Pushover pour la publication de messages utilise Body (voir ci-dessous) pour tous les types de requêtes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Query String]</p> </td> 
      <td> <p>Certains services Web peuvent utiliser une chaîne de requête pour spécifier d’autres paramètres. Ce n’est pas le cas dans notre exemple en tant que [!DNL Pushover] Le service web utilise [!UICONTROL Body] (voir ci-dessous) pour tous les types de requêtes.</p> </td> 
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
      <td> <p>Saisissez le contenu de la requête [!UICONTROL Body] au format JSON. Vous pouvez utiliser le module [!UICONTROL JSON] &gt; [!UICONTROL Créer JSON] comme expliqué dans la section <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">Corps JSON mappé à l’aide du module [!UICONTROL JSON] &gt; [!UICONTROL Créer JSON]</a> dans cet article. Vous pouvez également saisir le contenu JSON manuellement, en suivant la procédure décrite à la section <a href="#json-body-entered-manually" class="MCXref xref">Corps JSON saisi manuellement</a> dans cet article.</p> <p>Consultez la documentation de l’API du service Web pour connaître les paramètres requis pour ce service Web.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Corps JSON saisi manuellement

Spécifiez les paramètres et les valeurs au format JSON.

>[!INFO]
>
>**Exemple:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>
>
>"token":"123459evz8aepwtxydndydgyumbfx",
>
>
>"message":"Hello World!",
>
>
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>Votre USER_KEY. Vous pouvez le trouver dans votre [!DNL Pushover] tableau de bord.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Votre jeton API/clé API généré lorsque vous avez créé votre [!DNL Pushover] application.</p> </td> 
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

## Corps JSON mappé à l’aide de [!UICONTROL JSON] >[!UICONTROL Création de JSON] module

Le [!UICONTROL Création de JSON] facilite la spécification de JSON. Il vous donne également la possibilité de définir des valeurs de manière dynamique.

Pour plus d’informations sur les modules JSON, voir [Modules JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Saisissez ou mappez les valeurs à partir desquelles vous souhaitez créer JSON.

   ![](assets/json-values-350x288.png)

1. Connectez-vous au [!UICONTROL JSON] > [!UICONTROL Création de JSON] du module HTTP > Créer une requête.
1. Mappez la chaîne JSON à partir de la propriété [!UICONTROL Création de JSON] au module [!UICONTROL Demander du contenu] dans le champ [!UICONTROL HTTP] >[!UICONTROL Lancer une requête] module .

   Maintenant, lorsque vous exécutez le scénario, la notification push est envoyée à l’appareil qui a été enregistré dans votre [!DNL Pushover] compte .
