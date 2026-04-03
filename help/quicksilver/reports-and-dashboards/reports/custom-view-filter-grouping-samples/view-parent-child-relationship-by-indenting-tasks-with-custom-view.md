---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : permet d’afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches'
description: Vous pouvez maintenir la distinction des relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste de tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.
author: Courtney
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 78%

---

# Vue : afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches

<!--Audited: 11/2024-->

Vous pouvez maintenir la distinction des relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste de tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.

![Retrait parent enfant](assets/parent-child-indented-custom-view-350x94.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’une vue </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
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
1. Cliquez sur **Modifier le mode texte** et supprimez tout le texte existant.
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
