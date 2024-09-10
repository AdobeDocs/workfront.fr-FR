---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Utilisation d’états personnalisés comme états par défaut
description: Lorsqu’un statut personnalisé est défini comme statut par défaut, le nouveau statut par défaut est utilisé dans l’ensemble du système de diverses manières. L’utilisation du statut varie selon s’il est le statut par défaut au niveau du système ou au niveau du groupe.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 99%

---

# Utiliser les statuts personnalisés comme statuts par défaut

Lorsqu’un statut personnalisé est défini comme statut par défaut, le nouveau statut par défaut est utilisé dans l’ensemble du système de diverses manières. L’utilisation du statut varie selon s’il est le statut par défaut au niveau du système ou au niveau du groupe.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
     <p>Nouveau : Standard</p>
     <p>ou</p>
     <p>Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Statuts par défaut personnalisés au niveau du système

Lorsque vous définissez un statut personnalisé comme statut par défaut du système, tous les nouveaux groupes créés dans le système héritent de ce statut.

Les groupes qui existaient déjà lorsque vous avez défini le nouveau statut par défaut du système n’en héritent pas automatiquement.

Par exemple, supposons que deux groupes aient déjà été créés dans votre environnement Adobe Workfront (Marketing et Ventes). Vous créez un nouveau statut personnalisé qui équivaut au statut Actuel, et vous nommez ce statut « En cours ». Vous créez maintenant un nouveau groupe appelé Ingénierie. Dans ce scénario, le groupe Ingénierie hérite du nouveau statut par défaut, ce qui n’est pas le cas des groupes Marketing et Ventes.

## Statuts par défaut personnalisés au niveau du groupe

Un statut personnalisé que vous définissez comme statut par défaut du groupe est utilisé dans les circonstances suivantes :

* **Lorsque le système Workfront choisit un statut automatiquement, le statut par défaut du groupe est utilisé :** le statut personnalisé que vous avez défini comme statut par défaut du groupe est utilisé lorsque le système Workfront attribue automatiquement un statut à un objet.

  Par exemple, une tâche peut être configurée pour passer automatiquement au statut Terminée lorsque le pourcentage de réalisation atteint 100 %. Si vous créez un statut personnalisé qui équivaut à Terminée et que vous définissez ce statut personnalisé comme statut par défaut, Workfront modifie le statut de la tâche pour qu’il corresponde au nouveau statut par défaut.

  Les statuts personnalisés sont utilisés uniquement de cette manière avec les statuts de groupe associés à une tâche ou à un problème. Les statuts personnalisés ne peuvent pas être utilisés de cette manière pour les statuts associés à un projet.

* Le **statut d’un projet est déterminé par le groupe associé au projet** : si le groupe associé à un projet donné change, le statut du projet change en fonction des statuts par défaut définis pour le groupe. (Un groupe peut être associé à un projet via le champ Groupes lors de la modification du projet).

  Si ce groupe change, le statut du projet change si le nouveau groupe a un statut par défaut différent qui correspond au statut actuel du projet.

  Par exemple, un projet peut être associé au groupe Marketing, et le statut du projet est défini sur Planification. Le projet est modifié de manière à être associé au groupe Ventes. Le groupe Ventes a un statut de groupe personnalisé par défaut appelé Réflexion (et ce statut équivaut à Planification). Comme le groupe du projet a été modifié, le statut du projet passe maintenant à Réflexion.

Si vous êtes administrateur ou administratrice de groupe, consultez [Définir un statut par défaut pour un groupe](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Statuts des problèmes

Si le statut personnalisé est un statut de problème, les quatre types de problèmes doivent être activés pour celui-ci (rapport de bug, ordre de modification, problème et requête). Par exemple, dans le statut de problème ci-dessous, le statut Réouvert ne peut pas être utilisé comme statut par défaut, car le type de problème Ordre de modification n’est pas sélectionné :

![](assets/all-4-issue-types-enabled.png)

## Définir un statut personnalisé comme statut par défaut

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **Statuts**.
1. (Le cas échéant) Si vous définissez un statut par défaut pour un groupe, commencez à saisir le nom du groupe dans le menu situé dans le coin supérieur droit, puis sélectionnez-le lorsqu’il apparaît.
1. Ouvrez l’onglet **Projet**, **Tâches**, ou **Problèmes**, selon le type de statut que vous souhaitez définir comme statut par défaut.
1. Cliquez sur le menu déroulant **Définir les statuts par défaut**.
1. Dans la zone de liste déroulante qui s’affiche, à côté du statut que vous souhaitez définir par défaut, sélectionnez le statut de votre choix.
1. Cliquer sur **Enregistrer**.
1. Associez le projet au groupe où réside le statut.

   >[!NOTE]
   >
   >Si vous définissez le statut personnalisé d’un groupe et que vous affectez ensuite le projet à un autre groupe, le statut du projet sera rechargé et pourrait changer.

   1. Accédez au projet dans lequel vous souhaitez utiliser le statut personnalisé.
   1. Cliquez sur le menu Plus ![](assets/more-icon.png), puis sur **Modifier**.
   1. Dans la zone **Modifier le projet** qui s’affiche, dans le champ **Groupe** sous **Association de projets**, sélectionnez le groupe dans lequel réside le statut.
   1. Cliquez sur **Enregistrer les modifications**.
