---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: HTTP et gt ; autres modules
description: La variable [!DNL Adobe Workfront Fusion] L’application HTTP fournit divers modules de communication basés sur le protocole HTTP (Hypertext Transfer Protocol). HTTP est la base de la communication des données pour le World Wide Web. Vous pouvez utiliser les modules pour télécharger des pages et des fichiers web, appeler des webhooks et des points de terminaison d’API, etc.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# HTTP > Autres modules

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] nécessite une [!UICONTROL Adobe Workfront Fusion] en plus d’une [!UICONTROL Adobe Workfront] licence.

La variable [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] L’application fournit divers modules pour la communication basés sur le protocole HTTP (Hypertext Transfer Protocol). HTTP est la base de la communication des données pour le World Wide Web. Vous pouvez utiliser les modules pour télécharger des pages et des fichiers web, appeler des webhooks et des points de terminaison d’API, etc.

Le bon choix du module dépend du mécanisme d’authentification/d’autorisation de la ressource à laquelle vous souhaitez accéder. Vous trouverez ci-dessous des exemples de modules :

* Effectuer une requête : module universel destiné principalement aux ressources qui n’utilisent aucun type d’authentification/autorisation
* Effectuer une requête d’authentification de base : pour les ressources qui utilisent [!DNL HTTP] Authentification de base (BA)
* Effectuez une requête OAuth 2.0 : pour les ressources utilisant le protocole d’autorisation OAuth 2.0
* Effectuer une demande d’authentification de certificat client : pour les ressources utilisant le protocole d’autorisation qui nécessite un certificat côté client.
* Effectuez une demande d’autorisation de clé API : pour les ressources utilisant des clés API pour l’autorisation.

>[!NOTE]
>
>Si vous vous connectez à un produit Adobe qui ne possède pas encore de connecteur dédié, il est recommandé d&#39;utiliser le module Adobe Authenticator.
>
>Pour plus d’informations, voir [Module Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Modules de requête

Consultez les articles suivants pour obtenir des instructions spécifiques au module de requête :

* [[!UICONTROL HTTP] >[!UICONTROL Effectuer une requête] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Effectuer une requête d’autorisation de base] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Exécution d’une requête OAuth 2.0] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Lancer une demande d’autorisation de certificat client] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Lancer une demande d’autorisation de clé API]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Autres modules d’action

* [[!UICONTROL Obtention d’un fichier]](#get-a-file)
* [[!UICONTROL Résolution d’une URL cible]](#resolve-a-target-url)

### [!UICONTROL Obtention d’un fichier]

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

### [!UICONTROL Résolution d’une URL cible]

Ce module d’action résout une chaîne de redirections HTTP et renvoie une URL cible.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Saisissez ou mappez l’URL à résoudre, par exemple une [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Méthode [!UICONTROL] </td> 
   <td> <p>Indiquez si vous souhaitez utiliser la méthode [!UICONTROL HEAD] ou la méthode [!UICONTROL GET].</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modules itérateurs

### [!UICONTROL Récupération des en-têtes]

Ce module renvoie chaque en-tête (nom et valeur) du module HTTP spécifié dans un lot distinct.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module source]</td> 
   <td> <p> Sélectionnez le module à partir duquel vous souhaitez récupérer les en-têtes.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Génération de jetons Web JSON (JWT)

Il est possible de générer un jeton JWT à l’aide de fonctions intégrées :

En-tête :

![](assets/jwt-header-350x19.png)

Code pour le copier-coller :

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Charge utile :

![](assets/jwt-payload-350x17.png)

Code pour le copier-coller :

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Jeton :

![](assets/jwt-token-350x15.png)

Code pour le copier-coller :

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
