---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : ajouter une liste de tâches successives dans une colonne'
description: Vous pouvez ajouter une colonne à une vue de tâche pour afficher une liste des tâches ultérieures. La colonne Tâches ultérieures comprend le numéro de la tâche ultérieure ainsi que son nom.
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 69%

---

# Vue : ajouter une liste de tâches ultérieures dans une colonne

<!--Audited: 11/2024-->

Vous pouvez ajouter une colonne à une vue de tâche pour afficher une liste des tâches ultérieures. La colonne **Tâches ultérieures** comprend le numéro de la tâche ultéreure ainsi que son nom.

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’un filtre </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Ajouter une liste de tâches ultérieures dans une colonne

Pour ajouter cette colonne à une vue de tâche, procédez comme suit :

1. Accédez à une liste de tâches.
1. Développez le menu déroulant **Affichage**, puis cliquez sur **Nouvel affichage**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Basculer en mode texte**, puis sur **Modifier le mode texte**.
1. Supprimez tout le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.
