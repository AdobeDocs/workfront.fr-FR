---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Regroupement : ajouter un quatrième regroupement à une liste'
description: Vous pouvez avoir 4 regroupements dans un rapport de matrice. Pour plus d’informations sur les rapports de matrice, voir Créer un rapport de matrice.
author: Nolan
feature: Reports and Dashboards
exl-id: 1147a47b-c6e2-496e-b202-eefeb500054e
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 84%

---

# Regroupement : ajouter un quatrième regroupement à une liste

<!--Audited: 10/2024-->

Vous pouvez avoir 4 regroupements dans un rapport de matrice. Pour plus d’informations sur les rapports de matrice, voir [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

Vous ne pouvez avoir que 3 regroupements dans un rapport standard via l’interface standard. Pour ajouter un 4ème regroupement dans un rapport standard, vous devez utiliser le mode texte.

![Four_groupings_in_a_standard_report.png](assets/four-tier-grouping-for-tasks-350x239.png)

Par exemple, vous pouvez avoir un rapport de tâche qui est regroupé par Nom du projet, Statut de la progression et Date d’achèvement prévue, mais vous souhaitez également regrouper le rapport par Affecté au nom.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’un filtre </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter un quatrième regroupement à une liste

Pour ajouter un quatrième regroupement :

1. Cliquez sur **Basculer en mode texte**.
1. Supprimez le texte de la zone **Regrouper votre rapport**.
1. Remplacez le texte de la zone affichée par le code suivant :

   ```
   group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br>group.0.valuefield=project:name<br>group.0.valueformat=string<br>group.1.enumclass=com.attask.common.constants.ProgressStatusEnum<br>group.1.enumtype=TASK<br>group.1.linkedname=direct<br>group.1.namekey=progressStatus<br>group.1.type=enum<br>group.1.valuefield=progressStatus<br>group.1.valueformat=val<br>group.2.groupdatesby=WY<br>group.2.linkedname=direct<br>group.2.namekey=plannedCompletionDate<br>group.2.notime=false<br>group.2.valuefield=plannedCompletionDate<br>group.2.valueformat=atDateAsWeekString<br><strong>group.3.valuefield=assignedTo:name</strong><br style="font-weight: bold;"><strong>group.3.valueformat=HTML</strong><br>textmode=true
   ```

1. Cliquez sur **Terminé**, puis sur **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du regroupement, puis cliquez sur **Enregistrer le regroupement**.
