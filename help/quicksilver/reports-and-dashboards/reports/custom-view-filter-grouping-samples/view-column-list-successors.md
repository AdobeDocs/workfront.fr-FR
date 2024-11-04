---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Afficher : Ajouter une liste de successeurs de tâches dans une colonne"
description: Vous pouvez ajouter une colonne à une vue de tâche pour afficher une liste des tâches ultérieures. La colonne Tâches ultérieures comprend le numéro de la tâche ultérieure ainsi que son nom.
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 72%

---

# Vue : ajouter une liste de tâches ultérieures dans une colonne

<!--Audited: 11/2024-->

Vous pouvez ajouter une colonne à une vue de tâche pour afficher une liste des tâches ultérieures. La colonne **Tâches ultérieures** comprend le numéro de la tâche ultéreure ainsi que son nom.

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
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

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Ajouter une liste de tâches ultérieures dans une colonne

Pour ajouter cette colonne à une vue de tâche, procédez comme suit :

1. Accédez à une liste de tâches.
1. Développez le menu déroulant **Afficher**, puis cliquez sur **Nouvelle vue**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**, puis sur **Modifier le mode Texte**.
1. Supprimez tout le texte de la zone **Modifier le mode de texte** et remplacez-le par le code suivant :

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
