---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Consultez des graphiques pour comprendre les tendances de progression des objectifs dans les objectifs Adobe Workfront.
description: Vous pouvez consulter l’intégrité globale de vos objectifs et leur évolution dans le temps dans la section Graphiques des objectifs Adobe Workfront. Les graphiques de cette section ne ventilent pas la progression de chaque objectif, mais vous donnent à la place un aperçu holistique de l’état d’avancement de tous les objectifs ainsi que de leur tendance à l’avancement dans le temps au cours d’une période donnée.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Consultez des graphiques pour comprendre les tendances de progression des objectifs dans les objectifs Adobe Workfront.

<!-- drafted mostly for P&P release-->

Vous pouvez consulter l’intégrité globale de vos objectifs et leur évolution dans le temps dans la section Graphiques des objectifs Adobe Workfront. Les graphiques de cette section ne ventilent pas la progression de chaque objectif, mais vous donnent à la place un aperçu holistique de l’état d’avancement de tous les objectifs ainsi que de leur tendance à l’avancement dans le temps au cours d’une période donnée.

>[!IMPORTANT]
>
>Vous pouvez consulter le nombre total de vos objectifs dans la section Graphiques pour une période donnée. Toutefois, les objectifs de Workfront ne prennent en compte que les objectifs dont le statut est Principal et Fermé lors du calcul de l’état de progression global de l’objectif et du pourcentage de réalisation terminée.

## Exigences d’accès

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

Vous devez disposer des accès suivants pour effectuer les actions décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td> <p>Pour accéder aux fonctionnalités décrites dans cet article, vous devez acheter une licence supplémentaire pour les objectifs d’Adobe Workfront. </p> <p>Pour plus d’informations, voir <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Conditions requises pour utiliser les objectifs Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Affichage ou accès supérieur aux objectifs</p> <p><b>NOTE</b><p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir :</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Accorder l’accès aux objectifs Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> 
    <div> 
     <p>Affichage ou autorisations supérieures sur les objectifs</p> 
     <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partage d’un objectif dans les objectifs Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Types de graphiques dans les objectifs Workfront

Les graphiques suivants sont disponibles dans la section Graphiques ou Objectifs de Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Le graphique de l’intégrité des objectifs</td> 
   <td> <p>Un graphique à jauge qui affiche les éléments suivants :</p> 
    <ul> 
     <li>Nombre total d’objectifs pour la période sélectionnée. Les objectifs ayant un statut quelconque sont pris en compte. </li> 
     <li>Etat d’avancement des objectifs avec un état Principal et Fermé.</li> 
    </ul> <p>Pour plus d’informations sur la façon dont les objectifs de Workfront calculent l’état de progression, voir <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Présentation de la progression et de la condition des objectifs dans les objectifs Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Graphique de progression des objectifs</td> 
   <td> <p>Graphique en courbes qui affiche les mises à jour apportées aux objectifs par incréments hebdomadaires pendant la durée de l’objectif. Le graphique de progression de l’objectif affiche les éléments suivants :</p> 
    <ul> 
     <li>Pourcentage moyen attendu et réel atteignant tous les objectifs principaux et terminés au cours de la période sélectionnée. Le pourcentage de progression complète est ventilé en incréments hebdomadaires marqués par des noeuds. </li> 
     <li>Pourcentage moyen des progrès réalisés pour les objectifs principaux et clos depuis la semaine précédente. </li> 
    </ul> <p>Conseil : Le graphique de progression de l’objectif peut ne pas afficher d’informations lorsque des mises à jour sont effectuées sur les objectifs en dehors de la période sélectionnée. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Vérification de la progression de l’objectif dans les graphiques

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) > **Objectifs** dans le coin supérieur droit.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La zone Objectifs de Workfront s’ouvre alors.

1. Cliquez sur **Graphiques** dans le panneau de gauche.

   ![](assets/graphs-in-left-panel.png)

   La section Graphiques s’affiche.

   Par défaut, les objectifs affichés dans la section Graphiques sont limités par les critères suivants :

   * Filtres appliqués à la zone Graphiques.
   * Objectifs dont l’état est Principal et Version préliminaire.

1. (Facultatif) Sélectionnez le type d’informations à afficher en mettant à jour les filtres dans le coin supérieur droit de la section Graphiques.

   Pour plus d’informations sur les objectifs de filtrage, voir [Filtrage des informations dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   Si vous avez choisi d’afficher plusieurs périodes, un graphique de l’état (jauge) ainsi qu’un graphique de l’état d’avancement (ligne) s’affichent pour chaque période.

1. Consultez les informations du tableau ci-dessous lorsque vous passez en revue le graphique de l’intégrité des objectifs.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Nombre total d’objectifs | Le nombre au bas du graphique indique le nombre de tous les objectifs de la période sélectionnée, dans tous les états que vous avez sélectionnés. |
   |---|---|
   | Pourcentage moyen terminé | En haut du graphique, ce nombre indique le pourcentage moyen de réalisation d’objectifs principaux et fermés au cours de la période sélectionnée. |
   | Objectifs et progrès | Nombre d’objectifs pour chaque segment d’état de progression, lorsque vous passez la souris sur les segments du graphique. Seuls les objectifs dont l’état est Principal ou Fermé sont comptabilisés dans les segments. |


1. Consultez les informations du tableau ci-dessous lorsque vous passez en revue le graphique de progression de l’objectif.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Progression de la ligne de base</td> 
      <td>La ligne d’inclinaison verte indique la moyenne globale attendue en pourcentage d’objectifs principaux et fermés pour la période sélectionnée. Tous les objectifs d’une période donnée sont censés être atteints, de sorte que la progression de base est toujours de 100 % à la fin de la période. </td> 
     </tr> 
     <tr> 
      <td>Progression réelle</td> 
      <td> <p>La ligne bleue indique la moyenne globale réelle en pourcentage complète des objectifs principaux et fermés pour la période sélectionnée par incréments hebdomadaires. Chaque semaine pendant la durée de l’objectif est marquée par un noeud dans la ligne . </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passez le curseur de la souris sur un noeud week dans le graphique de progression de l’objectif et passez en revue les éléments suivants :

   * **Date de la semaine**: Mois, jour et année de la semaine sélectionnée.
   * **Progression**: Moyenne du pourcentage réel d’achèvement de tous les objectifs pour la semaine sélectionnée.
   * **Ligne de base**: Moyenne du pourcentage attendu de tous les objectifs pour la semaine sélectionnée.

1. (Facultatif) Cliquez sur **Progression** au bas du graphique de progression pour supprimer la ligne de progression globale réelle

   Ou

   Cliquez sur **Ligne de base** au bas du graphique de progression pour supprimer la progression attendue du graphique.

 
