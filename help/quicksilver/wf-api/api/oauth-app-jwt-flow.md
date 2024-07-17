---
content-type: api
navigation-topic: api-navigation-topic
title: Utilisation du flux JWT pour les applications OAuth 2 personnalisées
description: Utilisation du flux JWT pour les applications OAuth 2 personnalisées
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 8%

---

# Configurer et utiliser les applications OAuth 2 personnalisées de votre organisation à l’aide du flux JWT

Pour intégrer Workfront et permettre à votre application cliente de communiquer avec Workfront au nom de l’utilisateur ou de l’utilisatrice, vous devez :

* Créer une application OAuth2
* Création d’un certificat de clé publique
* Création d’un jeton Web JSON (JWT)

## Créer une application OAuth2

Pour plus d’informations sur la création de l’application OAuth2, voir [Création d’une application OAuth2 à l’aide de l’authentification du serveur (flux JWT)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) dans [Création d’applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Vous pouvez avoir jusqu’à dix applications OAuth2 à la fois.

## Création d’un certificat de clé publique

Le jeton JWT doit être signé et codé en base 64 pour être inclus dans la demande d’accès. Les bibliothèques JWT fournissent des fonctions pour exécuter ces tâches.

Le jeton doit être signé à l’aide de la clé privée d’un certificat de signature numérique. Si vous le faites, vous pouvez utiliser la clé privée de tout certificat associé pour signer votre JWT.

L’algorithme utilisé est RS256 (Signature RSA avec SHA-256). Il s’agit d’un algorithme asymétrique qui utilise une paire de clés publique/privée. Le fournisseur d’identité dispose d’une clé privée (secrète) utilisée pour générer la signature, et le consommateur du JWT obtient une clé publique pour valider la signature.

Pour générer la clé publique, effectuez **une** des opérations suivantes.

* Ouvrez votre terminal MacOS/Linux et exécutez la commande suivante, puis chargez `certificate_pub.crt` à l’aide du bouton **Ajouter la clé publique** dans la configuration de l’application OAuth2 dans Workfront.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Utilisez le bouton **Générer une paire de clés publique/privée** dans la configuration de l’application OAuth2 dans Workfront pour générer la RSA.

## Création d’un jeton Web JSON

Un jeton Web JSON pour l’authentification du compte de service nécessite un ensemble spécifique de revendications et doit être signé à l’aide d’un certificat de signature numérique valide. Nous vous recommandons d’utiliser l’une des bibliothèques ou des outils disponibles publiquement pour créer votre JWT.

Le tableau suivant contient des informations sur les champs qui peuvent être requis lorsque vous configurez le jeton JWT.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Obligatoire. Le paramètre d’expiration est un paramètre obligatoire qui mesure le temps absolu depuis 01/01/1970 GMT. Vous devez vous assurer que l’heure d’expiration est postérieure à l’heure du problème. Après cette période, le JWT n’est plus valide. </p> <p>Remarque : Nous vous recommandons d’avoir un jeton de durée de vie très courte (quelques minutes) afin qu’il expire peu après avoir été échangé contre un jeton d’accès. Chaque fois qu’un nouveau jeton d’accès est requis, un jeton JWT est signé et échangé. Il s’agit d’une approche plus sûre. Nous ne recommandons pas les jetons de longue durée qui sont réutilisés pour obtenir des jetons d’accès si nécessaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>Obligatoire. L’émetteur est votre ID de client à partir des détails de l’application OAuth2.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Obligatoire. Le sujet est votre ID utilisateur qui a créé la clé publique dans la configuration.</td> 
  </tr> 
 </tbody> 
</table>

## Exchange du JWT pour récupérer un jeton d’accès

1. Envoyez une demande de POST à :

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. Le corps de la requête doit contenir des paramètres codés URL avec votre ID client, votre secret client et votre JWT :

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
