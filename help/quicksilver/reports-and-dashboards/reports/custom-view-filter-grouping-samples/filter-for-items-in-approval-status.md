---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : afficher uniquement les éléments dont le statut est approbation'
description: Vous ne pouvez afficher que les éléments dont l’état est actuellement en attente d’approbation. Cela fonctionne de la même manière pour tout autre objet avec un état d’approbation.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# Filtre : afficher uniquement les éléments à l’état d’approbation ;

Vous ne pouvez afficher que les éléments dont l’état est actuellement en attente d’approbation. Cela fonctionne de la même manière pour tout autre objet avec un état d’approbation.

Vous pouvez placer les objets suivants dans un état de validation :

* Tâches
* Événements
* Projets

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
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification d’un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher uniquement les éléments à l’état d’approbation

1. Accédez au filtre que vous souhaitez personnaliser pour une liste de projets, par exemple.
1. Cliquez sur **Ajouter une règle de filtre** pour le **État** de l’objet de votre liste.\
   Par exemple, dans un rapport de projet, ajoutez **Planification égale au statut**, si vous souhaitez afficher uniquement les projets dont l’état est défini sur **Planification - Autorisation en attente**.

1. Cliquez sur **Passer en mode Texte**.
1. Modifiez le

   ```
   status
   ```

   ligne en ajoutant **:A** à la clé à 3 lettres de l’état :
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Cliquez sur **Terminé**, puis **Enregistrer le filtre**.

   La liste affiche uniquement les projets dont l’état est Planification - Approbation en attente .
