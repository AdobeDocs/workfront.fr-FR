---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : éliminer les éléments d’une liste en comparant deux champs'
description: Vous pouvez filtrer les éléments d’une liste en comparant deux de leurs champs. Par exemple, vous ne pouvez afficher que les tâches dont la date d’achèvement effective est ultérieure à la date d’achèvement prévue.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 79%

---

# Filtre : éliminer les éléments d’une liste en comparant deux champs

<!--Audited: 10/2024-->

Vous pouvez filtrer les éléments d’une liste en comparant deux de leurs champs. Par exemple, vous ne pouvez afficher que les tâches dont la date d’achèvement effective est ultérieure à la date d’achèvement prévue.

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
   <ul><li><p>Contributeur pour modifier un filtre </p></li>
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

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrer des éléments en comparant deux champs

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.

1. Ajoutez un filtre pour **Tâche:Date d’achèvement effective** > **Supérieur à** > **Sélectionnez une date**.

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
