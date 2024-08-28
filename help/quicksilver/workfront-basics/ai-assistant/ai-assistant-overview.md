---
title: "Présentation de l’assistant AI"
content-type: reference
description: Présentation de l’assistant AI
author: Becky
feature: Get Started with Workfront
source-git-commit: 3db36df88d4bb716cf4c37cd76b6d058a5a6f9b6
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 6%

---

# Présentation de l’assistant AI

L’assistant Workfront AI vous aide à accomplir votre travail en proposant des informations et des suggestions dans l’application dans une conversation en langage naturel. L’assistant IA peut vous offrir une expérience professionnelle plus fluide en

* Résumé d’éléments de travail ou de documents
* Trouver des instructions ou du matériel de référence pour les processus de travail
* Génération ou vérification de formules pour les champs calculés

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td><p>Nouveau : Tous</p>
       <p>ou</p>
       <p>Actuel : non disponible</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouvelle : standard</p>
       <p>ou</p>
       <p>Actuel : non disponible</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).## Conditions préalables requises pour l’assistant AI

## Conditions préalables à l’assistant AI

Pour activer l’assistant d’IA pour votre organisation, **tous** des éléments suivants doivent s’appliquer :

* Votre entreprise doit avoir migré vers Adobe IMS (système Identity Management).
* L’option Adobe de l’expérience unifiée doit être activée.
* Votre entreprise doit disposer d’un plan Workfront Select, Prime ou Ultimate.
* L&#39;Adobe doit avoir signé un accord d&#39;Adobe Gen AI sur le fichier

  Pour plus d’informations sur la signature de l’accord, voir [Signature de l’accord Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) dans cet article.

## Remarques concernant l’assistant d’IA

* L’assistant d’IA est sensible au contexte de la page ouverte. Par exemple, la saisie de &quot;Résumer ce projet&quot; dans l’assistant d’IA sur une page de projet renvoie un résumé de ce projet spécifique.
* L’administrateur Workfront doit activer l’assistant d’IA pour les utilisateurs de votre entreprise. L’assistant d’IA est activé via les niveaux d’accès.

  Pour plus d’informations, voir [Activation ou désactivation de l’assistant d’IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L’assistant de planification Workfront AI présente différentes fonctionnalités que l’assistant de planification Workfront AI.

  Pour plus d’informations sur l’assistant d’IA dans la planification Workfront, consultez la [présentation de l’assistant d’API de planification Adobe Workfront](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).


## Fonctionnalités disponibles dans l’assistant AI

L’assistant d’IA propose actuellement les fonctionnalités suivantes :

* Résumé des projets, tâches, problèmes ou documents.

  Pour plus d’informations, voir [Résumer à l’aide de l’assistant d’IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Fournissant des instructions ou des informations de référence extraites de la documentation Workfront sur Adobe Experience League.

  Pour plus d’informations, voir [Obtenir de l’aide à partir de l’assistant d’IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Générer ou affiner des formules pour des champs personnalisés calculés.

  >[!NOTE]
  >
  >Cette fonctionnalité est disponible uniquement pour les organisations des plans Workfront Prime ou Ultimate.

  Pour plus d’informations, voir [Génération ou révision de formules de champ calculé avec l’assistant d’IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

## Accéder à l’assistant AI

1. Dans la partie supérieure de n’importe quelle page Workfront, cliquez sur l’icône de l’assistant d’IA ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Entrez votre question ou une invite dans le panneau situé à droite de l&#39;écran.

   Si vous ne pouvez pas entrer dans ce panneau, votre organisation ne dispose pas d’un contrat d’Adobe Gen AI signé sur le fichier .

1. Si l’assistant d’IA ne répond pas à vos besoins, affinez votre invite et réessayez.

## Signez le contrat Adobe Gen AI

Si votre entreprise ne dispose pas d’un contrat d’Adobe de l’IA dédié au fichier, l’assistant d’IA ne peut pas être activé pour votre entreprise.

Si un utilisateur tente d’utiliser l’assistant d’intelligence artificielle lorsque le contrat d’Adobe d’IA Gen n’a pas été signé, un message s’affiche :

* Utilisateurs : les utilisateurs sont informés que l’assistant d’IA n’a pas été activé pour leur entreprise et qu’ils peuvent contacter leur administrateur Workfront pour le demander à leur entreprise.
* Administrateurs : les administrateurs sont informés qu’il n’existe pas de contrat Adobe Gen AI signé et peuvent demander qu’une copie de ce contrat soit envoyée pour signature.

Pour demander le contrat d’Adobe Gen AI :

1. En tant qu’administrateur Workfront, cliquez sur l’icône de l’assistant d’IA ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Commencez à saisir dans le panneau Assistant d’IA.
1. Lorsque le message d’accord Adobe Gen AI s’affiche, cliquez sur **Réviser l’accord**.
1. Saisissez le nom et l’adresse électronique de la personne de votre entreprise qui signera le contrat Adobe Gen AI.

   La convention sera alors transmise à cette personne pour signature. Une fois signé et renvoyé, l’assistant d’IA est activé pour votre entreprise.

