---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Présentation des types de dépendances des tâches
description: Les types de dépendances se rapportent aux relations de prédécesseur entre les tâches. Ils définissent le moment où la tâche dépendante peut commencer ou se terminer en fonction du début ou de la fin de son prédécesseur.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Présentation des types de dépendances des tâches

<!-- Audited: 12/2023 -->

Les types de dépendances se rapportent aux relations de prédécesseur entre les tâches. Ils définissent le moment où la tâche dépendante peut commencer ou se terminer en fonction du début ou de la fin de son prédécesseur.

>[!IMPORTANT]
>
>Adobe Workfront ne limite pas le démarrage ou la fin des tâches dépendantes en fonction des types de dépendances, sauf si les relations de prédécesseur sont appliquées. Pour plus d’informations sur l’application des prédécesseurs, voir [Application des prédécesseurs](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Vous devez spécifier le type de dépendance d’une relation précédente lorsque vous établissez cette relation entre vos tâches.

Pour plus d’informations sur les prédécesseurs, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Voici les types de dépendance Workfront :

* **Finish-Start (fs)**: la tâche du prédécesseur doit se terminer avant que la tâche dépendante puisse commencer. Il s’agit du type de dépendance par défaut, utilisé lorsqu’aucun autre type de dépendance n’est spécifié.
* **Finish-Finish (ff)**: la tâche du prédécesseur doit se terminer avant que la tâche dépendante ne puisse se terminer.
* **Start-Start (ss)**: la tâche du prédécesseur doit commencer avant que la tâche dépendante puisse commencer. Vous ne pouvez pas démarrer la tâche dépendante à moins que le prédécesseur n&#39;ait au moins commencé.
* **Start-Finish (sf)**: la tâche du prédécesseur doit commencer avant que la tâche dépendante ne puisse se terminer. Vous pouvez démarrer la tâche dépendante avant le début du prédécesseur, mais vous ne pouvez pas la terminer à moins que le prédécesseur n’ait commencé.
* **Scheduled-Start (sd)**: une tâche est planifiée sur le modèle Terminer-Démarrer, mais le type d’application réel est Terminer-Terminer. Lorsque vous utilisez cette option, la tâche dépendante est planifiée une fois la tâche du prédécesseur terminée. Toutefois, l’application le fait de sorte que la tâche dépendante puisse commencer à tout moment, mais ne peut pas se terminer tant que la tâche du prédécesseur n’est pas terminée.

>[!NOTE]
>
>Les abréviations des types de dépendance sont utilisées dans les listes de tâches pour définir les relations de prédécesseur. Pour plus d’informations, voir [Exemples de valeurs de prédécesseur dans une liste de tâches](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [Présentation des prédécesseurs de tâches](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

