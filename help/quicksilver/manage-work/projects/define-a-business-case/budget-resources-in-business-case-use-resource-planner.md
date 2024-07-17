---
navigation-topic: business-case-and-scorecards
title: Budgétiser les ressources dans l’analyse de rentabilité à l’aide du planificateur de ressources
description: Dans le cadre de la planification des ressources, vous pouvez utiliser le planificateur de ressources au niveau du projet pour planifier les rôles de tâche nécessaires à l’exécution du travail dans un projet lorsque vous créez l’analyse de cas.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 9%

---

# Budgétiser les ressources dans l’analyse de rentabilité à l’aide du planificateur de ressources

Dans le cadre de la planification des ressources, vous pouvez utiliser le planificateur de ressources au niveau du projet pour planifier les rôles de tâche nécessaires à l’exécution du travail dans un projet lorsque vous créez l’analyse de cas.

Pour plus d’informations sur la création d’un dossier d’affaires, voir [Création d’un dossier d’affaires pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Les informations que vous saisissez dans le planificateur de ressources au niveau du projet sont également visibles dans le planificateur de ressources au niveau du système. L’inverse est également vrai. Pour plus d’informations sur le planificateur de ressources, consultez la [présentation du planificateur de ressources](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Vous pouvez également budgétiser des ressources dans l’analyse de cas à l’aide du planificateur de scénario Adobe Workfront. Pour plus d’informations, voir [Ressources budgétaires dans l’analyse de cas à l’aide du planificateur de scénario](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans?lang=fr" target="_blank">Formule Adobe Workfront</a>*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>*</td> 
   <td> <p>Révision ou supérieur</p> <p>Important : Vous devez disposer d’une licence Plan pour modifier les informations de budget des ressources. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux éléments suivants : </p> 
    <ul> 
     <li> <p>Projets</p> </li> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Données financières</p> </li> 
    </ul> <p>Pour plus d’informations sur l’accès aux ressources du budget, voir également <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Accès aux ressources du budget dans Adobe Workfront</a>.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Adobe Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations sur le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Avant de commencer, vous devez effectuer les opérations suivantes :

* Respectez toutes les conditions préalables à la planification des ressources dans Adobe Workfront. Pour plus d’informations, voir [Présentation de Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Associez les groupes de ressources au projet.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

  >[!NOTE]
  >
  >Vous ne pouvez pas budgétiser les ressources affectées aux problèmes dans l’Analyse de cas. Vous pouvez les budgéter dans le planificateur de ressources au niveau du système. Pour plus d’informations sur le planificateur de ressources, consultez la [présentation du planificateur de ressources](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Bien qu’il ne s’agisse pas d’un prérequis, nous vous recommandons également d’indiquer les Heures planifiées pour les tâches du projet. Cela vous permet de comprendre le temps nécessaire à la réalisation d’une tâche, ce qui vous permet de prendre en compte le temps nécessaire au budget des ressources pour terminer la tâche. Pour plus d’informations sur l’association de tâches avec des heures planifiées, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Application de pools de ressources à un projet et à des ressources de budget dans l’analyse de cas

>[!IMPORTANT]
>
>Vous pouvez répartir vos ressources sur une période de 15 ans. Si vous planifiez des ressources pour un projet d’une durée supérieure à 15 ans, les informations de budget peuvent ne pas être exactes.

Pour appliquer des pools de ressources et des ressources de projet de budget dans l’Analyse de cas pour un projet sans pool de ressources :

1. Accédez au projet pour lequel vous souhaitez budgétiser les ressources.
1. Cliquez sur **Business Case** dans le panneau de gauche.
1. (Conditionnel) Si votre société ne dispose pas d’une licence pour le planificateur de scénario Workfront, cliquez sur **Modifier le budget des ressources** dans la section **Budget des ressources**, puis passez à l’étape 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Facultatif et conditionnel) Si les informations du projet ont été publiées à partir d’une initiative dans le planificateur de scénario, effectuez l’une des opérations suivantes :

   * Sélectionnez Resource Planner dans le champ **Choisir les heures à utiliser pour calculer le coût de la main-d&#39;oeuvre budgétisée du projet**, puis cliquez sur **Choisir > Modifier le budget de la ressource**.

     ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Si le planificateur de scénario a été sélectionné pour les ressources de budget du projet, cliquez sur **Modifier** > **Modifier le budget des ressources**.

     ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)

   Cette opération utilise les Heures budgétisées du projet pour calculer le coût de la main-d’oeuvre budgétisée du projet.

   Le planificateur de scénarios n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénarios Workfront, voir [Vue d’ensemble du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   >
   >Nous vous recommandons de prendre la décision d’utiliser le planificateur de ressources ou le planificateur de scénarios lorsque vous commencez à travailler sur un projet. Le fait de basculer fréquemment entre les deux au cours de la vie du projet peut créer des incohérences dans la manière dont vous répartissez les ressources pour le projet.

1. Dans le champ **Select Resource Pool** , spécifiez un ou plusieurs **Resource Pools**.

   Vous ne devez spécifier que les groupes de ressources contenant des utilisateurs actifs.

   >[!TIP]
   >
   >Si le projet est déjà associé à des groupes de ressources, le planificateur de ressources s’affiche par défaut. Pour ajouter d’autres groupes de ressources au projet, modifiez le projet. Pour plus d’informations sur la modification d’un projet, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquez sur **Appliquer**.

   Le planificateur de ressources s’affiche pour le projet sélectionné.

   Par défaut, les 20 premiers rôles de tâche associés à ce projet sont répertoriés dans la section Budget des ressources dans l’ordre alphabétique. 

   Pour plus d’informations sur le planificateur de ressources, consultez la [présentation du planificateur de ressources](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_records_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Facultatif et conditionnel) Développez les rôles de tâche pour afficher les utilisateurs qui y sont associés.

   >[!NOTE]
   >
   >Les utilisateurs actifs ne sont affichés sous les rôles de tâche qui leur sont associés que s’ils répondent aux critères suivants :
   >
   >   
   >   
   >   * Ils appartiennent à l’un des groupes de ressources du projet.
   >   * Les Heures budgétaires leur sont affectées.
   >   * Ils sont associés à l’un des rôles de tâche du projet.
   >   
   >

    

1. Cliquez sur **Today** pour revenir à la période actuelle.
1. (Facultatif) Cliquez sur **Semaine**, **Mois** ou **Trimestre** pour afficher les informations du projet dans différentes périodes.
1. (Facultatif) Cliquez sur le menu déroulant **Hours**, puis sélectionnez **Hours**,**FTE** ou **Cost** pour modifier la manière dont les informations s’affichent dans le planificateur de ressources. Les heures s’affichent par défaut.

1. (Facultatif) Cliquez sur **Exporter** pour exporter le planificateur de ressources vers un fichier Excel.

   >[!NOTE]
   >
   >Vous pouvez exporter des données pendant 12 périodes au maximum.

1. (Facultatif) Cliquez sur l’icône **Plein écran** ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) pour afficher le planificateur de ressources en mode Plein écran.

1. Mettez à jour le champ **BDG** (Heures budgétées) avec les valeurs Heure, ETR ou Coût pour les utilisateurs, les rôles ou le projet en effectuant l’une des opérations suivantes :

   * Estimez manuellement le nombre de valeurs Heures, ETR ou Coût pour les rôles, les utilisateurs ou le projet.

     Ou

   * Cliquez sur l’icône **Options** pour le projet ou les rôles de tâche et sélectionnez une option pour répartir automatiquement les heures entre les rôles, les utilisateurs ou le projet.

   Pour plus d’informations sur la planification dans la vue Projet du planificateur de ressources, voir [Ressources de budget dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   >
   >Vous pouvez budgéter les heures, les EFS ou les coûts de vos ressources pour n’importe quelle période affichée dans la zone Ressource budgétaire, indépendamment de la chronologie du projet. Par exemple, si vous souhaitez indiquer que vos ressources ne seront peut-être pas disponibles dans la chronologie du projet (où elles sont associées aux Heures planifiées), mais qu’elles pourront être disponibles à une autre période, vous pouvez le faire en les budgétisant pour les périodes où les Heures planifiées sont nulles, si c’est le moment où elles deviennent disponibles pour le travail.

1. (Facultatif) Pour savoir si vous pouvez déplacer les heures, les ETF ou les coûts budgétés vers une autre période, cliquez sur l’icône **Options**, puis **Ajuster les dates de budget**.

   Pour plus d’informations sur l’ajustement des dates budgétées, voir [Ajuster les dates de budgétisation dans le planificateur de ressources](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Cliquer sur **Enregistrer**.

   Si des taux de coût par heure sont associés à vos rôles de tâche, la budgétisation des ressources dans la zone Ressource/Budget calcule le **coût de la main-d’oeuvre budgété** du projet. Le Coût de la main-d&#39;oeuvre budgétisé est affiché dans la zone Budget des ressources de l&#39;Analyse de cas et dans le Récapitulatif des analyses de cas.

   >[!TIP]
   >
   >Le coût s’affiche dans l’Analyse de cas dans la devise du projet.

   Les informations de budget spécifiées dans l&#39;Analyse de cas sont également affichées dans le planificateur de ressources.

   Lorsque vous copiez un projet, vous avez la possibilité de copier les heures budgétées dans le nouveau projet. Seules les heures budgétées dans le planificateur de ressources sont copiées. Pour plus d’informations, voir [Copier un projet](../manage-projects/copy-project.md).
