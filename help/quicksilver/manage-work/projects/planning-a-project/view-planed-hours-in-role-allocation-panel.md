---
product-area: projects
navigation-topic: plan-a-project
title: Afficher le nombre d’heures prévues du projet dans le panneau Allocation des rôles
description: Vous pouvez afficher l’attribution des rôles pour tous les rôles de tâche affectés aux tâches dans un projet dans le panneau Affectation de rôle du projet.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: 67deb48ebc90dd4a93c2af1cb89442ee2486cb16
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 28%

---

# Afficher le nombre d’heures prévues du projet dans le panneau Allocation des rôles

Vous pouvez afficher l’attribution des rôles pour tous les rôles de tâche affectés aux tâches dans un projet dans le panneau Affectation de rôle du projet.

>[!NOTE]
>
>Cet article fait référence à l’affichage des rôles de tâche associés aux tâches et aux problèmes d’un projet, ainsi qu’à leurs heures planifiées allouées dans le panneau Attribution des rôles d’un projet. Pour plus d’informations sur la réconciliation des heures planifiées avec les heures des initiatives à l’aide du panneau Attribution des rôles lors de l’utilisation du planificateur de scénario Adobe Workfront, voir :
>
>* [Afficher l’attribution des rôles pour les projets et les initiatives dans la liste des tâches](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Afficher l’attribution des rôles pour les projets et les initiatives dans l’équilibreur de charge de travail](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Vous devez disposer d’une licence de planificateur de scénario pour afficher les heures d’initiative dans le panneau Attribution des rôles . Pour plus d’informations sur le planificateur de scénario, voir [Prise en main du planificateur de scénario](../../../scenario-planner/get-started-with-scenario-planning.md) .
>

## Conditions d’accès

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

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en affichage ou supérieur pour les projets</p> <p>Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures sur le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Vous devez disposer des éléments suivants :

* Tâches ou problèmes affectés aux rôles de tâche ou aux utilisateurs associés à un rôle de tâche.

  >[!TIP]
  >
  >Si les tâches ou les problèmes ne sont pas affectés, affectés à des équipes ou affectés à des utilisateurs sans rôle de tâche, les heures planifiées du projet sont nulles dans le panneau Affectation du rôle .

* Tâches et problèmes avec une durée supérieure à zéro.

## Afficher le nombre d’heures prévues du projet dans le panneau Allocation des rôles

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Projets**.
1. Cliquez sur le nom d’un projet auquel accéder. La page Projet s’ouvre alors.
1. Cliquez sur l’une des options suivantes dans le panneau de gauche :

   * **Tâches**
   * **Équilibreur de charge de travail**

1. Cliquez sur l’icône **Afficher l’attribution de rôles** ![](assets/show-role-allocation-icon.png) .

   Le panneau Attribution des rôles s’affiche.

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Consultez les informations suivantes dans le panneau **Affectation de rôle** :

   | champ | Description |
   |---|---|
   | **Rôle de tâche** | Rôles de tâche affectés aux tâches et problèmes du projet. Il peut s’agir de rôles de tâche affectés directement à des tâches et des problèmes ou de rôles de tâche associés à des utilisateurs affectés à des tâches et des problèmes du projet. |
   | **Nombre d’heures prévues** | Nombre total d’heures planifiées provenant de tâches et de problèmes affectés à des rôles de tâche ou d’utilisateurs associés à un rôle de tâche sur le projet. |

