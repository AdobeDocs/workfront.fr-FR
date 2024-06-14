---
product-area: projects
navigation-topic: manage-tasks
title: Associer des jalons à des tâches
description: Vous pouvez associer des jalons à des tâches pour indiquer le moment où vous atteignez des étapes importantes au cours de la durée de vie du projet. Vous devez associer un chemin de jalon à un projet avant de pouvoir associer des jalons à des tâches sur le projet.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 17%

---

# Associer des jalons à des tâches

<!--Audited: 01/2024-->

Vous pouvez associer des jalons à des tâches pour indiquer le moment où vous atteignez des étapes importantes au cours de la durée de vie du projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td> <p>Nouvelle licence : Standard</p> 
   <p>Licence actuelle : travail ou version ultérieure</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches</p> <p><b>NOTE</b>

Si vous n’y avez pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires ont été définies pour votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour la tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

+++

## Conditions préalables

Avant de pouvoir associer un jalon à une tâche, les éléments suivants doivent exister :

* L’administrateur de Workfront doit créer un chemin d’accès de jalon, comme décrit dans la section [Création d’un chemin de jalon](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Vous devez associer un chemin Milestone à un projet.

  Pour plus d’informations, voir [Modification de projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Pour associer un chemin de jalon à un projet, ce dernier doit être à l’état Planification ou Actuel .

  >[!TIP]
  >
  >Pour obtenir un meilleur aperçu de la progression des jalons dans vos projets à l’aide de la vue Milestone, vous devez créer des tâches parents et les associer à chaque phase majeure de votre projet. Ensuite, associez ces tâches parents à chacun des jalons de votre chemin d’accès de jalon.

## Associer un jalon à une tâche

Une fois qu’un chemin de jalon est associé à un projet, les tâches peuvent se voir attribuer un jalon.

1. Accédez à une tâche, puis cliquez sur le bouton **Plus** icon ![](assets/more-icon.png) à droite du nom de la tâche, puis **Modifier**.

   Les tâches et les jalons ont une relation 1:1. Vous ne pouvez pas joindre le même jalon à plusieurs tâches. Chaque tâche peut être associée à un seul jalon ou chaque jalon peut être associé à une seule tâche.

1. Cliquez sur **Paramètres**, puis sélectionnez un jalon dans la variable **Milestone** pour la tâche.
1. Cliquer sur **Enregistrer**.
1. (Facultatif) Dans une liste de tâches, ajoutez le **Icônes d’état** pour identifier les tâches qui comportent des jalons. L’indicateur de losange Milestone s’affiche dans la colonne Icônes d’état.

   Pour plus d’informations, voir [Création ou modification de vues dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![](assets/amwt3.png)

1. (Facultatif) Dans la liste des projets, sélectionnez la variable **Milestone** pour identifier la progression de vos tâches de jalon.

   ![](assets/milestone-view-project-list.png)
