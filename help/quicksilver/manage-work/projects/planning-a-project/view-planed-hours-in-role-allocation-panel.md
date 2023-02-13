---
product-area: projects
navigation-topic: plan-a-project
title: Affichage des heures planifiées du projet dans le panneau Attribution des rôles
description: Vous pouvez afficher l’attribution des rôles pour tous les rôles de tâche affectés aux tâches dans un projet dans le panneau Affectation de rôle du projet.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Affichage des heures planifiées du projet dans le panneau Attribution des rôles

Vous pouvez afficher l’attribution des rôles pour tous les rôles de tâche affectés aux tâches dans un projet dans le panneau Affectation de rôle du projet.

>[!NOTE]
>
>Cet article fait référence à l’affichage des rôles de tâche associés aux tâches et aux problèmes d’un projet, ainsi qu’à leurs heures planifiées allouées dans le panneau Attribution des rôles d’un projet. Pour plus d’informations sur la réconciliation des heures planifiées avec les heures des initiatives à l’aide du panneau Attribution des rôles lors de l’utilisation du planificateur de scénario Adobe Workfront, voir :
>
>* [Afficher l’affectation des rôles pour les projets et les initiatives dans la liste des tâches](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Afficher l’affectation des rôles pour les projets et les initiatives dans l’équilibreur de charge de travail](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Vous devez disposer d’une licence de planificateur de scénario pour afficher les heures d’initiative dans le panneau Attribution des rôles . Pour plus d’informations sur le planificateur de scénario, voir [Prise en main du planificateur de scénarios](../../../scenario-planner/get-started-with-scenario-planning.md) .

## Exigences d’accès

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur à la console Projets</p> <p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures sur le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Vous devez disposer des éléments suivants :

* Tâches ou problèmes affectés aux rôles de tâche ou aux utilisateurs associés à un rôle de tâche.

   >[!TIP]
   Si les tâches ou les problèmes ne sont pas affectés, affectés à des équipes ou affectés à des utilisateurs sans rôle de tâche, les heures planifiées du projet sont nulles dans le panneau Affectation du rôle .

* Tâches et problèmes avec une durée supérieure à zéro.

## Affichage des heures planifiées du projet dans le panneau Attribution des rôles

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Projets**.
1. Cliquez sur le nom d’un projet auquel accéder. La page Projet s’ouvre alors.
1. Cliquez sur l’une des options suivantes dans le panneau de gauche :

   * **Tâches**
   * **Équilibreur de charge de travail**

1. Cliquez sur le bouton **Afficher l’affectation des rôles** icon ![](assets/show-role-allocation-icon.png).

   Le panneau Attribution des rôles s’affiche.

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Consultez les informations suivantes dans la section **Attribution des rôles** panel : |Field | Description| |—|—| | **Rôle de tâche** |Rôles de tâche affectés aux tâches et problèmes du projet. Il peut s’agir de rôles de tâche affectés directement à des tâches et des problèmes ou de rôles de tâche associés à des utilisateurs affectés à des tâches et des problèmes du projet.  | | **Heures planifiées** |Nombre total d’heures planifiées provenant de tâches et de problèmes affectés à des rôles de tâche ou d’utilisateurs associés à un rôle de tâche sur le projet. |



