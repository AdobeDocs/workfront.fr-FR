---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Présentation de la date d’achèvement prévue pour les projets, tâches et problèmes
description: La date de fin prévue est un indicateur calculé en temps réel du moment où le projet, la tâche ou le problème sera terminé. Lorsque le projet, la tâche ou le problème est marqué comme terminé, la date d’achèvement prévue est remplacée par la date d’achèvement réel.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Présentation de la date d’achèvement prévue pour les projets, tâches et problèmes

La date de fin prévue est un indicateur calculé en temps réel du moment où le projet, la tâche ou le problème sera terminé. Lorsque le projet, la tâche ou le problème est marqué comme terminé, la date d’achèvement prévue est remplacée par la date d’achèvement réel.

Les sections suivantes décrivent comment la date d’achèvement prévue est déterminée pour les projets, les tâches et les problèmes, et comment la localiser.

## Exigences d’accès

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Passez en revue la date d’achèvement prévue ou ultérieure pour l’afficher dans un rapport.</p> <p>Une licence Plan pour créer un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur à la console Projets</p> <p>Pour créer un rapport, vous devez disposer des droits d’édition sur les rapports, les tableaux de bord et les calendriers.</p> <p>Vous devez disposer d’un accès en édition aux options Filtres, Vues et Groupements pour créer un rapport ou modifier le mode Liste.</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures d’un projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Comment Adobe Workfront détermine la date d’achèvement prévue

La date de fin prévue est un champ calculé qui ne peut pas être modifié manuellement.

Les critères utilisés pour déterminer la date de fin prévue diffèrent selon l’objet que vous affichez :

* **Projets :** La date d’achèvement prévue des projets correspond à la date d’achèvement prévue de la dernière tâche du projet.
* **Tâches :** La date d’achèvement prévue des tâches est déterminée selon les critères suivants :

   * **Mises à jour de l’état d’avancement de la tâche par la personne désignée pour la tâche :** Les mises à jour de progression incluent les modifications du pourcentage terminé et de l’état de la tâche.
   * **Date de validation :** Si la personne désignée par la tâche indique une date de validation, la date de fin prévue se modifie pour correspondre à la date de validation.

      Pour plus d’informations sur les dates de validation, voir l’article [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Prédécesseurs :** S’il n’y a aucun retard sur les tâches précédentes, la date de fin prévue doit correspondre à la date de fin prévue. En cas de retards, les tâches dépendantes affichent une date d’achèvement prévue supérieure à la date d’achèvement planifiée.

      Pour plus d’informations sur la date d’achèvement prévue des tâches, voir [Présentation de la date d’achèvement planifiée de la tâche](../../../manage-work/tasks/task-information/task-planned-completion-date.md).
   >[!IMPORTANT]
   >
   >Lorsque le prédécesseur d’une tâche comporte une date de fin réelle, les tâches dépendantes reçoivent une date de fin prévue, comme décrit dans le scénario suivant :
   >
   >
   >Si le projet comporte les tâches A, B et C, et que la tâche B est le successeur de la tâche A, la tâche C succède à la tâche B et qu’une date d’achèvement réelle est ajoutée à la tâche A, la date d’achèvement prévue est automatiquement recalculée pour la tâche B (à condition que la **Type de mise à jour** du projet est défini sur Automatique et En changement), mais il ne sera pas recalculé pour la tâche C. Actuellement, Workfront calcule la Date d’achèvement prévue pour les tâches qui sont à un niveau supérieur ou inférieur par rapport à la tâche mise à jour, pour des raisons de performances. 

* **Problèmes :**Le problème : la date de fin prévue est initialement définie pour correspondre à la date de fin prévue du problème.

   Si la personne désignée par le problème indique une date de validation, la date de fin prévue et la date de fin planifiée correspondent toutes deux à la date de validation.

   Pour plus d’informations sur les dates de validation, voir l’article [Présentation de la date de validation](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Afficher la date d’achèvement prévue

Vous pouvez afficher la date d’achèvement prévue des projets, tâches et problèmes dans les rapports. Vous pouvez afficher la date d’achèvement prévue des projets et tâches dans d’autres zones de Workfront. 

* [Affichage de la date d’achèvement prévue d’un projet](#view-the-projected-completion-date-of-a-project)
* [Afficher la date d’achèvement prévue d’une tâche](#view-the-projected-completion-date-of-a-task)
* [Afficher la date d’achèvement prévue d’un problème](#view-the-projected-completion-date-of-an-issue)

### Affichage de la date d’achèvement prévue d’un projet {#view-the-projected-completion-date-of-a-project}

1. Accédez au projet dans lequel vous souhaitez afficher la date de fin prévue.
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Recherchez la variable **Date d’achèvement prévue** dans le champ **Présentation** .

### Afficher la date d’achèvement prévue d’une tâche {#view-the-projected-completion-date-of-a-task}

1. Accédez à la tâche où vous souhaitez afficher la date de fin prévue.
1. Cliquez sur **Détails de la tâche** dans le panneau de gauche.
1. Recherchez la variable **Date d’achèvement prévue** dans le champ **Présentation** .

### Afficher la date d’achèvement prévue d’un problème {#view-the-projected-completion-date-of-an-issue}

Vous pouvez afficher la date d’achèvement prévue pour les problèmes uniquement dans un rapport de problèmes ou en mode Liste. La création d’un mode Liste est similaire à la création d’un mode dans un rapport.

Pour créer un rapport de problème qui inclut la date de fin prévue :

1. Créez un rapport de problèmes, comme décrit dans l’article . [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sélectionnez la **Colonnes (affichage)** .
1. Cliquez sur **Ajouter une colonne**, puis commencez à taper **Date d’achèvement prévue** dans le **Afficher dans cette colonne :** champ .

1. Sélectionnez-le lorsqu’il apparaît dans la liste, sous le **Problème** . 
1. Cliquez sur **Enregistrer + Fermer**.

   Le **Date d’achèvement prévue** est renseignée dans le rapport. 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
