---
product-area: projects
navigation-topic: use-predecessors
title: Créer des relations d’antériorité en enchaînant les tâches
description: Vous pouvez créer des relations de prédécesseur de plusieurs manières dans Adobe Workfront. Une méthode consiste à attacher des tâches.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 37%

---

# Créer des relations d’antériorité en enchaînant les tâches

Vous pouvez créer des relations de prédécesseur de plusieurs manières dans Adobe Workfront. Une méthode consiste à attacher des tâches.

Pour plus d’informations sur les tâches de prédécesseur, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

En enchaînant des tâches, vous pouvez permettre au système de créer automatiquement les relations de prédécesseur sur des tâches sélectionnées, plutôt que de créer manuellement une relation sur chaque tâche vous-même. Différents types de relations de prédécesseur peuvent toujours être utilisés entre les tâches.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux tâches et aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion sur les tâches et le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Tâches de chaîne pour créer des relations de prédécesseur

1. Accédez au projet contenant les tâches que vous souhaitez attacher.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. (Conditionnel) Sélectionnez **Enregistrement automatique** dans le coin supérieur droit de la liste des tâches, puis sélectionnez les tâches que vous souhaitez attacher.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >L’association de tâches dans une liste de tâches n’est pas possible lorsque vous enregistrez manuellement les modifications apportées aux tâches ou que vous utilisez le mode Planning d’exécution pour enregistrer les tâches.

1. Cliquez avec le bouton droit sur les tâches sélectionnées, puis cliquez sur **Chaîne**.
1. Sélectionnez l’un des types de dépendances suivants :

   * **Finish-Start**
   * **Finish-Finish**
   * **Start-Start**
   * **Start-Finish**

   Pour plus d’informations sur les types de dépendance de prédécesseur, voir [Présentation des types de dépendance de tâche](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Facultatif) Cliquez sur **Unchain** si certaines tâches ont été précédemment liées.

   >[!CAUTION]
   >
   >Seuls les prédécesseurs séquentiels sont supprimés à l’aide de l’option unchain lors des tâches de modification en masse.

   Les tâches sélectionnées sont désormais liées par les relations de prédécesseur.
