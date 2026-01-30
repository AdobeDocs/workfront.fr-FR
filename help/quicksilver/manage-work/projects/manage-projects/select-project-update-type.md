---
product-area: projects
navigation-topic: manage-projects
title: Sélectionner le type de mise à jour du projet
description: En sélectionnant un type de mise à jour pour un projet, vous pouvez contrôler la fréquence à laquelle les modifications que vous apportez à la chronologie du projet sont enregistrées sur les tâches parent ou sur le projet.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 64%

---

# Sélectionner le type de mise à jour du projet

En sélectionnant un type de mise à jour pour un projet, vous pouvez contrôler la fréquence à laquelle les modifications que vous apportez à la chronologie du projet sont enregistrées sur les tâches parent ou sur le projet.

Lorsque la chronologie du projet est mise à jour, elle est recalculée en fonction des changements apportés au projet, à ses tâches ou aux changements apportés à un autre projet dont la chronologie dépend.

Par exemple, les modifications suivantes apportées aux tâches du projet déclenchent une mise à jour de la chronologie du projet :

* Mise à jour des dates des tâches
* Modification des relations d’antériorité des tâches
* Modification des relations parents-enfants, en ajoutant ou en supprimant des affectations et en modifiant la contrainte de tâche ou le type de durée

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion d’un projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mettre à jour le type de mise à jour d’un projet

Lors de la mise à jour des tâches, leurs objets parents (tâches parents ou projet) sont mis à jour au moment indiqué par le type de mise à jour.  Pour spécifier un type de mise à jour pour votre projet :

1. Accédez au projet dont vous souhaitez spécifier le type de mise à jour.
1. Cliquez sur le menu Plus ![icône Plus](assets/more-icon.png) en regard du nom du projet, puis cliquez sur **Modifier** .

1. Cliquez sur **Paramètres** **du projet**.

   ![Champ de type de mise à jour de la zone d’édition du projet](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. Dans le champ **Type de mise à jour**, sélectionnez si vous voulez que Workfront calcule automatiquement la chronologie du projet quotidiennement, en cas de modification, ou si vous voulez que le ou la gestionnaire du projet la calcule manuellement.

   Sélectionnez l’une des options de la liste ci-dessous.

   >[!IMPORTANT]
   >
   >Si la chronologie d’un projet est supérieure à 15 ans, Workfront ne calcule pas la durée automatiquement ou en cas de modification. Le type de mise à jour d’un projet de plus de 15 ans est toujours manuel.

   * **Automatique et En cas de modification :** il s’agit du paramètre par défaut. La chronologie du projet est mise à jour chaque fois qu’une modification est apportée au projet ou à un autre projet dont la chronologie dépend. La chronologie du projet est également mise à jour chaque nuit.\
     Il s’agit du paramètre recommandé, car il garantit que la chronologie du projet est toujours à jour.

     Lorsque vous mettez à jour une tâche ou un projet et que vous déclenchez un recalcul de la chronologie, toutes les dates disponibles sont immédiatement affichées, ce qui vous permet de continuer à travailler. Pour les projets comportant plus de 100 tâches, les dates qui nécessitent des calculs plus longs sont grisées.

     ![Dates grisées lors de la modification sur la ligne](assets/dates-dimmed-when-insline-editing-350x146.png)

     Cela indique que le nouveau calcul n’est pas encore terminé et que les dates sont susceptibles d’être modifiées.

   * **Modification uniquement :** la chronologie du projet est mise à jour chaque fois qu’une modification est apportée au projet ou à un autre projet dont la chronologie dépend. Les mises à jour planifiées ne se produisent pas.\
     Vous pouvez sélectionner cette option si vous vous inquiétez des performances du système et si des modifications se produisent rarement dans le projet ou dans d’autres projets dont dépend la chronologie.

   * **Automatique uniquement :** la chronologie du projet est mise à jour chaque nuit ; elle n’est pas mise à jour immédiatement après l’application des modifications.\
     Vous pouvez sélectionner cette option si les performances du système vous préoccupent et si de nombreuses modifications interviennent chaque jour dans le projet ou dans d’autres projets dont la chronologie dépend.

     >[!NOTE]
     >
     >Un projet n’est pas automatiquement recalculé chaque nuit si son statut est Planification. Il n’est recalculé qu’en cas de modification.

   * **Manuel uniquement :** la chronologie du projet est mise à jour uniquement lorsque vous sélectionnez l’option **Recalculer les chronologies**, comme décrit dans la section « Recalcul manuel » de l’article [Recalculer les chronologies du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
     Vous pouvez sélectionner cette option si vous apportez de nombreuses modifications au projet en même temps et que vous souhaitez que le recalcul de la chronologie soit effectué après toutes les modifications (plutôt qu’après chaque modification individuelle).

1. Cliquer sur **Enregistrer**.
