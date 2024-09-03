---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : afficher le nom des tâches parent en majuscules »'
description: Vous pouvez ajouter cette colonne à une vue de tâche pour afficher le nom des tâches parent en majuscules.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 100%

---

# Vue : afficher le nom des tâches parent en majuscules

Vous pouvez ajouter cette colonne à une vue de tâche pour afficher le nom des tâches parent en majuscules.

![](assets/column-task-with-all-caps-parent-350x112.png)

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
   <td> <p>Demande pour modifier les filtres, les vues et les regroupements </p>
   <p>Plan pour modifier les rapports</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Accès Modifier aux filtres, vues et regroupements pour modifier une vue individuelle</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher le nom des tâches parent en majuscules

Pour créer cette colonne dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, sélectionnez **Personnaliser la vue**.\
   Ou\
   Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu de la colonne**, cliquez sur l’en-tête de la colonne qui indique le nom de la tâche dans la liste.
1. Cliquez sur **Basculer en mode texte**.
1. Placez la souris sur la zone du mode texte et cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant : <pre>descriptionkey=name<br>displayname=Task Name<br>textmode=true<br>valueexpression=IF({numberOfChildren}>&quot;0&quot;,UPPER({name}),{name})<br>valueformat=HTML<br>width=150<br></pre>

1. Cliquez sur **Enregistrer la vue**.
