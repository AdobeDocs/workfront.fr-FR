---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la date d’achèvement effective du projet
description: Les projets, les tâches et les problèmes ont une date d’achèvement effective dans Adobe Workfront. Il s’agit de la date à laquelle le projet, la tâche ou le problème a été marqué(e) comme étant terminé(e).
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
TQID: https://experienceleague.adobe.com/MoATj74YM1zoW2SsIGrpKY0gc9dHRKjlDvnPfT-kk2s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 490
ht-degree: 99%

---

# Vue d’ensemble de la date d’achèvement effective du projet

Les projets, les tâches et les problèmes ont une date d’achèvement effective dans Adobe Workfront. Il s’agit de la date à laquelle le projet, la tâche ou le problème a été marqué(e) comme étant terminé(e).

## Dates d’achèvement effectives

La date d’achèvement effective représente la date et l’heure réelles de l’achèvement du travail. Lorsqu’une tâche ou un problème est marqué(e) avec le statut Terminé, Workfront définit automatiquement la date du changement de statut de l’élément comme la date d’achèvement effective de la tâche ou du problème. Si cette date ne reflète pas exactement la date à laquelle la tâche ou le problème a été réellement achevé(e), vous pouvez alors modifier manuellement la date d’achèvement effective.

Par exemple, vous pouvez marquer une tâche ou un problème comme étant terminé(e) le lundi, mais vous savez que le travail a été effectué le vendredi précédent. Après avoir marqué la tâche ou le problème avec le statut Terminé, vous pouvez ensuite mettre à jour manuellement la date d’achèvement effective de la tâche ou du problème au vendredi précédent pour refléter l’achèvement réel.

Vous ne pouvez pas modifier manuellement la date d’achèvement effective d’un projet, mais vous pouvez modifier manuellement le statut d’un projet, ce qui peut entraîner une modification de sa date d’achèvement effective.

La date d’achèvement effective d’un projet est définie de l’une des manières suivantes :

* En mettant à jour manuellement le statut du projet : si le mode d’achèvement du projet est défini sur Manuel et que vous modifiez manuellement le statut du projet sur Terminé, cela déclenche la mise à jour de la date d’achèvement effective du projet à la date et à l’heure de la dernière tâche terminée.
* Automatiquement, lorsque la dernière tâche du projet est terminée : si le mode d’achèvement du projet est défini sur Automatique et que vous marquez la dernière tâche avec le statut Terminé ou que vous mettez à jour la date d’achèvement effective de la dernière tâche, la date d’achèvement effective du projet est également mise à jour avec cette date.

  Pour plus d’informations sur la définition du mode d’achèvement d’un projet, voir l’article [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront utilise la date d’achèvement effective de la tâche du projet qui s’est achevée en dernier comme date d’achèvement effective pour l’ensemble du projet.

Un administrateur ou une administrice Workfront ou de groupes détermine si Workfront utilise la date du jour ou la date d’achèvement prévue d’une tâche ou d’un problème lorsque ceux-ci sont définis avec les statut Terminé ou Fermé. Pour plus d’informations sur la définition des préférences de tâches et de problèmes, voir [Configurer les préférences de tâches et de problèmes à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Localiser les dates d&#39;achèvement effectives

La date d’achèvement effective se trouve dans les zones suivantes de Workfront :

* Zones des détails du projet, de la tâche et du problème.
* Zones Modifier le projet, la tâche et le problème.
* Zones Mises à jour du projet, de la tâche et du problème en tant que Mise à jour système.
* Listes ou rapports des projets, des tâches ou des problèmes.

Pour plus d’informations sur la création de rapports, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
