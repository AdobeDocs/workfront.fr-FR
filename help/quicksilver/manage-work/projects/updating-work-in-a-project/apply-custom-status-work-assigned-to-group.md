---
product-area: projects
navigation-topic: update-work-in-a-project
title: Application d’états à un travail associé à un groupe
description: Si un projet est associé à un groupe, vous pouvez appliquer les états au niveau du système ainsi qu’un état personnalisé associé à ce groupe au projet, à la tâche ou aux problèmes de ce projet.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Application d’états à un travail associé à un groupe

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Si un projet est associé à un groupe, vous pouvez appliquer les états au niveau du système ainsi qu’un état personnalisé associé à ce groupe au projet, ou les tâches et problèmes sur ce projet. Pour plus d’informations sur les états d’un groupe dans Adobe Workfront, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>Vous ne pouvez associer que des projets à des groupes. Les problèmes et les tâches héritent du groupe du projet auquel ils appartiennent.

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Mise à jour du groupe de projets et de l’état

Lorsque vous mettez à jour le groupe d’un projet, les options disponibles pour l’état des tâches, des problèmes ou du projet changent pour correspondre au groupe.

1. Accédez à un projet ou créez-en un, comme décrit dans la section [Création d’un projet](../../../manage-work/projects/create-projects/create-project.md).
1. Cliquez sur le bouton **Plus** icon ![](assets/more-icon.png), puis cliquez sur **Modifier**.

1. Dans le **Modifier le projet** qui s’affiche, près du bas de la **Présentation** , sélectionnez le groupe dans la **Groupe** menu déroulant.

1. Dans le **État** , sélectionnez l’état personnalisé.

   >[!NOTE]
   >
   >Si vous sélectionnez un autre groupe dans la variable **Groupe** menu déroulant, les états personnalisés dans le **État** change automatiquement pour établir une corrélation avec le nouveau groupe.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >

1. Sélectionnez l’état du projet. Les états personnalisés que vous avez créés et appliqués à ce groupe s’affichent dans la liste.
