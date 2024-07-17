---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vue : ajouter une liste de successeurs de tâches dans une colonne'
description: Vous pouvez ajouter une colonne à un affichage de tâche pour afficher la liste des successeurs des tâches. La colonne Réussites de la tâche comprend le numéro du successeur ainsi que le nom.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 46%

---

# Vue : ajouter une liste de projets ultérieurs de tâche dans une colonne

Vous pouvez ajouter une colonne à un affichage de tâche pour afficher la liste des successeurs des tâches. La colonne **Succès de la tâche** inclut le numéro du successeur ainsi que le nom.

![task_view_with_a_list_of_succeeded_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## Ajouter une liste de successeurs de tâches dans une colonne

Pour ajouter cette colonne à une vue de tâche :

1. Accédez à une vue de tâche existante.
1. Développez le menu déroulant Affichage et sélectionnez **Personnaliser la vue**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone **Afficher dans cette colonne**, puis cliquez sur **Cliquez pour modifier le texte**.

1. Supprimez tout le texte de la zone Mode Texte et remplacez-le par le code suivant :
   <pre>displayname=Task Recipiors<br>listsepariter=<br><br>listmethod=nested(succeeded).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}){taskNumber},' - ',{successor}.{name})<br>valueformat=HTML</pre>

1. Cliquez sur **Enregistrer la vue**.
