---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches »'
description: Vous pouvez maintenir la distinction entre les relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste des tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: ht
source-wordcount: '299'
ht-degree: 100%

---

# Vue : afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches

Vous pouvez maintenir la distinction entre les relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste des tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.

![](assets/parent-child-indented-custom-view-350x94.png)

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

## Afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches

1. Accédez au projet avec la liste des tâches que vous souhaitez exporter.
1. Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.

1. Nommez le filtre dans le coin supérieur gauche de l’écran.
1. Cliquez sur dans l’en-tête de colonne **Nom de la tâche**.

1. Sélectionner **Passer en mode Texte** dans le coin supérieur droit.
1. Cliquez n’importe où dans la zone de texte pour modifier le texte et supprimez tout le texte existant.
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
1. Cliquez sur **Enregistrer la vue**.
