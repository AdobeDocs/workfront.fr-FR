---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Vue d’ensemble du statut d’objectif dans Objectifs Adobe Workfront
description: Les statuts des objectifs indiquent si un objectif est actif et enregistre actuellement la progression, ou s’il est inactif, rédigé ou déjà atteint.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 6%

---

# Vue d’ensemble du statut d’objectif dans Objectifs Adobe Workfront

>[!IMPORTANT]
>
>Votre entreprise doit disposer des éléments suivants pour utiliser les fonctionnalités décrites dans cet article :
>
>* Pour le nouveau plan et la nouvelle structure de licence :
>
>   * Formule Workfront ultime
>    
>* Pour le plan actuel et la structure de licence :
>
>   * Formule Workfront Pro ou ultérieure
>   * Une licence Adobe Workfront Goals en plus d’une licence Workfront.
>
>Contactez votre gestionnaire de compte Workfront pour en savoir plus sur une licence Workfront Goals.
> 
>Pour plus d’informations sur l’accès aux objectifs Workfront, voir [Conditions requises pour utiliser les objectifs Workfront](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).

## Considération lors de la mise à jour des états d’objectif dans les objectifs Workfront

* Vous ne pouvez pas mettre à jour manuellement l’état des objectifs que vous avez créés ou qui ont été partagés avec vous. L’état des objectifs est mis à jour en fonction des actions que vous effectuez sur l’objectif. Par exemple, si vous activez un objectif, l’état En création passe à Actif.
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
   * [Activer les objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md)
   * [Suppression et désactivation d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Fermer et rouvrir desobjectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Présentation des états d’objectif dans les objectifs Workfront

Pour plus d’informations sur la création d’objectifs Workfront, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Pour plus d’informations sur l’activation des objectifs, voir [Activation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

Les objectifs peuvent avoir l’un des états suivants dans les objectifs Workfront :

* [Version préliminaire](#draft)
* [Actif](#active)
* [Inactif](#inactive)
* [Fermé](#closed)

### Brouillon {#draft}

* Il s’agit de l’état par défaut d’un objectif nouvellement créé. Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* Les objectifs de Workfront n’enregistrent pas de progrès sur un objectif ébauché.
* Vous ne pouvez pas mettre à jour la progression d’un objectif brouillé.
* Vous ne pouvez pas fermer ou désactiver les objectifs préliminaires car ils manquent d’informations sur la progression.
* Les objectifs élaborés ne contribuent pas au calcul de progression des autres objectifs et ne sont pas pris en compte dans les graphiques.
* Les objectifs préliminaires s’affichent dans les zones suivantes des objectifs de Workfront :

   * Liste d’objectifs
   * section Alignement des objectifs (uniquement en tant qu’objectif aligné)


>[!IMPORTANT]
>
>Après avoir défini l’état d’un objectif sur un autre état, l’objectif ne peut plus jamais être placé dans un état En création .

### Actif {#active}

* Vous ne pouvez activer un objectif en version préliminaire que lorsque vous l’associez à un résultat, à une activité ou que vous lui alignez un autre objectif. L’activation de l’objectif passe à l’état Actif. Pour plus d’informations sur l’activation des objectifs, voir [Activation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* Les objectifs de Workfront enregistrent la progression par rapport aux objectifs actifs.
* Les objectifs actifs contribuent au calcul de la progression d’autres objectifs et sont pris en compte dans les graphiques.
* Les objectifs actifs s’affichent dans les zones suivantes des objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs
   * La progression des objectifs actifs s’affiche dans les graphiques.

* Vous pouvez réactiver un objectif Fermé ou Inactif.

### Inactif {#inactive}

* Vous pouvez désactiver un objectif actif lorsque le propriétaire a arrêté de l’utiliser temporairement ou définitivement. Vous pouvez le conserver pour des informations historiques. Cela met à jour l’état de l’objectif en Inactif.

  Pour plus d’informations sur la désactivation des objectifs, reportez-vous à la section &quot;Désactivation des objectifs&quot; de l’article [Suppression et désactivation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Vous ne pouvez pas désactiver un objectif brouillon ou fermé.
* Vous pouvez réactiver un objectif inactif et continuer à travailler dessus.
* Les objectifs de Workfront ne calculent pas la progression des objectifs inactifs.
* Vous ne pouvez pas mettre à jour la progression d’un objectif inactif.
* Les objectifs inactifs ne contribuent pas au calcul de progression des autres objectifs et ne sont pas pris en compte dans les graphiques.
* Les buts inactifs ont un passé de progrès parce qu&#39;ils étaient autrefois actifs, contrairement aux objectifs préliminaires.
* Les objectifs inactifs s’affichent dans les zones suivantes des objectifs Workfront :

   * Liste d’objectifs
   * section Alignement des objectifs (uniquement en tant qu’objectifs alignés)

### Fermé {#closed}

* Vous pouvez fermer un objectif lorsque vous souhaitez indiquer que vous l’avez atteint ou que vous ne le travaillez plus, et ce, à l’avenir. Pour plus d’informations sur la fermeture des objectifs, voir [Fermer et rouvrir les objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md).

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
