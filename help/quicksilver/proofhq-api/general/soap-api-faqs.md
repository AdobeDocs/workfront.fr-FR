---
title: Questions fréquentes sur l’API SOAP
description: Questions fréquentes sur l’API SOAP
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 1%

---

# Questions fréquentes sur l’API SOAP

## Comment créer mon premier BAT de fichier ?

Il comprend 3 étapes simples :

**Étape 1** : téléchargez le fichier vers Workfront Proof en l’envoyant via une requête Post à  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Nous vous renverrons le hachage du fichier - c&#39;est très important ! Notez qu’à ce stade, vous ne verrez rien dans votre compte, tout ce que vous avez fait jusqu’à présent est de nous envoyer le fichier mais ne nous a pas dit quoi en faire.

**Étape 2** : si vous ne disposez pas encore d’ID de session, obtenez-en un à l’aide des méthodes doLogin() ou getSessionID() . Utilisez la première pour vous connecter à l’aide de l’adresse électronique et du mot de passe d’un utilisateur ou la seconde méthode si vous disposez de l’adresse électronique et du jeton d’authentification de l’utilisateur.

**Étape 3 :** Il est maintenant temps de créer votre BAT. Utilisez la méthode createProof() et envoyez-nous au moins les champs requis (il n’y en a actuellement que 5). Assurez-vous de définir le paramètre Hash sur le hachage de fichier renvoyé lors de l’&quot;étape 1&quot;, car cela nous permet de déterminer le fichier à utiliser lors de la création de votre BAT.

Si vous vous connectez maintenant à votre compte, vous verrez le BAT.

## Comment créer mon premier BAT d’instantané web ?

Il s’agit de deux étapes simples :

**Étape 1** : si vous n’avez pas encore d’ID de session, obtenez-en un à l’aide des méthodes doLogin() ou getSessionID() . Utilisez la première pour vous connecter à l’aide de l’adresse électronique et du mot de passe d’un utilisateur ou la seconde méthode si vous disposez de l’adresse électronique et du jeton d’authentification de l’utilisateur.

**Étape 2 :**Il est maintenant temps de créer votre BAT. Utilisez la méthode createProof() et envoyez-nous au moins les champs requis (il n’y en a actuellement que 5). Assurez-vous de définir le paramètre Hash sur &quot;web&quot; et le paramètre SourceName comme URL de la page web que vous souhaitez capturer.

Si vous vous connectez maintenant à votre compte, vous verrez le BAT.

## Quelle est la différence entre un bon à tirer et une version ?

Dans Workfront Proof, les versions s’affichent sous la forme d’un BAT unique. Cliquez sur une version spécifique de l’interface utilisateur web pour afficher les détails de cette version. En réalité, chaque version est un bon à tirer distinct et l’interface utilisateur Web les affiche ensemble.

Du point de vue de l’API, chaque version est un bon à tirer distinct et les bons à tirer sont liés par leurs identifiants.

**createProof()** crée toujours **version 1** du BAT. Supposons que, dans notre exemple, l’identifiant renvoyé pour ce BAT &quot;100&quot; soit.

Lors de l’utilisation de **createProofVersion()**, envoyez toujours l’identifiant de la version précédente. Si nous voulons créer **version 2** sur le BAT &quot;100&quot;, nous **transmettons &quot;100&quot; pour le paramètre ParentFileID** . Cela indique au système que ce BAT doit être la version 2 de l’ensemble. La méthode renvoie un identifiant de BAT unique. Par exemple, supposons qu’il s’agisse de &quot;101&quot;.

Si une troisième version, c&#39;est-à-dire **version 3**, vous devrez à nouveau appeler **createProofVersion()** et cette fois **transmettre &quot;101&quot; pour le ParentFileID** qui assurera que la liste liée des versions est correctement créée.

## Dois-je obtenir un nouvel ID de session avant chaque appel ?

Il est important de souligner que chaque ID de session est essentiellement un utilisateur exécutant les actions. 

Vous n’avez pas besoin d’obtenir un nouvel ID de session avant chaque appel à l’API et il restera valide pendant 24 heures. Le délai d’expiration est réinitialisé chaque fois que vous effectuez un appel vers l’API.

## Qu’est-ce qu’un BAT / une URL personnelle ?

**Team/Public** : chaque version de BAT possède une URL d’équipe (publique) unique. S’il est activé, le BAT s’ouvre en mode lecture seule. Vous pouvez obtenir l’URL de l’équipe à l’aide de la méthode [getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html) .

**Personnelle** : une URL personnelle est unique pour chaque réviseur et version de BAT. Si un jeu de BAT contient 3 versions et qu’un validant se trouve sur toutes les versions, le validant aura 3 URL personnelles uniques. Une URL personnelle ouvre la version du BAT avec le validant déjà identifié et doit donc être sécurisé et ne pas être partagé. Vous pouvez obtenir des URL personnelles en appelant la méthode [getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html) , puis en effectuant une itération sur chaque  [SOAPRecepientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html) et obtention du paramètre &quot;proof_url&quot;.

## >Comment inclure des paramètres personnalisés lors de l’ouverture de l’épreuve de miniature ?

L’épreuve en miniature vous permet d’incorporer l’outil de vérification dans votre propre page. Un paramètre &quot;referer&quot; peut être inclus dans le fichier minima afin de fournir une URL de redirection lorsqu’un utilisateur clique sur le bouton de fermeture dans le fichier minima. Vous pouvez inclure un certain nombre de paramètres personnalisés dans cette URL de redirection en les ajoutant à l’aide du caractère &quot;&amp;&quot; échappé, par exemple %26.

Par exemple, l’URL infaillible
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` doit être codé en tant que 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` pour que les paramètres personnalisés soient transmis.

## Comment créer un client de service Web Java ?

[Cette vidéo](https://screencast.com/t/xsSNrqs5b) explique comment créer un client de service Web Java à l’aide d’Eclipse et de la définition WSDL Workfront Proof.

