---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : afficher les projets en cours en attente d’approbation'
description: Le filtre de projet suivant affiche les projets dans le statut actuel - En attente d’approbation, où la personne connectée est sponsor du projet ou responsable de Portfolio.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 78%

---

# Filtre : afficher les projets en cours en attente d’approbation

<!--Audited: 10/2024-->

Le filtre de projet suivant affiche les projets dans le statut actuel - En attente d’approbation, où la personne connectée est sponsor du projet ou responsable de Portfolio.

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

## Filtre : projets en cours en attente d’approbation

Pour appliquer ce filtre :

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.

1. Cliquez sur **Mode texte**.
1. Dans la zone affichée, copiez et collez le code suivant :
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. Cliquez sur **Appliquer** > **Enregistrer comme nouveau**.
