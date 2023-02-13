---
product-area: projects
navigation-topic: manage-projects
title: Modification de l’état d’un projet
description: Vous pouvez modifier manuellement l’état d’un projet.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# Modification de l’état d’un projet

Vous pouvez modifier manuellement l’état d’un projet.

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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Modifier l’accès aux projets</p> <p><b>REMARQUE</b> Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations sur le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Considérations relatives à la mise à jour vers des états spécifiques

* **Lors de la mise à jour d’un projet à terminer :** Assurez-vous que toutes les tâches et tous les problèmes sont terminés sur le projet. Vous ne pouvez pas sélectionner l’état Terminé d’un projet, ni aucun autre état correspondant à Terminé lorsqu’il y a des tâches ou des problèmes qui n’ont pas été terminés sur le projet. Cela inclut l’approbation de toute tâche ou problème qui est à l’état Terminé en attente d’approbation.
* **Lors de la mise à jour d’un projet de la fin à actuel :** Si toutes les tâches et tous les problèmes du projet sont terminés, assurez-vous que le mode d’achèvement du projet est défini sur Manuel. Si le mode d’achèvement du projet est automatique, l’état du projet reste Terminé.

## Modification de l’état du projet

1. Accédez au projet dont vous souhaitez mettre à jour l’état.
1. Dans l’en-tête du projet, cliquez sur le nom de l’état dans la **État** , puis sélectionnez un nouvel état.

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Ou

   Cliquez sur le bouton **Plus** menu ![](assets/qs-more-menu.png) en regard du nom du projet, puis cliquez sur **Modifier** et sélectionnez un nouvel état dans le **État** , puis cliquez sur **Enregistrer**.

   L’état du projet est mis à jour vers celui que vous avez sélectionné.
