---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Vue d’ensemble du statut d’objectif dans Objectifs Adobe Workfront
description: Les statuts des objectifs indiquent si un objectif est actif et enregistre actuellement la progression, ou s’il est inactif, sous forme de brouillon ou déjà atteint.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 98%

---

# Vue d’ensemble du statut d’objectif dans Objectifs Adobe Workfront

>[!IMPORTANT]
>
>Votre organisation doit disposer des éléments suivants pour utiliser les fonctionnalités décrites dans cet article :
>
>* Pour la nouvelle structure de forfait et de licence :
>
>   * Formule Workfront ultime
>    
>* Pour la structure de forfait et de licence actuelle :
>
>   * Formule Workfront Pro ou ultérieure
>   * Une licence Objectifs Adobe Workfront en plus d’une licence Workfront.
>
>Contactez la personne chargée de la gestion de votre compte Workfront pour en savoir plus sur la licence Objectifs Workfront.
> 
>Pour plus d’informations sur l’accès à Objectifs Workfront, voir [Conditions requises pour utiliser Objectifs Workfront](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).

## À prendre en considération lors de la mise à jour des statuts d’objectif dans Objectifs Workfront

* Vous ne pouvez pas mettre à jour manuellement le statut des objectifs que vous avez créés ou qui ont été partagés avec vous. Le statut des objectifs est mis à jour en fonction des actions que vous effectuez sur l’objectif. Par exemple, si vous activez un objectif, le statut passe de Brouillon à Actif.
* Certaines restrictions existent. Parfois, vous ne pouvez pas modifier le statut d’un objectif, selon les règles suivantes :

  | De/À | Brouillon | Actif | Inactif | Fermé |
  |---|---|---|---|---|
  | Brouillon | - | Oui | Non | Non |
  | Actif | Non | - | Oui | Oui |
  | Inactif | Non | Oui | - | Non |
  | Fermé | Non | Oui | Non | - |

* L’ouverture d’un objectif fermé met également à jour la progression de l’objectif.
* Certaines actions que vous effectuez sur un objectif mettent également à jour son statut.Pour plus d’informations sur la mise à jour des statuts d’objectif, reportez-vous aux articles suivants :

   * [Créer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
   * [Activer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md)
   * [Supprimer et désactiver des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Fermer et rouvrir desobjectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Vue d’ensemble des statuts des objectifs dans Objectifs Workfront

Pour plus d’informations sur la création d’objectifs Workfront, voir [Créer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Pour plus d’informations sur l’activation des objectifs, voir [Activer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

Les objectifs peuvent avoir l’un des statuts suivants dans Objectifs Workfront :

* [Brouillon](#draft)
* [Actif](#active)
* [Inactif](#inactive)
* [Fermé](#closed)

### Brouillon {#draft}

* Il s’agit du statut par défaut d’un objectif nouvellement créé. Pour plus d’informations sur la création d’objectifs, voir [Créer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* Objectifs Workfront n’enregistre pas la progression d’un objectif ayant le satut brouillon.
* Vous ne pouvez pas mettre à jour la progression d’un objectif ayant le statut brouillon.
* Vous ne pouvez pas fermer ou désactiver les objectifs ayant le statut brouillon, car ils ne disposent pas d’informations de progression.
* Les objectifs ayant le statut brouillon ne contribuent pas au calcul de progression des autres objectifs et ne sont pas pris en compte dans les graphiques.
* Les objectifs ayant le statut brouillon s’affichent dans les zones suivantes d’Objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs (uniquement en tant qu’objectif aligné)


>[!IMPORTANT]
>
>Après modification de son statut, un objectif ne peut plus jamais être placé dans un statut Brouillon.

### Actif {#active}

* Vous ne pouvez activer un objectif au statut brouillon que lorsque vous l’associez à un résultat ou à une activité, ou que vous alignez un autre objectif sur celui-ci. L’activation de l’objectif fait passer son statut à Actif. Pour plus d’informations sur l’activation des objectifs, voir [Activer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* Objectifs Workfront enregistre la progression des objectifs actifs.
* Les objectifs actifs contribuent au calcul de la progression d’autres objectifs et sont pris en compte dans les graphiques.
* Les objectifs actifs s’affichent dans les zones suivantes d’Objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs
   * La progression des objectifs actifs s’affiche dans les graphiques.

* Vous pouvez réactiver un objectif Fermé ou Inactif.

### Inactif {#inactive}

* Vous pouvez désactiver un objectif actif lorsque la personne propriétaire a arrêté de l’utiliser temporairement ou définitivement. Vous pouvez le conserver pour des informations historiques. Cela fait passer le statut de l’objectif à Inactif.

  Pour plus d’informations sur la désactivation des objectifs, reportez-vous à la section « Désactiver des objectifs » de l’article [Supprimer et désactiver des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Vous ne pouvez pas désactiver un objectif brouillon ou fermé.
* Vous pouvez réactiver un objectif inactif et continuer à travailler dessus.
* Objectifs Workfront ne calcule pas la progression des objectifs inactifs.
* Vous ne pouvez pas mettre à jour la progression d’un objectif inactif.
* Les objectifs inactifs ne contribuent pas au calcul de progression des autres objectifs et ne sont pas pris en compte dans les graphiques.
* Les objectifs inactifs ont un historique de progression parce qu’ils étaient autrefois actifs, contrairement aux objectifs au statut brouillon.
* Les objectifs inactifs s’affichent dans les zones suivantes d’Objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs (uniquement en tant qu’objectifs alignés)

### Fermé {#closed}

* Vous pouvez fermer un objectif lorsque vous souhaitez indiquer que vous l’avez atteint ou que vous ne travaillez plus dessus et que vous n’y travaillerez plus à l’avenir. Pour plus d’informations sur la fermeture des objectifs, voir [Fermer et rouvrir des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >Si vous envisagez de travailler ultérieurement sur un objectif qui n’est pas encore atteint, nous vous recommandons de modifier le statut en Inactif au lieu de Fermé.

* Vous ne pouvez pas fermer des objectifs qui n’ont jamais été activés, comme les objectifs au statut brouillon.
* Vous pouvez rouvrir un objectif fermé et continuer à travailler dessus.
* Objectifs Workfront arrête d’enregistrer la progression sur les objectifs fermés.
* Vous ne pouvez pas mettre à jour la progression d’un objectif fermé.
* Les objectifs fermés s’affichent dans la zone suivante d’Objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs (uniquement en tant qu’objectifs alignés)
   * Les informations relatives aux objectifs fermés sont également prises en compte dans la section Graphiques.
