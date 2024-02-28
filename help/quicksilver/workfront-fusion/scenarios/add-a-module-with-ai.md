---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Génération d’un module à l’aide d’AI
description: Vous pouvez saisir une invite de texte pour créer un module HTTP configuré à l’invite.
author: Becky
feature: Workfront Fusion
source-git-commit: c80f9ab6d10aa9067b995c99107f98301fa17872
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# Génération d’un module à l’aide d’AI

<!--DO NOT DELETE - linked through CSH-->

Vous pouvez utiliser l’IA pour saisir une invite de texte décrivant ce que vous devez faire avec un module. Fusion génère ensuite un module HTTP qui se connecte au point de terminaison correct de l’API souhaitée.

Comme pour tout élément généré à partir de l’IA, nous vous recommandons de vérifier et de tester deux fois le module généré pour vous assurer qu’il fonctionne comme prévu.

## Applications de module AI actuellement prises en charge

Fusion AI peut actuellement générer des modules qui se connectent aux applications suivantes :

* Adobe Maestro
* Adobe Analytics
* Services Adobe PDF
* Adobe Marketo
* Adobe de Frame.io
* Dropbox
* NetSuite
* Calendrier Google
* Atlassian Jira
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## Génération d’un module

1. Ajoutez un module et sélectionnez **Génération avec l’IA** dans la liste des applications.

   Ou

   Cliquez avec le bouton droit sur une zone vide de l’éditeur de scénarios, puis sélectionnez **Génération avec l’IA**.
1. Saisissez une invite de texte dans la zone.

   Pour obtenir des conseils sur les invites, voir [Conseils pour créer des invites de texte](#tips-for-creating-text-prompts) dans cet article.
1. Ajoutez votre jeton API pour l’application dans le module .
1. Vérifiez le module pour vous assurer qu’il semble être configuré pour l’application et l’action appropriées.
1. (Conditionnel) Si le module n’est pas joint à votre scénario, faites-le glisser sur sa place.

Nous vous recommandons de tester le module pour vous assurer que le module généré fonctionne comme prévu.

## Conseils pour créer des invites de texte

Les invites de texte doivent inclure au minimum les informations suivantes :

* Application à laquelle vous vous connectez
* L’action que vous souhaitez effectuer

>[!INFO]
>
>**Exemples**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   Cela inclut l’application `Google Calendar` et l’action `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Cela inclut l’application `Spotify` et l’action `Retrieve popular songs`.

Tenez compte des points suivants lors de la création d’invites de texte :

* Comme chaque module Fusion effectue une seule action, votre invite de texte doit décrire une action spécifique.
* Utilisez un langage direct et simple.
* Vérifiez et testez votre module. S’il ne fonctionne pas comme prévu, affinez votre invite et réessayez.



