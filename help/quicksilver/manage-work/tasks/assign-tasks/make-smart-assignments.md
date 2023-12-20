---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Rendre des affectations intelligentes
description: Vous pouvez utiliser des affectations intelligentes pour identifier le meilleur utilisateur à effectuer le travail. Les affectations intelligentes sont des suggestions destinées aux utilisateurs qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche. Pour plus d’informations sur les affectations intelligentes, voir Présentation des affectations intelligentes .
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Rendre des affectations intelligentes

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>   
  
<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> 
-->

Vous pouvez utiliser des affectations intelligentes pour identifier le meilleur utilisateur à effectuer le travail. Les affectations intelligentes sont des suggestions destinées aux utilisateurs qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche. Pour plus d’informations sur les affectations intelligentes, voir [Présentation des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard</p>
      Ou
      <p>Actuel : travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux problèmes</p> <p>Affichage ou accès supérieur à la console Projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribuez à des autorisations ou à des autorisations supérieures avec la possibilité d’effectuer des affectations sur des tâches et des problèmes</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Rendre des affectations intelligentes

Les affectations intelligentes sont disponibles dans la plupart des emplacements où vous pouvez effectuer des affectations dans Workfront.

1. Dans les zones suivantes, cliquez sur le bouton **Affectations** ou **Attribuez-le à** field :   

   * une tâche, une liste de problèmes ou un rapport ;
   * Un en-tête de tâche ou de problème
   * Panneau Résumé de la tâche ou du problème
   * Le champ Affectations pour un élément répertorié dans la zone Accueil
   * Une tâche ou un problème dans les zones Planification ou Planification
   * Tâche ou problème dans l’équilibreur de charge de travail

1. Placez le curseur dans le champ d’affectation et attendez deux secondes. La variable **Suggestions d’affectation** ou le **Voici quelques recommandations :** s’affiche.

   <!--check the casing for "assignments" should be lower case in task lists??-->

   <!--replace the last sentence above with this when we release smarter assignments:
   The **Suggested assignments** list displays. 
   NOTE (********and add preview tags for the note*****)
   The list header displays **Here are a few recommendations** instead of **Suggested assignments** in an issue list.
   -->

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   Les utilisateurs affichés dans cette liste sont les suggestions d’affectation intelligente pour la tâche ou le problème.

   Pour plus d’informations sur l’emplacement d’affichage des affectations dynamiques, voir la section &quot;Localisation des suggestions d’affectation dynamique&quot; dans l’article. [Présentation des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. Sélectionnez l’utilisateur dans la liste de recommandations en cliquant sur son nom. Cliquer **M&#39;affecter** vous attribue l’élément de travail.

   >[!TIP]
   >
   >S’il n’existe aucune suggestion, la liste de suggestions ne s’ouvre pas.

1. (Facultatif) Si vous ne souhaitez pas utiliser l’un des utilisateurs recommandés dans la liste Affectations intelligentes, commencez à saisir le nom de l’utilisateur souhaité et sélectionnez le nom lorsqu’il apparaît dans la liste.
1. Cliquez sur **Entrée** pour effectuer l’affectation.

   L’utilisateur sélectionné est affecté à la tâche ou au problème.
