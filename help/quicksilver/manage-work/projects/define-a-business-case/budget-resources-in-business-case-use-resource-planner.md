---
navigation-topic: business-case-and-scorecards
title: Budget des ressources dans l’analyse de cas à l’aide du planificateur de ressources
description: Dans le cadre de la planification des ressources, vous pouvez utiliser le planificateur de ressources au niveau du projet pour planifier les rôles de tâche nécessaires à l’exécution du travail dans un projet lorsque vous créez l’analyse de cas.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# Budget des ressources dans l’analyse de cas à l’aide du planificateur de ressources

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Dans le cadre de la planification des ressources, vous pouvez utiliser le planificateur de ressources au niveau du projet pour planifier les rôles de tâche nécessaires à l’exécution du travail dans un projet lorsque vous créez l’analyse de cas.

Pour plus d’informations sur la création d’un cas d’entreprise, voir [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Les informations que vous saisissez dans le planificateur de ressources au niveau du projet sont également visibles dans le planificateur de ressources au niveau du système. L’inverse est également vrai. Pour plus d’informations sur le planificateur de ressources, voir [Présentation de Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Vous pouvez également budgétiser des ressources dans l’analyse de cas à l’aide du planificateur de scénario Adobe Workfront. Pour plus d’informations, voir [Budget des ressources dans l’analyse de cas à l’aide du planificateur de scénario](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Formule Adobe Workfront</a>*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>*</td> 
   <td> <p>Révision ou version ultérieure</p> <p>Important : Vous devez disposer d’une licence Plan pour modifier les informations de budget des ressources. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifiez l’accès aux éléments suivants : </p> 
    <ul> 
     <li> <p>Projets</p> </li> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Données financières</p> </li> 
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

* Respectez toutes les conditions préalables à la planification des ressources dans Adobe Workfront. Pour plus d’informations, voir [Présentation de Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Associez les groupes de ressources au projet.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   Vous ne pouvez pas budgétiser les ressources affectées aux problèmes dans l’Analyse de cas. Vous pouvez les budgéter dans le planificateur de ressources au niveau du système. Pour plus d’informations sur le planificateur de ressources, voir [Présentation de Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Bien qu’il ne s’agisse pas d’un prérequis, nous vous recommandons également d’indiquer les Heures planifiées pour les tâches du projet. Cela vous permet de comprendre le temps nécessaire à la réalisation d’une tâche, ce qui vous permet de prendre en compte le temps nécessaire au budget des ressources pour terminer la tâche. Pour plus d’informations sur l’association de tâches à des heures planifiées, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Application de pools de ressources à un projet et à des ressources de budget dans l’analyse de cas

>[!IMPORTANT]
Vous pouvez répartir vos ressources sur une période de 15 ans. Si vous planifiez des ressources pour un projet d’une durée supérieure à 15 ans, les informations de budget peuvent ne pas être exactes.

Pour appliquer des pools de ressources et des ressources de projet de budget dans l’Analyse de cas pour un projet sans pool de ressources :

1. Accédez au projet pour lequel vous souhaitez budgétiser les ressources.
1. Cliquez sur **Analyse de cas** dans le panneau de gauche.
1. (Conditionnel) Si votre société ne dispose pas d’une licence pour le planificateur de scénario Workfront, cliquez sur **Modifier le budget des ressources** dans le **Budget des ressources** , puis passez à l’étape 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Facultatif et conditionnel) Si les informations du projet ont été publiées à partir d’une initiative dans le planificateur de scénario, effectuez l’une des opérations suivantes :

   * Sélectionnez le planificateur de ressources dans la **Choisissez les heures à utiliser pour calculer le coût de la main-d&#39;oeuvre budgétisée du projet.** , puis cliquez sur **Choisissez > Modifier le budget des ressources**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Si le planificateur de scénario a été sélectionné pour la planification des ressources du projet, cliquez sur **Modifier** > **Modifier le budget des ressources**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   Cette opération utilise les Heures budgétisées du projet pour calculer le coût de la main-d’oeuvre budgétisée du projet.

   Le planificateur de scénario n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénario Workfront, voir [Présentation du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   Nous vous recommandons de prendre la décision d’utiliser le planificateur de ressources ou le planificateur de scénarios lorsque vous commencez à travailler sur un projet. Le fait de basculer fréquemment entre les deux au cours de la vie du projet peut créer des incohérences dans la manière dont vous répartissez les ressources pour le projet.

1. Dans le **Sélectionner un pool de ressources** champ, en spécifier un ou plusieurs **Groupes de ressources**.

   Vous ne devez spécifier que les groupes de ressources contenant des utilisateurs principaux.

   >[!TIP]
   Si le projet est déjà associé à des groupes de ressources, le planificateur de ressources s’affiche par défaut. Pour ajouter d’autres groupes de ressources au projet, modifiez le projet. Pour plus d’informations sur la modification d’un projet, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquez sur **Appliquer**.

   Le planificateur de ressources s’affiche pour le projet sélectionné.

   Par défaut, les 20 premiers rôles de tâche associés à ce projet sont répertoriés dans la section Budget des ressources dans l’ordre alphabétique. 

   Pour plus d’informations sur le planificateur de ressources, voir [Présentation de Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budget_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Facultatif et conditionnel) Développez les rôles de tâche pour afficher les utilisateurs qui y sont associés.

   >[!NOTE]
   Les utilisateurs principaux ne sont affichés sous les rôles de tâche qui leur sont associés que s’ils répondent aux critères suivants :
   * Ils appartiennent à l’un des groupes de ressources du projet.
   * Les Heures budgétaires leur sont affectées.
   * Ils sont associés à l’un des rôles de tâche du projet.


    

1. Cliquez sur **Aujourd&#39;hui** pour revenir à la période actuelle.
1. (Facultatif) Cliquez sur **Semaine**, **Mois** ou **Trimestre** pour afficher les informations du projet dans différentes périodes.
1. (Facultatif) Cliquez sur le **Heures** , puis sélectionnez **Heures**,**FTE** ou **Coût** pour modifier l’affichage des informations dans le planificateur de ressources. Les heures s’affichent par défaut.

1. (Facultatif) Cliquez sur **Exporter** pour exporter le planificateur de ressources vers un fichier Excel.

   >[!NOTE]
   Vous pouvez exporter des données pendant 12 périodes au maximum.

1. (Facultatif) Cliquez sur le **Plein écran** icon ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) pour afficher le planificateur de ressources en mode plein écran.

1. Mettez à jour le **BDG** (Hours budgétés) avec les valeurs Heure, ETR ou Coût pour les utilisateurs, les rôles ou le projet en effectuant l’une des opérations suivantes :

   * Estimez manuellement le nombre de valeurs Heures, ETR ou Coût pour les rôles, les utilisateurs ou le projet.

      Ou

   * Cliquez sur le bouton **Options** pour le projet ou les rôles de tâche et sélectionnez une option pour répartir automatiquement les heures entre les rôles, les utilisateurs ou le projet.
   Pour plus d’informations sur la planification dans la vue Projet du planificateur de ressources, voir [Ressources de budget dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   Vous pouvez budgéter les heures, les EFS ou les coûts de vos ressources pour n’importe quelle période affichée dans la zone Ressource budgétaire, indépendamment de la chronologie du projet. Par exemple, si vous souhaitez indiquer que vos ressources ne seront peut-être pas disponibles dans la chronologie du projet (où elles sont associées aux Heures planifiées), mais qu’elles pourront être disponibles à une autre période, vous pouvez le faire en les budgétisant pour les périodes où les Heures planifiées sont nulles, si c’est le moment où elles deviennent disponibles pour le travail.

1. (Facultatif) Pour savoir si vous pouvez déplacer les heures, les ETR ou les coûts prévus dans le budget vers une autre période, cliquez sur le bouton **Options** puis **Ajustement des dates de budget**.

   Pour plus d’informations sur l’ajustement des dates du budget, voir [Ajustement des dates de budget dans le planificateur de ressources](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Cliquer sur **Enregistrer**.

   Si des taux de coût par heure sont associés à vos rôles de tâche, la budgétisation des ressources dans la zone Budget des ressources calcule la valeur **Coût de la main-d&#39;oeuvre budgétisé** du projet. Le Coût de la main-d&#39;oeuvre budgétisé est affiché dans la zone Budget des ressources de l&#39;Analyse de cas et dans le Récapitulatif des analyses de cas.

   >[!TIP]
   Le coût s’affiche dans l’Analyse de cas dans la devise du projet.

   Les informations de budget spécifiées dans l&#39;Analyse de cas sont également affichées dans le planificateur de ressources.

   <!--drafted for Budgeted Hours: 
   <span class="preview">When you copy a project, you have the option to also copy the Budgeted Hours to the new project. Only hours budgeted in the Resource Planner are copied. For more information, see [Copy a project](../manage-projects/copy-project.md)</span>
   -->
