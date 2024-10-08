---
product-area: resource-management
navigation-topic: resource-planning
title: Rechercher le planificateur de ressources
description: Vous pouvez utiliser le planificateur de ressources pour gérer l’affectation de vos ressources aux projets. Vous pouvez accéder au planificateur de ressources pour un ou plusieurs projets en même temps à partir de la zone Business Case du projet.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 93%

---

# Rechercher le planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Vous pouvez utiliser le planificateur de ressources pour gérer l’affectation de vos ressources aux projets. Vous pouvez accéder au planificateur de ressources pour un ou plusieurs projets en même temps à partir de la zone Business Case du projet.

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
   <td><p>Nouveau : clair ou supérieur ;</br>
          Standard pour localiser le planificateur de ressources dans le menu principal</p>
       <p>ou</p>
       <p>Actuel : révision ou version ultérieure ;</br>
       Prévoyez de localiser le planificateur de ressources dans le menu principal.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Afficher ou supérieur à la gestion des ressources</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Visualiser les autorisations pour les projets et les utilisateurs et utilisatrices </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Assurez-vous que toutes les conditions préalables à l’accès et à l’utilisation du planificateur de ressources sont remplies avant de commencer à l’utiliser. Ainsi, vous vous assurez que le planificateur de ressources affiche les informations correctes avant de commencer à établir un budget de vos ressources.

Pour plus d’informations sur les conditions préalables à l’utilisation du planificateur de ressources, consultez l’article [Commencer avec le planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Rechercher le planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Vous pouvez localiser le planificateur de ressources dans deux zones de Workfront, selon que vous souhaitez établir le budget de vos ressources pour un ou plusieurs projets.

* [Utiliser le planificateur de ressources pour plusieurs projets](#use-the-resource-planner-for-multiple-projects)
* [Utiliser le planificateur de ressources pour un projet](#use-the-resource-planner-for-one-project)

### Utiliser le planificateur de ressources pour plusieurs projets {#use-the-resource-planner-for-multiple-projects}

Lorsque vous utilisez le planificateur de ressources pour plusieurs projets, les numéros d’attribution de vos ressources représentent les numéros de plusieurs projets.

Pour accéder à la section Planificateur dans la zone Ressources :

{{step1-to-resourcing}}

Le planificateur s’affiche par défaut.  Pour plus d’informations sur l’établissement d’un budget des ressources dans le planificateur de ressources, consultez l’article [Établir un budget des ressources dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Cliquez sur **Pools de ressources** dans le panneau de gauche.
Pour plus d’informations sur la création de groupes de ressources, consultez l’article [Créer des groupes de ressources](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Utiliser le planificateur de ressources pour un projet {#use-the-resource-planner-for-one-project}

Lorsque vous utilisez le planificateur de ressources pour un projet, les numéros d’affectation de vos ressources correspondent aux numéros du projet sélectionné.

1. Accédez à un projet pour lequel vous souhaitez établir un budget des ressources.
1. Cliquez sur **Business Case** dans le panneau de gauche.
1. Faites défiler l’écran jusqu’à la section **Établissement du budget des ressources** de le Business Case.
1. Cliquez sur **Modifier l’établissement du budget des ressources** pour ajouter des groupes de ressources à votre projet et commencer à établir le budget de vos ressources.

   >[!TIP]
   >
   >Vous ne pouvez ajouter un groupe de ressources dans la zone Établissement du budget des ressources du Business Case que si aucun projet de ressources n’est associé au projet. Lorsque le projet dispose déjà d’un groupe de ressources, les personnes du groupe et leurs fonctions s’affichent par défaut dans la zone d’établissement du budget des ressources.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Pour plus d’informations sur l’établissement du budget des ressources pour un projet, consultez l’article [Établir un budget de ressources dans le Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
