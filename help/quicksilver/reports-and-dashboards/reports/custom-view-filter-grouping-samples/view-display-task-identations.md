---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : afficher les mises en retrait de tâche dans une liste de tâches »'
description: Dans cette vue de tâche, vous pouvez ajouter du code à la colonne Nom de la tâche pour afficher les tâches mises en retrait selon la structure de répartition du travail du projet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 100%

---

# Vue : afficher les mises en retrait de tâche dans une liste de tâches

Dans cette vue de tâche, vous pouvez ajouter du code à la colonne Nom de la tâche pour afficher les tâches mises en retrait selon la structure de répartition du travail du projet.

![](assets/view-text-mode-indentation-task-list-350x171.png)

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
   <td> <p>Demander la modification d’un affichage </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher les mises en retraits de tâche dans une colonne de liste de tâches

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** et commencez à saisir « Nom de la tâche » dans le champ **Afficher dans cette colonne** puis sélectionnez-le lorsqu’il apparaît dans la liste.

1. Dans la nouvelle colonne, cliquez sur **Passer en mode texte**.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la ligne `valuefield=` et remplacez-le par le code suivant :

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Cliquez sur **Enregistrer**, puis sur **Enregistrer la vue**.
