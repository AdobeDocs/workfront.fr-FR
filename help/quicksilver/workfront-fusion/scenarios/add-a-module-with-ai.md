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
source-git-commit: 67e1d158b09ca339d25473ebedf8851155b2c1c0
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 3%

---

# Génération d’un segment de scénario à l’aide d’AI

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Cette fonctionnalité étant disponible dans Beta, elle est réservée à certains utilisateurs de Workfront.

Vous pouvez utiliser l’IA pour saisir une invite de texte décrivant ce que vous avez besoin d’une section de votre scénario. Fusion génère ensuite des modules qui exécuteront ces actions, que vous pouvez utiliser dans votre scénario.

Comme pour tout élément généré à partir de l’IA, nous vous recommandons de vérifier et de tester deux fois les modules générés pour vous assurer qu’ils fonctionnent comme prévu.

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

## Génération de modules

1. Commencez à ajouter un module et sélectionnez **Générer avec l’IA** dans la liste des applications.

   Ou

   Cliquez sur l’icône ![Générer avec l’IA](assets/generate-with-ai-icon-beta.png) de l’icône de génération avec l’IA près du bas de la page de l’éditeur de scénarios.

   Le panneau Assistant d’IA s’ouvre.
1. Saisissez une invite de texte dans la zone.

   Pour obtenir des conseils sur les invites, reportez-vous à la section [Conseils pour créer des invites de texte](#tips-for-creating-text-prompts) de cet article.

   Le module ou l’ensemble de modules est généré.
1. (Conditionnel) Si nécessaire, ajoutez votre jeton API pour l’application dans les modules.
1. Vérifiez les modules pour vous assurer qu’ils doivent être configurés pour l’application et l’action appropriées.
1. (Conditionnel) Si la section de scénario générée n’est pas jointe à votre scénario, faites-la glisser vers sa place.

Nous vous recommandons de tester les modules pour vous assurer qu’ils fonctionnent comme prévu.

## Conseils pour créer des invites de texte

Les invites de texte doivent inclure au minimum les informations suivantes :

* Application à laquelle vous vous connectez
* Action ou actions à effectuer

>[!IMPORTANT]
>
>Vous pouvez générer plusieurs modules à la fois, mais vous ne pouvez générer que des modules pour une application à la fois.

>[!INFO]
>
>**Exemples** :
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Cela inclut l&#39;application `Workfront Planning` et l&#39;action `delete records`. Cette invite crée trois modules, un pour chaque enregistrement qui sera supprimé.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Cela inclut l&#39;application `Workfront Planning` et l&#39;action `change campaign summary`.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Cela inclut l&#39;application `Workfront Planning` et l&#39;action `get field details`.
>
>L’exemple suivant n’est PAS correct :
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Cet exemple est incorrect car il comprend plusieurs applications.

Tenez compte des points suivants lors de la création d’invites de texte :

* Utilisez un langage direct et simple.
* Vérifiez et testez vos modules. S’il ne fonctionne pas comme prévu, affinez votre invite et réessayez.
