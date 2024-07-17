---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Groupement : répartition en pourcentage du projet 1"
description: Dans ce regroupement personnalisé de projets, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage de réalisation.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 42%

---

# Regroupement : ventilation en pourcentage des projets (1)

Dans ce regroupement personnalisé de projets, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage de réalisation.

Le regroupement suivant classe les projets par pourcentage de valeur complète dans l’un de ces regroupements :

* 0%
* 1 à 25 %
* 26 à 50 %
* 51 à 75 %
* 76 à 99 %
* 100%

![percent_complete_ventilation_custom_project_grouping_25__incréments.png](assets/percent-complete-breakdown-custom-350x56.png)

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
   <td> <p>Demande de modification d’un groupement </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Editer l'accès aux Filtres, Vues, Groupements pour modifier un groupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Répartition des groupes par pourcentage de projet

Pour appliquer ce groupement :

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Groupement**, sélectionnez **Nouveau groupement**.

1. Cliquez sur **Passer en mode Texte**.
1. Supprimez le texte de la zone et collez le code suivant dans l’espace disponible :
   <pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %", IF({percentComplete}&lt;=26,"0-25 %", IF({percentComplete}&lt;=51,"25-50 %",({percentComplete}&lt;=76,"50-75 %",IF({percentComplete}&lt;100,"75-99 %","100 %"))))<br>group.0.valueformat=string</pre>

1. Cliquez sur **Enregistrer le groupement**.
