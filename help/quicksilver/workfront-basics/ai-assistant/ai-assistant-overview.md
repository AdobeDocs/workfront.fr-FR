---
title: Assistant IA dans Workfront
content-type: reference
description: En savoir plus sur l’assistant IA dans Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 100%

---

# Assistant IA dans Workfront

L’assistant IA de Workfront vous aide à accomplir votre travail en offrant des informations et des suggestions in-app dans une conversation en langage naturel. L’assistant IA peut vous offrir une expérience de travail plus fluide grâce aux fonctionnalités suivantes :

* Résumé des éléments de travail ou des documents
* Recherche d’instructions ou de documents de référence pour les processus de travail
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
       <p>Actuel : non disponible</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : non disponible</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables pour l’assistant IA

Pour activer l’assistant IA pour votre organisation, **toutes** les conditions suivantes doivent être remplies :

* Votre organisation doit avoir migré vers Adobe IMS (système de gestion des identités).
* L’expérience unifiée Adobe doit être activée.
* Votre organisation doit disposer d’un plan Workfront Select, Prime ou Ultimate.
* Adobe doit disposer d’un contrat Adobe Gen AI signé.

  Pour plus d’informations sur la signature du contrat, voir [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) dans cet article.

## Considérations relatives à l’assistant IA

* L’assistant IA est sensible au contexte de la page que vous avez ouverte. Par exemple, la saisie de « Résumer ce projet » dans l’assistant IA sur une page de projet renvoie un résumé de ce projet spécifique.
* L’administration Workfront doit activer l’assistant IA pour les personnes de votre organisation. L’assistant IA est activé par le biais des niveaux d’accès.

  Pour plus d’informations, voir [Activer ou désactiver l’assistant IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L’assistant IA Workfront Planning dispose de fonctionnalités différentes de l’assistant IA Workfront.

  Pour plus d’informations sur l’assistant IA dans Workfront Planning, consultez la [Vue d’ensemble de l’assistant IA Adobe Workfront Planning](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* L’assistant IA n’est actuellement disponible qu’en anglais.


## Fonctionnalités disponibles dans l’assistant IA

L’assistant IA offre actuellement les fonctionnalités suivantes :

* Résumer des projets, tâches, problèmes ou documents.

  Pour plus d’informations, voir [Résumer à l’aide de l’assistant IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Instructions ou informations de référence extraites de la documentation Workfront sur Adobe Experience League.

  Pour plus d’informations, voir [Obtenir de l’aide de l’assistant IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Recherche d’éléments spécifiques dans Workfront.

  Pour plus d’informations, voir [Utilisation de l’assistant IA pour travailler sur des projets, des tâches et des problèmes](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Génération ou amélioration des formules pour les champs calculés personnalisés.

  >[!NOTE]
  >
  >Cette fonctionnalité n’est disponible que pour les organisations qui disposent de plans Workfront Prime ou Ultimate.

  Pour plus d’informations, voir [Générer ou réviser des formules de champs calculés avec l’assistant IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Synthèse des mises à jour, documents chargés et autres modifications notables concernant vos projets dans les délais suivants : 24 heures, 3 jours, 7 jours dans Priorités.

Pour plus d’informations, voir [Rattrapage du travail dans Priorités](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Types d’objet disponibles pour l’assistant IA

L’assistant IA peut interroger les données associées aux types d’objets suivants si la personne dispose des autorisations valides dans Workfront :

* Portefeuilles
* Programmes
* Projets
* Tâches
* Problèmes
* Formulaires personnalisés
* Utilisateurs et utilisatrices
* Enregistrements Workfront Planning


## Accéder à l’assistant IA

1. En haut d’une page Workfront, cliquez sur l’icône de l’assistant IA ![icône de l’assistant IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Saisissez votre question ou votre prompt dans le panneau situé à droite de l’écran.

   Si vous ne pouvez pas saisir du texte dans ce panneau, cela signifie que votre organisation ne dispose pas d’un contrat Adobe Gen AI signé.

1. Si l’assistant IA ne fournit pas la réponse dont vous avez besoin, rédigez un prompt plus précis et réessayez.

## Signature du contrat Adobe Gen AI

Si votre organisation ne dispose pas d’un contrat Adobe Gen AI signé, l’assistant IA ne peut pas être activé pour votre organisation.

Si un utilisateur ou une utilisatrice tente d’utiliser l’assistant IA alors que le contrat Adobe Gen AI n’a pas été signé, un message s’affiche :

* Utilisateurs et utilisatrices : ils sont informés que l’assistant IA n’a pas été activé pour leur organisation et qu’ils peuvent contacter leur administrateur ou administratrice Workfront pour en faire la demande.
* Administrateurs et administratrices : ils sont informés qu’il n’existe aucun contrat Adobe Gen AI signé et peuvent demander qu’une copie du contrat soit envoyée pour signature.

Pour demander le contrat Adobe Gen AI :

1. En tant qu’administrateur ou administratrice Workfront, cliquez sur l’icône de l’assistant IA ![icône de l’assistant IA](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Commencez la saisie dans le panneau de l’assistant IA.
1. Lorsque le message du contrat Adobe Gen AI s’affiche, cliquez sur **Examiner le contrat**.
1. Saisissez le nom et l’adresse e-mail de la personne de votre organisation qui va signer le contrat Adobe Gen AI.

   Le contrat sera envoyé à cette personne pour signature. Une fois signé et renvoyé, le contrat est examiné par Adobe, puis l’assistant IA est activé pour votre organisation.

   >[!NOTE]
   >
   >La vérification du contrat par Adobe et l’activation de l’assistant IA peuvent prendre 1 à 3 jours ouvrables après la signature et le renvoi du contrat.

## Conseils pour la création de prompts dans l’assistant IA

Utilisez les mots-clés suivants dans vos prompts pour fournir du contexte et aider à localiser les bonnes informations. Les mots-clé ne sont pas sensibles à la casse.

Lorsque vous saisissez votre prompt, incluez l’expression `using (keyword)`.

| Mot-clé | Effet |
| --- | --- | 
| `workfront` | Interagit avec Workfront. |
| `planning` | Interagit avec Workfront Planning. |
| `help` | Renvoie des informations issues de la documentation Experience League. |
| `formula` | Vérifie et renvoie les formules à utiliser dans la planification, la configuration ou les formulaires personnalisés. |
| `health` | Vérifie l’intégrité du projet auprès du conseiller d’intégrité du projet. |
| `summarize` | Affiche un résumé des éléments, par exemple lors du chargement d’un fichier ou de la synthèse d’un projet. |

>[!NOTE]
>
> Tous les mots-clés ne sont pas disponibles dans toutes les zones.
>
>* Le mot-clé `formula` est disponible uniquement dans la planification, la configuration et le créateur de formulaires personnalisés.
>* Le mot-clé `planning` est disponible uniquement dans Workfront Planning.





