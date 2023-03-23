---
product-area: resource-management
navigation-topic: resource-pools
title: Association des pools de ressources aux projets et aux modèles
description: Les pools de ressources sont des groupes d’utilisateurs qui vous aident à gérer les ressources dans Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: addcff71ff067be22e9ee80f997af545293fa5db
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Association des pools de ressources aux projets et aux modèles


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible pour tous les clients de l’environnement Aperçu et pour un groupe sélectionné de clients de l’environnement Production.</span>


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

Les pools de ressources sont des groupes d’utilisateurs qui vous aident à gérer les ressources dans Adobe Workfront.

Après avoir créé des pools de ressources, vous pouvez les associer à des projets ou à des modèles afin de planifier ultérieurement vos ressources sur les projets.

Nous vous recommandons de créer vos pools de ressources à l’avance, de les associer aux projets et de budgéter vos ressources avant le démarrage du projet.

Pour plus d’informations sur les pools de ressources, voir [Présentation des pools de ressources](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Pour plus d’informations sur la création de pools de ressources, voir [Création de pools de ressources](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à Gérer les groupes de ressources</p> <p>Modifier l’accès aux projets, aux modèles et aux utilisateurs</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérez les autorisations pour les projets, les modèles et les utilisateurs auxquels vous associez les pools de ressources</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Associer des pools de ressources à un projet ou à un modèle

Vous pouvez associer des pools de ressources à un modèle de la même manière que vous associez des pools de ressources à un projet. Cet article décrit comment associer des pools de ressources à des projets.

1. Accédez à un projet et cliquez sur le bouton **Plus** icon ![](assets/more-icon.png)en regard du nom du projet, puis cliquez sur **Modifier**.

1. Cliquez sur **Paramètres du projet**.

1. Commencez à saisir le nom d’un pool de ressources dans la variable **Groupes de ressources** puis sélectionnez-la dans la liste lorsqu’elle s’affiche.\
   Vous pouvez associer plusieurs pools de ressources à un projet ou à un modèle.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur la modification d’un projet et son association à des pools de ressources, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Pour plus d’informations sur la modification d’un modèle et son association à des pools de ressources, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Associez les pools de ressources à plusieurs projets ou modèles en bloc

Vous pouvez modifier plusieurs projets ou modèles en bloc et associer les mêmes pools de ressources à tous en même temps.

Vous pouvez associer des pools de ressources aux modèles de la même manière que vous associez des pools de ressources aux projets.

Pour associer des pools de ressources à plusieurs projets en bloc :

1. Accédez à une liste de projets.
1. Sélectionnez plusieurs projets, puis cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) en haut de la liste.

1. Cliquez sur **Paramètres**.
1. Commencez à saisir le nom d’un pool de ressources dans la variable **Groupes de ressources** puis sélectionnez-la dans la liste lorsqu’elle s’affiche.\
   Vous pouvez associer plusieurs pools de ressources aux projets ou aux modèles.

   >[!NOTE]
   >
   >* Dans l’environnement de production, lorsque vous modifiez des projets ou des modèles en bloc, seuls les pools de ressources communs à tous les projets ou modèles sélectionnés apparaissent dans ce champ. Si les projets sélectionnés ne comportent aucun pool de ressources partagées, ce champ est vide. Les pools de ressources que vous spécifiez ici remplaceront les pools de ressources individuels des projets ou modèles.
   >
   >* <span class="preview">Dans l’environnement Aperçu, lorsque vous modifiez des projets en bloc, un indicateur &quot;Plusieurs valeurs&quot; s’affiche si les projets sélectionnés disposent de pools de ressources différents. Si vous ajoutez des pools de ressources en bloc, tous les pools seront ajoutés au projet sélectionné, remplaçant les pools de ressources d’origine.</span>


   <span class="preview">![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)</span>

1. Cliquez sur **Enregistrer les modifications**.\
   Lorsque vos pools de ressources sont associés à vos projets ou à vos modèles, vous pouvez répartir les affectations utilisateur pour vos projets dans le planificateur de ressources.\
   Pour plus d’informations sur le planificateur de ressources, voir [Présentation de Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Pour plus d’informations sur la modification des projets en bloc, voir la section &quot;Modifier les projets en bloc&quot; dans [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Pour plus d’informations sur la modification des modèles en bloc, voir la section &quot;Modifier les modèles en bloc&quot; dans [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
