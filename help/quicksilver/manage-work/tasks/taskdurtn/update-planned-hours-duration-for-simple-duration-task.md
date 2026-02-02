---
product-area: projects
navigation-topic: task-duration
title: Mettre à jour les heures prévues et la durée d'une tâche avec un type de durée simple
description: Par défaut, Adobe Workfront calcule la durée d’une tâche avec un type de durée simple en fonction du nombre d’heures prévues. Cependant, vous pouvez également modifier manuellement le nombre d’heures prévues et la durée d’une tâche avec un type de durée simple dans certaines zones de Workfront.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 78%

---

# Mettre à jour le nombre d’heures prévues et la durée d’une tâche avec un type de durée simple

Par défaut, Adobe Workfront calcule la durée d’une tâche avec un type de durée simple en fonction du nombre d’heures prévues. Cependant, vous pouvez également modifier manuellement le nombre d’heures prévues et la durée d’une tâche avec un type de durée simple dans certaines zones de Workfront.

Vous pouvez modifier le nombre d’heures prévues et la durée d’une tâche avec un type de durée simple en ligne ou au niveau de la tâche dans la zone Affectations.

Pour plus d’informations sur la modification d’informations en ligne, voir [Modifier en ligne les éléments d’une liste dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

Cet article décrit comment vous pouvez mettre à jour le nombre d’heures prévues et la durée d’une tâche avec un type de durée simple au niveau de la tâche, dans la zone Affectations.

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
   <td><p>Standard ou supérieur</p> 
   <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux projets</p> <p>Modifier l’accès aux tâches</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès à la tâche </p></td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Mettre à jour le nombre d’heures prévues et la durée d’une tâche avec un type de durée simple

>[!IMPORTANT]
>
>Après avoir mis à jour manuellement la durée d’une tâche avec un type de durée simple, Workfront cesse de la calculer en fonction du nombre d’heures prévues.

Pour modifier le nombre d’heures prévues et la durée d’une tâche avec un type de durée simple dans la zone Affectations avancées, procédez comme suit :

1. Dans une liste de tâches, cliquez sur le nom de la tâche pour laquelle vous souhaitez modifier le type de durée.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’icône **Plus** ![Plus d’un objet](assets/qs-more-icon-on-an-object.png) en regard du nom de la tâche, cliquez sur **Modifier**, puis **Affectations**.
   * Cliquez sur le **Affecté à** ou sur le nom des affectations dans la zone Affectations de l’en-tête de la tâche, puis cliquez sur **Avancé**.

1. Saisissez une valeur totale pour le **Nombres d’heures prévues** pour toutes les affectations, par exemple 10 heures. Le nombre total d’heures prévues est réparti de manière égale entre toutes les ressources affectées à la tâche.
1. (Facultatif) Ajustez manuellement les heures prévues de chaque ressource affectée à la tâche. Le nombre total d’heures prévues pour la tâche est mis à jour pour refléter les nouvelles heures affectées individuellement à vos ressources.
1. Saisissez une valeur pour la **Durée** de la tâche, par exemple 2 jours.

   ![Ressources multiples de durée simple d&#39;affectations avancées](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Cliquer sur **Enregistrer**.
