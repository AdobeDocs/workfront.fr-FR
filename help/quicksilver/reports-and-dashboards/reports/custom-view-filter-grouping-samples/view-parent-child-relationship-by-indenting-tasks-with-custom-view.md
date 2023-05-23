---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : afficher la relation parent-enfant dans une tâche en mettant en retrait les'
description: Vous pouvez maintenir la distinction entre les relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste des tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 1%

---

# Afficher : afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches ;

Vous pouvez maintenir la distinction entre les relations parent-enfant dans une liste de tâches exportée en ajoutant une vue personnalisée à la liste des tâches et en vous assurant que cette vue est sélectionnée avant d’exporter la liste.

![](assets/parent-child-indented-custom-view-350x94.png)

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
   <td> <p>Demande de modification d’une vue </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification d’un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher la relation parent-enfant dans une tâche en mettant en retrait les tâches

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
