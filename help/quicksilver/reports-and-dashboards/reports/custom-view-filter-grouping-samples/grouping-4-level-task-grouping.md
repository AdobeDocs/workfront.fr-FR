---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Regroupement : regroupement de tâches à 4 niveaux pour le propriétaire du Portfolio, le propriétaire du programme, le propriétaire du projet et l’état du projet"
description: Ce groupement de tâches fournit 4 niveaux de groupement. Dans ce cas, les tâches sont regroupées par propriétaire de Portfolio, propriétaire de programme, propriétaire de projet et état du projet. Vous ne pouvez avoir que 3 niveaux de Regroupement au maximum à l'aide de l'interface standard. Pour ajouter un quatrième niveau, vous devez utiliser le mode Texte. Vous ne pouvez pas regrouper les rapports selon plus de 4 critères en même temps.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 33%

---

# Regroupement : regroupement de tâches à 4 niveaux pour la personne propriétaire du portfolio, la personne propriétaire du programme, la personne propriétaire du projet et le statut du projet

Ce groupement de tâches fournit 4 niveaux de groupement. Dans ce cas, les tâches sont regroupées par propriétaire de Portfolio, propriétaire de programme, propriétaire de projet et état du projet. Vous ne pouvez avoir que 3 niveaux de Regroupement au maximum à l&#39;aide de l&#39;interface standard. Pour ajouter un quatrième niveau, vous devez utiliser le mode Texte. Vous ne pouvez pas regrouper les rapports selon plus de 4 critères en même temps.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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

## Créez un groupe de tâches à 4 niveaux pour le propriétaire du Portfolio, le propriétaire du programme, le propriétaire du projet et l’état du projet.

Pour appliquer ce groupement :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Groupement**, sélectionnez **Nouveau groupement**.

1. Cliquez sur **Passer en mode Texte**.
1. Supprimez le texte dans la zone **Regrouper votre rapport**.
1. Remplacez le texte par le code suivant :
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Propriétaire<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:propriétaire:name<br>groupe.0.valueformat=string<br>groupe.1.linkedname=projet<br>groupe.1.name=Programme Propriétaire<br>groupe.1.notime=false}group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projecnerecnermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.3 amekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val<br></pre>

1. Cliquez sur **Enregistrer le groupement**.
