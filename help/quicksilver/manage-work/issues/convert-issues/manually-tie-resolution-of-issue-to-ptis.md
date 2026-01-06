---
product-area: projects
navigation-topic: convert-issues
title: Lier manuellement la résolution d'un problème à d'autres problèmes, tâches ou projets
description: Vous pouvez lier manuellement la résolution d’un problème à la résolution d’un projet, d’une tâche ou d’un problème sans le convertir. Le problème devient l’un des objets résolvables du projet, de la tâche ou du problème que vous sélectionnez. Lorsque vous procédez de la sorte, une modification du statut du projet, de la tâche ou du problème déclenche une modification du statut du problème d’origine.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 95%

---

# Lier manuellement la résolution d’un problème à d’autres problèmes, tâches ou projets

<!--Audited: 08/2025-->

Vous pouvez lier manuellement la résolution d’un problème à la résolution d’un projet, d’une tâche ou d’un problème sans le convertir. Le problème devient l’un des objets résolvables du projet, de la tâche ou du problème que vous sélectionnez. Lorsque vous procédez de la sorte, une modification du statut du projet, de la tâche ou du problème déclenche une modification du statut du problème d’origine.

>[!TIP]
>
>Lorsque vous liez la résolution d’un problème à la résolution d’un autre objet, vous ne pouvez plus modifier manuellement le statut du problème d’origine.

Pour plus d’informations sur les objets de résolution et les objets résolvables, consultez [Vue d’ensemble des objets de résolution et des objets résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

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
   <td><p>Contributeur ou version ultérieure</p> 
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l'accès aux événements, tâches, projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’accès au problème lié à un autre problème, une autre tâche ou un autre projet</p> <p>Autorisations Afficher ou autorisations supérieures au problème, à la tâche ou au projet que vous ajoutez au problème existant.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Conditions préalables

Avant de commencer, vous devez :

* posséder un problème dont vous souhaitez lier la résolution à un autre problème, une autre tâche ou un autre projet ;

* posséder un problème, une tâche ou un projet supplémentaire ;

## lier la résolution d’un problème à la résolution d’un autre problème, d’une autre tâche ou d’un autre projet.

1. Accédez au problème dont vous souhaitez lier la résolution à un autre problème ou à la résolution d’une tâche ou d’un projet.
1. Cliquez sur **Détails du problème** dans le panneau de gauche, puis développez la zone **Vue d’ensemble**.

   ![Icône Détails de l’événement](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Cliquez sur le champ **Résolu par** et effectuez une sélection parmi les types d’objets de résolution suivants :

   * **Projet**
   * **Tâche**
   * **Problème**

   Selon l’objet sélectionné, les champs suivants s’affichent :

   * **Résolution du projet**
   * **Résolution de la tâche**
   * **Résolution du problème**

1. Commencez à saisir le nom d’un projet, d’une tâche ou d’un problème spécifique dans le champ **Résolution du projet**, **Tâche**, ou **Problème** puis cliquez sur l’élément concerné lorsqu’il apparaît dans la liste.

   >[!NOTE]
   >
   >Vous ne pouvez pas lier la résolution d’un problème à la tâche ou au projet où le problème se trouve. La tâche ou le projet du problème ne s’affiche pas dans la Résolution de la tâche ou dans les champs Résolution de la tâche.


1. Cliquez sur **Enregistrer les modifications**.

   Le problème d’origine devient l’objet résolvable pour le projet, la tâche ou le problème que vous avez sélectionné(e) aux étapes 4 et 5. Cela signifie que le problème d’origine se termine lorsque l’objet de résolution (le projet, la tâche ou le problème auquel ou à laquelle vous l’avez lié) est terminé.

   >[!NOTE]
   >
   >Un projet, une tâche ou un problème peut présenter plusieurs problèmes comme objets résolvables.
