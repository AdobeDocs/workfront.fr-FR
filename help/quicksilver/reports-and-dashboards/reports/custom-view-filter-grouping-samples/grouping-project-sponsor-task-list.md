---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Regroupement : personne sponsor du projet pour une liste de tâches »'
description: Ce regroupement de tâches permet de regrouper les tâches en fonction de la personne sponsor du projet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 100%

---

# Regroupement : sponsor du projet pour une liste de tâches

Ce regroupement de tâches permet de regrouper les tâches en fonction de la personne sponsor du projet.

![](assets/grouping--project-sponsor-for-a-task-350x189.png)

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
   <td> <p>Demander à modifier un regroupement </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et regroupements pour modifier un regroupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Regrouper par personne sponsor du projet pour une liste de tâches

Pour appliquer ce regroupement :

1. Accédez à la liste de tâches.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Basculer en mode texte**.
1. Supprimez le texte dans la fenêtre de modification du texte.
1. Copiez et collez le code suivant dans la fenêtre de modification du texte :

   ```
   group.0.name=Project Sponsor<br>group.0.valuefield=project:sponsor:name<br>group.0.valueformat=string
   ```

1. Cliquez sur **Enregistrer le regroupement**.
