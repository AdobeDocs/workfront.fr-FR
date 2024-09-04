---
product-area: resource-management
navigation-topic: resource-pools
title: Association de groupes de ressources à des projets et des modèles
description: Les groupes de ressources sont des groupes d’utilisateurs et d’utilisatrices qui vous aident à gérer les ressources dans Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 94%

---

# Associer des groupes de ressources aux projets et aux modèles


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

Les groupes de ressources sont des groupes d’utilisateurs et d’utilisatrices qui vous aident à gérer les ressources dans Adobe Workfront.

Après avoir créé des groupes de ressources, vous pouvez les associer à des projets ou à des modèles afin de planifier ultérieurement vos ressources sur les projets.

Nous vous recommandons de créer vos groupes de ressources en amont, de les associer aux projets et de budgéter vos ressources avant le démarrage du projet.

Pour plus d’informations sur les groupes de ressources, voir [Vue d’ensemble des groupes de ressources](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Pour plus d’informations sur la création de groupes de ressources, voir [Créer des groupes de ressources](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td><p>Nouveau : Tous</p>
       <p>ou</p>
       <p>Actuel : Pro ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à Gérer les groupes de ressources</p> <p>Modifier l’accès aux projets, aux modèles et aux utilisateurs et utilisatrices</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Gérez les autorisations des projets, modèles et utilisateurs auxquels vous souhaitez associer les groupes de ressources.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Associer des groupes de ressources à un projet ou à un modèle

Vous pouvez associer des groupes de ressources à un modèle de la même manière que vous associez des groupes de ressources à un projet. Cet article décrit comment associer des groupes de ressources à des projets.

1. Accédez à un projet et cliquez sur l’icône **Plus** ![](assets/more-icon.png)en regard du nom du projet, puis cliquez sur **Modifier**.

1. Cliquez sur **Paramètres du projet**.

1. Commencez à saisir le nom d’un groupe de ressources dans le champ **Groupes de ressources** puis sélectionnez-le dans la liste lorsqu’il s’affiche.\
   Vous pouvez associer plusieurs groupes de ressources à un projet ou à un modèle.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur la modification d’un projet et son association à des groupes de ressources, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Pour plus d’informations sur la modification d’un modèle et son association à des groupes de ressources, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Associer des groupes de ressources à plusieurs projets ou modèles en bloc

Vous pouvez modifier plusieurs projets ou modèles en bloc et associer les mêmes groupes de ressources à tous ces projets ou modèles en même temps.

Vous pouvez associer des groupes de ressources aux modèles de la même manière que lorsque vous les associez à des projets.

Pour associer des groupes de ressources à plusieurs projets en bloc :

1. Accédez à une liste de projets.
1. Sélectionnez plusieurs projets, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) en haut de la liste.

1. Cliquez sur **Paramètres**.
1. Commencez à saisir le nom d’un groupe de ressources dans le champ **Groupes de ressources** puis sélectionnez-le dans la liste lorsqu’il s’affiche.\
   Vous pouvez associer plusieurs groupes de ressources aux projets ou aux modèles.

   >[!NOTE]
   >
   >* Lorsque vous modifiez des modèles en bloc, seuls les groupes de ressources communs à tous les modèles sélectionnés apparaissent dans ce champ. Si les modèles sélectionnés ne comportent aucun groupe de ressources partagées, ce champ est vide. Les groupes de ressources que vous spécifiez ici remplacent les groupes de ressources individuels des projets ou modèles.
   >
   >* Lorsque vous modifiez des projets en bloc, un indicateur « Plusieurs valeurs » s’affiche si les projets sélectionnés disposent de différents groupes de ressources. Si vous ajoutez des groupes de ressources en bloc pour les projets, tous les groupes sont ajoutés au projet sélectionné, remplaçant les groupes de ressources d’origine.

   ![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. Cliquez sur **Enregistrer les modifications**.\
   Lorsque vos groupes de ressources sont associés à vos projets ou à vos modèles, vous pouvez répartir les affectations des utilisateurs et des utilisatrices pour vos projets dans le planificateur de ressources.\
   Pour plus d’informations sur le planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Pour plus d’informations sur la modification des projets en bloc, voir la section « Modifier les projets en bloc » dans [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Pour plus d’informations sur la modification des modèles en bloc, voir la section « Modifier les modèles en bloc » dans [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
