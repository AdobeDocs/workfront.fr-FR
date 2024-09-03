---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Afficher et regrouper : afficher la durée effective du projet agrégée par la moyenne dans un regroupement »'
description: Vous pouvez ajouter la colonne suivante dans un rapport sur les projets afin d’afficher la durée effective agrégée sous la forme d’une moyenne dans un regroupement.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 100%

---

# Vue et regroupement : afficher la durée réelle du projet agrégée par la moyenne dans un regroupement

Vous pouvez ajouter la colonne suivante dans un rapport sur les projets afin d’afficher la durée effective agrégée sous la forme d’une moyenne dans un regroupement.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demander la modification d’un affichage </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher la durée effective du projet agrégée par la moyenne dans un regroupement

Pour ajouter cette colonne à une vue de projet, procédez comme suit :

1. (Recommandé) Pour de meilleurs résultats et pour afficher la valeur moyenne agrégée de la durée effective, un regroupement doit être ajouté à votre liste ou au rapport sur les projets.\
   Pour plus d’informations sur la création de regroupements, consultez l’article [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Accédez à une vue de projet existante.
1. Développez le menu déroulant « Vue », puis sélectionnez **Personnaliser la vue**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Basculer en mode texte**.
1. Passez la souris sur la zone **Afficher dans cette colonne**, puis cliquez sur **Cliquez pour modifier le texte**.

1. Supprimez tout le texte de la zone du mode texte et remplacez-le par le code suivant :
   <pre>aggregator.displayformat=compound <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=Project Actual Duration <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=actualDurationMinutes <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M:D <br>viewalias=actualduration</pre>

1. Cliquez sur **Enregistrer la vue**.
