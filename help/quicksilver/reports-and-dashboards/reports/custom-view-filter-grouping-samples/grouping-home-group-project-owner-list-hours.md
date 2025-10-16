---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Regroupement : groupe principal du propriétaire du projet dans une liste d''heures'
description: Vous pouvez afficher le nom du groupe principal de la personne propriétaire du projet dans une liste d’heures ou un rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 6491ab9b-c09e-4bdb-99c2-56bb44f66947
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 77%

---

# Regroupement : groupe principal de la personne propriétaire de projet dans une liste d’heures

<!--Audited: 10/2024-->

Vous pouvez afficher le nom du groupe principal de la personne propriétaire du projet dans une liste d’heures ou un rapport.

Le regroupement regroupe également les résultats en fonction du nom de la personne propriétaire du projet et du nom du projet.

![grouping_for_project_owner_home_group.png](assets/grouping-for-project-owner-home-group-350x51.png)

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

## Regroupement par groupe principal du propriétaire du projet dans une liste d’heures

Pour appliquer ce regroupement :

1. Accédez à une liste d’heures.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Basculer en mode texte**.
1. Supprimez le texte de la zone **Regrouper par**.
1. Remplacez le texte par le code suivant :

```
group.0.displayname=Home Group of Project Owner
group.0.valuefield=project:owner:homeGroup:name
group.0.valueformat=HTML
group.1.displayname=Project Owner
group.1.linkedname=projectOwnerMM
group.1.namekey=view.relatedcolumn
group.1.namekeyargkey.0=projectOwnerMM
group.1.namekeyargkey.1=name
group.1.valuefield=projectOwnerMM:name
group.1.valueformat=string
group.2.displayname=Project Name
group.2.linkedname=project
group.2.namekey=view.relatedcolumn
group.2.namekeyargkey.0=project
group.2.namekeyargkey.1=name
group.2.valuefield=project:name
group.2.valueformat=string
textmode=true
```

1. Cliquez sur **Terminé** > **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du regroupement, puis cliquez sur **Enregistrer le regroupement**.
