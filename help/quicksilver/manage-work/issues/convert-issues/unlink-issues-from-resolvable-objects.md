---
product-area: projects
navigation-topic: convert-issues
title: Annuler le lien entre les événements et leurs objets de résolution
description: Lorsque vous créez un projet ou une tâche en convertissant un problème en projet ou en tâche, vous avez la possibilité de conserver le problème d’origine. Votre administrateur ou administratrice Adobe Workfront doit activer cette préférence pour que vous disposiez de cette option lors de la conversion du problème. Pour plus d’informations sur la conversion de problèmes en projets et tâches, voir Vue d’ensemble de la conversion de problèmes dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 96%

---

# Détacher les problèmes de leurs objets de résolution

<!--Audited: 08/2025-->

Lorsque vous créez un projet ou une tâche en convertissant un problème en projet ou en tâche, vous avez la possibilité de conserver le problème d’origine. Votre administrateur ou administratrice Adobe Workfront doit activer cette préférence pour que vous disposiez de cette option lors de la conversion du problème.\
Pour plus d’informations sur la conversion de problèmes en projets et tâches, voir [Vue d’ensemble de la conversion de problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Lorsque vous décidez de conserver le problème qui a été converti dans le projet ou la tâche, la résolution du problème est liée au projet ou à la tâche. Le problème devient l’objet résolvable du projet ou de la tâche. Le projet ou la tâche sont les objets de résolution du problème.

Vous pouvez également lier manuellement un problème à un autre problème. Le deuxième problème devient l’objet de résolution du premier problème, dans ce cas.\
Pour plus d’informations sur la résolution d’objets, voir [Vue d’ensemble des objets de résolution et des objets résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>Le statut du problème ne peut pas être modifié, car il change automatiquement avec celui de l’objet de résolution.

Vous pouvez dissocier la résolution d’un problème de celle d’un projet, d’une tâche ou d’un problème en supprimant le projet, la tâche ou le problème du problème.

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
   <td> <p>Contributeur ou version ultérieure</p>
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Afficher l'accès aux tâches et projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur le problème</p> <p>Autorisations d’afficher sur la tâche ou le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Annuler le lien d’un problème avec un projet, une tâche ou un problème

1. Accédez au problème lié à un projet, une tâche ou un problème.
1. Cliquez sur la section **Détails du problème**.
1. Accédez à la zone **Vue d’ensemble** de la section **Détails du problème**.
1. Dans le champ **Résolu par**, supprimez le type d’objet résolvable.\
   Un problème peut être résolu par un projet, une tâche ou un problème.

   Cela supprime l’objet de résolution du problème.

1. Cliquez sur **Enregistrer** **les modifications**.\
   Le problème n’est plus lié à un projet, à une tâche ou à un problème, et vous pouvez désormais le résoudre indépendamment.
