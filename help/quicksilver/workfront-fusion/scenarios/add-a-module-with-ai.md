---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Génération d’un segment de scénario à l’aide de l’IA
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 1%

---

# Génération d’un segment de scénario à l’aide de l’IA

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Générer un segment de scénario à l’aide de l’IA](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-module-with-ai.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Cette fonctionnalité étant disponible dans Beta, elle n’est disponible que pour certains utilisateurs et utilisatrices de Workfront.

Vous pouvez utiliser l’IA pour saisir une invite de texte décrivant ce qu’une section de votre scénario doit faire. Fusion génère alors des modules qui exécutent ces actions, que vous pouvez utiliser dans votre scénario.

Comme pour tout ce qui est généré à partir de l’IA, nous vous recommandons de vérifier et de tester les modules générés pour vous assurer qu’ils fonctionnent comme prévu.

## Applications de module d’IA actuellement prises en charge

L’IA dédiée à Fusion peut actuellement générer des modules qui se connectent aux applications suivantes :

* Adobe Firefly
* Azure OpenAI
* Graphique Microsoft
* Planification d’Adobe Workfront
* Adobe Analytics
* Services Adobe PDF
* Adobe Marketo
* Adobe Frame.io
* Dropbox
* NetSuite
* Calendrier Google
* Atlassian Jira
* GitLab
* Spotifier
* Bitbucket
* OpenAI
* Slack

## Génération de modules

1. Commencez à ajouter un module et sélectionnez **Générer avec l’IA** dans la liste des applications.

   Ou

   Cliquez sur l’icône Générer avec l’IA ![Générer avec l’IA](assets/generate-with-ai-icon-beta.png) en bas de la page de l’éditeur de scénarios.

   Le panneau Assistant d’IA s’ouvre.
1. Saisissez une invite de texte dans la zone.

   Pour obtenir des conseils sur les invites, voir [Conseils pour créer des invites de texte](#tips-for-creating-text-prompts) dans cet article.

   L’assistant AI génère le module ou l’ensemble de modules.
1. (Conditionnel) Si nécessaire, ajoutez votre jeton API pour l’application dans les modules.
1. Vérifiez les modules pour vous assurer qu’ils sont configurés pour l’application et l’action appropriées.
1. (Conditionnel) Si la section du scénario généré n’est pas associée à votre scénario, faites-la glisser jusqu’à ce qu’elle soit en place.

Nous vous recommandons de tester les modules pour vous assurer qu’ils fonctionnent comme prévu.

## Conseils pour créer des invites de texte

Les invites de texte doivent inclure au minimum les informations suivantes :

* Application à laquelle vous vous connectez
* Action(s) à effectuer

>[!IMPORTANT]
>
>Vous pouvez générer plusieurs modules à la fois, mais vous ne pouvez générer des modules que pour une seule application à la fois.

>[!INFO]
>
>**Exemples** :
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Cela inclut le `Workfront Planning` de l’application et le `delete records` d’action. Cette invite crée trois modules, un pour chaque enregistrement qui sera supprimé.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Cela inclut le `Workfront Planning` de l’application et le `change campaign summary` d’action.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Cela inclut le `Workfront Planning` de l’application et le `get field details` d’action.
>
>L’exemple suivant n’est PAS correct :
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Cet exemple est incorrect, car il comprend plusieurs applications

Tenez compte des points suivants lors de la création d’invites de texte :

* Utilisez un langage direct et simple.
* Vérifiez et testez vos modules. S’il ne s’exécute pas comme prévu, affinez votre invite et réessayez.
