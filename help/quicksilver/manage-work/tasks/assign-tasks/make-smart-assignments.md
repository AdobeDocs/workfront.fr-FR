---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Créer des affectations intelligentes
description: Vous pouvez utiliser des affectations intelligentes pour identifier la meilleure personne pour effectuer le travail. Les affectations intelligentes sont des suggestions destinées aux utilisateurs et utilisatrices, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour le traitement. Pour plus d’informations sur les affectations intelligentes, voir Vue d’ensemble des affectations intelligentes.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 80%

---

# Créer des affectations intelligentes

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elles ne sont disponibles que dans l’environnement de prévisualisation pour toute la clientèle ou dans l’environnement de production pour les clientes et les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, consultez la section [Activer ou désactiver les versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, consultez la section [Vue d’ensemble de la version du quatrième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md).</span>

Vous pouvez utiliser des affectations intelligentes pour identifier la meilleure personne pour effectuer le travail.

Les affectations intelligentes sont des suggestions destinées aux utilisateurs et utilisatrices, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des éléments de travail à des ressources. Workfront base ses suggestions sur un algorithme qui détermine la ressource la plus appropriée pour le traitement.

<span class="preview">Il existe deux algorithmes distincts dans Workfront qui calculent les affectations intelligentes qui fonctionnent différemment pour les tâches et pour les problèmes.</span>

Pour plus d’informations sur les critères utilisés pour déterminer les affectations intelligentes, voir [Vue d’ensemble des affectations intelligentes](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard</p>
      Ou
      <p>Actuellement : Travail ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux tâches et aux problèmes</p> <p>Accès en affichage ou supérieur aux projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de contribution ou autorisations supérieures avec la possibilité d’affecter des tâches et des problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer des affectations intelligentes

Les affectations intelligentes sont disponibles dans la plupart des emplacements où vous pouvez effectuer des affectations dans Workfront.

1. Dans les zones suivantes, cliquez sur le champ **Affectations** ou **Affecter ceci à** :

   * Tâche, liste de problèmes ou rapport.
   * En-tête de tâche ou de problème.
   * Panneau Résumé de la tâche ou du problème.
   * <span class="preview">Une nouvelle tâche</span> ou une boîte Nouvelle problématique, lorsque vous ajoutez <span class="preview">une nouvelle tâche</span> ou un problème à un projet
   * Tâche ou problème dans l’équilibreur de charge de travail.

1. Placez le curseur dans le champ d’affectation et attendez deux secondes.

   Pour les problèmes, les affectations intelligentes s’affichent dans les sections suivantes :

   * **Utilisateurs et équipes**
   * **Fonctions**

   ![](assets/smart-assignments-issue-header.png)

   Pour les tâches, les affectations intelligentes s’affichent dans les sections suivantes, selon la phase du calcul de l’algorithme qui a identifié les affectations :

   * <span class="preview">**Affectations proposées** : affiche les affectations identifiées dans la première phase de l’algorithme d’affectation dynamique de tâche.</span>
   * **Utilisateurs et équipes**, **Rôles de tâche** ou <span class="preview">**Taux des rôles de tâche de carte**</span> : Affectations identifiées dans la seconde phase du calcul de l’algorithme de l’affectation dynamique de tâche.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Pour en savoir plus, consultez la section [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Sélectionnez la ressource dans la liste de recommandations en cliquant sur son nom.

1. (Facultatif) Cliquez sur **Me l’affecter** pour vous attribuer l’élément de travail.

   >[!TIP]
   >
   >S’il n’existe aucune suggestion, la liste de suggestions ne s’ouvre pas.

1. (Facultatif) Si vous ne souhaitez pas utiliser l’une des personnes recommandées dans la liste des affectations intelligentes, commencez à saisir le nom de la ressource souhaitée et sélectionnez le nom lorsqu’il apparaît dans la liste.
1. Cliquez sur **Entrée** pour donner l’affectation.

   La personne sélectionnée est alors affectée à la tâche ou au problème.
