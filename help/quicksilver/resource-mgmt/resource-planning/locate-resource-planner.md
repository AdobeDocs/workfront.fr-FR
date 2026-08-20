---
product-area: resource-management
navigation-topic: resource-planning
title: Rechercher le planificateur de ressources
description: Vous pouvez utiliser le planificateur de ressources pour gérer l’affectation de vos ressources aux projets. Vous pouvez accéder au planificateur de ressources pour un ou plusieurs projets en même temps à partir de la zone Business Case du projet.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
TQID: https://experienceleague.adobe.com/-p17GWsoDlmbZtZW3T47YGxOmgSOsMddnFfFXpW36C4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: d1573eb8-a2e8-4a06-9526-9c3410bf4914id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 8c7088d5d53b1519752e6ad0cd0caa79453e3d67
workflow-type: tm+mt
source-wordcount: 455
ht-degree: 88%

---

# Rechercher le planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Vous pouvez utiliser le planificateur de ressources pour gérer l’affectation de vos ressources aux projets. Vous pouvez accéder au planificateur de ressources pour un ou plusieurs projets en même temps à partir de la zone Business Case du projet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td>
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Léger ou supérieur pour un projet ; standard pour plusieurs projets</p>
       <p>Réviser ou plus pour un projet ; planifier plusieurs projets</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès Afficher ou supérieur à la gestion des ressources</p> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p>Visualiser les autorisations pour les projets et les utilisateurs et utilisatrices </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Assurez-vous que toutes les conditions préalables à l’accès et à l’utilisation du planificateur de ressources sont remplies avant de commencer à l’utiliser. Ainsi, vous vous assurez que le planificateur de ressources affiche les informations correctes avant de commencer à établir un budget de vos ressources.

Pour plus d’informations sur les conditions préalables à l’utilisation du planificateur de ressources, consultez l’article [Commencer avec le planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Rechercher le planificateur de ressources

Vous pouvez localiser le planificateur de ressources dans deux zones de Workfront, selon que vous souhaitez établir le budget de vos ressources pour un ou plusieurs projets.

* [Utiliser le planificateur de ressources pour plusieurs projets](#use-the-resource-planner-for-multiple-projects)
* [Utiliser le planificateur de ressources pour un projet](#use-the-resource-planner-for-one-project)

### Utiliser le planificateur de ressources pour plusieurs projets {#use-the-resource-planner-for-multiple-projects}

Lorsque vous utilisez le planificateur de ressources pour plusieurs projets, les numéros d’attribution de vos ressources représentent les numéros de plusieurs projets.

Pour accéder à la section Planificateur dans la zone Ressources :

{{step1-to-resourcing}}

Le planificateur s’affiche par défaut.  Pour plus d’informations sur l’établissement d’un budget des ressources dans le planificateur de ressources, consultez l’article [Établir un budget des ressources dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![ Planificateur de ressources par défaut ](assets/default-resource-planner.png)

1. Cliquez sur **Groupes de ressources** dans le panneau de gauche.
Pour plus d’informations sur la création de groupes de ressources, consultez l’article [Créer des groupes de ressources](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Utiliser le planificateur de ressources pour un projet {#use-the-resource-planner-for-one-project}

Lorsque vous utilisez le planificateur de ressources pour un projet, les numéros d’affectation de vos ressources correspondent aux numéros du projet sélectionné.

1. Accédez à un projet pour lequel vous souhaitez établir un budget des ressources.
1. Cliquez sur **Business Case** dans le panneau de gauche.
1. Faites défiler l’écran jusqu’à la section **Établissement du budget des ressources** de le Business Case.
1. Cliquez sur **Modifier l’établissement du budget des ressources** pour ajouter des groupes de ressources à votre projet et commencer à établir le budget de vos ressources.

   >[!TIP]
   >
   >Vous ne pouvez ajouter un pool de ressources que dans la zone de budgétisation des ressources de l&#39;Analyse de rentabilité lorsque le projet n&#39;est associé à aucun pool de ressources. <!--When the project already has a Resource Pool, the users in the pool and their job roles display in the Resource Budgeting area by default.-->

   ![Établissement du budget des ressources](assets/resource-budgeting-area-on-project.png)

   Pour plus d’informations sur la planification des ressources pour un projet, voir l’article [Budgéter les ressources dans le business case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
