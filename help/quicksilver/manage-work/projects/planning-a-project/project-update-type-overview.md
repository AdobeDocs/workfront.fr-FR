---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Aperçu du type de mise à jour du projet
description: Le type de mise à jour d’un projet indique comment Adobe Workfront calcule la chronologie d’un projet. Les modifications apportées au plan du projet peuvent entraîner des changements dans la chronologie du projet. La chronologie du projet doit être recalculée automatiquement ou manuellement pour s’assurer qu’elle est à jour par rapport à ces changements.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 70%

---

# Vue d’ensemble du type de mise à jour du projet

Le type de mise à jour d’un projet indique comment Adobe Workfront calcule la chronologie d’un projet. Les modifications apportées au plan du projet peuvent entraîner des changements dans la chronologie du projet. La chronologie du projet doit être recalculée automatiquement ou manuellement pour s’assurer qu’elle est à jour par rapport à ces changements.

Pour plus d’informations sur le recalcul de la chronologie d’un projet, voir [Recalculer les chronologies des projets](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Types de mises à jour de projets

Il existe quatre types de mises à jour pour un projet, selon le moment où vous souhaitez que Workfront recalcule la chronologie du projet. Choisissez un type de mise à jour dans la liste ci-dessous.

Pour plus d’informations sur la mise à jour du type de mise à jour du projet, voir [Sélectionner le type de mise à jour d’un projet](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Si la chronologie d’un projet est supérieure à 15 ans, Workfront ne calcule pas la durée automatiquement ou en cas de modification. Le type de mise à jour d’un projet de plus de 15 ans est toujours manuel.

* **Automatique et En cas de modification :** il s’agit du paramètre par défaut. La chronologie du projet est mise à jour chaque fois qu’une modification est apportée au projet ou à un autre projet dont la chronologie dépend. La chronologie du projet est également mise à jour chaque nuit.\
  Il s’agit du paramètre recommandé, car il garantit que la chronologie du projet est toujours à jour.

  Lorsque vous mettez à jour une tâche ou un projet et que vous déclenchez un recalcul de la chronologie, toutes les dates disponibles sont immédiatement affichées, ce qui vous permet de continuer à travailler. Pour les projets comportant plus de 100 tâches, les dates qui nécessitent des calculs plus longs sont grisées.

  ![](assets/dates-dimmed-when-insline-editing-350x146.png)

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
