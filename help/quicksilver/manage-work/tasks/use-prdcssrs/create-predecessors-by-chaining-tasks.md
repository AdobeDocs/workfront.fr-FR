---
product-area: projects
navigation-topic: use-predecessors
title: Créer des relations antérieures en chaînant des tâches
description: Vous pouvez créer des relations antérieures de plusieurs manières dans Adobe Workfront. Une méthode consiste à chaîner des tâches.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 100%

---

# Créer des relations antérieures en chaînant des tâches

Vous pouvez créer des relations antérieures de plusieurs manières dans Adobe Workfront. Une méthode consiste à chaîner des tâches.

Pour plus d’informations sur les tâches antérieures, consultez la section [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

En chaînant des tâches, vous permettez au système de créer automatiquement les relations antérieures sur les tâches sélectionnées, plutôt que de créer manuellement vous-même, une relation sur chaque tâche. Différents types de relations antérieures peuvent toujours être utilisés entre les tâches.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches et le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Chaîner des tâches pour créer des relations antérieures

1. Accédez au projet contenant les tâches que vous souhaitez chaîner.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. (Le cas échéant) Sélectionnez **Enregistrement automatique** dans le coin supérieur droit de la liste des tâches, puis sélectionnez les tâches que vous souhaitez chaîner.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

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
