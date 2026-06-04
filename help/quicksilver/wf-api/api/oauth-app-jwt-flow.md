---
content-type: api
navigation-topic: api-navigation-topic
title: Utiliser le flux JWT pour les applications OAuth 2 personnalisées
description: Utiliser le flux JWT pour les applications OAuth 2 personnalisées
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
TQID: https://experienceleague.adobe.com/uxF82lsimZlGpWRe8BEt80-9wb0rnwz7uhBHCI8nAig
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 462
ht-degree: 99%

---

# Configurer et utiliser les applications OAuth 2 personnalisées de votre organisation à l’aide du flux JWT

Pour intégrer Workfront et permettre à votre application client de communiquer avec Workfront au nom de l’utilisateur ou de l’utilisatrice, vous devez procéder comme suit :

* Créer une application OAuth2
* Créer un certificat de clé publique
* Créer un jeton web JSON (JWT)

## Créer une application OAuth2

Pour des instructions sur la création de l’application OAuth2, voir [Créer une application OAuth2 à l’aide de l’authentification serveur (flux JWT)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) dans [Créer des applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.

## Créer un certificat de clé publique

Le JWT doit être signé et encodé en Base64 pour être inclus dans la demande d’accès. Les bibliothèques JWT fournissent des fonctions permettant d’effectuer ces tâches.

Le jeton doit être signé à l’aide de la clé privée d’un certificat de signature numérique. Dans ce cas, vous pouvez utiliser la clé privée de tout certificat associé pour signer votre JWT.

L’algorithme utilisé est RS256 (signature RSA avec SHA-256). Il s’agit d’un algorithme asymétrique qui utilise une paire de clés publique/privée. Le fournisseur d’identité dispose d’une clé privée (secrète) utilisée pour générer la signature, et le client du JWT obtient une clé publique pour valider la signature.

Pour générer la clé publique, faites l’**une** des opérations suivantes.

* Ouvrez votre terminal MacOS/Linux et exécutez la commande suivante, puis chargez `certificate_pub.crt` en utilisant le bouton **Ajouter une clé publique** dans la configuration de l’application OAuth2 dans Workfront.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Utilisez le bouton **Générer une paire de clés publique/privée** dans la configuration de l’application OAuth2 dans Workfront pour générer le RSA.

## Créer un jeton web JSON

Un jeton web JSON pour l’authentification d’un compte de service nécessite un ensemble particulier de revendications et doit être signé à l’aide d’un certificat de signature numérique valide. Nous vous recommandons d’utiliser l’une des bibliothèques ou l’un des outils accessibles au public pour créer votre JWT.

Le tableau suivant contient des informations sur les champs qui peuvent être nécessaires lors de la configuration du jeton JWT.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Obligatoire. Le paramètre d’expiration est un paramètre obligatoire mesurant le temps absolu écoulé depuis le 01/01/1970 GMT. Vous devez vous assurer que l’heure d’expiration est postérieure à l’heure d’émission. Passé ce délai, le jeton JWT n’est plus valide. </p> <p>Note : nous vous recommandons d’utiliser un jeton à durée de vie très courte (quelques minutes), de sorte qu’il expire peu après avoir été échangé contre un jeton d’accès. Chaque fois qu’un nouveau jeton d’accès est requis, un JWT est signé et échangé. Il s’agit d’une approche plus sûre. Nous ne recommandons pas les jetons à longue durée de vie qui sont réutilisés pour obtenir des jetons d’accès en fonction des besoins.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>Requis. L’émetteur est l’ID du client ou de la cliente figurant dans les détails de l’application OAuth2.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Requis. Le sujet est l’ID de l’utilisateur ou l’utilisatrice qui a créé la clé publique lors de l’installation.</td> 
  </tr> 
 </tbody> 
</table>

## Échanger le JWT pour récupérer un jeton d’accès

1. Envoyez une requête POST à :

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. Le corps de la demande doit contenir des paramètres codés en URL avec votre identifiant client, votre secret client et votre JWT :

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
