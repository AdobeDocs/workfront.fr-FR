---
title: Questions fréquentes sur l’API SOAP
description: Questions fréquentes sur l’API SOAP
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 79b6370ec3283922a16435e8eb8069f7f9560c55
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 100%

---

# Questions fréquentes sur l’API SOAP

## Comment créer ma première épreuve de fichier ?

Il suffit de trois étapes simples :

**Étape 1** : chargez le fichier sur Workfront Proof en l’envoyant via une requête POST à [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Nous vous renverrons le hachage du fichier, c’est très important ! Notez qu’à ce stade, vous ne verrez rien sur votre compte, car vous n’avez fait que nous envoyer le fichier sans nous dire ce qu’il fallait en faire.

**Étape 2** : si vous n’avez pas encore d’identifiant de session, obtenez-en un en utilisant les méthodes doLogin() ou getSessionID(). Utilisez la première méthode pour vous « connecter » à l’aide de l’adresse e-mail et du mot de passe de l’utilisateur ou utilisatrice, ou la seconde si vous disposez de l’adresse e-mail et du jeton d’authentification de l’utilisateur ou utilisatrice.

**Étape 3 :** il est maintenant temps de créer votre épreuve. Utilisez la méthode createProof() et envoyez-nous au moins les champs obligatoires (actuellement, il n’y en a que 5). Veillez à ce que le paramètre Hachage corresponde au hachage du fichier renvoyé lors de l’étape 1, car cela nous permet de déterminer le fichier à utiliser lors de la création de votre épreuve.

Si vous vous connectez maintenant à votre compte, vous verrez l’épreuve.

## Comment créer ma première épreuve instantanée web ?

Il suffit de suivre deux étapes simples 

**Étape 1** : si vous n’avez pas encore d’identifiant de session, obtenez-en un en utilisant les méthodes doLogin() ou getSessionID(). Utilisez la première méthode pour vous « connecter » à l’aide de l’adresse e-mail et du mot de passe de l’utilisateur ou utilisatrice, ou la seconde si vous disposez de l’adresse e-mail et du jeton d’authentification de l’utilisateur ou utilisatrice.

**Étape 2 :**il est maintenant temps de créer votre épreuve. Utilisez la méthode createProof() et envoyez-nous au moins les champs obligatoires (actuellement, il n’y en a que 5). Veillez à définir le paramètre Hachage sur « web » et le paramètre SourceName en tant qu’URL de la page web que vous souhaitez capturer.

Si vous vous connectez maintenant à votre compte, vous verrez l’épreuve.

## Quelle est la différence entre une épreuve et une version ?

Dans Workfront Proof, les versions sont affichées comme une seule épreuve. En cliquant sur une version spécifique dans l’interface utilisateur web, les détails de cette version s’affichent. En réalité, chaque version est une épreuve distincte et l’interface utilisateur web les affiche ensemble.

Du point de vue de l’API, chaque version est une épreuve distincte et les épreuves sont reliées entre elles par leurs identifiants.

**createProof()** créera toujours la **version 1** de l’épreuve. Supposons, pour notre exemple, que l’identifiant renvoyé pour cette épreuve soit « 100 ».

Lorsque vous utilisez **createProofVersion()**, envoyez toujours l’identifiant de la version précédente. Si nous voulons créer la **version 2** sur l’épreuve « 100 », nous **passons « 100 » pour le paramètre ParentFileID**. Cela indique au système que cette épreuve doit être la version 2 de l’ensemble. La méthode renvoie un numéro d’identification d’épreuve unique, pour notre exemple, disons « 101 ».

Si une troisième version, c’est-à-dire la **version 3**, est nécessaire, vous devez appeler à nouveau **createProofVersion()** et, cette fois, **transmettre « 101 » pour le paramètre ParentFileID**, ce qui garantira que la liste liée des versions est correctement créée.

## Dois-je obtenir un nouvel identifiant de session avant chaque appel ?

Il est important de souligner que chaque identifiant de session correspond essentiellement à une personne effectuant les actions. 

Il n’est pas nécessaire d’obtenir un nouvel identifiant de session avant chaque appel API et il restera valide pendant 24 heures. Le délai d’expiration est réinitialisé chaque fois que vous faites un appel API.

## Qu’est-ce qu’une épreuve / URL personnelle ?

**Équipe/Publique** : chaque version d’épreuve a une URL d’équipe (publique) unique. Si cette option est activée, l’épreuve s’ouvrira en mode Lecture seule. Vous pouvez obtenir l’URL de l’équipe en utilisant la méthode [getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html).

**Personnelle** : une URL personnelle est unique pour chaque réviseur et réviseuse, et chaque version d’épreuve. Si un ensemble d’épreuves contient 3 versions et qu’un réviseur ou une réviseuse participe à toutes les versions, cette personne aura 3 URL personnelles uniques. Une URL personnelle ouvre la version d’épreuve avec le réviseur ou la réviseuse déjà identifié et doit donc être conservée en toute sécurité et ne pas être partagée. Les URL personnelles peuvent être obtenues en appelant la méthode [getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html), puis en itérant chaque [SOAPRecepientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html) et en obtenant le paramètre « proof_url ».

## Comment inclure des paramètres personnalisés lors de l’ouverture d’une mini-épreuve ?

La mini-épreuve vous permet d’intégrer l’outil de relecture dans votre propre page. Un paramètre « référent » peut être inclus dans la mini-épreuve afin de fournir une URL de redirection lorsqu’un utilisateur ou une utilisatrice clique sur le bouton de fermeture dans la mini-épreuve. Vous pouvez inclure un nombre illimité de paramètres personnalisés dans cette URL de redirection en les ajoutant à l’aide du caractère d’échappement « &amp; », par exemple %26.

Par exemple, l’URL de mini-épreuve
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` doit être encodée comme
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` pour que les paramètres personnalisés soient transmis.


