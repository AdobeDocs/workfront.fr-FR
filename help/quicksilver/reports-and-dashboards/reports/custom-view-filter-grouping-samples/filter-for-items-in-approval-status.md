---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : afficher uniquement les éléments ayant un statut d’approbation'
description: Vous pouvez afficher uniquement les éléments ayant un certain statut qui est actuellement Approbation en attente. Cela fonctionne de la même manière pour tout autre objet ayant un statut d’approbation.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 76%

---

# Filtre : afficher uniquement les éléments ayant un statut d’approbation

<!--Audited: 10/2024-->

Vous pouvez afficher uniquement les éléments ayant un certain statut qui est actuellement Approbation en attente. Cela fonctionne de la même manière pour tout autre objet ayant un statut d’approbation.

Vous pouvez conférer aux objets suivants un statut d’approbation :

* Tâches
* Problèmes
* Projets

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

## Afficher uniquement les éléments ayant un statut d’approbation

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.
1. Choisissez de filtrer par **Projet : statut**, puis sélectionnez le statut en fonction duquel vous souhaitez effectuer le filtrage dans la liste.

   Par exemple, dans un rapport de projet, ajoutez **Statut égal à planification**, si vous souhaitez afficher uniquement les projets dont le statut est **Planification - Approbation en attente**.
1. Cliquez sur **Mode texte**.
1. Modifiez la ligne de `status` en ajoutant **:A** à la clé de 3 lettres du statut :
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Cliquez sur **Appliquer** > **Enregistrer comme nouveau**.

   La liste n’affiche que les projets dont le statut est Planification - Approbation en attente.
