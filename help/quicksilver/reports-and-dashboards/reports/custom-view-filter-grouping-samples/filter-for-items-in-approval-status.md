---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Filtre : afficher uniquement les éléments ayant un statut d’approbation »'
description: Vous pouvez afficher uniquement les éléments ayant un certain statut qui est actuellement Approbation en attente. Cela fonctionne de la même manière pour tout autre objet ayant un statut d’approbation.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 100%

---

# Filtre : afficher uniquement les éléments ayant un statut d’approbation

Vous pouvez afficher uniquement les éléments ayant un certain statut qui est actuellement Approbation en attente. Cela fonctionne de la même manière pour tout autre objet ayant un statut d’approbation.

Vous pouvez conférer aux objets suivants un statut d’approbation :

* Tâches
* Problèmes
* Projets

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

## Afficher uniquement les éléments ayant un statut d’approbation

1. Accédez au filtre que vous souhaitez personnaliser pour une liste de projets, par exemple.
1. Cliquez sur **Ajouter une règle de filtrage** pour le champ **Statut** de l’objet de votre liste.\
   Par exemple, dans un rapport de projet, ajoutez **Statut égal à planification**, si vous souhaitez afficher uniquement les projets dont le statut est **Planification - Approbation en attente**.

1. Cliquez sur **Basculer en mode texte**.
1. Modifiez la

   ```
   status
   ```

   ligne en ajoutant **:A** à la clé de trois lettres du statut :
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Cliquez sur **Terminé**, puis sur **Enregistrer le filtre**.

   La liste n’affiche que les projets dont le statut est Planification - Approbation en attente.
