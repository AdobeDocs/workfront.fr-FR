---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : société et groupe principal de l''utilisateur affecté'
description: Cette vue de tâche affiche l’entreprise et le groupe principal de la personne propriétaire principale de la tâche. Il s’agit de valeurs qui ne sont pas disponibles dans l’interface standard, mais qui sont accessibles via le mode texte.
author: Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 68%

---

# Vue : entreprise et groupe principal de la personne affectée

<!--Audited: 11/2024-->

Cette vue de tâche affiche l’entreprise et le groupe principal de la personne propriétaire principale de la tâche. Il s’agit de valeurs qui ne sont pas disponibles dans l’interface standard, mais qui sont accessibles via le mode texte.

![Afficher la société et le groupe principal de l’utilisateur affecté](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## Vue de l’entreprise et du groupe principal de la personne affectée

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Affichage**, sélectionnez **Nouvel affichage**.

1. Dans la zone **Aperçu des colonnes**, éliminez toutes les colonnes à l’exception d’une seule.
1. Cliquez sur l’en-tête de la colonne restante, puis cliquez sur **Basculer en mode texte**.
1. Cliquez sur **Modifier le mode texte**.
1. Supprimez le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=assignedto
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=assignedTo:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=assignedTo:objCode
   column.1.link.valueformat=val
   column.1.linkedname=assignedTo
   column.1.listsort=nested(assignedTo).string(name)
   column.1.namekey=assignedto
   column.1.querysort=assignedTo:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=assignedTo:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Assigned To Company
   column.2.displayname=Assigned To Company
   column.2.linkedname=assignedTo:company
   column.2.listsort=nested(assignedTo:company).string(name)
   column.2.namekey=assignedto
   column.2.querysort=assignedTo:company:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=assignedTo:company:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Assigned To Home Group
   column.3.displayname=Assigned To Home Group
   column.3.linkedname=assignedTo:homeGroup
   column.3.listsort=nested(assignedTo:homeGroup).string(name)
   column.3.namekey=assignedto
   column.3.querysort=assignedTo:homeGroup:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=assignedTo:homeGroup:name
   column.3.valueformat=HTML
   column.3.width=150
   ```

1. Cliquez sur **Terminé** > **Enregistrer la vue**.
1. (Facultatif) Mettez à jour le nom de la vue, puis cliquez sur **Enregistrer la vue**.
