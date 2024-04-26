---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Réviser des graphiques pour comprendre les tendances de progression des objectifs dans Objectifs Adobe Workfront
description: Vous pouvez consulter l’intégrité globale de vos objectifs et leur évolution dans le temps dans la section Graphiques des objectifs Adobe Workfront. Les graphiques de cette section ne ventilent pas la progression de chaque objectif, mais vous donnent à la place un aperçu holistique de l’état d’avancement de tous les objectifs ainsi que de leur tendance à l’avancement dans le temps au cours d’une période donnée.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 8%

---

# Réviser des graphiques pour comprendre les tendances de progression des objectifs dans Objectifs Adobe Workfront

<!-- drafted mostly for P&P release-->

Vous pouvez consulter l’intégrité globale de vos objectifs et leur évolution dans le temps dans la section Graphiques des objectifs Adobe Workfront. Les graphiques de cette section ne ventilent pas la progression de chaque objectif, mais vous donnent à la place un aperçu holistique de l’état d’avancement de tous les objectifs ainsi que de leur tendance à l’avancement dans le temps au cours d’une période donnée.

>[!IMPORTANT]
>
>Vous pouvez consulter le nombre total de vos objectifs dans la section Graphiques pour une période donnée. Toutefois, les objectifs Workfront ne prennent en compte que les objectifs dont l’état est Actif et Fermé lors du calcul de l’état de progression global de l’objectif et du pourcentage terminé.

## Conditions d’accès

Pour effectuer les actions décrites dans cet article, vous devez disposer de l’accès suivant :

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Forfait Adobe Workfront</td>
 <td>
 <p>N’importe quelle</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront*</td>
 <td>
 <p>Nouvelle licence : contributeur ou contributrice ou supérieure</p>
 Ou
 <p>Licence actuelle : demande ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produit*</td>
 <td>
 <p> Nouvelle exigence de produit, l’une des options suivantes : </p>
<ul>
<li>Un forfait Select ou Prime Adobe Workfront et une licence Adobe Workfront Goals supplémentaire.</li>
<li>Un plan Workfront Ultimate qui inclut par défaut les objectifs de Workfront. </li></ul>
 <p>Ou</p>
 <p>Exigences actuelles du produit : formule Workfront et licence supplémentaire pour les objectifs Adobe Workfront. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Exigences pour l’utilisation des Objectifs Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Niveau d’accès</p></td>
 <td> <p>Modifier l’accès aux objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Afficher ou des autorisations supérieures à l’objectif pour l’afficher</p>
  <p>Gérer les autorisations sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, consultez <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans les Objectifs Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
     <li>L’état d’avancement des objectifs avec l’état Actif et Fermé.</li> 
    </ul> <p>Pour plus d’informations sur la façon dont les objectifs de Workfront calculent l’état de progression, voir <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Présentation de la progression et de la condition des objectifs dans les objectifs Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Graphique de progression des objectifs</td> 
   <td> <p>Graphique en courbes qui affiche les mises à jour apportées aux objectifs par incréments hebdomadaires pendant la durée de l’objectif. Le graphique de progression de l’objectif affiche les éléments suivants :</p> 
    <ul> 
     <li>Pourcentage moyen attendu et réel atteignant tous les objectifs actifs et fermés au cours de la période sélectionnée. Le pourcentage de progression complète est ventilé en incréments hebdomadaires marqués par des noeuds. </li> 
     <li>Pourcentage moyen des progrès réalisés pour les objectifs actifs et fermés depuis la semaine précédente. </li> 
    </ul> <p>Conseil : Il se peut que le graphique de progression de l’objectif n’affiche aucune information lorsque des mises à jour sont effectuées sur les objectifs en dehors de la période sélectionnée. </p> </td> 
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
   * Objectifs dont l’état est Actif et Version préliminaire.

1. (Facultatif) Sélectionnez le type d’informations à afficher en mettant à jour les filtres dans le coin supérieur droit de la section Graphiques.

   Pour plus d’informations sur les objectifs de filtrage, voir [Filtrage des informations dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Si vous avez choisi d’afficher plusieurs périodes, un graphique de l’état (jauge) ainsi qu’un graphique de l’état d’avancement (ligne) s’affichent pour chaque période.

1. Consultez les informations du tableau ci-dessous lorsque vous passez en revue le graphique de l’intégrité de l’objectif.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Nombre total d’objectifs | Le nombre au bas du graphique indique le nombre de tous les objectifs de la période sélectionnée, dans tous les états que vous avez sélectionnés. |
   |---|---|
   | Pourcentage moyen terminé | Dans la partie supérieure du graphique, ce nombre indique le pourcentage moyen d’objectifs actifs et fermés au cours de la période sélectionnée. |
   | Objectifs et progrès | Nombre d’objectifs pour chaque segment d’état d’avancement, lorsque vous passez la souris sur les segments du graphique. Seuls les objectifs dont l’état est Actif ou Fermé sont comptabilisés dans les segments. |


1. Consultez les informations du tableau ci-dessous lorsque vous passez en revue le graphique de progression de l’objectif.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Progression de base</td> 
      <td>La ligne d’inclinaison verte indique la moyenne globale attendue en pourcentage des objectifs actifs et fermés pour la période sélectionnée. Tous les objectifs d’une période donnée sont censés être atteints, de sorte que la progression de base est toujours de 100 % à la fin de la période. </td> 
     </tr> 
     <tr> 
      <td>Progression réelle</td> 
      <td> <p>La ligne bleue indique la moyenne globale réelle en pourcentage des objectifs actifs et fermés pour la période sélectionnée par incréments hebdomadaires. Chaque semaine pendant la durée de l’objectif est marquée par un noeud dans la ligne . </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passez le curseur de la souris sur un noeud week dans le graphique de progression de l’objectif et passez en revue les éléments suivants :

   * **Date de la semaine**: mois, jour et année de la semaine sélectionnée.
   * **Progression**: moyenne du pourcentage réel d’achèvement de tous les objectifs pour la semaine sélectionnée.
   * **Ligne de base**: moyenne du pourcentage attendu de tous les objectifs pour la semaine sélectionnée.

1. (Facultatif) Cliquez sur **Progression** au bas du graphique de progression pour supprimer la ligne de progression globale réelle

   Ou

   Cliquez sur **Ligne de base** au bas du graphique de progression pour supprimer la progression attendue du graphique.

 
