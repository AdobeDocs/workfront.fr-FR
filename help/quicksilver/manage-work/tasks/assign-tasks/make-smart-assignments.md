---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Créer des affectations intelligentes
description: Tirez parti des affectations intelligentes pour identifier la personne idéale à la réalisation du travail. Les affectations intelligentes sont des suggestions destinées aux utilisateurs et utilisatrices, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des éléments de travail à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche. Pour plus d’informations sur les affectations intelligentes, consultez la vue d’ensemble des affectations intelligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 75%

---

# Créer des affectations intelligentes

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elles sont disponibles uniquement dans l’environnement de prévisualisation pour toutes les clientes et tous les clients ou dans l’environnement de production pour les clientes et les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activer ou désactiver le versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, consultez la [présentation du troisième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Tirez parti des affectations intelligentes pour identifier la personne idéale à la réalisation du travail.

Les affectations intelligentes sont des suggestions destinées aux utilisateurs et utilisatrices, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des éléments de travail à des ressources. Workfront base ses suggestions sur un algorithme qui détermine la ressource la plus appropriée pour la tâche.

<span class="preview">Il existe deux algorithmes distincts dans Workfront qui calculent les affectations intelligentes qui fonctionnent différemment pour les tâches et pour les problèmes. </span>

Pour plus d’informations sur les critères utilisés pour déterminer les affectations intelligentes, voir [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle : standard</p>
      Ou
      <p>Actuellement : Travail ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès en modification aux tâches et problèmes</p> <p>Accès en affichage ou supérieur pour les projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de contribution ou supérieures avec la possibilité d’affecter des personnes à des tâches et des problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Créer des affectations intelligentes

Les affectations intelligentes sont disponibles dans la plupart des emplacements où vous pouvez effectuer des affectations dans Workfront.

1. Dans les zones suivantes, cliquez sur le champ **Affectations** ou **Affecter ceci à** :

   * Tâche, liste de problèmes ou rapport
   * En-tête de tâche ou de problème
   * Panneau Résumé de la tâche ou du problème
   * <span class="preview">Boîte de dialogue Nouvelle tâche ou Nouveau problème lorsque vous ajoutez une nouvelle tâche ou un problème à un projet</span>.
   * Champ Affectations pour un élément de la zone Accueil
   * Tâche ou problème dans l’équilibreur de charge de travail

1. Placez le curseur dans le champ Affectations et attendez deux secondes.

   <div class="preview">
   Une ou plusieurs des sections suivantes contenant des suggestions d’affectation dynamique s’affichent :

   * **Affectations proposées** : s’affiche pour les tâches. <!--remove the note when we go to production with smarter assignments-->

     >[!TIP]
     >
     >   L’en-tête de liste affiche **Voici quelques recommandations** au lieu de **Affectations proposées** dans l’environnement de production.
     >
   * **Utilisateurs et équipes** : s’affiche pour les tâches et les problèmes.
   * **Rôles de tâche** : s’affiche pour les tâches et les problèmes.
   * **Taux des rôles de tâche de carte** : s’affiche pour les tâches. Pour plus d’informations, voir [Gestion des cartes de taux](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   Pour les tâches, les affectations intelligentes s’affichent dans les sections suivantes, selon la phase du calcul de l’algorithme qui a identifié les affectations :

   * **Affectations proposées** : Affectations identifiées dans la première phase du calcul de l’algorithme de l’affectation dynamique de tâche. <span class="preview">Cette section n&#39;est pas disponible pour les problèmes.</span>
   * <span class="preview">**Utilisateurs et équipes**, **Rôles de tâche** ou **Taux des rôles de tâche de carte** : Affectations identifiées dans la seconde phase du calcul de l’algorithme de l’affectation dynamique de tâche. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Consultez [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md) pour en savoir plus.

1. Sélectionnez la personne dans la liste de recommandations en cliquant sur son nom.

1. (Facultatif) Cliquez sur **Me l’affecter** pour vous attribuer l’élément de travail.

   >[!TIP]
   >
   >S’il n’existe aucune suggestion, la liste de suggestions ne s’ouvre pas.

1. (Facultatif) Si vous ne souhaitez pas utiliser l’une des personnes recommandées dans la liste des affectations intelligentes, commencez à saisir le nom de la ressource souhaitée et sélectionnez le nom lorsqu’il apparaît dans la liste.
1. Cliquez sur **Entrée** pour donner l’affectation.

   La personne sélectionnée est alors affectée à la tâche ou au problème.
