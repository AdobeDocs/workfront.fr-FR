---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher et regrouper : afficher la durée réelle du projet agrégée par la moyenne dans un groupement'
description: Vous pouvez ajouter la colonne suivante dans un rapport de projet afin d’afficher la Durée réelle agrégée sous la forme d’une moyenne dans un regroupement.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 41%

---

# Vue et regroupement : afficher la durée effective du projet agrégée par la moyenne dans un regroupement

Vous pouvez ajouter la colonne suivante dans un rapport de projet afin d’afficher la Durée réelle agrégée sous la forme d’une moyenne dans un regroupement.

![ project_with_aggregate_real_duration_in_grouping_view.png{1](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demander la modification d’une vue </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher la durée réelle du projet agrégée par la moyenne dans un groupement

Pour ajouter cette colonne à une vue de projet :

1. (Recommandé) Pour de meilleurs résultats et pour afficher la valeur moyenne agrégée de la durée réelle, un Regroupement doit être ajouté à la liste ou au rapport de votre projet.\
   Pour plus d’informations sur la création de groupes, consultez l’article [Présentation des groupes dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Accédez à une vue de projet existante.
1. Développez le menu déroulant Affichage et sélectionnez **Personnaliser la vue**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone **Afficher dans cette colonne**, puis cliquez sur **Cliquez pour modifier le texte**.

1. Supprimez tout le texte de la zone Mode Texte et remplacez-le par le code suivant :
   <pre>aggator.displayformat=composé <br>aggator.function=AVG <br>aggator.namekey=view.relatedcolumn <br>aggator.namekeyargkey=actualduration <br>aggator.valuefield=realDurationMinutes <br>aggator.valueformat=val <br>displayname=Project Current Duration <br>durationunitfield=realduration valeur <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=realDurationMinutes <br>textmode=true <br>valuefield=realDurationMinutes <br>valueformat=composé#M:D <br>viewalias=actualduration</pre>

1. Cliquez sur **Enregistrer la vue**.
