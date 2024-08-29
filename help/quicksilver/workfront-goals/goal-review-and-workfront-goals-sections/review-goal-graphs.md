---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Réviser des graphiques pour comprendre les tendances de progression des objectifs dans Objectifs Adobe Workfront
description: Vous pouvez afficher l’intégrité globale de vos objectifs et la tendance de leur progression dans le temps dans la section Graphiques des objectifs Adobe Workfront. Les graphiques de cette section ne ventilent pas la progression de chaque objectif, mais vous donnent à la place un aperçu holistique du statut de la progression de tous les objectifs ainsi que la tendance de leur progression dans le temps au cours d’une période donnée.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 100%

---

# Réviser des graphiques pour comprendre les tendances de progression des objectifs dans Objectifs Adobe Workfront

<!-- drafted mostly for P&P release-->

Vous pouvez afficher l’intégrité globale de vos objectifs et la tendance de leur progression dans le temps dans la section Graphiques des objectifs Adobe Workfront. Les graphiques de cette section ne ventilent pas la progression de chaque objectif, mais vous donnent à la place un aperçu holistique du statut de la progression de tous les objectifs ainsi que la tendance de leur progression dans le temps au cours d’une période donnée.

>[!IMPORTANT]
>
>Vous pouvez consulter le nombre total de vos objectifs dans la section Graphiques pour une période donnée.Toutefois, les Objectifs Workfront ne prennent en compte que les objectifs dont le statut est Actif et Fermé lors du calcul du statut de la progression global de l’objectif et du pourcentage terminé.

## Conditions d’accès

Pour effectuer les actions décrites dans cet article, vous devez disposer de l’accès suivant :

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> 
   <p>Pour la nouvelle structure de forfait et de licence :
  <ul><li>Un forfait Ultimate </li></ul>
   </p>
<p>Pour la structure de forfait et de licence actuelle : 
<ul><li> Un forfait Pro ou supérieur </li>
  <li>Une licence Objectifs Adobe Workfront en plus d’une licence Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront*</td>
 <td>
 <p>Nouvelle licence : contributeur ou contributrice ou supérieure</p>
 Ou
 <p>Licence actuelle : demande ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produit*</td>
 <td>
 <p> Nouvelle exigence de produit, une des options suivantes : </p>
<ul>
<li>Un forfait Adobe Workfront Select ou Prime et une licence Objectifs Adobe Workfront supplémentaire.</li>
<li>Un forfait Workfront Ultimate qui inclut Objectifs Workfront par défaut. </li></ul>
 <p>Ou</p>
 <p>Exigence de produit actuelle : un forfait Workfront et une licence supplémentaire pour Objectifs Adobe Workfront. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Exigences pour l’utilisation des Objectifs Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Niveau d’accès</p></td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Autorisations d’affichage ou de niveau supérieur sur l’objectif pour l’afficher</p>
  <p>Autorisations de gestion sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, consultez <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans les Objectifs Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Types de graphiques dans Objectifs Workfront

Les graphiques suivants sont disponibles dans la section Graphiques ou dans Objectifs Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Graphique de l’intégrité des objectifs</td> 
   <td> <p>Graphique d’enregistrement qui affiche les éléments suivants :</p> 
    <ul> 
     <li>Nombre total d’objectifs pour la période sélectionnée. Les objectifs sont pris en compte, peu importe leur statut. </li> 
     <li>Statut de la progression des objectifs dont le statut est Actif et Fermé.</li> 
    </ul> <p>Pour plus d’informations sur la façon dont les Objectifs Workfront calculent le statut de la progression, voir <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Vue d’ensemble de la progression et du statut des objectifs dans Objectifs Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Graphique de progression de l’objectif</td> 
   <td> <p>Graphique en courbe qui affiche les mises à jour apportées aux objectifs par incréments hebdomadaires pendant la durée de l’objectif. Le graphique de progression de l’objectif affiche les éléments suivants :</p> 
    <ul> 
     <li>Pourcentage terminé moyen attendu et réel de tous les objectifs actifs et fermés au cours de la période sélectionnée. Le pourcentage terminé de progression est ventilé en incréments hebdomadaires marqués par des nœuds. </li> 
     <li>Le pourcentage moyen global de la progression des objectifs actifs et fermés depuis la semaine précédente. </li> 
    </ul> <p>Conseil : il se peut que le graphique de progression de l’objectif n’affiche aucune information lorsque des mises à jour sont effectuées sur les objectifs en dehors de la période sélectionnée. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Examiner la progression de l’objectif dans les graphiques

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) > **Objectifs** dans le coin supérieur droit.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La zone Objectifs Workfront s’ouvre alors.

1. Cliquez sur **Graphiques** dans le panneau de gauche.

   ![](assets/graphs-in-left-panel.png)

   La section Graphiques s’affiche.

   Par défaut, les objectifs affichés dans la section Graphiques sont limités par les critères suivants :

   * Filtres appliqués à la zone Graphiques.
   * Objectifs dont le statut est Actif et Brouillon.

1. (Facultatif) Sélectionnez le type d’informations à afficher en mettant à jour les filtres dans le coin supérieur droit de la section Graphiques.

   Pour plus d’informations sur le filtrage des objectifs, voir [Filtrer les informations dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Si vous avez choisi d’afficher plusieurs périodes, un graphique de l’intégrité de l’objectif (jauge) ainsi qu’un graphique de progression de l’objectif (courbe) s’affichent pour chaque période.

1. Consultez les informations du tableau ci-dessous lorsque vous passez en revue le graphique de l’intégrité de l’objectif.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Nombre total d’objectifs | Le nombre au bas du graphique indique le nombre de tous les objectifs de la période sélectionnée, dans tous les statuts que vous avez sélectionnés. |
   |---|---|
   | Pourcentage terminé moyen | Dans la partie supérieure du graphique, ce nombre indique le pourcentage moyen d’objectifs actifs et fermés au cours de la période sélectionnée. |
   | Objectifs et leur progression | Nombre d’objectifs pour chaque segment du statut de la progression, lorsque vous pointez sur les segments du graphique. Seuls les objectifs dont le statut est Actif ou Fermé sont comptabilisés dans les segments. |


1. Consultez les informations du tableau ci-dessous lorsque vous passez en revue le graphique de progression de l’objectif.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Progression de référence</td> 
      <td>La ligne verte indique le pourcentage terminé global moyen attendu des objectifs actifs et fermés pour la période sélectionnée. Tous les objectifs d’une période donnée sont censés être atteints, de sorte que la progression de référence est toujours de 100 % à la fin de la période. </td> 
     </tr> 
     <tr> 
      <td>Progression en cours</td> 
      <td> <p>La ligne bleue indique le pourcentage terminé global moyen réel des objectifs actifs et fermés pour la période sélectionnée par incréments hebdomadaires. Chaque semaine pendant la durée de l’objectif est représentée par un nœud sur la ligne. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Pointez sur un nœud représentant une semaine dans le graphique de progression de l’objectif et passez en revue les éléments suivants :

   * **Date de la semaine** : mois, jour et année de la semaine sélectionnée.
   * **Progression** : moyenne du pourcentage terminé réel de tous les objectifs pour la semaine sélectionnée.
   * **Référence** : moyenne du pourcentage terminé attendu de tous les objectifs pour la semaine sélectionnée.

1. (Facultatif) Cliquez sur **Progression** au bas du graphique de progression pour supprimer la ligne de progression globale en cours.

   Ou

   Cliquez sur **Référence** au bas du graphique de progression pour supprimer la ligne de progression attendue du graphique.

 
