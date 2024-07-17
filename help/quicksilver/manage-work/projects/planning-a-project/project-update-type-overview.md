---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble du type de mise à jour du projet
description: Le type de mise à jour d’un projet indique comment Adobe Workfront calcule la chronologie d’un projet. Les modifications apportées au plan du projet peuvent déclencher des modifications dans la chronologie du projet. La chronologie du projet doit être automatiquement ou manuellement recalculée pour s’assurer qu’il est à jour avec ces modifications.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 12%

---

# Vue d’ensemble du type de mise à jour du projet

Le type de mise à jour d’un projet indique comment Adobe Workfront calcule la chronologie d’un projet. Les modifications apportées au plan du projet peuvent déclencher des modifications dans la chronologie du projet. La chronologie du projet doit être automatiquement ou manuellement recalculée pour s’assurer qu’il est à jour avec ces modifications.

Pour plus d’informations sur le recalculage de la chronologie du projet, voir [Recalculer la chronologie du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Types de mise à jour de projet

Il existe quatre types de mise à jour pour un projet, selon le moment où Workfront doit recalculer la chronologie du projet. Sélectionnez un Type de mise à jour dans la liste ci-dessous.

Pour plus d’informations sur la mise à jour du type de mise à jour du projet, voir [Sélectionner le type de mise à jour du projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).

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
