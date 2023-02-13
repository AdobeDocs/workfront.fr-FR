---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : afficher la relation parent-enfant dans une tâche en mettant en retrait les'
description: Vous pouvez maintenir la distinction entre les relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste des tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# Afficher : afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches ;

Vous pouvez maintenir la distinction entre les relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste des tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.  

![](assets/parent-child-indented-custom-view-350x94.png)

1. Accédez au projet avec la liste des tâches que vous souhaitez exporter.
1. Cliquez sur le bouton **Affichage** , puis sélectionnez **Nouvelle vue**.

1. Nommez le filtre dans le coin supérieur gauche de l’écran.
1. Cliquez sur dans le **Nom de la tâche** en-tête de colonne.

1. Sélectionner **Passer en mode Texte** dans le coin supérieur droit.
1. Cliquez n’importe où dans la zone de texte pour modifier le texte et supprimez tout le texte existant.
1. Collez le texte suivant :

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. Cliquer sur **Enregistrer**.
1. Cliquez sur **Enregistrer la vue**.
