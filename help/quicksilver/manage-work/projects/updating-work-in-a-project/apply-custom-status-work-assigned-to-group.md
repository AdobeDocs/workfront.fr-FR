---
product-area: projects
navigation-topic: update-work-in-a-project
title: Appliquer des statuts aux travaux associés à un groupe
description: Si un projet est associé à un groupe, vous pouvez appliquer les états au niveau du système ainsi qu’un état personnalisé associé à ce groupe au projet, à la tâche ou aux problèmes de ce projet.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 36%

---

# Appliquer des statuts aux travaux associés à un groupe

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Si un projet est associé à un groupe, vous pouvez appliquer les états au niveau du système ainsi qu’un état personnalisé associé à ce groupe au projet, ou les tâches et problèmes sur ce projet. Pour plus d’informations sur les états des groupes dans Adobe Workfront, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>Vous ne pouvez associer que des projets à des groupes. Les problèmes et les tâches héritent du groupe du projet auquel ils appartiennent.

## Conditions d’accès

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
   <td> <p>Modifier l’accès aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Mise à jour du groupe de projets et de l’état

Lorsque vous mettez à jour le groupe d’un projet, les options disponibles pour l’état des tâches, des problèmes ou du projet changent pour correspondre au groupe.

1. Accédez à un projet ou créez un projet, comme décrit dans la section [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).
1. Cliquez sur l&#39;icône **Plus** ![](assets/more-icon.png), puis sur **Modifier**.

1. Dans la zone **Modifier le projet** qui s’affiche, près du bas de la section **Aperçu** , sélectionnez le groupe dans le menu déroulant **Groupe** .

1. Dans le menu déroulant **Status**, sélectionnez l’état personnalisé.

   >[!NOTE]
   >
   >Si vous sélectionnez un autre groupe dans le menu déroulant **Groupe**, les états personnalisés dans le menu **État** changent automatiquement pour établir une corrélation avec le nouveau groupe.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >
   >

1. Sélectionnez le statut du projet. Les états personnalisés que vous avez créés et appliqués à ce groupe s’affichent dans la liste.
