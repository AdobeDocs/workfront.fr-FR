---
title: FAQ sur les API SOAP
description: FAQ sur les API SOAP
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# FAQ sur les API SOAP

## Comment créer mon premier BAT de fichier ?

Il comprend 3 étapes simples :

**Étape 1**: Téléchargez le fichier sur le BAT Workfront en l’envoyant via une requête Post à  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Nous vous renverrons le hachage du fichier - c&#39;est très important ! Notez qu’à ce stade, vous ne verrez rien dans votre compte, tout ce que vous avez fait jusqu’à présent est de nous envoyer le fichier mais ne nous a pas dit quoi en faire.

**Étape 2**: Si vous ne disposez pas encore d’un ID de session, obtenez-en un à l’aide des méthodes doLogin() ou getSessionID() . Utilisez la première pour vous connecter à l’aide de l’adresse électronique et du mot de passe d’un utilisateur ou la seconde méthode si vous disposez de l’adresse électronique et du jeton d’authentification de l’utilisateur.

**Étape 3 :** Il est maintenant temps de créer votre bon à tirer. Utilisez la méthode createProof() et envoyez-nous au moins les champs requis (il n’y en a actuellement que 5). Assurez-vous de définir le paramètre Hash sur le hachage de fichier renvoyé lors de l’&quot;étape 1&quot;, car cela nous permet de déterminer le fichier à utiliser lors de la création de votre BAT.

Si vous vous connectez maintenant à votre compte, vous verrez le BAT.

## Comment créer mon premier BAT d’instantané web ?

Il s’agit de deux étapes simples :

**Étape 1**: Si vous ne disposez pas encore d’un ID de session, obtenez-en un à l’aide des méthodes doLogin() ou getSessionID() . Utilisez la première pour vous connecter à l’aide de l’adresse électronique et du mot de passe d’un utilisateur ou la seconde méthode si vous disposez de l’adresse électronique et du jeton d’authentification de l’utilisateur.

**Étape 2 :**Il est maintenant temps de créer votre BAT. Utilisez la méthode createProof() et envoyez-nous au moins les champs requis (il n’y en a actuellement que 5). Assurez-vous de définir le paramètre Hash sur &quot;web&quot; et le paramètre SourceName comme URL de la page web que vous souhaitez capturer.

Si vous vous connectez maintenant à votre compte, vous verrez le BAT.

## Quelle est la différence entre un bon à tirer et une version ?

Dans Workfront, les versions de BAT s’affichent sous la forme d’un BAT unique. Cliquez sur une version spécifique de l’interface utilisateur web pour afficher les détails de cette version. En réalité, chaque version est un bon à tirer distinct et l’interface utilisateur Web les affiche ensemble.

Du point de vue de l’API, chaque version est un bon à tirer distinct et les bons à tirer sont liés par leurs identifiants.

**createProof()** sera toujours créé **version 1** de la preuve. Supposons que, dans notre exemple, l’identifiant renvoyé pour ce BAT &quot;100&quot; soit.

Lors de l’utilisation de **createProofVersion()** toujours envoyer l’identifiant de la version précédente. Si nous voulons créer **version 2** sur le BAT &quot;100&quot;, nous **transmettez &quot;100&quot; pour le ParentFileID** . Cela indique au système que ce BAT doit être la version 2 de l’ensemble. La méthode renvoie un identifiant de BAT unique. Par exemple, supposons qu’il s’agisse de &quot;101&quot;.

Si une troisième version, c’est-à-dire **version 3** est requis ; vous allez appeler **createProofVersion()** encore une fois et cette fois **transmettez &quot;101&quot; pour le ParentFileID** qui s’assure que la liste liée des versions est correctement créée.

## Dois-je obtenir un nouvel ID de session avant chaque appel ?

Il est important de souligner que chaque ID de session est essentiellement un utilisateur exécutant les actions. 

Vous n’avez pas besoin d’obtenir un nouvel ID de session avant chaque appel à l’API et il restera valide pendant 24 heures. Le délai d’expiration est réinitialisé chaque fois que vous effectuez un appel vers l’API.

## Qu’est-ce qu’un BAT / une URL personnelle ?

**Équipe/Public**: Chaque version de BAT comporte une URL d’équipe (publique) unique. S’il est activé, le BAT s’ouvre en mode lecture seule. Vous pouvez obtenir l’URL de l’équipe à l’aide du [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) .

**Personal**: Une URL personnelle est unique pour chaque réviseur et version de BAT. Si un jeu de BAT contient 3 versions et qu’un validant se trouve sur toutes les versions, le validant aura 3 URL personnelles uniques. Une URL personnelle ouvre la version du BAT avec le validant déjà identifié et doit donc être sécurisé et ne pas être partagé. Vous pouvez obtenir des URL personnelles en appelant la fonction [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) puis effectuer une itération sur chaque  [SOAPRecepientObject](http://api.proofhq.com/home/objects/soaprecipientobject) et obtention du paramètre &quot;proof_url&quot;.

## >Comment inclure des paramètres personnalisés lors de l’ouverture de l’épreuve de miniature ?

L’épreuve en miniature vous permet d’incorporer l’outil de vérification dans votre propre page. Un paramètre &quot;referer&quot; peut être inclus dans le fichier minima afin de fournir une URL de redirection lorsqu’un utilisateur clique sur le bouton de fermeture dans le fichier minima. Vous pouvez inclure un certain nombre de paramètres personnalisés dans cette URL de redirection en les ajoutant à l’aide du caractère &quot;&amp;&quot; avec échappement, par exemple. %26.

Par exemple, l’URL infaillible
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` doit être codé en tant que 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` pour que les paramètres personnalisés soient transmis.

## Comment créer un client de service Web Java ?

[Cette vidéo](http://screencast.com/t/xsSNrqs5b) indique comment créer un client de service Web Java à l’aide d’Eclipse et de la définition WSDL de BAT Workfront.
