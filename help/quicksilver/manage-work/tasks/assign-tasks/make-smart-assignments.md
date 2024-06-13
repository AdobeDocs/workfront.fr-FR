---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Créer des affectations intelligentes
description: Vous pouvez utiliser des affectations intelligentes pour identifier le meilleur utilisateur à effectuer le travail. Les affectations intelligentes sont des suggestions destinées aux utilisateurs, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche. Pour plus d’informations sur les affectations intelligentes, voir Présentation des affectations intelligentes .
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 10%

---

# Créer des affectations intelligentes

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients ou dans l’environnement Production pour les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Présentation de la version du troisième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Vous pouvez utiliser des affectations intelligentes pour identifier le meilleur utilisateur à effectuer le travail.

Les affectations intelligentes sont des suggestions destinées aux utilisateurs, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources. Workfront base ses suggestions sur un algorithme qui détermine la ressource la plus appropriée pour la tâche.

<span class="preview">Il existe deux algorithmes distincts dans Workfront pour les tâches et les problèmes. </span>

Pour plus d’informations sur les critères utilisés pour déterminer les affectations intelligentes, voir [Présentation des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

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
   <td> <p>Nouveau : Standard</p>
      Ou
      <p>Actuel : travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux problèmes</p> <p>Affichage ou accès supérieur à la console Projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribuez à des autorisations ou à des autorisations supérieures avec la possibilité d’effectuer des affectations sur des tâches et des problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Créer des affectations intelligentes

Les affectations intelligentes sont disponibles dans la plupart des emplacements où vous pouvez effectuer des affectations dans Workfront.

1. Dans les zones suivantes, cliquez sur le bouton **Affectations** ou **Attribuez-le à** field :

   * une tâche, une liste de problèmes ou un rapport ;
   * Un en-tête de tâche ou de problème
   * Panneau Résumé de la tâche ou du problème
   * <span class="preview">Une boîte de dialogue Nouvelle tâche ou Nouveau problème lorsque vous ajoutez une nouvelle tâche ou un problème à un projet.</span>
   * Le champ Affectations pour un élément répertorié dans la zone Accueil
   * Tâche ou problème dans l’équilibreur de charge de travail

1. Placez le curseur dans le champ d’affectation et attendez deux secondes.

   <div class="preview">
   Une ou plusieurs des sections suivantes contenant des suggestions d’affectation dynamique s’affichent :

   * **Affectations proposées**: s’affiche pour les tâches.

     >[!TIP]
     >
     >   L’en-tête de liste s’affiche. **Voici quelques recommandations :** au lieu de **Affectations proposées** dans l’environnement de production.
     >
   * **Autres affectations**: s’affiche pour les tâches et les problèmes.
   * **Utilisateurs et équipes**: s’affiche pour les tâches et les problèmes.
   * **Rôles de tâche**: s’affiche pour les tâches et les problèmes.
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   Pour les tâches, les affectations intelligentes s’affichent dans les sections suivantes, selon la phase du calcul de l’algorithme qui a identifié les affectations :

   * **Affectations proposées**: affectations identifiées dans la première phase du calcul de l’algorithme de l’affectation dynamique de tâche. <span class="preview">Cette section n’est pas disponible pour les problèmes.</span>
   * <span class="preview">**Autres affectations**, **Utilisateurs et équipes**, ou **Rôles de tâche**: affectations identifiées dans la seconde phase du calcul de l’algorithme de l’affectation dynamique de tâche. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Pour plus d’informations, voir [Présentation des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Sélectionnez l’utilisateur dans la liste de recommandations en cliquant sur son nom.

1. (Facultatif) Cliquez sur **M&#39;affecter** pour vous attribuer l’élément de travail.

   >[!TIP]
   >
   >S’il n’existe aucune suggestion, la liste de suggestions ne s’ouvre pas.

1. (Facultatif) Si vous ne souhaitez pas utiliser l’un des utilisateurs recommandés dans la liste Affectations intelligentes, commencez à saisir le nom de la ressource souhaitée et sélectionnez le nom lorsqu’il apparaît dans la liste.
1. Cliquez sur **Entrée** pour effectuer l’affectation.

   L’utilisateur sélectionné est affecté à la tâche ou au problème.
