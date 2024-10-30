---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Groupement : Répartition en pourcentage de la tâche 1"
description: '« Dans ce regroupement personnalisé de projets, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage terminé. » Les répartitions indiquent la valeur de pourcentage terminé avec des paliers de 25 % : 0 à 25 %, 25 à 50 %, etc. »'
author: Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 83%

---

# Regroupement : répartition 1 du pourcentage de tâche

<!--Audited: 10/2024-->

Dans ce regroupement de projets personnalisé, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage terminé. Les répartitions indiquent la valeur de pourcentage terminé avec des paliers de 25 % : 0 à 25 %, 25 à 50 %, etc.

Le regroupement suivant classe les tâches par valeur de pourcentage terminé en 6 regroupements différents :

* 0%
* 1 % à 25 %
* 26 % à 50 %
* 51 % à 75 %
* 76 % à 99 %
* 100%

![task_25__ventilation_regroupement.png](assets/task-25--breakdown-grouping-350x412.png)

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

## Regrouper par ventilation en pourcentage des tâches

Pour appliquer ce regroupement :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.
1. Cliquez sur **Ajouter un groupement**.

1. Cliquez sur **Passer en mode texte**.
1. Supprimez le texte dans la zone **Group by**.
1. Remplacez le texte par le code suivant :

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=26,"0-25 %",IF({percentComplete}<=51,"26-50 %",IF({percentComplete}<=76,"51-75 %",IF({percentComplete}<100,"76-99 %","100 %")))))
   group.0.valueformat=string
   ```

1. Cliquez sur **Done** > **Save Grouping**.
1. (Facultatif) Mettez à jour le nom du groupement, puis cliquez sur **Enregistrer le groupement**.
