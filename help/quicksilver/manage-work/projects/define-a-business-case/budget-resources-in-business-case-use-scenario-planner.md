---
navigation-topic: business-case-and-scorecards
title: Budget des ressources dans l’analyse de cas à l’aide du planificateur de scénario
description: Dans le cadre de la planification des ressources, vous pouvez utiliser le planificateur de scénario Adobe Workfront pour planifier les rôles de tâche nécessaires à l’exécution du travail dans un projet lorsque vous créez l’analyse de cas.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: ffd7a588c0c9449b7a6aa18e6df7baa7c9872926
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# Budget des ressources dans l’analyse de cas à l’aide du planificateur de scénario

Dans le cadre de la planification des ressources, vous pouvez utiliser le planificateur de scénario Adobe Workfront pour planifier les rôles de tâche nécessaires à l’exécution du travail dans un projet lorsque vous créez l’analyse de cas.

Pour plus d’informations sur la création d’un cas d’entreprise, voir [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Les informations sur les rôles de tâche de l’initiative associée au projet que vous saisissez dans le planificateur de scénario au niveau du système sont visibles dans la zone Ressource et budget de l’analyse de cas du projet lorsque vous publiez l’initiative. Le planificateur de scénario n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénario Workfront, voir [Présentation du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

Vous pouvez également budgétiser des ressources dans l’analyse de cas à l’aide du planificateur de ressources. Pour plus d’informations, voir :

* [Ressources budgétaires dans l’analyse de cas](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Nous vous recommandons de prendre la décision d’utiliser le planificateur de ressources ou le planificateur de scénarios lorsque vous commencez à travailler sur un projet. Le fait de basculer fréquemment entre les deux au cours de la vie du projet peut créer des incohérences dans la manière dont vous répartissez les ressources pour le projet.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Professionnel ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour le planificateur de scénario Adobe Workfront pour accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention du planificateur de scénario Workfront, voir <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser le planificateur de scénarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifiez l’accès aux éléments suivants : </p> 
    <ul> 
     <li> <p>Projets</p> </li> 
     <li> <p>Données financières</p> </li> 
     <li> <p>Planificateur de scénarios </p> </li> 
    </ul> <p>Pour plus d’informations sur l’accès aux ressources du budget, reportez-vous également à la section <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Accès aux ressources de budget nécessaires dans Adobe Workfront</a>.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Adobe Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations sur le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer, vous devez effectuer les opérations suivantes :

* Créez un plan à l’aide du planificateur de scénarios.

   Pour plus d’informations, voir [Créer et modifier des plans dans le planificateur de scénarios](../../../scenario-planner/create-and-edit-plans.md).

* Créez une initiative sur le plan et liez-la à un projet.

   Veillez à indiquer les informations sur les rôles de tâche requis pour l’initiative et à mettre à jour le projet lié avec ces informations.

   Pour plus d’informations, voir les articles suivants :

   * [Créer et modifier des initiatives dans le planificateur de scénarios](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importation de projets dans des plans dans le planificateur de scénarios](../../../scenario-planner/import-projects-to-plans.md)
   * [Mettre à jour ou créer des projets en publiant des initiatives dans le planificateur de scénarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Bien qu’il ne s’agisse pas de conditions préalables, nous vous recommandons également de procéder comme suit :

   * Affectez des tâches au projet aux rôles de tâche prévus dans le planificateur de scénario.
   * Indiquez le nombre d’heures planifiées pour les tâches du projet.

      Cela vous permet de comprendre la quantité de travail qu’une tâche peut nécessiter, ce qui permet de décider du temps que les ressources doivent prévoir pour terminer la tâche.

      Pour plus d’informations sur l’association de tâches à des heures planifiées, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Budget des ressources dans l’analyse de cas à l’aide du planificateur de scénario pour les projets liés aux initiatives

>[!IMPORTANT]
Vous pouvez répartir vos ressources sur une période de 15 ans. Si vous planifiez des ressources pour un projet d’une durée supérieure à 15 ans, les informations de budget peuvent ne pas être exactes.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Accédez au projet pour lequel vous souhaitez budgétiser les ressources.

   >[!TIP]
   Il s’agit d’un projet lié à une initiative du planificateur de scénario dont l’initiative liée a été publiée au moins une fois.

1. Cliquez sur **Analyse de cas** dans le panneau de gauche.
1. (Conditionnel) Dans la variable **Budget des ressources** effectuez l’une des opérations suivantes :

   * Si vous venez de publier des informations à partir du planificateur de scénarios, sélectionnez le planificateur de scénarios dans la variable **Choisissez les heures à utiliser pour calculer le coût de la main-d&#39;oeuvre budgétisée du projet.** dans la zone Resource Budgeting, puis cliquez sur **Choisir**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Si le planificateur de ressources a été précédemment sélectionné pour les ressources de budget du projet, cliquez sur **Modifier** > **Planification du scénario** > **Choisir**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront utilise les heures de rôle requises de l’initiative liée pour calculer le coût de la main-d’oeuvre budgétisée du projet. Il s’agit de l’option recommandée. Le coût s’affiche dans l’Analyse de cas dans la devise du projet.

      >[!IMPORTANT]
      Lorsque vous utilisez le planificateur de scénario pour budgétiser les ressources du projet, le coût de la main-d’oeuvre budgétisée s’affiche dans les zones suivantes de Workfront :
      * Budget des ressources de l’analyse de cas
      * Le planificateur de scénario au niveau du système en tant que coût du personnel de l’initiative liée au projet. Pour plus d’informations, voir [Créer et modifier des initiatives dans le planificateur de scénarios](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Facultatif) Cliquez sur **Afficher dans le planificateur de scénarios** pour ouvrir le plan contenant l’initiative liée au projet. Le planificateur de scénario s’ouvre alors dans un nouvel onglet du navigateur.
1. (Facultatif) Mettez à jour les informations sur l’initiative. Pour plus d’informations, voir [Créer et modifier des initiatives dans le planificateur de scénarios](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   Vous devez publier l’initiative après chaque modification de la zone Ressource/Budget sur le projet à mettre à jour.
