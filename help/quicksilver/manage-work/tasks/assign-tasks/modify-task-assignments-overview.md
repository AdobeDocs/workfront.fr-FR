---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Présentation de la modification des affectations de tâche
description: Vous pouvez affecter des tâches à des personnes, à des équipes ou à des fonctions, ou en annuler l’affectation. Vous pouvez affecter plusieurs ressources simultanément ou une seule ressource. Vous pouvez affecter une tâche à la fois ou plusieurs tâches en masse.
author: Lisa
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 96%

---

# Vue d’ensemble de la modification des affectations de tâches

Vous pouvez affecter des tâches à des personnes, à des équipes ou à des fonctions, ou en annuler l’affectation. Vous pouvez affecter plusieurs ressources simultanément ou une seule ressource. Vous pouvez affecter une tâche à la fois ou plusieurs tâches en masse.

>[!TIP]
>
>Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
>
>Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
>
>* Réaffectez la tâche aux ressources actives.
>* Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.
>

Cet article contient des informations générales sur l’impact de la modification des affectations de tâches. Pour plus d’informations sur l’affectation de tâches, consultez les articles suivants :

* Pour plus d’informations sur l’affectation de tâches, voir [Affecter des tâches](../../../manage-work/tasks/assign-tasks/assign-tasks.md) et [Modifier plusieurs affectations de personnes dans une liste de tâches](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Pour plus d’informations sur la modification des affectations sur plusieurs tâches dans la zone Planning, voir « Modifier plusieurs affectations de personnes à des tâches dans les zones Planning ».
* Pour plus d’informations sur l’affectation de tâches à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’affectation du travail dans l’équilibreur de charge de travail](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Certaines informations de cet article s’appliquent également aux affectations à des problèmes. Pour plus d’informations sur l’affectation des problèmes et pour des considérations supplémentaires, voir [Vue d’ensemble de la modification des affectations de problèmes](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Quand modifier les affectations de personnes sur les tâches ?

Vous pouvez modifier les affectations de personnes sur des tâches pour diverses raisons, notamment :

* Des utilisateurs et utilisatrices rejoignent ou quittent votre équipe.
* Une personne prend des vacances qui s’étendent au-delà des dates d’échéance de tâche

  >[!NOTE]
  >
  >Lorsque les personnes sont affectées au travail, leur disponibilité en fonction de leurs plannings affecte les dates prévues et projetées des tâches. Pour plus d’informations sur les plannings, voir [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Un rôle ou une personne pécifique devient cessionnaire de plusieurs tâches et vous souhaitez modifier rapidement tous les éléments pour qu’ils soient affectés à une autre utilisateur ou un autre rôle.

## Considérations relatives à plusieurs affectations pour les fonctoins, les équipes et les utilisateurs et utilisatrices

Tenez compte des points suivants lorsque vous affectez plusieurs ressources à un élément de travail :

* Les utilisateurs et utilisatrices peuvent avoir plusieurs fonctions associées à leur profil. Pour plus d’informations sur l’association d’utilisateurs et d’utilisatrices à des fonctions, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Les tâches ou les problèmes sont généralement affectés en premier à une ou plusieurs fonctions ou à une équipe. Lorsque les projets sont prêts à démarrer, ils doivent peut-être également être affectés aux utilisateurs et utilisatrices.\
  Si une tâche ou un problème est assigné à une ou plusieurs fonctions, puis que vous affectez également un utilisateur ou une utilisatrice, Adobe Workfront décide quelle fonction associer à l’utilisateur ou à l’utilisatrice supplémentaire (le cas échéant) selon les règles suivantes :

   * Si une seule fonction est attribuée et qu’elle correspond au rôle principal de l’utilisateur ou de l’utilisatrice, la tâche ou le problème est affecté(e) uniquement à l’utilisateur ou à l’utilisatrice qui remplit son rôle principal.
   * Si plusieurs rôles sont affectés et qu’au moins un des rôles correspond aux rôles secondaires de l’utilisateur ou de l’utilisatrice, la tâche ou le problème est alors assigné(e) à l’utilisateur ou à l’utilisatrice qui remplit l’un de ses autres rôles (que Workfront sélectionne au hasard s’il existe plusieurs correspondances) ainsi que les rôles supplémentaires affectés.
   * Si une ou plusieurs fonctions sont affectées et qu’il n’y a aucune correspondance avec les rôles de l’utilisateur ou de l’utilisatrice, la tâche ou le problème est affecté à la fois au ou aux rôles et à l’utilisateur ou l’utilisatrice.

* Si une tâche ou un problème est affecté à une équipe et que vous affectez également un utilisateur ou une utilisatrice, la tâche ou le problème reste affecté(e) à la fois à l’équipe et à l’utilisateur ou à l’utilisatrice.

## Impact de la suppression des cessionnaires sur les heures de tâche et les pourcentages d’allocation

La suppression de personnes peut affecter les heures de tâche et les pourcentages d’allocation. L’effet de la suppression d’une personne sur la tâche dépend du type de durée sélectionné pour la tâche. Pour plus d&#39;informations sur le type de durée, voir [Présentation de la durée de la tâche et du type de durée](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Lorsque vous supprimez un utilisateur d’une tâche avec les types de durée suivants :

* **Simple :** le nombres d’heures prévues affectées à cette personne est soustrait du nombre total d’heures prévues de la tâche.

  >[!IMPORTANT]
  >
  >Cela peut avoir une incidence négative sur le plan du projet, car cela modifie le nombre total d’heures prévues pour la tâche et le projet.

* **Piloté par l’effort :** le pourcentage d’allocation ne change pas pour les autres personnes.
* **Calcul d’affectation :** les pourcentages d’allocation des autres personnes sont ajustés de sorte que le total soit égal à 100 %.
* **Calcul de travail :** le pourcentage d’allocation ne change pas pour les autres personnes.

## Remarques concernant l’annulation de l’affectation de tâches

Vous pouvez supprimer des affectations d’une tâche à la fois ou vous pouvez supprimer des affectations de plusieurs tâches en masse.

Pour plus d’informations sur la suppression d’affectations de tâches en masse, voir [Modifier plusieurs affectations d’utilisateurs et utilisatrices dans une liste de tâches](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Tenez compte des points suivants lors de la suppression d’affectations de tâches :

* Lorsque vous annulez l’affectation d’une personne à une tâche, la tâche reste affectée à la fonction que la personne remplissait dans la tâche.
* Lorsque vous annulez l’affectation d’une fonction ou d’une équipe à une tâche, celle-ci reste non affectée si elle n’est affectée à aucune autre ressource.
