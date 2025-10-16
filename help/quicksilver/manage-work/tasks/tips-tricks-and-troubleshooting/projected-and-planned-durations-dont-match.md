---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: La durée prévisionnelle ne correspond pas à la durée prévue
description: 'Cet article décrit la résolution de problèmes dans Adobe Workfront en cas de réception du message suivant : ''La durée prévue d''une tâche/d''un événement est passée à 0 et ne correspond pas à la durée prévue.'''
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 83%

---

# La durée prévisionnelle ne correspond pas à la durée prévue.

## Problème

Vous recevez le message d’erreur suivant : « La durée prévisionnelle d’une tâche / d’un problème est passée à 0 et ne correspond pas à la durée prévue ».

## Cause

Cela est dû au fait que la date de début prévisionnelle correspond à la date d’achèvement prévisionnelle.

## Solution

De nombreux facteurs peuvent faire correspondre les dates de début et d’achèvement prévisionnelles. Ce problème est en grande partie lié à l’affectation du temps sur la tâche ou le problème en question.

La plupart du temps, en fonction du type de durée de la tâche et de sa contrainte de tâche, la date d’achèvement prévisionnelle de l’affectation doit souvent être prolongée. Cependant, dans certains cas, en fonction de la configuration du type de durée et de la contrainte de tâche, cette valeur peut-être nulle.

Ci-dessous, vous trouverez une liste des éléments essentiels à examiner dans ces situations, accompagnée de liens vers des articles complémentaires :

* Date d’achèvement prévisionnelle : [vue d’ensemble de la date d’achèvement prévisionnelle pour les projets, tâches et problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)
* Contrainte de tâche : [vue d’ensemble de la contrainte de tâche](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)
* Type de durée : [vue d’ensemble de la durée et du type de durée de la tâche](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)

Si la date d’achèvement prévisionnelle, la contrainte de tâche ou le type de durée fonctionnent comme prévu, contactez le service d’assistance pour un diagnostic plus approfondi.
