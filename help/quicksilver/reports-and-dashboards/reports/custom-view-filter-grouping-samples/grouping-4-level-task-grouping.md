---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Regroupement : regroupement de tâches à 4 niveaux pour la personne propriétaire du portfolio, la personne propriétaire du programme, la personne propriétaire du projet et le statut du projet »'
description: Ce regroupement de tâches propose 4 niveaux de regroupement. Dans ce cas, les tâches sont regroupées par personne propriétaire du portfolio, personne propriétaire du programme, personne propriétaire du projet et statut du projet. L’interface standard ne permet pas d’avoir plus de 3 niveaux de regroupement. Pour ajouter un quatrième niveau, vous devez utiliser le mode texte. Vous ne pouvez pas regrouper les rapports selon plus de 4 critères à la fois.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 100%

---

# Regroupement : regroupement de tâches à 4 niveaux pour la personne propriétaire du portfolio, la personne propriétaire du programme, la personne propriétaire du projet et le statut du projet

Ce regroupement de tâches propose 4 niveaux de regroupement. Dans ce cas, les tâches sont regroupées par personne propriétaire du portfolio, personne propriétaire du programme, personne propriétaire du projet et statut du projet.L’interface standard ne permet pas d’avoir plus de 3 niveaux de regroupement. Pour ajouter un quatrième niveau, vous devez utiliser le mode texte. Vous ne pouvez pas regrouper les rapports selon plus de 4 critères à la fois.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <td> <p>Demander à modifier un regroupement </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et regroupements pour modifier un regroupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer un groupe de tâches à 4 niveaux pour la personne propriétaire du portfolio, la personne propriétaire du programme, la personne propriétaire du projet et le statut du projet

Pour appliquer ce regroupement :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Passer en mode texte**.
1. Supprimez le texte dans la zone **Regrouper votre rapport**.
1. Remplacez le texte par le code suivant :
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. Cliquez sur **Enregistrer le regroupement**.
