---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : afficher uniquement les éléments ayant un statut de validation'
description: Vous ne pouvez afficher que les éléments dont l’état est actuellement en attente d’approbation. Cela fonctionne de la même manière pour tout autre objet avec un état d’approbation.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 39%

---

# Filtre : afficher uniquement les éléments ayant un statut d’approbation

Vous ne pouvez afficher que les éléments dont l’état est actuellement en attente d’approbation. Cela fonctionne de la même manière pour tout autre objet avec un état d’approbation.

Vous pouvez placer les objets suivants dans un état de validation :

* Tâches
* Problèmes
* Projets

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher uniquement les éléments à l’état d’approbation

1. Accédez au filtre que vous souhaitez personnaliser pour une liste de projets, par exemple.
1. Cliquez sur **Ajouter une règle de filtre** pour le champ **État** de l’objet de votre liste.\
   Par exemple, dans un rapport de projet, ajoutez **Status Equal Planning**, si vous souhaitez afficher uniquement les projets dont l’état est **Planning - En attente d’approbation**.

1. Cliquez sur **Passer en mode Texte**.
1. Modifiez la variable

   ```
   status
   ```

   en ajoutant **:A** à la clé à 3 lettres de l’état :
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Cliquez sur **Terminé**, puis sur **Enregistrer le filtre**.

   La liste affiche uniquement les projets dont l’état est Planification - Approbation en attente .
