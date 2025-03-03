---
content-type: reference
product-area: projects
navigation-topic: financials
title: Comprendre le coût budgété de la main-d’œuvre et les heures budgétées pour les projets
description: Comprendre le coût budgété de la main-d’œuvre et les heures budgétées pour les projets
author: Lisa
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 98%

---

# Comprendre le coût budgété de la main-d’œuvre et les heures budgétées pour les projets

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Vous pouvez budgéter vos ressources pour le travail à l’aide du planificateur de ressources Adobe Workfront.

Lorsque vous budgétez vos ressources pour le travail sur les projets, Workfront calcule le coût budgété de la main-d’œuvre pour les rôles, les projets et les personnes en fonction des valeurs de coût par heure.

Le coût budgété de la main-d’œuvre du planificateur de ressources d’un projet est un calcul entre le coût associé aux fonctions affectées pour effectuer le travail sur le projet et le nombre d’heures estimé (heures budgétées du planificateur de ressources) qui peuvent être nécessaires à chaque rôle pour effectuer le travail.

>[!IMPORTANT]
>
>Le coût budgété de la main-d’œuvre du planificateur de ressources pour les personnes n’a aucune incidence sur celui du projet. Seul le coût du travail pour les fonctions affecte le coût du projet.

## Vue d’ensemble du coût budgété de la main-d’œuvre pour les fonctions et le projet

Workfront utilise le coût budgété de la main-d’œuvre des fonctions sur le projet pour calculer le coût budgété de la main-d’œuvre du projet.

>[!TIP]
>
>Le coût budgété de la main-d’œuvre d’un projet dans le business case s’affiche en tant que coût budgété de la main-d’œuvre du planificateur de ressources dans les rapports et les listes.

Le **coût budgété de la main-d’œuvre** (ou coût budgété de la main-d’œuvre du planificateur de ressources) d’un projet est calculé selon la formule suivante :

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

Les champs utilisés dans le calcul ci-dessus se réfèrent aux éléments suivants :

* Heures budgétées pour les fonctions dans la zone Établissement du budget des ressources du projet ou du planificateur de ressources.

  Pour plus d’informations sur l’établissement du budget des ressources dans le planificateur de ressources, consultez la section « Établissement du budget des ressources dans le planificateur de ressources » de l’article [Vue d’ensemble du planificateur de ressources](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

  Pour plus d’informations sur l’établissement du budget des ressources dans la zone Établissement du budget des ressources du business case, voir [Établissement du budget des ressources dans le business case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* Le **Taux de coût par heure d’une fonction** dans le calcul ci-dessus fait référence au coût associé à chaque fonction sur le projet.\
  Pour plus d’informations sur la création et la gestion des fonctions et leur association aux taux de coût, consultez l’article [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront calcule toutes les informations relatives aux coûts en utilisant la devise du projet. Si vous spécifiez des heures budgétées pour vos ressources dans le planificateur de ressources, l’option permettant de changer la devise du projet est désactivée.\
>Pour plus d’informations sur la modification de la devise d’un projet, consultez l’article [Modifier la devise du projet](../../../manage-work/projects/project-finances/change-project-currency.md).

## Vue d’ensemble du coût budgété de la main-d’œuvre pour les personnes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>Le coût budgété de la main-d’œuvre par personne n’a aucune incidence sur le coût budgété de la main-d’œuvre du projet. Seul le coût de main-d’œuvre des fonctions sur un projet affecte le coût budgété de la main-d’œuvre du planificateur de ressources du projet.
> 
>Le total de tous les coûts de main-d’œuvre de toutes les personnes peut ou non correspondre au coût budgété de la main-d’œuvre du planificateur de ressources pour les fonctions associées aux utilisateurs et utilisatrices.
>
>Si vous estimez les heures budgétées pour les personnes dans le planificateur de ressources, les coûts qui y sont associés sont ceux des fonctions associées aux utilisateurs et utilisatrices.Ce ne sont pas des coûts associés aux personnes ou à leurs taux.

Si les personnes sont associées aux fonctions sur le projet et que leurs heures sont budgétées dans le planificateur de ressources, leur coût budgété de la main-d’œuvre s’affiche sous les noms suivants, selon l’emplacement où vous les affichez dans Workfront :

* [!UICONTROL **Coût budgété de la main-d’œuvre**] : la zone Établissement du budget des ressources du business case sous leurs rôles respectifs.

  ![Coût budgété de la main-d’œuvre dans l’analyse de rentabilité](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**] : planificateur de ressources lors de l’affichage des informations dans la vue Projet et rôle par coût.

  ![Coût budgété de la main-d’œuvre dans les planifications de ressources](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Les personnes s’affichent dans la zone Établissement du budget des ressources du business case sous leurs rôles respectifs ou dans le planificateur de ressources si elles répondent aux exigences suivantes :

* Elles sont associées à l’une des fonctions du projet.
* Elles ont des heures budgétées spécifiées dans le planificateur de ressources.
* Un taux de coût par heure est associé à leur profil.

  Pour plus d’informations sur l’ajout de taux par heure aux personnes, consultez l’article [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* La personne fait partie de l’un des groupes de ressources associés au projet.

Le coût budgété de la main-d’œuvre d’une personne est calculé selon la formule suivante :

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Localiser le coût budgété de la main-d’œuvre d’un projet

Le coût budgété de la main-d’œuvre tel qu’il est reflété dans la zone Établissement du budget des ressources du business case ou du planificateur de ressources s’affiche dans les zones suivantes de Workfront sous les noms suivants :

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nom d’affichage du coût budgété de la main-d’œuvre</strong></td> 
     <td><strong>Zone de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Coût budgété de la main-d'œuvre</td> 
     <td>Zone Établissement du budget des ressources du business case</td> 
    </tr> 
    <tr> 
     <td>Coût budgété</td> 
     <td><p>Vue Coût du rapport d’utilisation</p><p>Pour plus d’informations, voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Afficher des informations sur l’utilisation</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Vues Projet ou Rôle du planificateur de ressources, par coût</td> 
    </tr> 
    <tr> 
     <td>Coût budgété de la main-d’œuvre du projet du planificateur de ressources</td> 
     <td> <p>Rapport du projet</p> <p>Rapport du projet (données financières)</p> <p>Rapport sur la tâche</p> <p>Rapport sur le problème</p> <p>Rapport sur les heures budgétées</p> <p>Pour plus d’informations sur la création d’un rapport, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Si vous utilisez le planificateur de scénario d’Adobe Workfront pour budgétiser les ressources du projet, le coût de la main-d’œuvre dans la zone Budget des ressources du business case est le même que le coût de la main-d’œuvre de l’initiative liée au projet. Le planificateur de scénarios n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénarios Workfront, voir [Vue d’ensemble du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md). Pour plus d’informations sur la planification des ressources à l’aide du planificateur de scénario, consultez [Budgétiser les ressources dans le business case à l’aide du planificateur de scénarios](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Localiser les heures budgétées d’un projet

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

Les heures budgétées affectent la valeur du coût de la main-d’œuvre budgétée (ou du coût budgété du planificateur de ressources) du projet.

Le coût de la main-d’œuvre budgétée d’un projet est le coût associé aux rôles affectés pour terminer le travail sur le projet et le nombre d’heures estimé (heures budgétées) nécessaire à chaque rôle pour terminer le travail.

Vous pouvez afficher les Heures budgétées dans Workfront dans les champs répertoriés dans le tableau ci-dessous.

>[!NOTE]
>
>Toute autre mention d’« Heures budgétées » dans Workfront fait référence aux heures budgétées à l’aide de fonctionnalités obsolètes qui ont été supprimées de Workfront. Il s’agit de champs en lecture seule qui ne sont pas mis à jour avec les informations actuelles lorsque vous utilisez les outils de budget des ressources actuelles.

Les heures budgétées tel qu’elles apparaissent dans la zone de budgétisation des ressources du business case ou du planificateur de ressources, s’affichent dans les zones suivantes de Workfront, sous les noms suivants :

* **Heures** : zone Établissement du budget des ressources du business case
* **BDG** : planificateur de ressources affiché par heures
* **Heures budgétées** : rapport d’utilisation avec la vue Heures
Pour plus d’informations, consultez [Afficher des informations sur l’utilisation des ressources](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Hrs budgétées** : rapport sur les heures budgétées

  L’objet Heure budgétée du rapport Heure budgétée fait référence à des informations relatives à un outil de gestion des ressources obsolète. Seul le champ « Hrs budgétées » de ce rapport fait référence aux heures budgétées dans le planificateur de ressources ou la zone Établissement du budget des ressources de l’analyse de rentabilité du projet.

  Pour plus d’informations sur la création d’un rapport, consultez l’article **Créer un rapport personnalisé**.
* **Heures budgétées du planificateur de ressources** : dans les rapports suivants :

   * Rapport du projet
   * Rapport du projet (données financières)
   * Rapport sur la tâche
   * Rapport sur le problème
   * Rapport sur les heures budgétées
