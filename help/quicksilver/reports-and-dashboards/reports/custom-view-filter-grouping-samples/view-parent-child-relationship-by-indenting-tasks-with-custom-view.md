---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches'
description: Vous pouvez maintenir la distinction des relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste de tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 86%

---

# Vue : afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches

<!--Audited: 11/2024-->

Vous pouvez maintenir la distinction des relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste de tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.

![](assets/parent-child-indented-custom-view-350x94.png)

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p> Actuel : 
   <ul>
   <li>Demander la modification d’un affichage</li> 
   <li>Prévoir de modifier un rapport</li>
   </ul>
     </p>
     <p> Nouveau : 
   <ul>
   <li>Contributeur à la modification d’une vue</li> 
   <li>Standard pour modifier un rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher la relation parent-enfant dans une tâche en indentant les tâches

1. Accédez au projet contenant la liste de tâches que vous souhaitez exporter.
1. Cliquez sur le menu déroulant **Vue** et sélectionnez **Nouvelle vue**.
1. Cliquez sur l’en-tête de la colonne **Nom de la tâche**.
1. Sélectionnez **Passer en mode Texte** dans le coin supérieur droit.
1. Cliquez sur **Modifier le mode Texte** et supprimez tout le texte existant.
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

1. Cliquez sur **Terminé** > **Enregistrer la vue**.
