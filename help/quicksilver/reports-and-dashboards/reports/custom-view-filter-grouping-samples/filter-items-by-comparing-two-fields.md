---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Filtre : éliminer les éléments d’une liste en comparant deux champs »'
description: Vous pouvez filtrer les éléments d’une liste en comparant deux de leurs champs. Par exemple, vous ne pouvez afficher que les tâches dont la date d’achèvement effective est ultérieure à la date d’achèvement prévue.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 84eb5bda612ee518a195190349427c706994030b
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 100%

---

# Filtre : éliminer les éléments d’une liste en comparant deux champs

Vous pouvez filtrer les éléments d’une liste en comparant deux de leurs champs. Par exemple, vous ne pouvez afficher que les tâches dont la date d’achèvement effective est ultérieure à la date d’achèvement prévue.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Filtrer des éléments en comparant deux champs

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.

1. Cliquez sur **Ajouter une règle de filtre** et ajoutez **Date d’achèvement effective** > **Supérieure à** > **Sélectionner une date**.

   >[!TIP]
   >
   >Sélectionnez le modificateur de filtre à utiliser pour le champ sélectionné, le cas échéant.

1. Cliquez sur **Basculer en mode texte**.
1. Dans la zone **Définir des règles de filtrage pour votre rapport**, ajoutez le code suivant :

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Cliquez sur **Terminé**, puis sur **Enregistrer le filtre**.
