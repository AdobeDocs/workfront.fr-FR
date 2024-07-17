---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Vue d’ensemble de la modification des affectations de tâches
description: Vous pouvez affecter des tâches à des utilisateurs, à des équipes ou à des rôles de tâche, ou en annuler l’affectation. Vous pouvez affecter plusieurs ressources simultanément ou une seule ressource. Vous pouvez affecter une tâche à la fois ou plusieurs tâches en bloc.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 9%

---

# Vue d’ensemble de la modification des affectations de tâches

Vous pouvez affecter des tâches à des utilisateurs, à des équipes ou à des rôles de tâche, ou en annuler l’affectation. Vous pouvez affecter plusieurs ressources simultanément ou une seule ressource. Vous pouvez affecter une tâche à la fois ou plusieurs tâches en bloc.

>[!TIP]
>
>Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
>
>Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
>
>* Réaffectez l’élément de travail aux ressources actives.
>* Associez les personnes d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.
>

Cet article contient des informations générales sur l’impact de la modification des affectations de tâche. Pour plus d’informations sur l’affectation de tâches, consultez les articles suivants :

* Pour plus d’informations sur l’affectation de tâches, voir [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md) et [Modification de plusieurs affectations d’utilisateurs dans une liste de tâches](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Pour plus d’informations sur la modification des affectations sur plusieurs tâches dans la zone Planification, voir &quot;Modification de plusieurs affectations d’utilisateurs à des tâches dans les zones Planification&quot;.
* Pour plus d’informations sur l’affectation de tâches à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’affectation de travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Certaines informations de cet article s’appliquent également aux affectations à des problèmes. Pour plus d’informations sur l’affectation des problèmes et des considérations supplémentaires, voir [Présentation de la modification des affectations de problèmes](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Quand modifier les affectations d’utilisateurs sur les tâches

Vous pouvez modifier les affectations d’utilisateurs pour des tâches pour diverses raisons, notamment :

* Les utilisateurs rejoignent ou quittent votre équipe
* Un utilisateur prend des vacances qui s’étendent au-delà des dates d’échéance de tâche

  >[!NOTE]
  >
  >Lorsque les utilisateurs sont affectés au travail, leur disponibilité en fonction de leurs plannings affecte les Dates Prévues et Prévues des tâches. Pour plus d’informations sur les plannings, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Un rôle ou un utilisateur spécifique est défini comme responsable de plusieurs tâches et vous souhaitez modifier rapidement tous les éléments à affecter à un autre utilisateur ou rôle.

## Considérations relatives à plusieurs affectations pour les rôles de tâche, les équipes et les utilisateurs

Tenez compte des points suivants lorsque vous affectez plusieurs ressources à une tâche :

* Les utilisateurs peuvent avoir plusieurs rôles de tâche associés à leur profil. Pour plus d’informations sur l’association d’utilisateurs à des rôles de tâche, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Les tâches ou les problèmes sont généralement affectés en premier à un ou plusieurs rôles de tâche ou à une équipe. Lorsque les projets sont prêts à démarrer, ils doivent peut-être également être affectés aux utilisateurs.\
  Si une tâche ou un problème est assigné à un ou plusieurs rôles, puis que vous affectez également un utilisateur, Adobe Workfront décide quel rôle de tâche associer à l’utilisateur supplémentaire (le cas échéant) selon les règles suivantes :

   * Si un seul rôle de tâche est attribué et qu’il correspond au rôle de Principal de l’utilisateur, la tâche ou le problème est affecté uniquement à l’utilisateur qui remplit son rôle de Principal.
   * Si plusieurs rôles sont affectés et qu’au moins un des rôles correspond aux rôles secondaires de l’utilisateur, la tâche ou le problème est alors assigné à l’utilisateur qui remplit l’un de ses Autres rôles — que Workfront sélectionne au hasard s’il existe plusieurs correspondances — ainsi que les rôles supplémentaires affectés.
   * Si un ou plusieurs rôles de tâche sont affectés et qu’il n’y a aucune correspondance avec les rôles de l’utilisateur, la tâche ou le problème est affecté à la fois au rôle ou aux rôles ainsi qu’à l’utilisateur.

* Si une tâche ou un problème est assigné à une équipe et que vous affectez également un utilisateur, la tâche ou le problème reste assigné à l’équipe et à l’utilisateur.

## L’impact de la suppression des personnes désignées sur les heures de tâche et les pourcentages d’attribution

La suppression d’utilisateurs peut affecter les heures de tâche et les pourcentages d’attribution. L’effet de la suppression d’un utilisateur sur la tâche dépend du type de durée sélectionné pour la tâche. Pour plus d’informations sur le type de durée, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Lorsque vous supprimez un utilisateur d’une tâche avec les types de durée suivants :

* **Simple :** Les heures planifiées affectées à cet utilisateur sont soustraites du nombre total d’heures planifiées de la tâche.

  >[!IMPORTANT]
  >
  >Cela peut avoir une incidence négative sur le plan du projet, car cela modifie le nombre total d’heures planifiées pour la tâche et le projet.

* **Effort Driven :** Le pourcentage d’attribution ne change pas pour les autres utilisateurs.
* **Attribution calculée :** Les pourcentages d’attribution des autres utilisateurs sont ajustés de sorte que le total soit égal à 100 %.
* **Travail calculé :** Le pourcentage d’attribution ne change pas pour les autres utilisateurs.

## Remarques concernant l’annulation de l’affectation de tâches

Vous pouvez supprimer des affectations d’une tâche à la fois ou vous pouvez supprimer des affectations de plusieurs tâches en bloc.

Pour plus d’informations sur la suppression des affectations des tâches en bloc, voir [Modification de plusieurs affectations d’utilisateurs dans une liste de tâches](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Tenez compte des points suivants lors de la suppression d’affectations de tâches :

* Lorsque vous annulez l’affectation d’un utilisateur à une tâche, la tâche reste affectée au rôle de tâche que l’utilisateur a rempli dans la tâche.
* Lorsque vous annulez l’affectation d’un rôle de tâche ou d’une équipe à une tâche, celle-ci reste non affectée si elle n’est affectée à aucune autre ressource.
