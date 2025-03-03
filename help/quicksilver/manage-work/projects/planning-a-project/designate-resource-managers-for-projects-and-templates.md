---
product-area: projects;templates
navigation-topic: plan-a-project
title: Désigner des personnes gestionnaires de ressources pour un projet ou un modèle
description: Vous pouvez désigner des personnes gestionnaires de ressources pour un projet afin d’indiquer qui est responsable de la gestion des ressources sur le projet.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 98%

---

# Désigner des personnes gestionnaires de ressources pour un projet ou un modèle

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

Vous pouvez désigner des personnes gestionnaires de ressources pour un projet afin d’indiquer qui est responsable de la gestion des ressources sur le projet. Il s’agit d’un champ informatif qui n’est connecté à aucun outil de gestion des ressources.

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## Conditions d’accès

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès Modifier aux projets et aux modèles</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion sur le projet ou le modèle</p>

<p><b>NOTE</b>

Les personnes ajoutées en tant que gestionnaires de ressources à un projet ou à un modèle obtiennent immédiatement les autorisations Gérer sur le projet ou le modèle.</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Remarques relatives aux personnes gestionnaires de ressources

>[!NOTE]
>
>Personne gestionnaire de ressources n’est pas une fonction ; il s’agit d’un champ disponible sur un projet ou un modèle que vous pouvez mettre à jour manuellement.

* Vous pouvez désigner jusqu’à 30 personnes comme gestionnaires de ressources pour un projet ou modèle individuel.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* Vous ne pouvez pas désigner d’équipes ou de groupes comme gestionnaires de ressources. Vous ne pouvez désigner que des personnes comme gestionnaires de ressources.

* Les personnes que vous désignez comme gestionnaires de ressources sur un projet ou un modèle ne font pas automatiquement partie de l’équipe de projet.

  Pour plus d’informations sur les équipes de projet, voir [Gérer l’équipe de projet](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* Vous pouvez désigner des personnes gestionnaires de ressources pour les projets ou les modèles de projet. Lorsque vous désignez des personnes gestionnaires de ressources sur un modèle de projet, toutes les personnes que vous désignez comme gestionnaires de ressources sur le modèle deviennent automatiquement gestionnaires de ressources sur tous les projets créés à l’aide de ce modèle.
* Vous pouvez afficher le champ Personne gestionnaire de ressources dans les zones suivantes :

   * Lors de la modification d’un projet, comme décrit dans cet article.
   * Lors de la modification d’un modèle, comme décrit dans cet article.
   * Lors de la création de rapports de projet ou de modèle. Pour plus d’informations sur la création de rapports, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * Lors de la création ou de la personnalisation d’une vue de projet ou de modèle pour une liste. Pour plus d’informations, voir [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* Vous pouvez ajouter ou supprimer rapidement des personnes gestionnaires de ressources sur plusieurs projets ou modèles en ajoutant le champ Personne gestionnaire de ressources à une vue de liste ou de projet et en modifiant ce champ à l’aide de la modification intégrée.

## Désigner des personnes gestionnaires de ressources pour un projet

1. Effectuez l’une des opérations suivantes :

   * Pour ajouter des personnes gestionnaires de ressources à un seul projet, accédez au projet pour lequel vous souhaitez désigner une ou plusieurs personnes comme gestionnaires de ressources, puis cliquez sur le **Menu Plus** en regard du nom du projet, puis sur **Modifier**.

   * Pour ajouter simultanément des personnes gestionnaires de ressources à plusieurs projets, accédez à une liste de projets, sélectionnez les projets pou lesquels vous souhaitez désigner une ou plusieurs personnes comme gestionnaires de ressources, puis cliquez sur **Modifier**.

     Les personnes gestionnaires de ressources existantes ne sont pas supprimées des projets en cours de modification ; les personnes que vous ajoutez de cette manière sont ajoutées en tant que gestionnaires de ressources sur le projet en plus des personnes gestionnaires de ressources existantes.

   * Pour ajouter des personnes gestionnaires de ressources à un nouveau projet, commencez à créer un projet.

     Pour plus d’informations sur la création d’un projet, voir [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

1. Dans la section **Vue d’ensemble** dans la boîte de dialogue Modifier le projet, cliquez dans le champ **Personne gestionnaire de ressources**.
1. Commencez à saisir le nom de la personne que vous souhaitez ajouter en tant que personne gestionnaire de ressources pour le projet, puis cliquez sur le nom lorsqu’il apparaît dans la liste.

   Répétez cette étape pour ajouter plusieurs personnes gestionnaires de ressources pour le projet.

1. Cliquez sur **Enregistrer les modifications**.

## Désigner des personnes gestionnaires de ressources pour un modèle

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Modèles**.

1. Effectuez l’une des opérations suivantes :

   * Pour ajouter des personnes gestionnaires de ressources à un seul modèle, accédez au modèle dans lequel vous souhaitez désigner une ou plusieurs personnes gestionnaires de ressources, puis cliquez sur le **menu Plus** en regard du nom du modèle, puis sur **Modifier**.

   * Pour ajouter simultanément des personnes gestionnaires de ressources à plusieurs modèles, accédez à une liste de modèles et sélectionnez les modèles auxquels vous souhaitez désigner une ou plusieurs personnes gestionnaires de ressources, puis cliquez sur **Modifier**.

     Les personnes gestionnaires de ressources existantes ne sont pas supprimées des modèles que vous modifiez ; les utilisateurs et utilisatrices que vous ajoutez de cette manière sont ajoutés en tant que gestionnaires de ressources sur le modèle en plus des personnes gestionnaires de ressources existantes.

   * Pour ajouter des personnes gestionnaires de ressources à un nouveau modèle, cliquez sur **Nouveau modèle**, puis sur le **menu Plus** en regard du nom du modèle, puis sur **Modifier**.

1. Dans la section **Vue d’ensemble**, cliquez sur le champ **Gestionnaire des ressources**.
1. Commencez à saisir le nom de la personne que vous souhaitez ajouter en tant que gestionnaire de ressources pour le modèle, puis cliquez sur le nom lorsqu’il apparaît dans la liste.

   Répétez cette étape pour ajouter plusieurs personnes gestionnaires de ressources au modèle.

1. Cliquez sur **Enregistrer les modifications**.
