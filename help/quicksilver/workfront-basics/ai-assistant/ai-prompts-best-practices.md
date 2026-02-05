---
title: Invites de l’assistant AI et bonnes pratiques
content-type: reference
description: Découvrez les bonnes pratiques relatives à l’utilisation de l’assistant AI et consultez une liste d’exemples d’invites.
author: Jenny
feature: Get Started with Workfront
exl-id: 34a60482-e060-49f9-bbaf-8aed85845e26
source-git-commit: dc472e93541641ee1c960ec7246365200f522a17
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 4%

---

# Invites de l’assistant AI et bonnes pratiques

L’assistant d’IA Workfront est un outil puissant qui peut vous aider à accomplir votre travail plus efficacement en fournissant des informations utiles sur vos données de compte et des types d’objets spécifiques.

Dans cet article, vous découvrirez les bonnes pratiques actuelles pour l’assistant AI, notamment comment écrire des invites claires, sur quels types d’objets vous pouvez demander des informations et comment accéder à des ressources supplémentaires pour vérifier les informations si nécessaire.

Pour plus d’informations sur l’assistant AI, voir [Présentation de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

>[!NOTE]
>
>À mesure que les fonctionnalités de l’assistant AI évolueront, le type de requêtes et de questions que vous pourrez lui poser augmentera. Nous vous recommandons de lire cet article à mesure que de nouvelles fonctionnalités d’assistant AI sont publiées pour en savoir plus sur les invites disponibles que vous pouvez utiliser.


## Types d’objet disponibles pour l’assistant AI

L’assistant AI peut fournir des données pour les types d’objets suivants :

* Portefeuilles
* Programmes
* Projets
* Tâches
* Problèmes
* Formulaires personnalisés
* Utilisateurs et utilisatrices
* Enregistrements Workfront Planning

>[!NOTE]
>
>Vous devez disposer de l’autorisation nécessaire dans votre niveau d’accès pour un objet avant de pouvoir demander ses données à l’assistant AI.

## Bonnes pratiques

### Entrer des invites claires

Pour accéder aux informations les plus utiles de l’assistant AI, il est important de créer des invites qui vous donnent la réponse que vous recherchez. La liste suivante contient des principes qui peuvent vous aider à formuler au mieux les invites appropriées :

* **Utilisez un langage clair et spécifique** : en évitant les invites vagues et générales, l&#39;assistant AI sera mieux à même de vous guider vers les données que vous essayez de recevoir.
* **N’inclure pas de délais** : donner des délais spécifiques à l’assistant d’IA pour un objet permettra de réduire les données à traiter et donnera lieu à des informations plus ciblées dans sa réponse.
* **Ne demandez qu’une seule chose à la fois** : lorsque plusieurs requêtes non liées sont incluses dans une seule invite, l’assistant AI ne sera pas en mesure de fournir les informations appropriées.

Pour plus d’informations sur les invites recommandées, consultez la section suivante de cet article : [Exemples d’invites](#prompt-examples).


### Vérifier les réponses de l’assistant AI

À ce stade du développement de l’assistant AI, il est recommandé de vérifier les informations fournies lors de la demande d’informations sur les processus Workfront. Pour ce faire, cliquez sur le lien de l’article fourni dans la section Sources de la réponse de l’invite.

![Section Sources](assets/sources-section.png)

Pour plus d’informations sur les invites pour les processus Workfront, voir [Invites pour en savoir plus sur les actions Workfront](#prompts-to-learn-about-workfront-actions) dans cet article.


## Exemples de prompts

Les tableaux ci-dessous contiennent des exemples d’invites que vous pouvez utiliser pour générer des informations sur votre travail et en savoir plus sur les processus ou actions Workfront spécifiques que vous souhaitez effectuer.

### Invites pour trouver des informations sur votre travail

<table>
    <tr>
        <td><b>Type d’objet</b></td>
        <td><b>Invite</b></td>
    </tr>
        <tr>
        <td>Projets</td>
        <td><em>Quelle est la date d'échéance de [NOM DU PROJET] ?</em>
        </td>
    </tr>
    <tr>
        <td>Projets</td>
        <td><em>Quel est le statut de [PROJECT NAME] ?</em>
        </td>
    </tr>
    <tr>
        <td>Projets </td>
        <td><em>Qui est le propriétaire du projet pour [PROJECT NAME] ?</em></td>
    </tr>
    <tr>
        <td>Tâches</td>
        <td><em>Quelles tâches me sont assignées cette semaine ?</em></td>
    </tr>
       <tr>
        <td>Problèmes </td>
        <td><em>Quels événements ouverts sont affectés à mon équipe ?</em></td>
           <tr>
        <td>Utilisateurs et utilisatrices</td>
        <td><em>Qui fait partie de l'équipe créative de [NOM DU PROJET] ?</em></td>
    </tr>
           <tr>
        <td>Utilisateurs et utilisatrices </td>
        <td><em>Combien de tâches sont affectées à [USER] ?</em></td>
    </tr>
   </table>


### Invites pour en savoir plus sur les actions de Workfront

<table>
    <tr>
        <td><b>Type d’objet</b></td>
        <td><b>Invite</b></td>
    </tr>
    <tr>
        <td>Projets</td>
        <td><em>Comment créer un projet à partir d’un modèle ?</em>
        </td>
    </tr>
    <tr>
        <td>Projets </td>
        <td><em>Quelle est la différence entre un projet et un programme ?</em></td>
    </tr>
    <tr>
        <td>Tâches</td>
        <td><em>Comment affecter une tâche à plusieurs utilisateurs ?</em></td>
    </tr>
       <tr>
        <td>Tâches</td>
        <td><em>Que signifie le statut Prêt à démarrer ?</em></td>
    </tr>
       <tr>
        <td>Problèmes </td>
        <td><em>Comment convertir une demande en tâche ?</em></td>
    </tr>
           <tr>
        <td>Problèmes </td>
        <td><em>Quel est le cycle de vie d’un problème dans Workfront ?</em></td>
    </tr>
        </tr>
           <tr>
        <td>Problèmes </td>
        <td><em>Comment escalader une demande ?</em></td>
    </tr>
           <tr>
        <td>Documents</td>
        <td><em>Comment télécharger une nouvelle version d’un document ?</em></td>
    </tr>
           <tr>
        <td>Documents </td>
        <td><em>Puis-je définir des workflows d'approbation de document ?</em></td>
    </tr>
   </table>


## Limites actuelles de l’assistant AI

L’assistant d’IA est un outil puissant, mais il existe certains types de questions et de demandes pour lesquelles il ne peut pas fournir de données à ce stade de développement. Le tableau ci-dessous contient des exemples d’invites pour lesquelles l’assistant IA ne peut pas afficher de données.

<table>
    <tr>
        <td><b>Type d’invite</b></td>
        <td><b>Exemple</b></td>
    </tr>
    <tr>
        <td>Questions sur les configurations personnalisées</td>
        <td><em>Quelle logique d’intégration personnalisée est en cours d’exécution dans votre instance Workfront ?</em>
        </td>
    </tr>
    <tr>
        <td>Questions relatives aux données en dehors de Workfront </td>
        <td><em>Pouvez-vous me montrer mon calendrier Outlook pour aujourd'hui ?</em></td>
    </tr>
             <tr>
        <td>Questions relatives aux produits Adobe non intégrés </td>
        <td><em>Comment modifier un PDF dans Acrobat à partir d’ici ?</em></td>
         <tr>
        <td>Questions qui nécessitent un jugement humain</td>
        <td><em>Ce projet devrait-il être suspendu ?</em></td>
    </tr>
    </tr>
       <tr>
        <td>Demandes de mises à jour en bloc</td>
        <td><em>Réaffectez toutes les tâches en retard pour [USER].</em></td>
    </tr>
       <tr>
        <td>Demandes d’analyse prédictive</td>
        <td><em>Proposez un nouveau plan de projet basé sur nos données historiques.</em></td>
    </tr>
           <tr>
        <td>Demandes d’informations au-dessus de votre niveau d’accès</td>
        <td><em>Répertoriez tous les taux de facturation du compte.</em></td>
    </tr>
           <tr>
        <td>Demandes contenant des informations vagues </td>
        <td><em>Réparer mon projet.</em></td>
    </tr>
   </table>
