---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vue : variance de ligne de base pour la durée et le travail planifié dans une vue de tâche"
description: Affichez la variance de ligne de base pour la durée et le travail planifié.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2a1eef9c-016c-4a04-acda-6070fcb0e23d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 27%

---

# Vue : écart de référence pour la durée et le travail prévu dans une vue de tâche

Cette vue affiche les éléments suivants dans une vue de tâche :

* Informations sur les tâches avec des informations de tâche de base.
* Différence entre la durée et la durée de référence par défaut.
* Différence entre le travail planifié et le travail planifié par défaut.

>[!NOTE]
>
> Les données affichées dans la vue suivante comparent les valeurs réelles de la tâche aux valeurs associées aux tâches de la ligne de base par défaut.

 

![baseline_variance_in_a_task_view.png](assets/baseline-variance-in-a-task-view-350x38.png)

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

## Affichage de la variance de ligne de base pour la durée et le travail planifié dans un affichage de tâche

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Affichage**, sélectionnez **Nouvelle vue**.

1. Supprimez toutes les colonnes de la vue, sauf la première.
1. Avec la première colonne sélectionnée, cliquez sur **Passer en mode Texte**.
1. Copiez le texte ci-dessous et collez-le dans la première colonne de la vue :
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br> 0.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.étich=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.0.displayname=Task Name<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=int Int(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valuefield=durationFieldLong<br>column.1.value<br>column.1.viewalias=duration<br>column.1.width=100<br>column.1.displayname=Task Duration<br>column.2.descriptionkey=view.relatedcolumn<br>column.2.descriptionkeyargkey.0=defaultbaselinetask<br>column.2.keyargkey.1=duration<br>column.2.linkedname=defaultBaselineTask<br>column.2.listsort=intAsInt(durationMinutes)<br>column.2.namekey=duration<br>column.2.namekeyargkey.0=defaultbaselinetask.abbr{35.column 2.namekeyargkey.1=duration.abbr<br>column.2.querysort=defaultBaselineTask:durationMinutes<br>column.2.shortview=false<br>column.2.étich=0<br>column.2.value=defaultBaselineTask:durationFieldLong<br>column.2.value format=composé<br>column.2.viewalias=defaultBaselineTask:duration<br>column.2.width=100<br>column.2.displayname=Dflt Baseline Tâche : Dur<br>column.2.durationunitfield=durationUnit.value<br>column.3.description=Durance"column 3.linkedname=direct<br>column.3.listsort=intAsInt(durationMinutes)<br>column.3.name=Duration Variance<br>column.3.querysort=durationMinutes<br>column.3.shortview=false<br>column.3.étich=0<br>column.3.value=CONCAT(SUB({duration},{defaultBaselineTask}).<br>{duration})/480," Days")<br>column.3.valueformat=HTML<br>column.3.viewalias=duration<br>column.3.width=100<br>column.3.displayname=Duration Variance<br>column.4.description=workrequired<br>column.4.linkedname=direct<br>column.4.listsort=doubleAsDouble(workRequired)<br>column.4.namekey=workrequired.abbr<br>column.4.querysort=workRequired<br>column.4.shortview=false<br>column.4.étich=0<br>column.4.valuefield=workFieldLong<br>column.4.4 ueformat=composé<br>column.4.viewalias=workrequired<br>column.4.width=100<br>column.4.displayname=Work Req<br>column.5.description=view.relatedcolumn<br>column.5.descriptionkeyargkey.0=defaultbaselinetask<br>column.5.descriptionkeyargkey.1=workrequired<br>column.5.linkedname=defaultBaselineTask<br>column.5.listsort=doubleAsDouble(workRequired)<br>column.5.namekey=view.relatedcolumn<br>column.5.namekeyargkey.0=defaultbaseteletinetcolumn ask.abbr<br>column.5.namekeyargkey.1=workrequired.abbr<br>column.5.querysort=defaultBaselineTask:workRequired<br>column.5.shortview=false<br>column.5.étich=0<br>column.5.valuefield=defaultBaselineTask:work Long<br>column.5.valueformat=composé<br>column.5.viewalias=defaultBaselineTask:workrequired<br>column.5.width=100<br>column.5.displayname=Dflt Baseline Tâche : workflow Req<br>column.6.descriptionkey=workrequired<br>column 6.linkedname=direct<br>column.6.listsort=doubleAsDouble(workRequired)<br>column.6.name=Effort Variance<br>column.6.querysort=workRequired<br>column.6.shortview=false<br>column.6.étich=0<br>column.6.value=CONCAT(SUB({workRequired},{defaultBaselineTask}).{workRequired})/60," Hours")<br>column.6.valueformat=HTML<br>column.6.viewalias=workrequired<br>column.6.width=100<br>column.6.displayname=Effort Variance</pre>

1. Cliquez sur **Enregistrer la vue**.