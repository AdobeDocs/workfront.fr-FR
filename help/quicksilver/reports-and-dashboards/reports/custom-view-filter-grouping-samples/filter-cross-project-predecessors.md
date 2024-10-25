---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Filtre : afficher les projets transversaux antérieurs incomplets »'
description: Ce filtre de tâches renvoie des projets transversaux antérieurs incomplets.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 57%

---

# Filtre : afficher les projets transversaux antérieurs incomplets

<!--Audited: 10/2024-->

Ce filtre de tâches renvoie des projets transversaux antérieurs incomplets.

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

## Filtrer les projets transversaux antérieurs

Pour appliquer ce filtre :

1. Accédez à une liste de tâches ou à un rapport de tâches.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.

1. (Conditionnel) Cliquez sur **Mode Texte** si vous avez accédé au filtre à partir d’une liste ou **Basculer vers le mode Texte**, si vous avez accédé au filtre à partir d’un rapport.
1. Dans la nouvelle zone, collez le code suivant :
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Conditionnel) Cliquez sur **Enregistrer le filtre** si vous avez accédé au filtre à partir d’un rapport, ou sur **Appliquer**, puis sur **Enregistrer comme nouveau** si vous avez accédé au filtre à partir d’une liste de tâches.
