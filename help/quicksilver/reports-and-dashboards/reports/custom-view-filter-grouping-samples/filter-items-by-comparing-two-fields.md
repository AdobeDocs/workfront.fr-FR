---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : éliminer les éléments d’une liste en comparant deux champs'
description: Vous pouvez filtrer les éléments d’une liste en comparant deux de leurs champs. Par exemple, vous ne pouvez afficher que les tâches dont la date d’achèvement effective est ultérieure à la date d’achèvement prévue.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 77%

---

# Filtre : éliminer les éléments d’une liste en comparant deux champs

<!--Audited: 10/2024-->

Vous pouvez filtrer les éléments d’une liste en comparant deux de leurs champs. Par exemple, vous ne pouvez afficher que les tâches dont la date d’achèvement effective est ultérieure à la date d’achèvement prévue.

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

## Filtrer des éléments en comparant deux champs

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.

1. Ajoutez un filtre pour **Tâche:Actual Date d’achèvement** > **Supérieur à** > **Sélectionner une date**.

   >[!TIP]
   >
   >Sélectionnez le modificateur de filtre à utiliser pour le champ sélectionné, le cas échéant.

1. Cliquez sur **Mode texte**.
1. Dans la zone affichée, ajoutez le code suivant :

   ```
   actualCompletionDate=FIELD:plannedCompletionDate
   actualCompletionDate_Mod=gt
   ```

1. Cliquez sur **Appliquer** > **Enregistrer comme nouveau**.
