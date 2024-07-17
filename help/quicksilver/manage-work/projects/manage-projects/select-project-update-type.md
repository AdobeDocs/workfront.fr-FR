---
product-area: projects
navigation-topic: manage-projects
title: Sélectionner le type de mise à jour du projet
description: En sélectionnant un type de mise à jour pour un projet, vous pouvez contrôler la fréquence d’enregistrement des modifications apportées à la chronologie du projet sur les tâches parentes ou le projet.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 30%

---

# Sélectionner le type de mise à jour du projet

En sélectionnant un type de mise à jour pour un projet, vous pouvez contrôler la fréquence d’enregistrement des modifications apportées à la chronologie du projet sur les tâches parentes ou le projet.

Lorsque la chronologie du projet est mise à jour, elle est recalculée en fonction des modifications apportées au projet, à ses tâches ou à un autre projet dont la chronologie dépend.

Par exemple, les modifications suivantes apportées aux tâches du projet déclenchent une mise à jour de la chronologie.  du projet :

* Mettre à jour les dates des tâches
* Modifier les relations entre les prédécesseurs des tâches
* Modifier les relations parents-enfants, en ajoutant ou en supprimant des affectations et en modifiant la contrainte de tâche ou le type de durée

## Conditions d’accès

<!-- drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>N’importe quelle </p> </td> 
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
   <td> <p>Autorisations de gestion d’un projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Mise à jour du type de mise à jour d’un projet

Lorsque les tâches sont mises à jour, leurs objets parents (tâches parents ou projet) sont mis à jour au moment indiqué par le type de mise à jour.  Pour spécifier un type de mise à jour pour votre projet :

1. Accédez au projet dont vous souhaitez spécifier le type de mise à jour.
1. Cliquez sur le menu Plus ![](assets/more-icon.png) en regard du nom du projet, puis cliquez sur **Modifier** .

1. Cliquez sur **Projet** **Paramètres**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. Dans le champ **Type de mise à jour**, choisissez si vous souhaitez que Workfront calcule automatiquement la chronologie du projet tous les jours, en cas de modification, ou si vous souhaitez que le chef de projet le calcule manuellement.

   Sélectionnez parmi les options de la liste ci-dessous. 

   >[!IMPORTANT]
   >
   >Si le délai d’un projet dépasse 15 ans, Workfront ne calcule pas le délai automatiquement ni lors de la modification. Le type de mise à jour d’un projet de plus de 15 ans est toujours manuel.

   * **Automatique et Après modification :** Il s’agit du paramètre par défaut. La chronologie du projet est mise à jour chaque fois qu’une modification se produit dans le projet ou dans un autre projet dont elle dépend. La chronologie du projet est également mise à jour chaque nuit. \
     Il s’agit du paramètre recommandé, car il garantit que la chronologie du projet est toujours à jour.

     Lorsque vous mettez à jour une tâche ou un projet et que vous déclenchez un nouveau calcul de chronologie, toutes les dates disponibles s’affichent immédiatement, ce qui vous permet de continuer à travailler. Sur les projets comportant plus de 100 tâches, les dates nécessitant des calculs plus longs sont grisées.

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

     Cela indique que le recalcul n’est pas encore terminé et que les dates sont susceptibles d’être modifiées.

   * **Modifier uniquement :** La chronologie du projet est mise à jour chaque fois qu’une modification se produit dans le projet ou dans un autre projet dont dépend la chronologie ; les mises à jour planifiées ne se produisent pas.\
     Vous pouvez sélectionner cette option si vous vous souciez des performances du système et si des modifications surviennent rarement dans le projet ou dans d’autres projets dont dépend la chronologie.

   * **Automatique uniquement :** La chronologie du projet est mise à jour chaque nuit ; elle n’est pas mise à jour immédiatement après les modifications.\
     Vous pouvez sélectionner cette option si vous vous souciez des performances du système et si de nombreuses modifications se produisent chaque jour dans le projet ou dans d’autres projets dont dépend la chronologie.

     >[!NOTE]
     >
     >Un projet n&#39;est pas automatiquement recalculé chaque nuit s&#39;il est à l&#39;état Planification . Il ne recalcule qu’en cas de modification.

   * **Manuel uniquement :** La chronologie du projet est mise à jour uniquement lorsque vous sélectionnez l’option **Recalculer les chronologies**, comme décrit dans la section &quot;Recalcul manuel&quot; de l’article [Recalculer les chronologies du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
     Sélectionnez cette option si vous apportez de nombreuses modifications au projet en même temps et que vous souhaitez que le recalcul de la chronologie se produise après toutes les modifications (plutôt qu’après chaque modification individuelle).

1. Cliquer sur **Enregistrer**.
