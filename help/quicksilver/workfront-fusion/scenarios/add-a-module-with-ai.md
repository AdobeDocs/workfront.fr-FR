---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Générer un module à l’aide de l’AI
description: Vous pouvez saisir une invite de texte pour créer un module HTTP configuré à l’invite.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: fe096ba36da9b56e0e38f6061481b66cfbeee5c6
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 5%

---

# Générer un module à l’aide de l’AI

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Cette fonctionnalité n’étant encore qu’au début du développement, elle est disponible que pour les utilisateurs Workfront internes.

Vous pouvez utiliser l’IA pour saisir une invite de texte décrivant ce que vous devez faire avec un module. Fusion génère ensuite un module HTTP qui se connecte au point de terminaison correct de l’API souhaitée.

Comme pour tout élément généré à partir de l’IA, nous vous recommandons de vérifier et de tester deux fois le module généré pour vous assurer qu’il fonctionne comme prévu.

## Applications de module AI actuellement prises en charge

Fusion AI peut actuellement générer des modules qui se connectent aux applications suivantes :

* Adobe Firefly
* Azure OpenAI
* Graphique Microsoft
* Planification d’Adobe Workfront
* Adobe Analytics
* Services Adobe PDF
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

1. Ajoutez un module et sélectionnez **Générer avec l’IA** dans la liste des applications.

   Ou

   Cliquez avec le bouton droit de la souris sur une zone vide de l’éditeur de scénarios, puis sélectionnez **Générer avec l’IA**.
1. Saisissez une invite de texte dans la zone.

   Pour obtenir des conseils sur les invites, reportez-vous à la section [Conseils pour créer des invites de texte](#tips-for-creating-text-prompts) de cet article.
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
>**Exemples** :
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   Cela inclut l&#39;application `Google Calendar` et l&#39;action `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Cela inclut l&#39;application `Spotify` et l&#39;action `Retrieve popular songs`.

Tenez compte des points suivants lors de la création d’invites de texte :

* Comme chaque module Fusion effectue une seule action, votre invite de texte doit décrire une action spécifique.
* Utilisez un langage direct et simple.
* Vérifiez et testez votre module. S’il ne fonctionne pas comme prévu, affinez votre invite et réessayez.
