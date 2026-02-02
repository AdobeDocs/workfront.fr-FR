---
product-area: projects
navigation-topic: use-predecessors
title: Créer des relations antérieures en chaînant des tâches
description: Vous pouvez créer des relations antérieures de plusieurs manières dans Adobe Workfront. Une méthode consiste à chaîner des tâches.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 96%

---

# Créer des relations antérieures en chaînant des tâches

Vous pouvez créer des relations antérieures de plusieurs manières dans Adobe Workfront. Une méthode consiste à chaîner des tâches.

Pour plus d’informations sur les tâches antérieures, consultez la section [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

En chaînant des tâches, vous permettez au système de créer automatiquement les relations antérieures sur les tâches sélectionnées, plutôt que de créer manuellement vous-même, une relation sur chaque tâche. Différents types de relations antérieures peuvent toujours être utilisés entre les tâches.

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches et le projet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Chaîner des tâches pour créer des relations antérieures

1. Accédez au projet contenant les tâches que vous souhaitez chaîner.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. (Le cas échéant) Sélectionnez **Enregistrement automatique** dans le coin supérieur droit de la liste des tâches, puis sélectionnez les tâches que vous souhaitez chaîner.

   ![Icône d’enregistrement automatique en surbrillance](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >Le chaînage de tâches dans une liste de tâches n’est pas possible lorsque vous enregistrez manuellement les modifications apportées aux tâches ou lorsque vous utilisez le mode « Planification chronologique » pour enregistrer les tâches.

1. Cliquez avec le bouton droit sur les tâches sélectionnées, puis cliquez sur **Chaîner**.
1. Sélectionnez l’un des types de dépendances suivants :

   * **Terminer-Démarrer**
   * **Terminer-Terminer**
   * **Démarrer-Démarrer**
   * **Démarrer-Terminer**

   Pour plus d’informations sur les types de dépendance des prédécesseurs, consultez la section [Vue d’ensemble des types de dépendances des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Facultatif) Cliquez sur **Annuler le chaînage** si certaines des tâches ont déjà été chaînées.

   >[!CAUTION]
   >
   >Seuls les prédécesseurs séquentiels sont supprimés à l’aide de l’option « Annuler le chaînage » lors des tâches de modification en masse.

   Les tâches sélectionnées sont désormais liées par les relations antérieures.
