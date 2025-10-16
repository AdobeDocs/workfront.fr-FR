---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Regroupement : sponsor du projet pour les heures'
description: Ce regroupement d’heures organise les heures en fonction du sponsor du projet dans lequel les heures sont consignées. L’interface du Report Builder standard pour les regroupements d’heures ne fournit pas de mappage au champ Sponsor du projet. Vous devez utiliser l’interface Mode texte pour accéder à ce champ.
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 80%

---

# Regroupement : sponsor du projet pour les heures

<!--Audited: 10/2024-->

Ce regroupement d’heures organise les heures en fonction du sponsor du projet dans lequel les heures sont consignées. L’interface du Report Builder standard pour les regroupements d’heures ne fournit pas de mappage au champ Sponsor du projet. Vous devez utiliser l’interface Mode texte pour accéder à ce champ.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## Regrouper par sponsor du projet pour les heures

Pour appliquer ce regroupement :

1. Accédez à une liste d’heures.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Basculer en mode texte**.
1. Supprimez le texte de la zone qui s’affiche et remplacez-le par le code suivant :

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. Cliquez sur **Terminé**.
1. Mettez à jour le nom du regroupement, puis cliquez sur **Enregistrer le regroupement**.
