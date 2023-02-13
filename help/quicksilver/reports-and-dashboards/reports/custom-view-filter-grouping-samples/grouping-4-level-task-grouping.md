---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Groupement : Regroupement de tâches à 4 niveaux pour le propriétaire du Portfolio, le propriétaire du programme, le propriétaire du projet et l’état du projet'
description: Ce groupement de tâches fournit 4 niveaux de groupement. Dans ce cas, les tâches sont regroupées par propriétaire de Portfolio, propriétaire de programme, propriétaire de projet et état du projet. Vous ne pouvez avoir que 3 niveaux de Regroupement au maximum à l'aide de l'interface standard. Pour ajouter un quatrième niveau, vous devez utiliser le mode Texte. Vous ne pouvez pas regrouper les rapports selon plus de 4 critères en même temps.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Regroupement : Regroupement de tâches à 4 niveaux pour le propriétaire du Portfolio, le propriétaire du programme, le propriétaire du projet et l’état du projet

Ce groupement de tâches fournit 4 niveaux de groupement. Dans ce cas, les tâches sont regroupées par propriétaire de Portfolio, propriétaire de programme, propriétaire de projet et état du projet. Vous ne pouvez avoir que 3 niveaux de Regroupement au maximum à l&#39;aide de l&#39;interface standard. Pour ajouter un quatrième niveau, vous devez utiliser le mode Texte. Vous ne pouvez pas regrouper les rapports selon plus de 4 critères en même temps.

![four_tier_regroupement_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Créez un groupe de tâches à 4 niveaux pour le propriétaire du Portfolio, le propriétaire du programme, le propriétaire du projet et l’état du projet.

Pour appliquer ce groupement :

1. Accédez à une liste de tâches.
1. Dans la **Regroupement** menu déroulant, sélectionnez **Nouveau groupement**.

1. Cliquez sur **Passer en mode Texte**.
1. Supprimez le texte de la section **Regrouper votre rapport** zone.
1. Remplacez le texte par le code suivant :

   <pre>group.0.linkedname=project<br>group.0.name=Propriétaire du Portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:propriétaire:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Propriétaire du programme<br>group.1.notime=false<br>group.1.valuefield=project:program:propriétaire:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.name.keyargkey.0=project<br>group.3.name.keyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. Cliquez sur **Enregistrer le groupement**.
