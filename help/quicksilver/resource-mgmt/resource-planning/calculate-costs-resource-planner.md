---
product-area: resource-management
navigation-topic: resource-planning
title: Calcul des coûts dans le planificateur de ressources
description: Vous pouvez budgéter vos ressources dans le planificateur de ressources Adobe Workfront à l’aide des valeurs de coût, au lieu des valeurs Heures ou ETR. Les valeurs de coût ne sont pas disponibles pour la vue **Vue par utilisateur** dans le planificateur de ressources.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: 61a107e1ee8a415fd94e73fc65fa5f59f7de02d1
workflow-type: tm+mt
source-wordcount: '1390'
ht-degree: 0%

---

# Calcul des coûts dans le planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

Vous pouvez budgéter vos ressources dans le planificateur de ressources Adobe Workfront à l’aide des valeurs de coût, au lieu des valeurs Heures ou ETR. Les valeurs de coût ne sont pas disponibles pour la variable **Afficher par utilisateur** dans le planificateur de ressources.

>[!IMPORTANT]
>
>Vous devez associer les utilisateurs et les rôles de tâche aux taux de coût par heure afin d’afficher les informations de coût dans le planificateur de ressources.\
>Pour plus d’informations sur l’association des taux de coût par heure aux rôles de tâche, voir [Création et gestion des rôles de tâche](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>Pour plus d’informations sur l’association des taux de coût par heure avec les utilisateurs, voir [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Avant de budgéter vos ressources, assurez-vous de bien comprendre le travail à faire (heures planifiées, EPT ou coût) et l’heure à laquelle vos utilisateurs sont ouverts au travail (heures disponibles, EPT ou coût).\
Pour plus d’informations sur la compréhension des informations dans le planificateur de ressources lors de la planification par heures ou par éditeur de texte enrichi, voir [Vue d’ensemble des heures, de l’éditeur de texte enrichi et des coûts dans les vues Projet et Rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à l’option Modifier les priorités et les heures du budget dans le planificateur de ressources</p> <p>Modifier l’accès aux données financières, aux projets et aux utilisateurs</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations des projets pour lesquels vous souhaitez budgétiser les informations avec la possibilité de Gérer les finances</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher les informations dans le planificateur de ressources par coût

Par défaut, les informations de disponibilité et d’attribution sont affichées dans Heures dans le planificateur de ressources.

Pour afficher les informations disponibles, prévues et budgétées par coût dans le planificateur de ressources :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Ressource**.
1. Accédez au planificateur de ressources.
1. (Conditionnel) Sélectionnez **Afficher par projet** ou **Afficher par rôle**.\
   Par défaut **Afficher par projet** est sélectionnée.\
   Les informations d’attribution et de disponibilité s’affichent dans la section Heures.

1. Dans la **Heures** menu déroulant, sélectionnez **Coût**.

   Si vous n’avez pas accès aux données financières à votre niveau d’accès, cette option n’est pas disponible.\
   Si les projets ont une devise différente de celle du système, le coût de ces projets s’affiche dans le planificateur de ressources converti dans la devise du système. Votre administrateur système définit la devise système.\
   Pour plus d’informations sur la configuration de la devise système dans Workfront et des taux de conversion, voir [Configurer les taux de change](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![cost_in_the_planner_with_no_records.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Calcul du coût disponible dans le planificateur de ressources

Pour afficher les valeurs de coûts disponibles dans le planificateur de ressources, vous devez disposer des éléments suivants :

* Taux de coût par heure pour les utilisateurs et les rôles
* Informations sur la disponibilité des utilisateurs.

   L’obtention d’informations sur la disponibilité des utilisateurs dépend de la manière dont votre administrateur Workfront configure les préférences de gestion des ressources.\
   Pour plus d’informations sur le calcul de la disponibilité des utilisateurs et la définition des préférences de gestion des ressources, voir [Configuration des préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Le tableau suivant illustre le mode de calcul du coût disponible dans le planificateur de ressources :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Coût disponible</strong> </th> 
   <th><strong>Calcul</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Coût disponible de l’utilisateur</td> 
   <td> <p>Le coût disponible par utilisateur est calculé à l’aide de la formule suivante :</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>NOTE</b>

Si le profil de l&#39;utilisateur ne comporte pas de taux Coût par heure, le taux coût par heure du rôle de tâche sous lequel il est répertorié est utilisé dans le calcul. Si aucun rôle n’est associé à l’utilisateur, le coût utilisateur disponible est de 0 €. </p> </td>
</tr> 
  <tr> 
   <td>Coût disponible du rôle</td> 
   <td> <p>Le coût disponible par rôle est calculé à l’aide de la formule suivante :</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>NOTE</b>

Si le rôle n’a pas de taux de coût par heure, le coût du rôle disponible est de 0 $.</p> </td>
</tr> 
  <tr> 
   <td>Coût disponible du projet</td> 
   <td> <p>Le coût disponible par projet est calculé à l’aide de la formule suivante :</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Calcul du coût planifié dans le planificateur de ressources

Bien que vous ne puissiez pas afficher les informations de tâche dans le planificateur de ressources, les coûts planifiés des utilisateurs, des rôles et des projets sont calculés en prenant en compte les informations de tâche suivantes :

* Type d’affectation sur la tâche.\
   Vous pouvez laisser une tâche non assignée ou affecter les entités suivantes à une tâche :

   * Un utilisateur (avec ou sans rôle de tâche)
   * Un rôle
   * Une équipe\
      Une tâche affectée à une équipe est considérée comme non assignée, du point de vue du planificateur de ressources.

* Le **Type de coût** des tâches du projet.\
   Pour plus d’informations sur le type de coût d’une tâche, voir [Suivi des coûts](../../manage-work/projects/project-finances/track-costs.md).

>[!NOTE]
>
>Les coûts planifiés de l’utilisateur n’influencent pas le coût planifié du projet. Seul le rôle Les coûts prévus affectent les coûts prévus du projet, dans le planificateur de ressources.

Les scénarios suivants se présentent lors du calcul du coût planifié pour les utilisateurs, les rôles et le projet :

* Lorsque la variable **Type de coût** est **Heure de l’utilisateur **et il existe **aucune affectation** sur la tâche :

   * **Coût planifié du rôle et de l’utilisateur**:

      Le rôle et les coûts planifiés de l’utilisateur sont de 0,00 $.

   * **Coût planifié du projet**:

      Le coût prévu du projet est de 0,00 $.

* Lorsque la variable **Type de coût** is **Heure de l’utilisateur** et il y a une **affectation d’utilisateur** sur la tâche :

   * **Coût planifié du rôle et de l’utilisateur**:

      Le coût planifié de l’utilisateur est calculé à l’aide de la formule suivante :



      ```
      User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate
      ```

      Si un utilisateur a un taux de coût dans son profil, ce taux est utilisé pour calculer le coût planifié. Sinon, le taux de coût par heure au niveau du système de leur rôle Principal est utilisé.

      >[!NOTE]
      >
      >L’utilisateur peut être affecté à la tâche avec l’un de ses rôles de tâche secondaires, mais le taux du rôle de tâche Principal est utilisé ici à la place.

      Le rôle Coût planifié est calculé à l’aide de la formule suivante :

      ```
      Role Planned Cost = SUM(User Planned Cost)
      ```

   * **Coût planifié du projet**:

      Le coût prévu du projet est de 0,00 $.

* Lorsque la variable **Type de coût** is **Heure de l’utilisateur** et il y a une **affectation de rôle** sur la tâche :

   * **Coût planifié du rôle et de l’utilisateur**:

      Le coût planifié de l’utilisateur est de 0,00 $.

      Le rôle Coût planifié est calculé à l’aide de la formule suivante :

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Le taux de coût par heure au niveau du système du rôle de tâche affecté à la tâche est utilisé pour calculer le coût planifié.

   * **Coût planifié du projet**:

      Le coût prévu du projet est de 0,00 $.

* Lorsque la variable **Type de coût** is **Heure du rôle** et il y a **aucune affectation** sur la tâche :

   * **Coût planifié du rôle et de l’utilisateur**:

      Le rôle et les coûts planifiés de l’utilisateur sont de 0,00 $.

   * **Coût planifié du projet**:

      Le coût prévu du projet est de 0,00 $.

* Lorsque la variable **Type de coût** is **Heure du rôle** et il y a une **affectation d’utilisateur** sur la tâche :

   * **Coût planifié du rôle et de l’utilisateur**:

      Le coût planifié de l’utilisateur est de 0,00 $.

      Le rôle Coût planifié est calculé selon la formule suivante :

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Workfront examine le rôle de tâche que l’utilisateur remplit sur la tâche pour calculer le coût planifié du rôle.

      Si l’utilisateur n’est associé à aucun rôle dans la tâche, le coût planifié est de 0,00 $.

   * **Coût planifié du projet**:

      Le coût planifié du projet est calculé à l’aide de la formule suivante :

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

* Lorsque la variable **Type de coût** is **Heure du rôle** et il y a une **affectation de rôle** sur la tâche :

   * **Coût planifié du rôle et de l’utilisateur**:

      Le coût planifié de l’utilisateur est de 0,00 $.

      Le rôle Coût planifié est calculé selon la formule suivante :

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Workfront examine le rôle de tâche que l’utilisateur remplit sur la tâche pour calculer le coût planifié du rôle.

   * **Coût planifié du projet**:

      Le coût planifié du projet est calculé à l’aide de la formule suivante :

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## Calcul du coût budgété dans le planificateur de ressources

Pour afficher les valeurs de coût budgété dans le planificateur de ressources, vous devez disposer des éléments suivants :

* Heures budgétées pour les rôles, les utilisateurs et les projets.
* Taux de coût par heure pour les utilisateurs et les rôles.

>[!NOTE]
>
>Les Heures budgétisées pour les projets sont calculées à partir des Heures budgétisées pour les rôles, et non sur celles des utilisateurs.

Le tableau suivant illustre le mode de calcul du coût budgété dans le planificateur de ressources :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Coût budgété</strong> </th> 
   <th><strong>Calcul</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Coût budgétaire des utilisateurs</td> 
   <td> <p>Le Coût budgété par utilisateur est calculé à l'aide de la formule suivante :</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>NOTE</b>

Si le profil de l’utilisateur ne comporte pas de coût par heure, le coût utilisateur budgété est de 0,00 €.</p> </p> </td>
</tr> 
  <tr> 
   <td>Coût budgétaire des rôles</td> 
   <td> <p>Le coût alloué au rôle est calculé à l’aide de la formule suivante :</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>NOTE</b>

Si le rôle n’a pas de taux de coût par heure, le coût du rôle budgété est de 0,00 $.</p> </p> </td>
</tr> 
  <tr> 
   <td>Coût budgété du projet</td> 
   <td> <p>Le coût budgété par projet est calculé à l'aide de la formule suivante :</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
