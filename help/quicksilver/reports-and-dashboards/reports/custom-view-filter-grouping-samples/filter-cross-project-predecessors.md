---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : afficher les projets transversaux antérieurs incomplets'
description: Ce filtre de tâches renvoie des projets transversaux antérieurs incomplets.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 52%

---

# Filtre : afficher les projets transversaux antérieurs incomplets

<!--Audited: 10/2024-->

Ce filtre de tâches renvoie des projets transversaux antérieurs incomplets.

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

## Filtrer les projets transversaux antérieurs

Pour appliquer ce filtre :

1. Accédez à une liste de tâches ou à un rapport de tâche.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.

1. (Conditionnel) Cliquez sur **Mode texte** si vous avez accédé au filtre à partir d’une liste ou **Passer en mode texte** si vous avez accédé au filtre à partir d’un rapport.
1. Dans la nouvelle zone, collez le code suivant :
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. (Conditionnel) Cliquez sur **Enregistrer le filtre** si vous avez accédé au filtre à partir d’un rapport, ou sur **Appliquer**, puis sur **Enregistrer en tant que nouveau** si vous avez accédé au filtre à partir d’une liste de tâches.
