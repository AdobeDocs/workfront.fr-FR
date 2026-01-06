---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Aperçu du statut des objectifs dans les objectifs Adobe Workfront
description: Les statuts des objectifs indiquent si un objectif est actif et enregistre actuellement la progression, ou s’il est inactif, sous forme de brouillon ou déjà atteint.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 90%

---

# Vue d’ensemble du statut des objectifs dans Objectifs Adobe Workfront

<!--Audited: 4/2025-->

>[!NOTE]
>
>Votre entreprise peut choisir de continuer à utiliser les objectifs Adobe Workfront si elle a déjà acheté ce package par le passé. Pour plus de détails, contactez votre représentant de compte.
>
>Adobe Workfront Goals ne peut plus être acheté.
>
>Pour plus d’informations sur l’accès aux Objectifs Workfront, voir la section [Conditions requises pour utiliser les Objectifs Workfront](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).

<!--Old:

>[!IMPORTANT]
>
>Your organization must have the following to use the functionality described in this article:
>
>* For the new plan and license structure:
>
>   * The Ultimate Workfront plan 
>    
>* For the current plan and license structure: 
>
>   * A Pro or higher Workfront plan
>   * An Adobe Workfront Goals license in addition to a Workfront license.
>
>Contact your Workfront account manager to learn about a Workfront Goals license.    
> 
>For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](/help/quicksilver/workfront-goals/goal-management/access-needed-for-wf-goals.md).   -->

## À prendre en considération lors de la mise à jour des statuts d’objectif dans les Objectifs Workfront

* Vous ne pouvez pas mettre à jour manuellement le statut des objectifs que vous avez créés ou qui ont été partagés avec vous. Le statut des objectifs est mis à jour en fonction des actions que vous effectuez sur l’objectif. Par exemple, si vous activez un objectif, le statut passe de Brouillon à Actif.
* Certaines restrictions existent et, parfois, vous ne pouvez pas modifier le statut d’un objectif, selon les règles suivantes :

  | De/À | Brouillon | Actif | Inactif | Fermé |
  |---|---|---|---|---|
  | Brouillon | - | Oui | Non | Non |
  | Actif | Non | - | Oui | Oui |
  | Inactif | Non | Oui | - | Non |
  | Fermé | Non | Oui | Non | - |

* L’ouverture d’un objectif fermé met également à jour la progression de l’objectif.
* Certaines actions que vous effectuez sur un objectif mettent également à jour son statut. Pour plus d’informations sur la mise à jour des statuts d’objectif, consultez les articles suivants :

   * [Créer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
   * [Activer des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md)
   * [Supprimer et désactiver des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Fermer et rouvrir des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Présentation des statuts des objectifs dans les objectifs Workfront

Pour plus d’informations sur la création d’objectifs Workfront, voir [Créer des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

Pour plus d’informations sur l’activation des objectifs, voir [Activer des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).

Les objectifs peuvent avoir l’un des statuts suivants dans les Objectifs Workfront :

* [Brouillon](#draft)
* [Actif](#active)
* [Inactif](#inactive)
* [Fermé](#closed)

### Brouillon {#draft}

* Il s’agit du statut par défaut d’un objectif nouvellement créé. Pour plus d’informations sur la création d’objectifs, voir [Créer des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
* Les Objectifs Workfront n’enregistrent pas la progression d’un objectif ayant le satut brouillon.
* Vous ne pouvez pas mettre à jour la progression d’un objectif ayant le statut brouillon.
* Vous ne pouvez pas fermer ou désactiver les objectifs ayant le statut brouillon, car ils ne disposent pas d’informations de progression.
* Les objectifs ayant le statut brouillon ne contribuent pas au calcul de progression des autres objectifs et ne sont pas pris en compte dans les graphiques.
* Les objectifs ayant le statut brouillon s’affichent dans les zones suivantes des Objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs (uniquement en tant qu’objectif aligné)


>[!IMPORTANT]
>
>Après modification de son statut, un objectif ne peut plus jamais être placé dans un statut Brouillon.

### Actif {#active}

* Vous ne pouvez activer un objectif au statut brouillon que lorsque vous l’associez à un résultat ou à une activité, ou que vous alignez un autre objectif sur celui-ci. L’activation de l’objectif fait passer son statut à Actif. Pour plus d’informations sur l’activation des objectifs, voir [Activer des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
* Les Objectifs Workfront enregistrent la progression des objectifs actifs.
* Les objectifs actifs contribuent au calcul de la progression d’autres objectifs et sont pris en compte dans les graphiques.
* Les objectifs actifs s’affichent dans les zones suivantes des Objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs
   * La progression des objectifs actifs s’affiche dans les graphiques.

* Vous pouvez réactiver un objectif Fermé ou Inactif.

### Inactif {#inactive}

* Vous pouvez désactiver un objectif actif lorsque la personne propriétaire a arrêté de l’utiliser temporairement ou définitivement. Vous pouvez le conserver pour des informations historiques. Cela fait passer le statut de l’objectif à Inactif.

  Pour plus d’informations sur la désactivation des objectifs, reportez-vous à la section « Désactiver des objectifs » de l’article [Supprimer et désactiver des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Vous ne pouvez pas désactiver un objectif brouillon ou fermé.
* Vous pouvez réactiver un objectif inactif et continuer à travailler dessus.
* Les Objectifs Workfront ne calculent pas la progression des objectifs inactifs.
* Vous ne pouvez pas mettre à jour la progression d’un objectif inactif.
* Les objectifs inactifs ne contribuent pas au calcul de progression des autres objectifs et ne sont pas pris en compte dans les graphiques.
* Les objectifs inactifs ont un historique de progression parce qu’ils étaient autrefois actifs, contrairement aux objectifs au statut brouillon.
* Les objectifs inactifs s’affichent dans les zones suivantes des Objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs (uniquement en tant qu’objectifs alignés)

### Fermé {#closed}

* Vous pouvez fermer un objectif lorsque vous souhaitez indiquer que vous l’avez atteint ou que vous ne travaillez plus dessus et que vous n’y travaillerez plus à l’avenir. Pour plus d’informations sur la fermeture des objectifs, voir [Fermer et rouvrir les objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/close-and-reopen-goals.md).

  >[!TIP]
  >
  >Si vous envisagez de travailler ultérieurement sur un objectif qui n’est pas encore atteint, nous vous recommandons de modifier le statut en Inactif au lieu de Fermé.

* Vous ne pouvez pas fermer des objectifs qui n’ont jamais été activés, comme les objectifs au statut brouillon.
* Vous pouvez rouvrir un objectif fermé et continuer à travailler dessus.
* Les Objectifs Workfront arrêtent d’enregistrer la progression sur les objectifs fermés.
* Vous ne pouvez pas mettre à jour la progression d’un objectif fermé.
* Les objectifs fermés s’affichent dans la zone suivante des Objectifs Workfront :

   * Liste d’objectifs
   * Section Alignement des objectifs (uniquement en tant qu’objectifs alignés)
   * Les informations relatives aux objectifs fermés sont également prises en compte dans la section Graphiques.
