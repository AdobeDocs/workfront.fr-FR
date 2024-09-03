---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : afficher la relation parent-enfant dans une tâche en indentant les tâches. »'
description: Vous pouvez maintenir la distinction des relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste de tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 100%

---

# Vue : afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches

Vous pouvez maintenir la distinction des relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste de tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.

![](assets/parent-child-indented-custom-view-350x94.png)

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

## Afficher la relation parent-enfant dans une tâche en indentant les tâches

1. Accédez au projet contenant la liste de tâches que vous souhaitez exporter.
1. Cliquez sur le menu déroulant **Vue** et sélectionnez **Nouvelle vue**.

1. Nommez le filtre dans le coin supérieur gauche de l’écran.
1. Cliquez sur l’en-tête de la colonne **Nom de la tâche**.

1. Sélectionnez **Passer en mode Texte** dans le coin supérieur droit.
1. Cliquez n’importe où dans la zone de texte pour modifier le texte et supprimer tout texte existant.
1. Collez le texte suivant :


```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
```

1. Cliquer sur **Enregistrer**.
1. Cliquez sur **Enregistrer la.vue**.
