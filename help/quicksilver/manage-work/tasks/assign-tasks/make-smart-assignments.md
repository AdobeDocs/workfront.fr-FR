---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Rendre des affectations intelligentes
description: Vous pouvez utiliser des affectations intelligentes pour identifier le meilleur utilisateur à effectuer le travail. Les affectations intelligentes sont des suggestions destinées aux utilisateurs, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche. Pour plus d’informations sur les affectations intelligentes, voir Présentation des affectations intelligentes .
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 75a67f1eb32d9ec03e27a0dbe2fde1bfaf3a7d1f
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Rendre des affectations intelligentes

<!--Audited: 02/2024-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients.</span>

<span class="preview">Pour plus d’informations sur le calendrier de publication actuel, voir [Présentation de la version du deuxième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Vous pouvez utiliser des affectations intelligentes pour identifier le meilleur utilisateur à effectuer le travail.

Les affectations intelligentes sont des suggestions destinées aux utilisateurs, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources. Workfront base ses suggestions sur un algorithme qui détermine la ressource la plus appropriée pour la tâche.

<span class="preview">Il existe deux algorithmes distincts dans Workfront pour les tâches et les problèmes. </span>

Pour plus d’informations sur les critères utilisés pour déterminer les affectations intelligentes, voir [Présentation des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard</p>
      Ou
      <p>Actuel : travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux problèmes</p> <p>Affichage ou accès supérieur à la console Projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribuez à des autorisations ou à des autorisations supérieures avec la possibilité d’effectuer des affectations sur des tâches et des problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Rendre des affectations intelligentes

Les affectations intelligentes sont disponibles dans la plupart des emplacements où vous pouvez effectuer des affectations dans Workfront.

1. Dans les zones suivantes, cliquez sur le bouton **Affectations** ou **Attribuez-le à** field :

   * une tâche, une liste de problèmes ou un rapport ;
   * Un en-tête de tâche ou de problème
   * Panneau Résumé de la tâche ou du problème
   * <span class="preview">Une boîte de dialogue Nouvelle tâche ou Nouveau problème lorsque vous ajoutez une nouvelle tâche ou un problème à un projet.</span>
   * Le champ Affectations pour un élément répertorié dans la zone Accueil
   * Tâche ou problème dans l’équilibreur de charge de travail

1. Placez le curseur dans le champ d’affectation et attendez deux secondes.

   <span class="preview">La variable **Suggestions d’affectation** s’affiche.</span> <!--check the casing for "assignments" should be lower case in task lists??-->

   >[!TIP]
   >
   >   L’en-tête de liste s’affiche. **Voici quelques recommandations :** au lieu de **Suggestions d’affectation** dans une liste de problèmes.

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   Pour les problèmes, les suggestions d’affectation dynamique s’affichent dans la variable **Affectations proposées** zone.

   Pour les tâches, les affectations intelligentes s’affichent dans les sections suivantes, selon la phase du calcul de l’algorithme qui a identifié les affectations :

   * **Affectations proposées**: affectations identifiées dans la première phase du calcul de l’algorithme de l’affectation dynamique de tâche.
   * <span class="preview">**Autres affectations**: affectations identifiées dans la seconde phase du calcul de l’algorithme de l’affectation dynamique de tâche. Cette section n’est pas disponible pour les problèmes. </span> <!--replace this with the new UI: "Other assignments"-->

   ![](assets/smart-assignments-task-list.png)

   Pour plus d’informations, voir [Présentation des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Sélectionnez l’utilisateur dans la liste de recommandations en cliquant sur son nom.

1. (Facultatif) Cliquez sur **M&#39;affecter** pour vous attribuer l’élément de travail.

   >[!TIP]
   >
   >S’il n’existe aucune suggestion, la liste de suggestions ne s’ouvre pas.

1. (Facultatif) Si vous ne souhaitez pas utiliser l’un des utilisateurs recommandés dans la liste Affectations intelligentes, commencez à saisir le nom de la ressource souhaitée et sélectionnez le nom lorsqu’il apparaît dans la liste.
1. Cliquez sur **Entrée** pour effectuer l’affectation.

   L’utilisateur sélectionné est affecté à la tâche ou au problème.
