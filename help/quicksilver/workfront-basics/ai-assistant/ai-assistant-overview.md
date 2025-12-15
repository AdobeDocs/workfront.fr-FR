---
title: Assistant AI dans Workfront
content-type: reference
description: En savoir plus sur l’assistant IA dans Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: 44db621643c76ab1f2c1b51d5e81cb0d1f827a58
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 7%

---

# Assistant AI dans Workfront

L’assistant d’IA de Workfront vous aide à accomplir votre travail en offrant des informations et des suggestions in-app dans une conversation en langage naturel. AI Assistant peut vous offrir une expérience de travail plus fluide en :

* Résumé des éléments de travail ou des documents
* Trouver des instructions ou des documents de référence pour les processus de travail
* Génération ou vérification de formules pour les champs calculés

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td><p>Nouveau : Tous</p>
       <p>ou</p>
       <p>Current: Not available</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Current: Not available</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables pour l’assistant AI

Pour activer l’assistant AI pour votre entreprise, **toutes** les conditions suivantes doivent être remplies :

* Votre organisation doit avoir migré vers Adobe IMS (système Identity Management)
* L’expérience unifiée Adobe doit être activée
* Votre organisation doit disposer d’un plan Select, Prime ou Ultimate Workfront
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans le fichier .

  Pour plus d’informations sur la signature du contrat, voir [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) dans cet article.

## Considérations relatives à l’assistant AI

* L’assistant AI est contextuel par rapport à la page que vous avez ouverte. Par exemple, la saisie de « Résumer ce projet » dans l’assistant AI sur une page de projet renvoie un résumé de ce projet spécifique.
* L’administrateur Workfront doit activer l’assistant AI pour les utilisateurs de votre entreprise. L’assistant AI est activé par le biais des niveaux d’accès.

  Pour plus d’informations, voir [Activer ou désactiver l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L’assistant AI Planning Workfront dispose de fonctionnalités différentes de l’assistant AI Workfront.

  Pour plus d’informations sur l’assistant AI dans Workfront Planning, consultez [Présentation de l’assistant AI Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* L’assistant AI n’est actuellement disponible qu’en anglais.


## Fonctionnalité disponible dans l’assistant d’IA

L’assistant AI offre actuellement les fonctionnalités suivantes :

* Résumer des projets, tâches, événements ou documents.

  Pour plus d’informations, voir [Résumer à l’aide de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* en fournissant des instructions ou des informations de référence extraites de la documentation de Workfront sur Adobe Experience League.

  Pour plus d’informations, voir [Obtenir de l’aide de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Recherche d’éléments spécifiques dans Workfront.

  Pour plus d’informations, voir [Utiliser l’assistant AI pour travailler avec des projets, des tâches et des événements](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Générer ou affiner des formules pour les champs calculés personnalisés.

  >[!NOTE]
  >
  >Cette fonctionnalité n’est disponible que pour les organisations qui disposent de plans Prime ou Ultimate Workfront.

  Pour plus d’informations, voir [Générer ou réviser des formules de champs calculés avec l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Résumant les mises à jour, les documents chargés et les autres modifications notables concernant vos projets dans les délais suivants : 24 heures, 3 jours, 7 jours dans Priorités.

Pour de plus amples renseignements, voir [Rattrapage du travail dans Priorités](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Types d’objet disponibles pour l’assistant AI

L’assistant AI peut interroger les données associées aux types d’objets suivants si l’utilisateur dispose des autorisations valides dans Workfront :

* Portefeuilles
* Programmes
* Projets
* Tâches
* Problèmes
* Formulaires personnalisés
* Utilisateurs et utilisatrices
* Enregistrements Workfront Planning


## Accéder à l’assistant IA

1. En haut d’une page Workfront, cliquez sur l’icône de l’assistant AI ![icône de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Saisissez votre question ou votre invite dans le panneau situé à droite de l’écran.

   Si vous ne pouvez pas saisir du texte dans ce panneau, cela signifie que votre entreprise ne dispose pas d’un contrat Adobe Gen AI signé dans ce fichier.

1. Si l’assistant AI ne fournit pas la réponse dont vous avez besoin, affinez votre invite et réessayez.

## Signer le contrat Adobe Gen AI

Si votre organisation ne dispose pas d’un contrat Adobe Gen AI signé, l’assistant AI ne peut pas être activé pour votre organisation.

Si un utilisateur tente d’utiliser l’assistant AI alors que le contrat Adobe Gen AI n’a pas été signé, un message s’affiche :

* Utilisateurs : les utilisateurs sont informés que l’assistant AI n’a pas été activé pour leur organisation et qu’ils peuvent contacter leur administrateur Workfront pour en faire la demande.
* Administrateurs : les administrateurs sont informés qu’il n’existe pas de contrat Adobe Gen AI signé et peuvent demander qu’une copie du contrat soit envoyée pour signature.

Pour demander le contrat Adobe Gen AI :

1. En tant qu’administrateur Workfront, cliquez sur l’icône de l’assistant AI ![icône de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Commencez la saisie dans le panneau de l’assistant d’IA.
1. Lorsque le message du contrat Adobe Gen AI s’affiche, cliquez sur **Vérifier le contrat**.
1. Saisissez le nom et l’adresse e-mail de la personne de votre entreprise qui signera le contrat Adobe Gen AI.

   L&#39;accord sera envoyé à cette personne pour signature. Une fois signé et renvoyé, le contrat est examiné par Adobe, puis l’assistant AI est activé pour votre organisation.

   >[!NOTE]
   >
   >Veuillez patienter 1 à 3 jours ouvrables après la signature et le renvoi du contrat pour qu’Adobe examine et active l’assistant AI.

## Conseils pour la création d’invites dans l’assistant AI

Utilisez les mots-clés suivants dans vos invites pour fournir du contexte et aider à localiser les informations correctes. Les mots-clés ne respectent pas la casse.

Lorsque vous saisissez votre invite, incluez l’expression `using (keyword)`.

| Mot-clé | Effet |
|---|---|
| `workfront` | Interagit avec Workfront. |
| `planning` | Interagit avec Workfront Planning. |
| `help` | Renvoie des informations issues de la documentation Experience League. |
| `formula` | Vérifie et renvoie les formules à utiliser dans Planning, Setup ou les formulaires personnalisés. |
| `health` | Vérifie l’intégrité du projet auprès du conseiller d’intégrité du projet. |
| `summarize` | Affiche un résumé des éléments, par exemple lors du chargement d’un fichier ou de la synthèse d’un projet. |

>[!NOTE]
>
> Tous les mots-clés ne sont pas disponibles dans toutes les zones.
>
>* Le mot-clé `formula` est disponible uniquement dans Planning, Setup et le créateur de formulaires personnalisés.
>* Le mot-clé `planning` est disponible uniquement dans Workfront Planning.





