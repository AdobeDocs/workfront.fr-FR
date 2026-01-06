---
product-area: projects
navigation-topic: plan-a-project
title: Voir les heures prévues du projet dans le panneau Affectation des rôles
description: Vous pouvez visualiser l’affectation des rôles pour toutes les fonctions affectées aux éléments de travail d’un projet dans le panneau Affectation des rôles du projet.
author: Alina, Lisa
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 61%

---

# Voir les heures prévues du projet dans le panneau Affectation des rôles

Vous pouvez visualiser l’affectation des rôles pour toutes les fonctions affectées aux éléments de travail d’un projet dans le panneau Affectation des rôles du projet.

>[!NOTE]
>
>Cet article fait référence à l’affichage des fonctions associées aux tâches et aux problèmes d’un projet, et aux heures prévues qui leur sont affectées dans le panneau d’affectation des rôles d’un projet. Pour plus d’informations sur le rapprochement des heures prévues et des heures d’initiatives à l’aide du panneau d’affectation des rôles lors de l’utilisation du planificateur de scénarios Adobe Workfront, voir ce qui suit :
>
>* [Afficher l’affectation des rôles pour les projets et les initiatives dans la liste des tâches](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Afficher l’affectation des rôles pour les projets et les initiatives dans l’équilibreur de charge de travail](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Vous devez disposer d’une licence de Planificateur de scénarios pour afficher les heures d’initiative dans le panneau Attribution des rôles. Pour plus d’informations sur le planificateur de scénarios, voir [Prise en main du planificateur de scénarios](../../../scenario-planner/get-started-with-scenario-planning.md).
>
>Si votre société a acheté le planificateur de scénarios Adobe par le passé, il bénéficie d’une clause d’antériorité. Le planificateur de scénarios ne peut plus être acheté.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Adobe Workfront Ultimate</p>
   <p>Adobe Workflow Ultimate</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Léger ou supérieur</p>
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux projets</p>
   <p>Modifier l’accès au planificateur de scénarios pour mettre à jour les heures des initiatives</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations en affichage ou autorisations supérieures sur le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

able style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
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
</table>-->

## Conditions préalables

Vous devez disposer des éléments suivants :

* Tâches ou problèmes affectés à des fonctions ou à des personnes associées à une fonction.

  >[!TIP]
  >
  >Si les tâches ou les problèmes ne sont pas affectés, s’ils sont affectés à des équipes ou s’ils sont affectés à des personnes sans fonction, le nombre d’heures prévues du projet est égal à zéro dans le panneau Affectation des rôles.

* Tâches et problèmes dont la durée est supérieure à zéro.

## Voir les heures prévues du projet dans le panneau Affectation des rôles

{{step1-to-projects}}

1. Cliquez sur le nom d’un projet pour y accéder. La page Projet s’ouvre.
1. Cliquez sur l’un des éléments suivants dans le panneau de gauche :

   * **Tâches**
   * **Équilibreur de charge de travail**

1. Cliquez sur l’icône **Afficher l’attribution des rôles** ![Afficher l’icône d’attribution des rôles](assets/show-role-allocation-icon.png).

   Le panneau Affectation des rôles s’affiche.

   ![Panneau d’affectation des rôles avec les heures prévues uniquement](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Consultez les informations suivantes dans le panneau **Affectation des rôles** :

   | champ | Description |
   |---|---|
   | **Fonction** | Fonctions affectées aux tâches et événements du projet. Il peut s’agir de fonctions affectées directement à des tâches et à des événements, ou de fonctions associées à des utilisateurs affectés à des tâches et à des événements du projet. |
   | **Nombre d’heures prévues** | Nombre total d&#39;heures prévues pour les tâches et les événements affectés aux fonctions ou aux utilisateurs associés à une fonction dans le projet. |

