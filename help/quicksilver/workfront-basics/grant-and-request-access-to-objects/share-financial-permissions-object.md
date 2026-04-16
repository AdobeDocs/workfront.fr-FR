---
title: Partager des autorisations financières sur un objet
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Votre administrateur ou administratrice Adobe Workfront peut vous accorder un accès pour afficher ou modifier des données financières lors de l’attribution de votre niveau d’accès. Pour plus d’informations, voir Accorder l’accès aux données financières.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e974adc053a076a4370aa0c4ec41fea700d836be
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 56%

---

# Partager des autorisations financières sur un objet

Votre administrateur ou administratrice Adobe Workfront peut vous accorder un accès pour afficher ou modifier des données financières lors de l’attribution de votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux données financières](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Outre le niveau d’accès accordé aux utilisateurs et aux utilisatrices, vous pouvez leur octroyer des autorisations d’affichage ou de gestion des finances pour des projets, des tâches ou des problèmes spécifiques que vous pouvez partager.

Pour plus d’informations sur ce que les utilisateurs et utilisatrices de chaque niveau d’accès peuvent effectuer avec les données financières, voir la section [Données financières](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Conditions d’accès

<!--
drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Plan</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Afficher ou un accès supérieur aux projets, tâches, événements et données financières</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> Afficher les autorisations ou supérieures pour les projets, les tâches et les événements qui incluent au moins Afficher les taux de facturation, Afficher les taux de coûts et Afficher les autorisations financières générales</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Partager un objet et accorder des autorisations financières

Tenez compte des points suivants lors de l’octroi d’autorisations financières aux objets :

* Vous pouvez accorder des autorisations financières aux projets, tâches et événements.
* Les autorisations peuvent être héritées : si vous disposez des autorisations Afficher les finances générales pour un projet, vous héritez automatiquement des autorisations Afficher les finances générales pour les tâches et les événements du projet.
* L’octroi d’autorisations pour les taux de facturation et de coût permet à l’utilisateur d’afficher ou de modifier les taux sur cet objet. Les autorisations d&#39;accès aux finances générales permettent à l&#39;utilisateur d&#39;afficher ou de modifier des champs finances générales (non liés aux taux de facturation ou de coûts) sur l&#39;objet.

Pour accorder des autorisations financières à un objet :

1. Accédez à une tâche, à un projet ou à un problème que vous souhaitez partager avec d’autres personnes.
1. Près du nom de l’objet, cliquez sur **Partager**.

1. Dans le champ **Accorder un accès `<Object name>` à** commencez à saisir le nom d’un utilisateur, d’une équipe, d’un rôle, d’un groupe ou d’une entreprise avec lequel vous souhaitez partager l’objet.

   >[!TIP]
   >
   >Vous pouvez partager un objet uniquement avec des utilisateurs et utilisatrices, des équipes, des rôles ou des entreprises actifs.

1. Cliquez sur la liste déroulante située à droite du nom de l’utilisateur et sélectionnez l’une des options suivantes :

   * **Afficher**
   * **Contribuer**
   * **Gérer**

1. Dans le même menu déroulant, cliquez sur l’icône d’options avancées à côté du niveau d’autorisation, puis effectuez l’une des opérations suivantes :

   * Pour tout niveau d’autorisation, sélectionnez **Afficher les taux de facturation**, **Afficher les taux de coût** et **Afficher les finances générales** selon les besoins.
   * Pour les autorisations **Gérer** uniquement, sélectionnez **Modifier les taux de facturation**, **Modifier les taux de coût** et **Modifier les finances générales** si nécessaire.

1. Cliquer sur **Enregistrer**.

## Autorisation financière pour tous les niveaux de partage

Le tableau suivant affiche les autorisations financières que les utilisateurs obtiennent lorsque vous leur accordez des autorisations d&#39;affichage, de contribution ou de gestion sur des objets :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Actions</strong> </th> 
   <th><strong>Gérer</strong> </th> 
   <th><strong>Contribuer</strong> </th> 
   <th><strong>Afficher</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Gérer des enregistrements de facturation</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Modifier les taux de facturation</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Modifier les taux de dépenses</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>  
  <tr> 
   <td>Modifier les finances générales</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>
  <tr> 
   <td>Afficher les taux de facturation</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Afficher les taux de dépenses</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>  
  <tr> 
   <td>Afficher les finances générales</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Afficher des informations par coût dans les outils de planification des ressources</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Budgétiser les ressources dans les outils de planification des ressources*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Afficher les ressources dans les outils de planification des ressources*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Nécessite un accès supplémentaire à la gestion des ressources.

Pour plus d’informations sur l’accès à la gestion des ressources, voir [Accorder l’accès à la gestion des ressources](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

<!--
These rows removed from last table.

  <tr> 
   <td>Manage/ View Role Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Manage/ View User Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 

-->
