---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filtre : supprimer des éléments d’une liste en comparant deux champs'
description: Vous pouvez filtrer les éléments d’une liste en comparant deux de leurs champs. Par exemple, vous ne pouvez afficher que les tâches dont la date de fin réelle de la tâche est supérieure à la date de fin planifiée.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Filtre : éliminer des éléments d’une liste en comparant deux champs

Vous pouvez filtrer les éléments d’une liste en comparant deux de leurs champs. Par exemple, vous ne pouvez afficher que les tâches dont la date de fin réelle de la tâche est supérieure à la date de fin planifiée.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Filtrage des éléments en comparant deux champs

1. Accédez à une liste de tâches.
1. Dans la **Filtrer** menu déroulant, sélectionnez **Nouveau filtre**.

1. Cliquez sur **Ajouter une règle de filtre** et ajouter **Date d’achèvement réelle** >**Supérieur à** > **Sélectionner une date**.

   >[!TIP]
   >
   >Sélectionnez le modificateur de filtre à utiliser pour le champ sélectionné, le cas échéant.

1. Cliquez sur **Passer en mode Texte**.
1. Dans le **Définition de règles de filtrage pour votre rapport** ajoutez le code suivant :

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Cliquez sur **Terminé**, puis **Enregistrer le filtre**.
