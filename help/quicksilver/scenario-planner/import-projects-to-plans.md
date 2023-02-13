---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importation de projets dans des plans dans le planificateur de scénarios
description: Vous pouvez importer des projets existants dans un plan. Les projets importés sont convertis en initiatives et vous pouvez les gérer dans le cadre du plan comme vous le feriez pour gérer une nouvelle initiative. Le projet original reste lié à la nouvelle initiative.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---

# Importation de projets dans des plans dans [!DNL Scenario Planner]

Vous pouvez importer des projets existants dans un plan. Les projets importés sont convertis en initiatives et vous pouvez les gérer dans le cadre du plan comme vous le feriez pour gérer une nouvelle initiative. Le projet original reste lié à la nouvelle initiative.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produit</b> </td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour la variable [!DNL Adobe Workfront Scenario Planner] pour accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention de [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>Accès à [!UICONTROL Modifier] ou supérieur à la variable [!DNL Scenario Planner]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Autorisations [!UICONTROL Gérer] pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demande d’accès à un plan dans le planificateur de scénarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Observations relatives à l’importation de projets dans les plans en tant que nouvelles initiatives

* Vous devez créer des projets avant de pouvoir les importer dans un plan en tant que nouvelles initiatives.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Vous devez avoir au moins [!UICONTROL Affichage] autorisations pour les projets afin de pouvoir les importer dans un plan en tant que nouvelle initiative.
* Vous pouvez importer le même projet dans plusieurs plans.
* Les projets que vous souhaitez importer doivent comporter des dates incluses dans la période de votre plan. Vous ne pouvez pas importer de projets avec un [!UICONTROL Date d’achèvement prévue] avant le début du plan ou une [!UICONTROL Date de début planifiée] plus tard que la fin du plan.
* Vous ne pouvez pas importer plus de 100 projets à la fois.
* Certaines informations sur le projet sont également importées dans le plan et deviennent des informations sur l’initiative. Pour plus d’informations sur les informations de projet importées dans le plan et qui deviennent des informations sur l’initiative, voir la section [Informations sur le projet importées dans le plan](#project-information-imported-into-the-plan) dans cet article.
* Les modifications qui se produisent sur les projets liés n’affectent pas les initiatives du plan.
* Les modifications qui surviennent sur les initiatives du plan n’affectent pas automatiquement les modifications de l’Initiative des projets liés ; elles n’affectent les projets liés que lorsque vous publiez l’initiative à partir du plan. Pour plus d’informations sur l’impact des initiatives de publication sur les projets liés, voir [Mettez à jour ou créez des projets en publiant des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* La suppression d’une initiative créée par l’importation d’un projet ne supprime pas le projet.
* La suppression d’un projet lié à une initiative ne supprime pas l’initiative.

## Informations sur le projet importées dans le plan {#project-information-imported-into-the-plan}

Lorsque vous importez un projet dans un plan, certaines informations de projet sont également importées dans le plan et elles deviennent des informations sur l’initiative. Le tableau suivant indique quelles informations de projet deviennent des informations d’initiative lorsque vous importez un projet dans un plan :

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Informations sur le projet</td> 
   <td>Informations sur l’initiative </td> 
  </tr> 
  <tr> 
   <td>Nom du projet</td> 
   <td>Nom de l’initiative</td> 
  </tr> 
  <tr> 
   <td>Dates prévues pour le projet</td> 
   <td> <p>Les mois de début et de fin de l'initiative.</p> <p>Si un projet démarre ou se termine au milieu d’un mois, les dates importées sont étendues pour couvrir un mois entier du plan. Par exemple, si les dates prévues du projet sont du 20 mars au 5 mai 2020, les dates de l’initiative importée sont de mars à mai 2020.</p> <p>Si la date de début ou de fin planifiée dépasse la durée du plan, une indication visuelle indique que l’initiative importée commence avant ou se termine après le plan. </p> </td> 
  </tr> 
  <tr> 
   <td>Rôles de tâche affectés aux tâches et aux problèmes</td> 
   <td> <p>Fonctions d'initiative. </p> <p>Note:   <p>Si un utilisateur modifie les rôles pendant la durée du projet, les rôles importés dépendent de l’état de l’affectation lorsque vous importez le projet. Les scénarios suivants existent :</p> 
     <ul> 
      <li> <p>Si un utilisateur affecté à une tâche ou à un problème a modifié son rôle après avoir marqué son affectation comme [!UICONTROL Terminé], [!DNL Workfront] importe à l’initiative le rôle que l’utilisateur a rempli avant de marquer l’affectation comme [!UICONTROL Terminé].</p> </li> 
      <li> <p>Si un utilisateur affecté à une tâche ou à un problème a modifié le rôle pendant la durée du projet, mais que son affectation à la tâche ou au problème n’est pas marquée comme [!UICONTROL Terminé] lorsque vous importez le projet, [!DNL Workfront] importe uniquement le rôle actuel de l’utilisateur affecté. </p> </li> 
     </ul> <p>Pour plus d’informations sur l’état d’une affectation, voir "État d’affectation" dans <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossaire de l’Adobe [!DNL Workfront] terminologie</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projet [!UICONTROL Heures planifiées] associées aux rôles de tâche affectés à des tâches ou des problèmes</td> 
   <td> <p><span>Selon que le plan est configuré pour utiliser les EPT ou les heures, les [!UICONTROL Heures planifiées] des tâches du projet deviennent</span> [!UICONTROL EPF requises] <span>ou [!UICONTROL Heures requises] sur le plan</span>. </p> <p>Pour plus d’informations sur la configuration d’un plan d’utilisation des ETF ou des heures, voir <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Créez et modifiez des plans dans le [!DNL Scenario Planner]</a>. </p> <p>Tenez compte des points suivants :</p> 
    <ul> 
     <li> <p>[!DNL Workfront] utilise les rôles de tâche affectés aux tâches et aux problèmes ou les rôles de tâche auxquels les utilisateurs affectés à des tâches ou des problèmes sont associés sur le projet et les transfère vers la nouvelle initiative en tant que rôles de tâche requis. </p> </li> 
     <li> <p>Lorsque le plan est configuré pour utiliser les EPT, les heures planifiées associées aux rôles de travail sur les tâches et les problèmes du projet sont d’abord converties en EPT. Cet éditeur de texte enrichi est ensuite affecté au rôle de travail de l’initiative. <span>Les heures planifiées sont réparties de manière égale dans [!DNL Workfront]. Si une tâche ou un problème s’étend sur plusieurs mois, le nombre d’heures planifiées pour chaque mois pendant la durée de l’initiative est converti en ETP mensuel et transféré à chaque mois de l’initiative.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><span>Par exemple, si une tâche est affectée à un rôle de tâche pour 80 heures planifiées en septembre, le rôle de tâche importé affiche 0,5 EPT pour l’initiative en septembre.</span> </p> </li> 
     <li> <p>[!DNL Workfront] calcule l’éditeur de texte enrichi des rôles de tâche requis associés à l’initiative à l’aide de la formule suivante :</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Conseil : Le [!DNL Scenario Planner] suppose qu’il y a 160 heures de travail par mois.</p> <p>Par exemple, si un projet a une durée de 1 200 minutes et qu’un rôle de tâche sur le projet est associé à 600 minutes des heures planifiées, son ETR est de 0,5. Lors de l’importation du projet, l’ETR du rôle de tâche requis sur la nouvelle initiative est de 0,5 pour chaque mois de l’initiative. </p> </li> 
     <li>Lorsqu’un rôle de tâche est attribué à une tâche sur le projet sans heure planifiée, l’éditeur de texte enrichi requis pour le rôle de tâche de l’initiative est défini sur zéro par défaut. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Lorsqu’un rôle de tâche est affecté à une tâche sur le projet avec une durée [!UICONTROL] nulle, l’éditeur de texte enrichi requis <span>ou heures</span> pour que le rôle de tâche de l’initiative soit nul par défaut, même si la tâche a des Heures planifiées. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Importation de projets dans un plan

>[!IMPORTANT]
>
>Après avoir importé des projets dans un plan, ils deviennent des initiatives sur le plan. Bien que les deux éléments soient liés, ils existent en tant qu’entités indépendantes et ne s’affectent pas automatiquement lors de leur mise à jour.
>
>Les événements suivants se produisent :
>
>* Les modifications apportées au projet n’ont aucune incidence sur l’initiative une fois le projet importé dans le plan. Ces modifications incluent les modifications apportées aux affectations de rôles de tâche.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* Les modifications apportées à l’initiative affectent les informations de la variable [!DNL Scenario Planner] sur le projet uniquement lorsque vous publiez l’initiative sur le projet correspondant. Sinon, elles n’affectent pas la variable [!UICONTROL Heures planifiées] informations relatives aux tâches et aux problèmes du projet.
>
>  Pour plus d’informations sur l’impact des initiatives de publication sur les projets liés, voir  [Mettre à jour ou créer des projets en publiant des initiatives dans le planificateur de scénarios](../scenario-planner/publish-scenarios-update-projects.md).

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Workfront], puis cliquez sur [!DNL Scenarios] pour accéder au [!DNL Scenario Planner].

1. Cliquez sur le nom d&#39;un plan dans lequel vous souhaitez importer des projets.
1. Cliquez sur **[!UICONTROL Nouvelle initiative]**, puis cliquez sur **[!UICONTROL Importation de projets]**.

   Le [!UICONTROL Importation de projets] s’affiche. Les projets dont les dates sont incluses dans la période de votre plan s’affichent dans une liste.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Les projets dont l’état est défini s’affichent dans la liste.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Facultatif) Cliquez sur le **[!UICONTROL Icône Filtrer]** ![](assets/filter-nwepng.png)et sélectionnez un filtre disponible dans la liste pour réduire le nombre de projets sur votre liste. Par défaut, la liste des projets est filtrée par le filtre de projet actuellement sélectionné de l’utilisateur dans une liste de projets.

1. (Facultatif) Cliquez sur le **[!UICONTROL Icône Rechercher]** ![](assets/search-icon.png) et ajoutez un mot-clé affiché dans n’importe quel champ de l’écran. Les éléments contenant le mot de recherche s’affichent automatiquement dans la liste et tous les éléments sont masqués.

1. (Conditionnel) Cliquez sur le bouton **[!UICONTROL Icône X]** pour supprimer la recherche et afficher tous les projets.
1. Sélectionnez jusqu’à 100 projets et cliquez sur **[!UICONTROL Importer]**.

   Les projets sont importés au fur et à mesure de nouvelles initiatives.

   Notez les points suivants :

   * Icône de projet ![](assets/project-icon-sp.png) s’affiche à droite du nom de l’initiative.
   * Si le calendrier du projet dépasse la durée du plan, la barre de l’initiative se termine par une marge pointue à gauche (lorsque la date de début est antérieure à la date du plan) ou à droite (lorsque la date de fin est supérieure à la date du plan).

      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * Le nombre de mois et les rôles de tâche ont été mis à jour pour correspondre à ceux du projet.
   >[!TIP]
   >
   >Les coûts associés aux rôles de travail sont mis à jour au niveau de l’initiative et ne sont pas importés du projet.

1. Cliquez sur la barre représentant la nouvelle initiative pour ouvrir le panneau des détails de l’initiative à droite.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   Dans le **[!UICONTROL Durée de l’initiative]** Consultez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Durée de l’initiative]</td> 
      <td>Il s’agit de la durée de l’initiative en mois. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>Les dates de début et de fin de l’initiative. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Project]</td> 
      <td> <p>Les dates de début planifié [!UICONTROL] et de fin du projet lié.</p> <p>Conseil : Si les informations [!UICONTROL Project] sont manquantes, le projet a été supprimé.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Modifiez le nom de l’initiative. Par défaut, il correspond au nom du projet.
1. (Facultatif) Effectuez l’une des opérations suivantes :

   * Mise à jour des rôles de tâche dans **[!UICONTROL Rôles de tâche requis]** section
   * Mettez à jour le **[!UICONTROL Coûts fixes]** dans le **[!UICONTROL Coûts]** section

   * Cliquez sur **[!UICONTROL Mise à jour des rôles de tâche disponibles]** ou **[!UICONTROL Mettre à jour le budget disponible]** résoudre les conflits entre la nouvelle initiative et d&#39;autres initiatives du plan.

1. (Conditionnel) Cliquez sur **[!UICONTROL Appliquer]** pour enregistrer les modifications apportées à votre initiative.
1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer les modifications apportées à votre plan.
1. (Facultatif) Pour mettre à jour les modifications que vous apportez à l’initiative vers le projet à partir duquel elle a été importée, publiez le projet à partir du plan. Pour plus d’informations sur les plans de publication, voir [Mettez à jour ou créez des projets en publiant des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Facultatif) Cliquez sur l’icône du projet pour accéder au projet lié.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
