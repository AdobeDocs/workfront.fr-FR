---
product-area: resource-management
navigation-topic: resource-planning
title: Budgétiser des ressources dans le planificateur de ressources à l’aide des vues Projet et Rôle
description: Vous pouvez budgéter les ressources dans le planificateur de ressources Adobe Workfront à l’aide des vues Projet et Rôle . Vous ne pouvez pas budgétiser les ressources à l’aide de la vue Utilisateur dans le planificateur de ressources.
author: Alina
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2165'
ht-degree: 8%

---

# Budgétiser des ressources dans le planificateur de ressources à l’aide des vues Projet et Rôle

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

La fonction principale du planificateur de ressources est de budgéter vos ressources pour le travail qui doit être effectué sur les projets.

>[!IMPORTANT]
>
>Vous ne pouvez budgétiser vos ressources que si vous appliquez les vues **Afficher par projet** ou **Afficher par rôle** au planificateur de ressources.

Avant de commencer à budgéter les informations dans le planificateur de ressources, consultez les articles suivants :

* [Vue d’ensemble du planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Accès requis pour budgétiser les ressources dans Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Vue d’ensemble des informations sur les heures, ETP et les coûts dans les vues Projet et Rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à l’option Modifier les priorités et les heures du budget dans le planificateur de ressources</p> <p>Modifier l’accès aux données financières pour les ressources du budget parCost</p> <p>Modifier l’accès aux projets et aux utilisateurs</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour les projets pour lesquels vous souhaitez obtenir des informations sur le budget</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Ressources de budget dans le planificateur de ressources

* [Ressources de budget dans la vue Projet](#budget-resources-in-the-project-view)
* [Ressources de budget dans la vue Rôle](#budget-resources-in-the-role-view)
* [Ressources budgétaires en bloc](#budget-resources-in-bulk)

### Ressources de budget dans la vue Projet {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Ressource**.
1. Le **planificateur** s’affiche par défaut.
1. (Conditionnel) Sélectionnez la vue **Vue par projet**.
1. Développez les projets et les rôles de tâche pour gérer l’affectation pour le projet, les rôles de tâche ou les utilisateurs.
1. Pour répartir le budget entre les utilisateurs, effectuez l’une des opérations suivantes :

   * Dans la colonne **BDG**, indiquez manuellement un nombre d’heures, d’ETR ou de coûts prévus pour les utilisateurs.

   * Cliquez sur le menu **Plus** pour le rôle de tâche de l’utilisateur, puis cliquez sur **Définir les heures planifiées des utilisateurs comme budgétées**.\
     Les Heures budgétisées de chaque utilisateur sont calculées à l&#39;aide de la formule suivante :

     ```
     User Budgeted Hours = User Planned Hours
     ```

1. Pour attribuer un budget aux rôles de tâche, effectuez l’une des opérations suivantes :

   * Dans la colonne **BDG**, indiquez manuellement un nombre d’heures, d’ETR ou de coûts prévus pour le rôle de tâche.

     >[!NOTE]
     >
     >Le rôle Heures budgétisées est ajouté aux heures budgétisées du projet.

   * (Conditionnel) Si vous avez prévu des heures dans le budget pour les utilisateurs, cliquez sur le menu **Plus** pour le rôle de tâche, puis cliquez sur **Nombre total d’heures dans le budget de l’utilisateur pour le rôle**.\
     Les Heures budgétisées pour chaque rôle sont calculées à l&#39;aide de la formule suivante :

     ```
     Role Budgeted Hours = SUM(User Budgeted Hours)
     ```

   * Cliquez sur le menu **Plus** du projet, puis sur **Définir les heures planifiées des rôles comme budget**.\
     Les Heures budgétisées pour chaque rôle sont calculées à l&#39;aide de la formule suivante :\
     *

     ```
     Role Budgeted Hours = Role Planned Hours
     ```

     >[!NOTE]
     >   
     >* Le rôle Heures budgétisées est ajouté aux heures budgétisées du projet.
     >* Les utilisateurs peuvent être inclus dans le budget pour les rôles Principal et Autre (ou secondaire).
     >* Le **pourcentage de disponibilité de l’éditeur de texte enrichi** pour les rôles de l’utilisateur doit être un nombre différent de 0 % pour que les heures disponibles affichent une valeur dans le planificateur de ressources pour un rôle de tâche. Si un utilisateur est associé à un rôle avec un **pourcentage de disponibilité de l’éditeur de texte enrichi** de 0 %, la valeur des heures disponibles est zéro pour ce rôle de tâche. Dans ce cas, le rôle peut afficher une **valeur réseau** négative.\
     >Pour plus d’informations sur le **pourcentage de disponibilité de l’éditeur de texte enrichi** pour les rôles de tâche, consultez l’article [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   * Dans la colonne **BDG**, indiquez manuellement un nombre d’heures, d’ETR ou de coûts prévus dans le budget pour le projet. Cette opération répartit le nombre d’heures budgétées du projet sur chaque rôle du projet. Les scénarios suivants sont possibles :

      * Si le nombre d’heures budgétées du projet que vous indiquez est égal au nombre d’heures planifiées du projet, le nombre d’heures planifiées du projet correspond au nombre d’heures planifiées du rôle.
      * Si le nombre d’heures budgétées du projet que vous spécifiez n’est pas égal aux heures planifiées du projet, le nombre d’heures planifiées du projet est réparti en fonction du pourcentage d’heures planifiées nécessaires pour chaque rôle.\
        Par exemple, si un projet comporte 20 heures planifiées et qu’elles sont réparties entre deux rôles (12 heures planifiées pour le consultant et 8 heures planifiées pour l’ingénieur) et que vous budgétez 30 heures pour le projet, les heures sont réparties comme suit : le rôle de consultant reçoit 18 heures planifiées et le rôle d’ingénieur reçoit 12 heures budgétées.

1. Pour répartir le budget du projet, effectuez l’une des opérations suivantes :

   * Budget des rôles du projet, comme décrit à l’étape 7.\
     Les Heures budgétisées du projet sont calculées selon la formule suivante :

     ```
     Project Budgeted Hours = SUM(Role Budgeted Hours)
     ```

   * Dans la colonne **BDG**, indiquez manuellement un nombre d’heures, d’ETR ou de coûts prévus dans le budget pour le projet.\
     Cela met à jour les heures budgétisées du rôle, comme décrit à l’étape 7.\
     ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. Cliquer sur **Enregistrer**.\
   Une fois que vous avez budgété vos ressources dans le planificateur de ressources, les Heures budgétisées de vos ressources et les coûts associés sont répertoriés dans le Business Case de chaque projet.\
   Pour plus d’informations sur la compréhension de la section Ressource/Budget de l’Analyse de cas, reportez-vous à la section &quot;Ressource/Budget&quot; de l’article [Présentation des domaines de l’Analyse de cas](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facultatif) Sélectionnez la vue Utilisateur pour signaler toute suraffectation ou sous-utilisation de l’utilisateur entre les Heures disponibles et les Heures planifiées pour chaque utilisateur. Les heures budgétisées ne sont pas visibles dans la vue Utilisateur.

   Pour plus d’informations sur la façon dont Workfront calcule la disponibilité d’un utilisateur, voir [Configuration des préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Ressources de budget dans la vue Rôle {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

Vous devez disposer des autorisations Modifier de gestion des ressources et des données financières et Gérer les finances sur les projets afin de répartir les ressources dans le planificateur de ressources. Si vous ne disposez que d’un accès en vue à au moins un projet répertorié sous un rôle de tâche, vous ne pouvez pas budgéter les affectations pour le rôle dans la vue Rôle. Vous pouvez toujours allouer un budget pour les projets pour lesquels vous disposez des autorisations de gestion.

Pour plus d’informations sur l’accès aux ressources de budget, consultez l’article [Accès aux ressources de budget dans Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Pour les affectations de budget dans le planificateur de ressources dans la**** vue Rôle :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Ressource**.
1. Le **planificateur** s’affiche par défaut.
1. (Conditionnel) Sélectionnez la vue **Vue par rôle**.
1. Développez les rôles de tâche et les projets pour gérer l’affectation pour le projet, les rôles de tâche ou les utilisateurs.
1. Pour budgétiser l’allocation pour les utilisateurs, effectuez l’une des opérations suivantes :

   * Dans la colonne **BDG**, indiquez manuellement un nombre d’heures, d’ETR ou de coûts prévus pour les utilisateurs.
   * Cliquez sur le menu **Plus** pour le projet, puis sur **Définir les heures planifiées des utilisateurs comme budgétées**.\
     Les Heures budgétisées de chaque utilisateur sont calculées à l&#39;aide de la formule suivante :

     ```
     User Budgeted Hours = User Planned Hours
     ```

1. Pour attribuer un budget aux rôles de tâche, effectuez l’une des opérations suivantes :

   * Dans la colonne **BDG**, spécifiez manuellement un nombre d’heures, d’ETR ou de coûts prévus pour les rôles de tâche.\
     Cette option répartit les heures avec rôle et budget sur les heures du projet pour les projets que vous avez accès à la gestion.

   * Cliquez sur le menu **Plus** pour le rôle de tâche, puis sur **Définir les heures planifiées des projets comme budget.**Le rôle Heures budgétisées est calculé à l’aide de la formule suivante :\
     *

     ```
     Role Budgeted Hours = SUM(Project Budgeted Hours)
     ```

     *Les Heures budgétisées du projet sont calculées à l’aide de la formule suivante :

     ```
     Project Budgeted Hours = Project Planned Hours
     ```

   * Dans la colonne **BDG**, spécifiez manuellement un nombre d’heures, d’ETR ou de coûts budgétés pour les projets répertoriés sous le rôle de tâche.\
     Cela ajoute le nombre d’heures budgétées du projet au rôle .

   >[!NOTE]
   >
   >Les utilisateurs peuvent être inclus dans le budget pour les rôles Principal et Autre (ou secondaire). Le **pourcentage de disponibilité de l’éditeur de texte enrichi** pour les rôles de l’utilisateur doit être un nombre différent de 0 % pour que les heures disponibles affichent une valeur dans le planificateur de ressources pour un rôle de tâche. Si un utilisateur est associé à un rôle avec un **pourcentage de disponibilité de l’éditeur de texte enrichi** de 0 %, la valeur des heures disponibles est zéro pour ce rôle de tâche. Dans ce cas, le rôle peut afficher une **valeur réseau** négative.\
   >Pour plus d’informations sur le **pourcentage de disponibilité de l’éditeur de texte enrichi** pour les rôles de tâche, consultez l’article [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Pour répartir le budget du projet, effectuez l’une des opérations suivantes :

   * Dans la colonne **BDG**, indiquez manuellement un nombre d’heures, d’ETR ou de coûts prévus dans le budget pour les projets.\
     Cela met également à jour les heures budgétisées pour les rôles sous lesquels le projet est répertorié.

   * Cliquez sur le menu **Plus** pour le rôle de tâche, puis sur **Définir les heures planifiées des projets comme budgétées**.\
     Les Heures budgétisées du projet sont calculées selon la formule suivante :

     ```
     Project Budgeted Hours = Project Planned Hours
     ```

     Les heures budgétisées du projet sont ajoutées aux heures budgétisées du rôle.

   * (Conditionnel) Si vous avez prévu le budget des heures pour les utilisateurs, cliquez sur le menu **Plus** pour le projet, puis cliquez sur **Nombre total d’heures budgétées des utilisateurs pour le projet**.\
     Le calcul des heures budgétisées du projet est effectué à l’aide de la formule suivante :

     ```
     Project Budgeted Hours = SUM(User Budgeted Hours)
     ```

     ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. Cliquer sur **Enregistrer**.\
   Une fois que vous avez budgété vos ressources dans le planificateur de ressources, les Heures budgétisées de vos ressources et les coûts associés sont répertoriés dans le Business Case de chaque projet.\
   Pour plus d’informations sur la compréhension de la section Ressource/Budget de l’analyse de cas, consultez l’article [Ressources budgétaires dans l’analyse de cas ](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Facultatif) Sélectionnez la vue **Vue par utilisateur** pour remarquer toute suraffectation ou sous-utilisation de l’utilisateur entre les heures disponibles et les heures planifiées de chaque utilisateur. Les heures budgétisées ne sont pas visibles dans la vue Vue par utilisateur.

### Ressources budgétaires en bloc {#budget-resources-in-bulk}

Vous pouvez répartir les budgets de vos ressources en bloc lorsque vous utilisez des liens rapides. Les liens rapides sont disponibles uniquement pour les vues Projet et Rôle.

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Lorsque vous utilisez les liens rapides vers les allocations budgétaires pour les ressources, la budgétisation n&#39;est automatiquement appliquée qu&#39;aux périodes affichées à l&#39;écran. Si la chronologie d’un projet s’étend sur une période plus longue que celle affichée à l’écran, vous devez faire défiler la page de gauche à droite, puis utiliser les liens rapides pour budgéter automatiquement vos ressources.

Pour répartir vos ressources en masse :

1. Accédez à .\
   Pour plus d’informations sur l’accès au planificateur de ressources, voir la section &quot;Accès au planificateur de ressources&quot; dans l’article [Présentation de Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   La liste des projets que vous pouvez gérer s’affiche dans la liste.

1. (Facultatif) Développez chaque projet pour afficher la liste des rôles de tâche qui lui sont associés.\
   Ou
1. (Facultatif) Sélectionnez **Afficher par rôle**, puis développez chaque rôle pour afficher la liste des projets qui lui sont associés.
1. Passez la souris sur le nom d’un projet ou d’un rôle de tâche.
1. Cliquez sur l’icône **Plus** ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png) qui s’affiche à l’extrémité droite du nom du projet ou du rôle.

1. Cliquez sur l’une des options disponibles pour spécifier automatiquement le montant des heures budgétaires (BDG) pour d’autres objets.

   Selon que vous avez cliqué sur l’icône Plus sur un projet ou un rôle, les options de budget en bloc diffèrent. Le tableau ci-dessous illustre les options disponibles pour les projets et les rôles :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>Vue du projet</strong> </td> 
      <td><strong>Affichage du rôle</strong> </td> 
     </tr> 
     <tr> 
      <td>Options du projet</td> 
      <td> 
       <ul> 
        <li><strong>Définir les heures planifiées des rôles comme budgétées</strong> : sélectionnez cette option pour que les heures planifiées du rôle soient identiques à leurs heures planifiées. Le total des heures budgétisées pour les rôles s’affichera pour les heures budgétisées du projet. </li> 
        <li><strong>Ajuster les dates de budget</strong> : sélectionnez cette option pour passer les heures budgétaires à une autre période.<br>Pour plus d’informations sur l’ajustement des dates de budget, voir <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Ajuster les dates de budget dans le planificateur de ressources</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Définir les heures planifiées des utilisateurs comme étant budgétées</strong> : sélectionnez cette option pour que les heures budgétisées de l’utilisateur deviennent identiques aux heures planifiées de l’utilisateur. </li> 
        <li><strong>Nombre total d’heures budgétées des utilisateurs pour le projet</strong> : sélectionnez cette option pour ajouter toutes les heures budget de l’utilisateur et afficher le total en tant qu’heures budgétées pour le projet et pour le rôle. Nous vous recommandons d’utiliser cette option après avoir budgété manuellement vos utilisateurs ou après avoir utilisé l’option précédente en premier. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Options de rôle</td> 
      <td> 
       <ul> 
        <li><strong>Définir les heures planifiées des utilisateurs comme étant budgétées</strong> : sélectionnez cette option pour que les heures planifiées de l’utilisateur soient identiques à ses heures planifiées. </li> 
        <li><strong>Nombre total d’heures budgétisées par les utilisateurs pour le rôle</strong> : sélectionnez cette option pour ajouter toutes les heures budgétisées de l’utilisateur et afficher le total en tant qu’heures budgétisées pour le rôle et le projet. Nous vous recommandons d’utiliser cette option après avoir budgété manuellement vos utilisateurs ou après avoir utilisé l’option précédente en premier. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Définir les heures planifiées des projets comme budgétées</strong> : sélectionnez cette option pour que les heures planifiées du projet deviennent identiques aux heures planifiées du projet. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Certaines des options peuvent ne pas s’afficher si certaines des conditions préalables à l’utilisation du planificateur de ressources sont manquantes.
   >
   >
   >Pour plus d’informations sur les conditions préalables requises pour un budget précis dans le planificateur de ressources, voir la section &quot;Conditions préalables requises pour travailler dans le planificateur de ressources&quot; dans l’article [Présentation du planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md) .\
   >Par exemple, certaines des options peuvent ne pas s’afficher dans les scénarios suivants :
   >
   >   
   >   
   >   * Lorsque les projets ne sont pas associés à un pool de ressources
   >   * Lorsque les groupes de ressources associés aux projets ne contiennent pas d’utilisateurs
   >   * Lorsque les groupes de ressources associés aux projets contiennent des utilisateurs sans rôle de tâche qui leur sont associés.
   >   
   >
