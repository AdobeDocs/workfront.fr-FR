---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Regroupement : groupement de tâches à 4 niveaux pour le propriétaire du Portfolio, le propriétaire du programme, le propriétaire du projet et l’état du projet"
description: Ce regroupement de tâches propose 4 niveaux de regroupement. Dans ce cas, les tâches sont regroupées par personne propriétaire du portfolio, personne propriétaire du programme, personne propriétaire du projet et statut du projet. L’interface standard ne permet pas d’avoir plus de 3 niveaux de regroupement. Pour ajouter un quatrième niveau, vous devez utiliser le mode texte. Vous ne pouvez pas regrouper les rapports selon plus de 4 critères à la fois.
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 87%

---

# Regroupement : regroupement de tâches à 4 niveaux pour la personne propriétaire du portfolio, la personne propriétaire du programme, la personne propriétaire du projet et le statut du projet

<!--Audited: 10/2024-->

Ce regroupement de tâches propose 4 niveaux de regroupement. Dans ce cas, les tâches sont regroupées par personne propriétaire du portfolio, personne propriétaire du programme, personne propriétaire du projet et statut du projet. L’interface standard ne permet pas d’avoir plus de 3 niveaux de regroupement. Pour ajouter un quatrième niveau, vous devez utiliser le mode texte. Vous ne pouvez pas regrouper les rapports selon plus de 4 critères à la fois.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
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

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un groupe de tâches à 4 niveaux pour la personne propriétaire du portfolio, la personne propriétaire du programme, la personne propriétaire du projet et le statut du projet

Pour appliquer ce regroupement :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Basculer en mode texte**.
1. Supprimez le texte de la zone **Regrouper votre rapport**.
1. Remplacez le texte de la zone affichée par le code suivant :
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. Cliquez sur **Terminé**, puis sur **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du groupement, puis cliquez sur **Enregistrer le groupement**.
