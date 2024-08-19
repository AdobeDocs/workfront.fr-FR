---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Utilisation d’états personnalisés comme états par défaut
description: Lorsqu’un état personnalisé est défini comme état par défaut, le nouvel état par défaut est utilisé dans l’ensemble du système de différentes manières. La manière dont il est utilisé dépend de sa définition comme état par défaut au niveau du système ou comme état par défaut au niveau du groupe.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 9%

---

# Utilisation d’états personnalisés comme états par défaut

Lorsqu’un état personnalisé est défini comme état par défaut, le nouvel état par défaut est utilisé dans l’ensemble du système de différentes manières. La manière dont il est utilisé dépend de sa définition comme état par défaut au niveau du système ou comme état par défaut au niveau du groupe.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Statuts personnalisés au niveau du système par défaut

Lorsque vous définissez un état personnalisé comme état système par défaut, tous les nouveaux groupes créés dans le système héritent de cet état.

Les groupes qui existaient déjà lorsque vous définissez le nouvel état du système par défaut n’héritent pas automatiquement.

Supposons, par exemple, qu’il existe déjà deux groupes créés dans votre environnement Adobe Workfront (Marketing et ventes). Vous créez un état personnalisé qui correspond à Actuel et appelez l’état En cours. Vous créez maintenant un nouveau groupe appelé Ingénierie. Dans ce scénario, le groupe Ingénieur hérite du nouveau statut par défaut ; ce n’est pas le cas des groupes Marketing et Ventes.

## Statuts personnalisés au niveau du groupe par défaut

Un état personnalisé que vous définissez comme état de groupe par défaut est utilisé dans les cas suivants :

* **Lorsque le système Workfront choisit automatiquement un état, l’état par défaut du groupe est utilisé :** L’état personnalisé que vous définissez comme état par défaut du groupe est utilisé lorsque le système Workfront attribue automatiquement un état à un objet.

  Par exemple, une tâche peut être configurée pour passer automatiquement à l’état Terminé lorsque le pourcentage terminé atteint 100 %. Si vous créez un état personnalisé qui correspond à Terminé et que vous définissez ce statut personnalisé comme état par défaut, Workfront remplace l’état de la tâche par le nouveau statut par défaut.

  Les états personnalisés sont ainsi utilisés uniquement avec les états de groupe associés à une tâche ou à un problème. Les états personnalisés ne peuvent pas être utilisés de cette manière pour les états associés à un projet.

* L’état **d’un projet est déterminé par le groupe associé au projet** : si le groupe associé à un projet donné change, l’état du projet change en fonction des états par défaut définis pour le groupe. (Un groupe peut être associé à un projet via le champ Groupes lors de la modification du projet.)

  Si ce groupe change, l’état du projet change si un état par défaut différent est défini pour le nouveau groupe et correspond à l’état actuel du projet.

  Par exemple, un projet peut être associé au groupe Marketing et l’état du projet est défini sur Planification. Le projet est modifié de sorte qu’il soit désormais associé au groupe Ventes . Le groupe des ventes possède un état de groupe par défaut personnalisé appelé Penser (et ce statut correspond à Planification). Comme le groupe sur le projet a été modifié, l’état du projet passe désormais à Penser.

Si vous êtes administrateur de groupe, voir [Définir un état comme état par défaut pour un groupe](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Statuts des problèmes

Si l’état personnalisé est un état de problème, les quatre types de problème doivent être activés pour celui-ci (rapport de bogue, ordre de modification, problème et requête). Par exemple, dans l’état ci-dessous, l’état Réouvert ne peut pas être utilisé comme état par défaut, car le type de problème Modifier l’ordre n’est pas sélectionné :

![](assets/all-4-issue-types-enabled.png)

## Définir un état personnalisé comme état par défaut

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **États**.
1. (Conditionnel) Si vous définissez un état par défaut pour un groupe, commencez à saisir le nom du groupe dans le menu dans le coin supérieur droit, puis sélectionnez-le lorsqu’il s’affiche.
1. Ouvrez l’onglet **Projet**, **Tâches** ou **Problèmes**, selon le type d’état que vous souhaitez définir comme état par défaut.
1. Cliquez sur le menu déroulant **Définir les états par défaut** .
1. Dans la liste déroulante qui s’affiche, en regard de l’état dans lequel vous souhaitez définir l’état par défaut, sélectionnez l’état par défaut de votre choix.
1. Cliquer sur **Enregistrer**.
1. Associez le projet au groupe où réside l’état.

   >[!NOTE]
   >
   >Si vous définissez l’état personnalisé d’un groupe et que vous attribuez ensuite le projet à un autre groupe, l’état du projet se recharge et peut changer.

   1. Accédez au projet dans lequel vous souhaitez utiliser l’état personnalisé.
   1. Cliquez sur le menu Plus ![](assets/more-icon.png), puis sur **Modifier**.
   1. Dans la zone **Edit Project** (Modifier le projet) qui s’affiche, dans le champ **Group** sous **Project association**, sélectionnez le groupe où réside l’état.
   1. Cliquez sur **Enregistrer les modifications**.
