---
product-area: enterprise-scenario-planner-product-area
keywords: publier,plans,projets,scénario,scénarios
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mettre à jour ou créer des projets en publiant des initiatives dans le planificateur de scénarios
description: Vous pouvez créer des projets à partir d’initiatives existantes et également mettre à jour des projets précédemment liés à des initiatives en publiant des scénarios dans le planificateur de scénarios Adobe Workfront.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: 9babe17ad862925440e555f881bf753fb443b67d
workflow-type: tm+mt
source-wordcount: '1722'
ht-degree: 100%

---

# Mettre à jour ou créer des projets en publiant des initiatives dans le [!DNL Scenario Planner]

La publication d’un scénario à partir du [!DNL Adobe Workfront Scenario Planner] effectue les opérations suivantes :

* Crée des projets à partir des initiatives du scénario et les relie entre eux.
* Met à jour les projets déjà liés aux initiatives du scénario avec les informations de l’initiative liée. Les projets peuvent également être liés à des initiatives lorsque vous les importez dans un plan. Pour plus d’informations, voir [Importer des projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] forfait*</p> </td> 
   <td>[!UICONTROL Business] ou niveau supérieur</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td> <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td>Produit </td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour le [!DNL Adobe Workfront Scenario Planner] afin d’accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention du [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser le [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>Niveau d’accès*</p> </td> 
   <td> 
    <ul> 
    <li>Accès [!UICONTROL Edit] au [!DNL Scenario Planner] et aux projets</li></ul>

<p><b>NOTE</b>

Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour plus d’informations sur la manière dont l’équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet</p> </td> 
   <td> 
    <ul> 
     <li>Autorisations [!UICONTROL Manage] pour le plan </li> 
     <li>Autorisations [!UICONTROL Manage] pour les projets publiés</li> 
    </ul> <p>Pour plus d’informations sur la demande d’un accès supplémentaire aux projets, voir <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Demander l’accès à un plan dans le [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur l’accès au [!DNL Workfront Scenario Planner], voir [Accès nécessaire pour utiliser le  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

## Conditions préalables

Avant de commencer :

* Vous devez créer et enregistrer un plan avant de pouvoir publier des initiatives à partir de celui-ci.
* Le paramètre Autoriser les utilisateurs à créer des projets sans utiliser de modèle doit être activé dans la zone Préférences du projet de la configuration. Pour plus d’informations, voir [Configurer les préférences du projet à l’échelle du système](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Considérations relatives à la publication d’initiatives dans des projets

* Vous ne pouvez publier qu’un seul scénario à partir d’un plan.
* Une initiative ne peut être liée qu’à un seul projet.
* Un projet peut être lié à plusieurs initiatives lorsque les initiatives appartiennent à différents plans.

  >[!TIP]
  >
  >Lorsqu’un projet existe sur plusieurs plans et que vous publiez des informations sur le projet à partir de tous les plans, la dernière publication remplace les informations du [!DNL Scenario Planner] existantes sur le projet.

* Si des initiatives ont été créées sur le plan en important des projets dans le plan, la publication de l’initiative met également à jour les projets liés avec les informations de l’initiative.

  >[!TIP]
  >
  >Vous pouvez importer le même projet dans plusieurs plans. La publication peut remplacer les informations d’initiative sur un projet lié à plusieurs initiatives.

  Pour plus d’informations sur la création d’initiatives par import de projets, voir [Importer des projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Les modifications apportées au projet ne sont pas reflétées dans l’initiative liée.



## Publier des initiatives

>[!IMPORTANT]
>
>Si vous apportez des modifications aux initiatives du plan, y compris la résolution de conflits, vous devez republier l’initiative pour que les nouvelles informations soient visibles sur le projet. Ces informations ne s’affichent sur les projets liés aux initiatives que lorsque vous publiez l’initiative correspondante. Pour plus d’informations sur la résolution des conflits entre les initiatives, voir [Résoudre les conflits d’initiative dans le  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **[!UICONTROL Scénarios]**.
1. (Facultatif et le cas échéant) Si vous souhaitez publier à partir d’un plan existant, cliquez sur l’icône **[!UICONTROL Filtrer]** ![](assets/filter-nwepng.png) dans le coin supérieur droit du plan et sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Affiche tous les plans que vous possédez ou qui ont été partagés avec vous. Il s’agit du paramètre par défaut. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL My plans]</td> 
      <td>Affiche les plans que vous avez créés.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Shared with me]</td> 
      <td> <p>Affiche les plans que vous n’avez pas créés mais qui ont été partagés avec vous.</p> <p>Important : pour publier les plans partagés avec vous, vous devez disposer d’autorisations de [!UICONTROL Manage]. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Rechercher]** ![](assets/search-icon.png) et commencez à saisir le nom d’un plan pour le trouver rapidement dans la liste.
1. (Le cas échéant) Pour publier à partir d’un nouveau plan, créez un plan.

   Pour plus d’informations sur la création de plans, consultez la section [Créer et modifier des plans dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. (Facultatif) Cliquez sur le nom d’un plan existant et créez des scénarios pour le plan.

   Pour plus d’informations sur la création de scénarios pour un plan, consultez la section [Créer et comparer des scénarios de plan dans le [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Facultatif) Mettez à jour les initiatives d’un plan existant ou nouveau ou créez-les.

   Pour plus d’informations sur la création d’initiatives, consultez la section [Créer et modifier des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Cliquez sur **[!UICONTROL Enregistrer le plan]**.
1. Sélectionnez le scénario que vous souhaitez publier dans le menu déroulant **[!UICONTROL Scénario initial]**, puis cliquez sur **[!UICONTROL Aller à Publier]** ![](assets/go-to-publish-button-icon.png) dans le coin supérieur droit.

   Ou

   Cliquez sur **[!UICONTROL Comparer les scénarios]**, pointez sur la carte de scénario à partir de laquelle vous souhaitez publier, puis cliquez sur **[!UICONTROL Aller à Publier]** ![](assets/go-to-publish-button-icon.png).

   La page [!UICONTROL Publier les initiatives] s’affiche avec la liste de toutes les initiatives du scénario. Si l’une des initiatives a été précédemment publiée, l’icône du projet ![](assets/project-icon-sp.png) s’affiche après leur nom et la date de la **[!UICONTROL Dernière publication]** est renseignée dans la liste.

   >[!TIP]
   >
   >Les initiatives créées par l’import de projets affichent également l’icône du projet ![](assets/project-icon-sp.png) à droite de leur nom.

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Facultatif et le cas échéant) Si vous souhaitez publier à partir d’un plan existant, cliquez sur l’icône **[!UICONTROL Filtrer]** ![](assets/filter-nwepng.png) dans le coin supérieur droit du plan et sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Affiche toutes les initiatives du scénario sélectionné. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Published]</td> 
      <td>Affiche les initiatives que vous ou une autre personne avez publiées précédemment. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unpublished]</td> 
      <td> <p>Affiche les initiatives non publiées. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Rechercher]** ![](assets/search-icon.png) et commencez à saisir le nom d’une initiative pour la trouver rapidement dans la liste.
1. Sélectionnez une ou plusieurs initiatives à publier et créez ou mettez à jour des projets à partir de celles-ci, puis cliquez sur **[!UICONTROL Publier les initiatives]**.

   Un nouveau projet est alors créé à partir de chaque initiative sélectionnée ou les projets connectés existants sont mis à jour, si les initiatives publiées étaient déjà liées à un projet.

   >[!TIP]
   >
   >Les nouveaux projets portent le même nom que les initiatives publiées.

1. (Le cas échéant) Effectuez l’une des opérations suivantes :

   * Si vous avez publié une seule initiative, cliquez sur **[!UICONTROL Voir le projet associé]** pour ouvrir le projet créé ou mis à jour à partir de l’initiative.
   * Si vous avez publié plusieurs initiatives, cliquez sur **[!UICONTROL Voir les projets associés]** pour ouvrir la liste des projets publiés à partir des différentes initiatives. [!DNL Workfront] applique par défaut le filtre Projets du [!DNL Scenario Planner] à la liste des projets. Les derniers projets publiés s’affichent en haut de la liste.

     ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Accédez aux sections suivantes pour afficher les informations sur l’initiative du projet :

   * **Section [!UICONTROL Mises à jour]** : une mise à jour de publication indique que le projet a été créé ou mis à jour à partir de l’initiative. La mise à jour contient le nom de l’initiative qui a créé ou mis à jour le projet et le nom lié du plan qui contient l’initiative. Cliquez sur le nom du plan dans la mise à jour pour l’ouvrir dans le [!DNL Scenario Planner].

     ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **Zone [!UICONTROL Vue d’ensemble] de la section [!UICONTROL Détails du projet]** : une nouvelle section [!DNL Scenario Planner] est créée dans cette zone qui contient les informations de l’initiative liée.

     ![](assets/scenario-planner-on-project-details-350x135.png)

     Les informations suivantes sur l’initiative sont publiées dans la zone [!DNL Scenario Planner] de la section [!UICONTROL Détails du projet] :

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span>Durée de l’initiative correspondante lorsque le projet est lié à une initiative. Ce champ n’est pas modifiable.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Last Published Date]</span> </td> 
        <td><span>Date à laquelle le projet a été publié pour la dernière fois à partir d’une initiative correspondante.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Start Date]</span> </td> 
        <td><span>Premier jour du mois de début de l’initiative, lorsque le projet est lié à une initiative.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative End Date]</span> </td> 
        <td><span>Dernier jour du mois de fin de l’initiative, lorsque le projet est lié à une initiative. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs and Hours]</span> </td> 
        <td> <p>Informations sur les fonctions associées et leur affectations de temps pour l’initiative. Cela inclut :</p> 
         <ul> 
          <li>Nom de la fonction</li> 
          <li>Nombre d’ETP</li> 
          <li> <p>Nombre d’heures pour tous les ETP</p> <p>Vous pouvez estimer le nombre de fonctions nécessaires à votre plan ou à votre initiative à l’aide d’heures ou d’EPT.</p> <p>Pour plus d’informations, voir <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Créer et modifier des plans dans le planificateur de scénarios</a>. </p> </li> 
         </ul> 
      <p><b>CONSEIL</b>

     Si le nombre de fonctions est différent pour chaque mois de l’initiative, ce champ affiche le nombre maximum de rôles requis pour l’initiative. Par exemple, si vous avez besoin d’un consultant ou d’une consultante pour janvier et de deux pour février, la colonne affiche 2ETP et le nombre d’heures correspondant pour 2 ETR pour tous les mois.</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >Tous les utilisateurs et utilisatrices disposant d’un accès en [!UICONTROL Affichage] au projet peuvent afficher la section [!DNL Scenario Planner] dans la zone [!UICONTROL Vue d’ensemble]. Vous pouvez vérifier si cette zone s’affiche dans la section [!UICONTROL Détails] à l’aide d’un modèle de disposition. Si aucun modèle de disposition n’est associé aux utilisateurs et utilisatrices, cette zone s’affiche par défaut.
     >
     >   
     >   
     >   * Pour plus d’informations sur l’ajout ou la suppression de zones dans la section [!UICONTROL Détails] à l’aide d’un modèle de disposition, voir [Personnaliser la vue [!UICONTROL Détails] à l’aide d’un modèle de disposition](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * Pour plus d’informations sur l’affichage d’informations dans la zone [!UICONTROL Vue d’ensemble] des [!UICONTROL Détails du projet], voir [[!UICONTROL Gérer les] informations dans la zone [!UICONTROL Vue d’ensemble] du projet](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **Le panneau [!UICONTROL Affectation des rôles] de l’[!UICONTROL Équilibreur de charge de travail] ou la liste des tâches du projet** : les informations sur l’affectation des rôles de l’initiative sont renseignées dans cette zone, en plus de l’affectation des rôles sur le projet.

     Pour plus d’informations, voir [Vue d’ensemble de la réconciliation des affectations de ressources entre les projets et les initiatives](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![](assets/role-allocation-panel-350x174.png)

     Une modification apportée aux dates ou aux ressources du projet n’affecte pas l’initiative correspondante ni les zones du projet qui contiennent les informations sur l’initiative.

   * **La zone [!UICONTROL Établissement du budget de ressources] de l’[!UICONTROL Analyse de rentabilité] du projet** : nouvelle option de gestion des ressources de projet utilisant des informations du [!DNL Scenario Planner] ajoutée dans la zone [!UICONTROL Établissement du budget de ressources] de l’[!UICONTROL Analyse de rentabilité] du projet.

     Pour plus d’informations, voir [Budgétiser les ressources dans l’[!UICONTROL Analyse de rentabilité] à l’aide du  [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![](assets/sp-in-business-case-selected-350x110.png)

1. (Facultatif) Passez en revue les informations suivantes dans le [!DNL Scenario Planner] après avoir publié un scénario :

   * Le scénario publié devient le premier scénario une fois que vous avez publié des initiatives à partir de celui-ci.
   * Vous ne pouvez pas publier à partir d’un autre scénario après avoir publié un scénario au moins une fois.
   * L’option [!UICONTROL Aller à Publier] est supprimée de tous les autres scénarios une fois qu’au moins une initiative a été publiée à partir d’un scénario.
   * Un indicateur vert s’affiche en regard des icônes de projet des initiatives publiées dans le plan.

     ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * Un indicateur vert « Publié » s’affiche en haut du scénario et sur la carte du scénario ; le champ Publié est renseigné sur la carte du scénario pour indiquer le nombre d’initiatives du scénario qui ont été publiées.

     ![](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >Si tous les projets publiés à partir des initiatives du scénario sont supprimés, l’indication que le scénario a été publié est supprimée. Pour plus d’informations, voir [Supprimer des projets](../manage-work/projects/manage-projects/delete-projects.md).

1. (Facultatif) Mettez à jour les informations sur l’initiative et répétez le processus décrit ci-dessus pour republier l’initiative et mettre à jour les informations de l’initiative sur le projet lié.

   Pour plus d’informations sur la modification d’initiatives, voir [Créer et modifier des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


