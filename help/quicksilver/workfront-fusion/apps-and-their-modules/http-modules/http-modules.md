---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: HTTP > Autres modules
description: L’application HTTP  [!DNL Adobe Workfront Fusion]  fournit divers modules de communication basés sur le protocole HTTP (Hypertext Transfer Protocol). HTTP est la base de la communication des données pour le World Wide Web. Vous pouvez utiliser les modules pour télécharger des pages et des fichiers web, appeler des webhooks et des points de terminaison d’API, etc.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 100%

---

# HTTP > Autres modules

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] nécessite une licence [!UICONTROL Adobe Workfront Fusion] en plus d’une licence [!UICONTROL Adobe Workfront].

L’application HTTP[!DNL Adobe Workfront Fusion]  fournit divers modules pour la communication basés sur le protocole HTTP (Hypertext Transfer Protocol). HTTP est la base de la communication des données pour le World Wide Web. Vous pouvez utiliser les modules pour télécharger des pages et des fichiers web, appeler des webhooks et des points de terminaison d’API, etc.

Le bon choix du module dépend du mécanisme d’authentification/d’autorisation de la ressource à laquelle vous souhaitez accéder. Vous trouverez ci-dessous des exemples de modules :

* Effectuer une requête : module universel destiné principalement aux ressources qui n’utilisent aucun type d’authentification/autorisation.
* Effectuer une requête d’authentification de base : pour les ressources qui utilisent l’authentification de base (BA) [!DNL HTTP].
* Effectuer une requête OAuth 2.0 : pour les ressources utilisant le protocole d’autorisation OAuth 2.0.
* Effectuer une demande d’authentification de certificat client : pour les ressources utilisant le protocole d’autorisation qui nécessite un certificat côté client.
* Effectuer une demande d’autorisation de clé API : pour les ressources utilisant des clés API pour l’autorisation.

>[!NOTE]
>
>Si vous vous connectez à un produit Adobe qui n’a pas encore de connecteur dédié, il est recommandé d’utiliser le module Adobe Authenticator.
>
>Pour plus d’informations, voir [Module Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Modules de requête

Consultez les articles suivants pour obtenir des instructions spécifiques aux modules de requête :

* [[!UICONTROL HTTP] > Module [!UICONTROL Effectuer une requête]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] > Module [!UICONTROL Effectuer une requête d’autorisation de base]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [Module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête OAuth 2.0]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [Module [!UICONTROL HTTP] > [!UICONTROL Effectuer une demande d’autorisation de certificat client]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Effectuer une requête d’autorisation de clé API]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Autres modules d’action

* [[!UICONTROL Obtenir un fichier]](#get-a-file)
* [[!UICONTROL Résoudre une URL cible]](#resolve-a-target-url)

### [!UICONTROL Obtenir un fichier]

Ce module d’action télécharge un fichier à partir de l’URL spécifiée. Une fois le fichier téléchargé, vous pouvez continuer à traiter le fichier (mapper les données du fichier) à l’aide d’autres modules dans le scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Saisissez ou mappez l’URL du fichier à télécharger. </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Résoudre une URL cible]

Ce module d’action résout une chaîne de redirections HTTP et renvoie une URL cible.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Saisissez ou mappez l’URL à résoudre, par exemple une URL [!DNL bit.ly].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method] </td> 
   <td> <p>Indiquez si vous souhaitez utiliser la méthode [!UICONTROL HEAD] ou la méthode [!UICONTROL GET].</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modules itérateurs

### [!UICONTROL Récupérer des en-têtes]

Ce module renvoie chaque en-tête (nom et valeur) du module HTTP spécifié dans un lot distinct.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Sélectionnez le module à partir duquel vous souhaitez récupérer les en-têtes.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Générer des jetons web JSON (JWT)

Il est possible de générer un jeton JWT à l’aide de fonctions intégrées :

En-tête :

![](assets/jwt-header-350x19.png)

Code à copier-coller :

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Payload :

![](assets/jwt-payload-350x17.png)

Code à copier-coller :

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Jeton :

![](assets/jwt-token-350x15.png)

Code à copier-coller :

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
