---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : afficher le nom des tâches parentes sous la forme de majuscules"
description: Vous pouvez ajouter cette colonne à une vue de tâche pour afficher le nom des tâches parentes dans toutes les majuscules.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 41%

---

# Vue : afficher le nom des tâches parent en majuscules

Vous pouvez ajouter cette colonne à une vue de tâche pour afficher le nom des tâches parentes dans toutes les majuscules.

![](assets/column-task-with-all-caps-parent-350x112.png)

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
   <td> <p>Demande de modification des filtres, des vues et des regroupements </p>
   <p>Prévision de la modification des rapports</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue individuelle</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher le nom des tâches parentes sous forme de majuscules

Pour créer cette colonne dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Affichage**, sélectionnez **Personnaliser la vue**.\
   Ou\
   Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, cliquez sur l’en-tête de la colonne qui indique le nom de la tâche dans la liste.
1. Cliquez sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant : <pre>descriptionkey=name<br>displayname=Task Name<br>textmode=true<br>valueexpression=IF({numberOfChildren}>&quot;0&quot;,UPPER({name}),{name})<br>valueformat=HTML<br>width=150<br></pre>

1. Cliquez sur **Enregistrer la vue**.
