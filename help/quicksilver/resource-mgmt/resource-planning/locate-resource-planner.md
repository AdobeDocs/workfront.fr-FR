---
product-area: resource-management
navigation-topic: resource-planning
title: Localisation du planificateur de ressources
description: '"(Ceci est ressorti de cet article : rédigez ce contenu dans l’article lorsque celui-ci est disponible : /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)'''
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Localisation du planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Vous pouvez utiliser le planificateur de ressources pour gérer l’allocation de vos ressources aux projets. Vous pouvez accéder au planificateur de ressources pour plusieurs projets en même temps ou pour un seul projet, à partir de la zone Analyse de cas du projet.

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
   <td> <p>Révision ou version ultérieure<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>Planifiez l’emplacement du planificateur de ressources ou d’une version ultérieure dans la zone globale.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Afficher l’accès ou une version ultérieure à la gestion des ressources</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations pour les projets et les utilisateurs </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Assurez-vous que toutes les conditions préalables requises pour accéder au planificateur de ressources et l’utiliser sont remplies avant de commencer à l’utiliser. Ainsi, vous vous assurez que le planificateur de ressources affiche les informations correctes avant de commencer à budgéter vos ressources.

Pour plus d’informations sur les conditions préalables du planificateur de ressources, voir [Prise en main de la planification des ressources](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Localisation du planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Vous pouvez localiser le planificateur de ressources dans deux zones de Workfront, selon que vous souhaitez budgétiser vos ressources pour plusieurs projets ou pour un seul projet.

* [Utilisation du planificateur de ressources pour plusieurs projets](#use-the-resource-planner-for-multiple-projects)
* [Utilisation du planificateur de ressources pour un projet](#use-the-resource-planner-for-one-project)

### Utilisation du planificateur de ressources pour plusieurs projets {#use-the-resource-planner-for-multiple-projects}

Lors de l’utilisation du planificateur de ressources pour plusieurs projets, les nombres d’allocation de vos ressources représentent des nombres sur plusieurs projets.

Pour accéder à la section Planificateur dans la zone Ressource :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Ressource**. Le planificateur s’affiche par défaut.  Pour plus d’informations sur la planification des ressources dans le planificateur de ressources, reportez-vous à l’article [Ressources de budget dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Pointez sur le panneau de gauche, puis cliquez sur **Groupes de ressources**.\
   Pour plus d’informations sur la création de pools de ressources, voir [Création de pools de ressources](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Utilisation du planificateur de ressources pour un projet {#use-the-resource-planner-for-one-project}

Lors de l’utilisation du planificateur de ressources pour un projet, les nombres d’allocation de vos ressources représentent les nombres du projet sélectionné.

1. Accédez à un projet pour lequel vous souhaitez budgéter les ressources.
1. Cliquez sur **Analyse de cas** dans le panneau de gauche.
1. Faites défiler l’écran jusqu’à **Budget des ressources** de l’Analyse de cas.
1. Cliquez sur **Modifier le budget des ressources** pour ajouter des pools de ressources à votre projet et commencer à budgéter vos ressources.

   >[!TIP]
   >
   >Vous pouvez uniquement ajouter un pool de ressources dans la zone Ressource de l’analyse de cas lorsque le projet n’est associé à aucun pool de ressources. Lorsque le projet dispose déjà d’un pool de ressources, les utilisateurs de ce pool et leurs rôles de tâche s’affichent par défaut dans la zone Ressource de budget.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Pour plus d’informations sur la planification des ressources pour un projet, reportez-vous à l’article . [Ressources budgétaires dans l’analyse de cas](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
