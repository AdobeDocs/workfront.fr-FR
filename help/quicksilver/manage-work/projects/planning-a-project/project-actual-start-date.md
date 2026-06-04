---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la date de début effective du projet
description: Les projets, les tâches et les problèmes ont une date de début effective dans Adobe Workfront. Pour les tâches et les problèmes, il s’agit de la date à laquelle ils ont été marqués comme En cours. Pour les projets, il s’agit de la date à laquelle la première tâche du projet est marquée comme En cours ou est terminée.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/DWzx7-PW4nb78Q-XuI0AUjcCOFFap-f3qunguTclLpE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 530
ht-degree: 52%

---

# Vue d’ensemble de la date de début effective du projet

Les projets, les tâches et les problèmes ont une date de début effective dans Adobe Workfront. Pour les tâches et les problèmes, il s’agit de la date à laquelle ils ont été marqués comme En cours. Pour les projets, il s’agit de la date à laquelle la première tâche du projet est marquée comme En cours ou est terminée.

## Conditions d’accès

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
   <td><p>Léger ou supérieur</p> 
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur sur un projet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

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
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Considérations relatives aux dates de début effectives dans Workfront

* La date de début effective se trouve dans la section Détails des projets, tâches et problèmes.
* La date de début effective d&#39;un projet, d&#39;une tâche ou d&#39;un événement n&#39;est pas renseignée lorsque ces éléments sont créés.
* La date de début effective est renseignée lorsque le travail commence réellement sur le projet, la tâche ou l&#39;événement.
* La date de début réelle ne s’affiche pas dans l’onglet Détails du projet si le travail n’a pas encore commencé.

  La date de début réelle apparaît vide dans les onglets Détails de la tâche et de l&#39;événement si le travail n&#39;a pas encore commencé.

* Vous pouvez modifier manuellement la date de début réelle d&#39;une tâche ou d&#39;un événement, mais vous ne pouvez pas modifier la date de début réelle d&#39;un projet.

## Considérations relatives aux dates de début effectives des projets

* Workfront définit automatiquement la date effective d’un projet dans les cas suivants :

   * Une personne cessionnaire de tâche modifie le statut d’une tâche, passant de *Nouveau* à tout autre statut qui n’équivaut pas à *Nouveau*.

   * Une personne cessionnaire de tâche modifie le pourcentage de tâche terminé.

     >[!IMPORTANT]
     >
     >La date de début effective du projet n&#39;est pas renseignée lorsque le projet est marqué comme Actuel. Le travail réel doit commencer sur les tâches du projet avant que la date de début réelle du projet ne soit renseignée.

     Dans ce cas, la date de début effective du projet est définie sur la date et l’heure auxquelles ces actions se sont produites pour la première tâche du projet. Cela indique que le projet a réellement commencé à cette date et cette heure.

## Localiser la date de début réelle d’un projet

La date de début réelle d&#39;un projet se trouve dans les zones suivantes :

* dans la section Détails d’un projet ;
* Dans un rapport ou une vue de projet, lorsque vous ajoutez la **Date de début effective** pour l&#39;objet de projet dans le rapport.

  Pour plus d’informations sur la création de rapports, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour localiser la date de début réelle dans la section Détails du projet :

{{step1-to-projects}}

1. Cliquez sur le projet pour lequel vous souhaitez afficher la date de début effective.
1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis accédez à la section **Aperçu**.

   ![Date de début réelle du projet mise en surbrillance](assets/nwe-project-actual-start-date--highlighted-350x367.png)

   La **Date de début effective** s’affiche avec d’autres dates de projet.


