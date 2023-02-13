---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Présentation de l’état des objectifs dans les objectifs Adobe Workfront
description: Les statuts des objectifs indiquent si un objectif est principal et enregistre actuellement des progrès, ou s’il est inactif, rédigé ou déjà atteint.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 4%

---

# Présentation de l’état des objectifs dans les objectifs Adobe Workfront

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>Votre entreprise doit disposer des éléments suivants pour utiliser les fonctionnalités décrites dans cet article :
>
>* A Pro ou version ultérieure [Formule Adobe Workfront](https://www.workfront.com/plans).
>* Une licence Adobe Workfront Goals en plus d’une licence Workfront.
>
>Contactez votre gestionnaire de compte Workfront pour en savoir plus sur une licence Workfront Goals.

Pour plus d’informations sur l’accès aux objectifs de Workfront, voir [Conditions requises pour utiliser les objectifs Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


Les statuts des objectifs indiquent si un objectif est principal et enregistre actuellement des progrès, ou s’il est inactif, rédigé ou déjà atteint.

## Considération lors de la mise à jour des états d’objectif dans les objectifs Workfront

* Vous ne pouvez pas mettre à jour manuellement l’état des objectifs que vous avez créés ou qui ont été partagés avec vous. L’état des objectifs est mis à jour en fonction des actions que vous effectuez sur l’objectif. Par exemple, l’activation d’un objectif modifie l’état En création en Principal.
* Certaines restrictions existent et, parfois, vous ne pouvez pas modifier l’état d’un objectif en un autre état, selon les règles suivantes :

   | De/À | Brouillon | Actif | Inactif | Fermé |
   |---|---|---|---|---|
   | Brouillon | - | Oui | Non | Non |
   | Actif | Non | - | Oui | Oui |
   | Inactif | Non | Oui | - | Non |
   | Fermé | Non | Oui | Non | - |

* L’ouverture d’un objectif fermé met également à jour la progression de l’objectif.
* Certaines actions que vous effectuez sur un objectif mettent également à jour son état. Pour plus d’informations sur la mise à jour des états d’objectif, reportez-vous aux articles suivants :

   * [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
   * [Activation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md)
   * [Suppression et désactivation d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Fermer et rouvrir les objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Présentation des états d’objectif dans les objectifs Workfront

Pour plus d’informations sur la création d’objectifs Workfront, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Pour plus d’informations sur l’activation des objectifs, voir [Activation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

Les objectifs peuvent avoir l’un des états suivants dans les objectifs Workfront :

* [Brouillon](#draft)
* [Actif](#active)
* [Inactif](#inactive)
* [Fermé](#closed)

### Brouillon {#draft}

* Il s’agit de l’état par défaut d’un objectif nouvellement créé. Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* Les objectifs de Workfront n’enregistrent pas de progrès sur un objectif ébauché.
* Vous ne pouvez pas mettre à jour la progression d’un objectif brouillé.
* Vous ne pouvez pas fermer ou désactiver les objectifs préliminaires car ils manquent d’informations sur la progression.
* Les objectifs élaborés ne contribuent pas au calcul de progression des autres objectifs et ne sont pas pris en compte dans les graphiques.
* Les objectifs préliminaires s’affichent dans les zones suivantes des objectifs Workfront :

   * Liste d’objectifs
   * section Alignement de l’objectif (uniquement en tant qu’objectif aligné)


>[!IMPORTANT]
>
>Après avoir défini l’état d’un objectif sur un autre état, l’objectif ne peut plus jamais être placé dans un état En création .

### Actif {#active}

* Vous ne pouvez activer un objectif en version préliminaire que lorsque vous l’associez à un résultat, à une activité ou que vous lui alignez un autre objectif. L’activation de l’objectif passe à l’état Principal. Pour plus d’informations sur l’activation des objectifs, voir [Activation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* Les objectifs de Workfront enregistrent la progression par rapport aux objectifs principaux.
* Les objectifs principaux contribuent au calcul de la progression des autres objectifs et sont pris en compte dans les graphiques.
* Les objectifs principaux s’affichent dans les zones suivantes des objectifs de Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs
   * La progression des objectifs principaux s’affiche dans les graphiques.

* Vous pouvez réactiver un objectif Fermé ou Inactif.

### Inactif {#inactive}

* Vous pouvez désactiver un objectif principal lorsque le propriétaire a arrêté de l’utiliser temporairement ou définitivement. Vous pouvez le conserver pour des informations historiques. Cela met à jour l’état de l’objectif en Inactif.

   Pour plus d’informations sur la désactivation des objectifs, reportez-vous à la section &quot;Désactivation des objectifs&quot; de l’article. [Suppression et désactivation d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Vous ne pouvez pas désactiver un objectif brouillon ou fermé.
* Vous pouvez réactiver un objectif inactif et continuer à travailler dessus.
* Les objectifs de Workfront ne calculent pas la progression des objectifs inactifs.
* Vous ne pouvez pas mettre à jour la progression d’un objectif inactif.
* Les objectifs inactifs ne contribuent pas au calcul de progression des autres objectifs et ne sont pas pris en compte dans les graphiques.
* Les objectifs inactifs ont un passé de progrès parce qu&#39;ils étaient autrefois principaux, contrairement aux objectifs préliminaires.
* Les objectifs inactifs s’affichent dans les zones suivantes des objectifs Workfront :

   * Liste d’objectifs
   * section Alignement des objectifs (uniquement en tant qu’objectifs alignés)

### Fermé {#closed}

* Vous pouvez fermer un objectif lorsque vous souhaitez indiquer que vous l’avez atteint ou que vous ne le travaillez plus, et que vous ne le ferez plus à l’avenir. Pour plus d’informations sur la fermeture des objectifs, voir [Fermer et rouvrir les objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >Si vous envisagez de travailler ultérieurement sur un objectif qui n’est pas encore atteint, nous vous recommandons de modifier le statut en Inactif au lieu de Fermé.

* Vous ne pouvez pas fermer des objectifs qui n’ont jamais été activés, comme les objectifs préliminaires.
* Vous pouvez rouvrir un objectif fermé et continuer à travailler dessus.
* Les objectifs de Workfront arrêtent d’enregistrer la progression sur les objectifs fermés.
* Vous ne pouvez pas mettre à jour la progression d’un objectif fermé.
* Les objectifs fermés s’affichent dans la zone suivante des objectifs Workfront :

   * Liste d’objectifs
   * section Alignement des objectifs (uniquement en tant qu’objectifs alignés)
   * Les informations relatives aux objectifs fermés sont également prises en compte dans la section Graphiques .
