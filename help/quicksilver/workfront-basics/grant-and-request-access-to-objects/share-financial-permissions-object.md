---
title: Partage des autorisations financières sur un objet
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Votre administrateur Adobe Workfront peut vous accorder l’accès à l’affichage ou à la modification de données financières lors de l’attribution de votre niveau d’accès. Pour plus d’informations, voir Octroi de l’accès aux données financières.
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 3%

---

# Partage des autorisations financières sur un objet

Votre administrateur Adobe Workfront peut vous accorder l’accès à l’affichage ou à la modification de données financières lors de l’attribution de votre niveau d’accès. Pour plus d’informations, voir [Accorder l&#39;accès aux données financières](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Outre le niveau d’accès que les utilisateurs reçoivent, vous pouvez leur accorder des autorisations d’ Affichage ou de Gestion des finances pour des projets, tâches ou problèmes spécifiques que vous avez accès au partage.

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec les données financières, voir la section [Données financières](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial&nbsp;Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Vous devez disposer des éléments suivants pour partager des informations de données financières sur les objets :

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur à Projets, tâches, problèmes et données financières</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations ou des autorisations supérieures pour les projets, les tâches et les problèmes qui incluent au moins les autorisations Afficher les autorisations Finance</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Partage d’un objet et octroi d’autorisations financières

Tenez compte des points suivants lors de l’octroi d’autorisations financières aux objets :

* Vous pouvez accorder des autorisations financières aux projets, aux tâches et aux problèmes.
* Les autorisations peuvent être héritées : si vous disposez des autorisations Afficher le financement pour un projet, vous héritez automatiquement des autorisations Afficher le financement pour les tâches et les problèmes du projet.

Pour accorder des autorisations financières à un objet :

1. Accédez à une tâche, à un projet ou à un problème que vous souhaitez partager avec d’autres personnes.
1. Près du nom de l’objet, cliquez sur le menu Plus ![](assets/more-icon.png), puis cliquez sur **Partage**.

1. Dans le **Give `<Object name>` accès à** commencez à saisir le nom d’un utilisateur, d’une équipe, d’un rôle, d’un groupe ou d’une société avec lequel vous souhaitez partager l’objet.

   >[!TIP]
   >
   >Vous pouvez partager un objet uniquement avec des utilisateurs, équipes, rôles ou entreprises principaux.

1. Si un menu déroulant s’affiche à droite du nom que vous avez sélectionné, cliquez sur l’une des options suivantes disponibles :

   * **L&#39;afficher**
   * **Y contribuer**
   * **Le gérer**

      ![](assets/12.png)      ![](assets/13.png) ![](assets/14.png)

1. Dans le même menu déroulant, cliquez sur **Paramètres avancés**, puis effectuez l’une des opérations suivantes :

   * Si vous avez sélectionné l’une des trois options de l’étape précédente, veillez à **Afficher Finance** est sélectionnée.
   * Si vous avez sélectionné **Gérer les finances** à l’étape précédente, veillez à **Gérer les finances** est sélectionnée.

1. Cliquer sur **Enregistrer**.

## Autorisation financière pour tous les niveaux de partage

Le tableau suivant affiche les autorisations financières obtenues par les utilisateurs lorsque vous leur accordez des autorisations Afficher, Contribuer ou Gérer sur des objets : 

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
   <td>Gestion des enregistrements de facturation</td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gérer/afficher la facturation et les taux de coût des rôles</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gérer/afficher les taux de facturation et de coûts des utilisateurs</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher Finance</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td>Affichage des informations par coût dans les outils de planification des ressources</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ressources budgétaires dans les outils de planification des ressources*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Affichage des ressources dans les outils de planification des ressources*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Nécessite un accès supplémentaire à la gestion des ressources.

Pour plus d’informations sur l’accès à Resource Management, voir [Accorder l’accès à la gestion des ressources](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
