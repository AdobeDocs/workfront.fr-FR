---
product-area: projects
navigation-topic: manage-tasks
title: Associer des jalons à des tâches
description: Vous pouvez associer des jalons à des tâches pour indiquer le moment où vous atteignez des étapes importantes au cours de la durée de vie du projet.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Associer des jalons à des tâches

Vous pouvez associer des jalons à des tâches pour indiquer le moment où vous atteignez des étapes importantes au cours de la durée de vie du projet.

## Exigences d’accès

<!--drafted - replace table for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
  <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour la tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir associer un jalon à une tâche, les éléments suivants doivent exister :

* L’administrateur de Workfront doit créer un chemin d’accès de jalon, comme décrit dans la section [Création d’un chemin de jalon](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Pour associer un chemin de jalon à un projet, ce dernier doit être à l’état Planification ou Actuel .

>[!TIP]
>
>Pour obtenir un meilleur aperçu de la progression des jalons dans vos projets à l’aide de la vue Milestone, vous devez créer des tâches parents et les associer à chaque phase majeure de votre projet. Ensuite, associez ces tâches parents à chacun des jalons de votre chemin d’accès de jalon.

## Associer un jalon à une tâche

1. Accédez à un projet, puis cliquez sur le bouton **Plus** icon ![](assets/more-icon.png), puis **Modifier**.
1. En utilisant la variable **Paramètres** , définissez le chemin d’accès au jalon à utiliser sur le projet.
1. Cliquer sur **Enregistrer**.

   Une fois qu’un chemin de jalon est associé à un projet, les tâches peuvent se voir attribuer un jalon.

1. Accédez à une tâche, puis cliquez sur le bouton **Plus** icon ![](assets/more-icon.png), puis **Modifier**.

   Les tâches et les jalons ont une relation 1:1. Vous ne pouvez pas joindre le même jalon à plusieurs tâches. Chaque tâche peut être associée à un seul jalon ou chaque jalon peut être associé à une seule tâche.

1. Cliquez sur **Paramètres**, puis sélectionnez un jalon dans la variable **Milestone** pour la tâche.
1. Cliquez sur **Enregistrer**.
1. (Facultatif) Dans une liste de tâches, ajoutez le **Icônes d’état** pour identifier les tâches qui comportent des jalons.

   ![](assets/amwt3.png)

1. (Facultatif) Dans une liste de projets, sélectionnez l’option **Milestone** pour identifier la progression de vos tâches de jalon.

   ![Screen_Shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)
